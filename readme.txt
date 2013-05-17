USAGE:
  1. set background color
    :call bgimg#set_bg(0xFFFFFF) " 0xRRGGBB
    For Example:
    :call bgimg#set_bg(str2nr(synIDattr(hlID('Normal'), 'bg#')[1:], 16))
  2. set background image
    :call bgimg#set_image("path/to/img.bmp")

Image will be drawn for background color you set.
Be aware of bitmap header version.  LoadImage() doesn't support newer one.
