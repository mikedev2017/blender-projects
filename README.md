This project was created with Blender. You can download Blender from [Blender.org](https://www.blender.org/). 
The `pyramid_projector_eggzample.blend` file included in this repo contains everything you need to create 
a video for a pyramid hologram projector. You can find instructions for building a pyramid hologram 
projector [here](http://www.instructables.com/id/No-CD-case-no-tape-3D-hologram-pyramid-the-quickes/).

You can download the `egg-hologram.mp4` video included in this repo, if you just want to test the hologram.

To create your own hologram animation, follow the steps below:

1. Replace the egg in the default view with the object you wish to display.
	
	**tip:** Keep the new object the same scale as the egg to ensure that
	your hologram displays properly in the pyramid projector.

2. Set the active camera to the front-camera (select the front camera and press 
   ctrl+ numpad 0 to set the camera as active).

3. Render the frames as a sequence of PNG images by selecting PNG from the render
   settings Output section. By default, it is set to render to the `my-images` 
   folder in the repo.
   
    **Note:** The eggzample holgram is 3 seconds (72 frames) long. For the best 
	results and experience, make sure that each image sequence is 72 frames as well.
	This lets you quickly swap the existing image strips in the Video Sequence editor
	for your new one.

    **Important:** The Video Sequence Editor (VSE) takes priority over the default view render. Make 
    sure the *Sequencer* option is unchecked in the *Post Processing* render settings section, when 
	rendering the PNG image sequences.

4. Repeat step 2 and 3 for each camera view (make sure to change the name of the output file, 
   so you don't overwrite the existing images).

5. Once all your images are rendered for each view, change to the Video Editing screen.

    The project is set up with the hologram layout.

6. Import each camera view PNG set as an image strip. With the current frame set to 1,
   go to *Add* &rarr; *Image* and select the image sequence. Click *Add Image Strip* to 
   add the image sequence to the timeline.

7. Once each image sequence is imported, you can replace the existing eggzample easily. Select 
   the front render view image sequence and shift+right-click select the *egg-hologram-front* 
   image strip. Select *Strip* &rarr; *Sequencer Swap Data* to replace the existing image strip 
   with your own and keep the same transform data.

    **Note:** You can only swap data if the image strips are the same length. If your animation is a 
	different length, you must replace the existing image strips with your own and add the same 
	transforms.

8. Render the finished video (make sure the *sequencer* option is checked, or the default view will render 
   instead).

Hope you enjoy this project, and it makes it easier for you to create some awesome holograms!
