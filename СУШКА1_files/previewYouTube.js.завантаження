var i, c, y, v, s, n;
v = document.getElementsByClassName("youtube");
if (v.length > 0) {
	s = document.createElement("style");
	s.type = "text/css";
	s.innerHTML = '.video_block iframe{min-height: 300px;width: 100%;}.youtube{min-height: 300px;background-color:#000;max-width:100%;height:inherit;overflow:hidden;position:relative;cursor:hand;cursor:pointer}.youtube .thumb{bottom:0;display:block;left:0;margin:auto;max-width:100%;position:absolute;right:0;top:0;width:100%;height:auto} .youtube:hover .play {background-position: 0px -50px;} .youtube .play{background-position: 0px -50px;  -webkit-background-size: 100% auto;background-size: 100% auto;position: absolute;height: 50px;width: 69px;transition: none;top: 0;left: 0;right: 0;bottom: 0;margin: auto;background:url("data:image/png;base64,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") no-repeat} ';
	document.body.appendChild(s)
}
for (n = 0; n < v.length; n++) {
	y = v[n];
	i = document.createElement("img");
	i.setAttribute("src", "https://i.ytimg.com/vi/" + y.id + "/hqdefault.jpg");
	i.setAttribute("class", "thumb");
	c = document.createElement("div");
	c.setAttribute("class", "play");
	y.appendChild(i);
	y.appendChild(c);
	y.onclick = function() {
		var a = document.createElement("iframe");
		a.setAttribute("src", "https://www.youtube.com/embed/" + this.id + "?autoplay=1&autohide=1&border=0&wmode=opaque&enablejsapi=1&rel=0&showinfo=0");
		a.setAttribute("allowfullscreen","");
		a.style.width = this.style.width;
		a.style.height = this.style.height;
		this.parentNode.replaceChild(a, this)
	}
};
//<div class="video_block">
//<div class="youtube" id="AsVwk9bvIU4"></div>
//</div>