<!-- this is the container that holds this whole thing! you can change the color from white to something else to change the color of the text -->
<div class="container-fluid px-5 row justify-content-center" style="color:{{c!Text Color!}};">
    
    <!-- Here's the container that holds the actual content! you can change the number in col-md-6 to any number between 1 and 12 to make it narrower or wider, the "md" part makes sure it'll be full-width on mobile devices -->
    <div class="card p-4 col-md-6" style="border-width:3px;background-color:{{c!Main Background Color!}};border-color:{{c!Outside Border Color!}};">
<!-- Bottom left icons -->
        <i class="{{i!Decorative Icon!}}" style="position:absolute;left:0;bottom:95px;transform: translate(-35%,-40%);color:{{c!Icon Color!}};font-size:1.75em"></i>
        <i class="{{i!Decorative Icon!}}" style="position:absolute;left:0;bottom:65px;transform: translate(-80%,-20%);color:{{c!Icon Color!}};font-size:1.75em;"></i>
        <i class="{{i!Decorative Icon!}}" style="position:absolute;left:0;bottom:30px;transform: translate(-40%,+0%);color:{{c!Icon Color!}};font-size:2.25em"></i>
        <i class="{{i!Decorative Icon!}}" style="position: absolute;left:0;bottom:0;transform: translate(-50%,+50%);color:{{c!Icon Color!}};font-size:2.75em;"></i>
        <i class="{{i!Decorative Icon!}}" style="position:absolute;left:30px;bottom:0;transform: translate(+0%,+50%);color:{{c!Icon Color!}};font-size:1.75em"></i>
        <!-- Top right icons -->
        <i class="{{i!Decorative Icon!}}" style="position:absolute;right:0;top:95px;transform: translate(+35%,+40%);color:{{c!Icon Color!}};font-size:1.75em"></i>
        <i class="{{i!Decorative Icon!}}" style="position:absolute;right:0;top:65px;transform: translate(+80%,+20%);color:{{c!Icon Color!}};font-size:1.75em;"></i>
        <i class="{{i!Decorative Icon!}}" style="position:absolute;right:0;top:30px;transform: translate(+40%,+0%);color:{{c!Icon Color!}};font-size:2.25em"></i>
        <i class="{{i!Decorative Icon!}}" style="position: absolute;right:0;top:0;transform: translate(+50%,-50%);color:{{c!Icon Color!}};font-size:2.75em;"></i>
        <i class="{{i!Decorative Icon!}}" style="position:absolute;right:30px;top:0;transform: translate(+0%,-50%);color:{{c!Icon Color!}};font-size:1.75em"></i>
        <!-- Top content, which includes the icon, name, and basic info like age, species, etc. To get stuff on separate lines, you'll need to put a <br> tag on the line above it, since it's set to float right now so the text wraps around the icon. If a line of text is too long, it might make things look weird, you might need to add a <br> tag to break up the line of text if that happens -->
        <div class="container-fluid row">
            <div class="col-sm-5 pb-2 pb-md-0">
                <img class="img-thumbnail img-fluid" src="{{u!Icon URL!}}" style="border-width:0;background-color:{{c!Inner Border Color!}};padding:3px;">
            </div>
            <div class="col-sm-7 pt-2 pt-md-0">
                <h1 class="display-4 fa" style="letter-spacing:5px;font-size:1.75rem;">{{!Name!}}</h1>
		{{%Info%
                <p class="lead fa" style="letter-spacing:1px;font-size:1em;line-height:1.5;"><i class="{{i%Info Icon%}}"></i> <span style="font-weight:600;">{{%Info Type%}}:</span><span style="font-weight:500;"> {{%Info Content%}}</span></p>
		%end%}}
            </div>
        </div>
        <!-- HIIIII I'm Wolfie!!! :D Nice to meet you! I'm so glad you've stopped by and visited me :3 Here's some of my interests and dislikes if you wanna be friends! | likes: Resident Evil, Dragon Ball, animals, Overwatch, cosplay, k-pop/rock/metal/v-kei, art | dislikes: anyone mean/bullies ofc, proshippers, basic dni criteria here ig, and anyone who doesn't like animals GRR   -->
        <div class="card mt-4 p-3" style="max-height:200px;overflow:auto;border-width:3px;background-color:{{c!Story Background Color!}};border-color:{{c!Inner Border Color!}};">
            <div class="card-body">
                <h2 class="fa" style="letter-spacing:1px;">Story</h2>
		{{%Story Content%
                <p>{{l%Paragraph%}}</p>
                %end%}}
            </div>
        </div>
	{{?Pagedoll?
        <!-- this is a pagedoll that will always be on the bottom right corner, you can remove it if you'd like, you might need to adjust the width percentage so it looks good with whatever image you have here -->
        <img style="position:absolute;right:0px;bottom:0;transform: translate(+50%,+50%);max-width:{{n!Pagedoll Width Percentage!}}%;" src="{{u!Pagedoll URL!}}">
	?end?}}
    </div>
</div>
<!-- CREDITS, DO NOT REMOVE! also remember to credit the artist(s) of whatever images you use here, you can add a second link for image credit if the two images you're using are made by different artists -->
<div class="mt-2 text-center">
    {{%Image Credits%<a href="{{u%Image Credit Link%}}" title="{{%Image Credit Title%}}"><i class="fa fas fa-image" style="color:{{c!Icon Color!}};"></i></a> %end%}}<a href="https://toyhou.se/PunkWasp" title="code credit: PunkWasp"><i class="fa fas fa-code" style="color:{{c!Icon Color!}};"></i></a>
</div>
