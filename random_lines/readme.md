# Drawing Graphics in C#
This project demonstrates a simple way to draw lines in a Windows Form. Here we create a `Bitmap` then use a `Graphics` object to draw lines on it. The `Bitmap` is then assigned to `PictureBox.Image` and displayed to the user.

### Initializing Bitmap and Graphics Objects
* Initializing a bitmap takes a little time, so for graphs which update frequently it is to your advantage to declare them as class-level variables and initialize them once when the program loads.
* In this example we initialize the bitmap to match the size of `PictureBox` which it will later be drawn on. 
* You'll have to re-initialize the bitmap and graphics objects if the size changes, but this can be done by adding a `SizeChanged` event handler to PictureBox1.
* By default the Bitmap has a transparent background. Use `gfx.Clear()` to fill the entire image with a solid color.
* If you want lines to be anti-aliased (a prettier output but a slight decrease in speed) set the `gfx.SmoothingMode`.

