responsive.less
Author: Paul Mist
Twitter: @paulmist

EXAMPLE USAGE
-------------

--- Import to your .less styles ---

@import 'responsive.less';

--- .width() ---

Convert px based width to %
where 480px is our desired element width
and 960px is the context in which it
sits, or it parent's width -

#div{
	.width(960, 480);	
}

--- .padding() ---

Convert px based padding to %
where 10px (the usual 'top right bottom left' order applies)
is our desired element's padding
and 480px is the element width

#div{
	.padding(480, 10, 10, 10, 10);	
}

Individual properties are also available e.g.

#div{
	.padding-left(480, 10);
}

--- .margin() ---

Convert px based margin to %
where 10px (the usual 'top right bottom left' order applies)
is our desired element's margin
and 480px is the context in which it
sits, or it parent's width -

#div{
	.margin(480, 10, 10, 10, 10);	
}

Individual properties are also available e.g.

#div{
	.margin-left(480, 10);
}