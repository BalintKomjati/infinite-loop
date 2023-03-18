# Smooth Infinite Zoom  

### A user friendly colab notebook to generate infinite loop videos in minutes (works on free colab plan)
  
👇 Click here to craft your own video  
<a target="_blank" href="https://colab.research.google.com/github/BalintKomjati/smooth-infinite-zoom/blob/main/smooth_infinite_zoom.ipynb">
  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
</a>



### Examples:

Dream of a Distant Galaxy:

https://user-images.githubusercontent.com/47415815/220372351-76a8b510-a42c-4025-99d3-9b6976cf10c4.mp4

<br>
Downtown Alley:

https://user-images.githubusercontent.com/47415815/220378972-d8612868-22bc-4c41-8fa8-92c97caa7df1.mp4

<br>
Ancient Mechanism:

https://user-images.githubusercontent.com/47415815/220441286-d8f14b54-502a-4016-8cba-10df963ac83a.mp4

<br>
Colorful Fractals:

https://user-images.githubusercontent.com/47415815/220379181-bf5c6624-1680-4480-ab27-ad4439edb1a2.mp4
  
<br>  
Cave of Skulls:

https://user-images.githubusercontent.com/47415815/220379362-4ef3d810-9b4c-4376-8200-29eba8ef16c3.mp4

Videos above were generated using the default settings in the notebook. Other than random seed only 1st part of the prompt was changed according to the video title (with slight alternations in some cases) e.g. prompt = "glowing colorful fractals, concept art, HQ, 4k".  

### Credits

 - Original idea and 1st version of the notebook was created by [hardmaru](https://github.com/hardmaru)
 - Thereafter [BalintKomjati](https://github.com/BalintKomjati) made the following improvements:
    - Adopted to run on Google Colab
    - Introduced "interpolation" between outpainted images to create smoother videos. This allows to use wider outpainting masks which tend to generate larger coherent structures, without unpleasant jumps between frames.
    - Put the whole product into a intuitive, user friendly notebook (at least that was the intention :) )


### Backlog of potential improvements (contributions are welcome):

 - AUTOMATIC1111 integration
 - Add the possibility for the output to "drift" between prompts (now uses the same prompt for all images with different seed)
 - Fix the issue that any resolution higer than 512 will drastically decrease the network's imagination resulting the generated video rather boring. (e.g. upscale after each inpainting step?)
 - Make movement in the video more realistic without "fisheye" distorsions
 - Possibility to change movement of the camera during video (e.g. turns in any direction)
 - Generate video in non-cubic resolution (now only cubic is possible)
