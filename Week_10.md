## Week 10 - The Wall and the Move

### What I wanted to build
A Hugging Face Space designed to test how different language models handle viewpoint reasoning and spatial consistency when describing the same scene from multiple camera angles. Instead of focusing on image generation quality alone, the project studies whether models can preserve important spatial relationships such as foreground/background positioning, scale, visibility, occlusion, and object placement when the perspective changes. Users can compare multiple lightweight language models across viewpoints like bird’s-eye view, low angle, close-up, and over-the-shoulder using the same scene prompt and generation settings.

The project was created as a response to the limitations discovered while experimenting with lightweight AI image-editing systems. Many small/free models could imitate the vocabulary of camera angles but struggled with the deeper spatial consequences of changing perspective. Perspective Evidence Lab turns that limitation into a reproducible experiment by allowing users to systematically compare outputs, identify inconsistencies, and evaluate how well models preserve spatial logic rather than simply generating fluent text.

### What Space 2 can do
The_Image_Editor is a lightweight AI image-editing Space that generates alternate camera-angle versions of an uploaded image based on a user’s prompt. Users can upload an image, choose a new viewpoint such as bird’s-eye view, low angle, or side view, and guide the transformation with additional prompt details. The Space is designed to experiment with AI-based perspective transformation while preserving as much of the original scene identity, subject placement, and visual composition as possible.

### The wall I hit
Although The_Image_Editor can generate alternate viewpoints of an uploaded image, the outputs are often not accurate or spatially consistent enough to produce meaningful or testable results. Lightweight image-editing models running on free CPU hardware struggle to preserve object proportions, depth, textures, and scene identity when changing perspectives. More reliable image-editing and novel-view models exist, but they are typically too large and computationally expensive to run effectively on free Hugging Face CPU Spaces. As a result, the project shifted toward studying the limitation itself rather than depending entirely on live image generation.

### The move I chose for Space 3
Originally, the project focused on building an AI image editor capable of generating the same scene from different camera angles. However, during testing, it became clear that lightweight image-editing models running on free hardware could imitate camera-angle prompts without reliably preserving the deeper spatial structure of the original scene. Because of these limitations, the research direction shifted away from trying to perfect image generation and toward testing perspective reasoning more directly through text-generation models.

This led to the creation of Perspective Evidence Lab, where language models are compared based on how well they preserve spatial relationships when describing the same scene from different viewpoints. Instead of evaluating image realism, the project now focuses on measurable reasoning factors such as foreground/background changes, visibility, occlusion, scale, and viewpoint consistency. This change turned the project from a search for a better model into a reproducible experiment about the limitations of AI spatial reasoning itself.

### What the move made possible
Shifting from image editing to testing text-generation models made the project more reproducible, measurable, and research-focused. Instead of relying on unstable image outputs from lightweight models, I could now systematically compare how different language models respond to the same scene and viewpoint instructions under controlled settings. This made it possible to directly evaluate spatial reasoning factors such as foreground/background relationships, occlusion, scale, visibility, and viewpoint consistency using scoring rubrics and repeated experiments.

The move also allowed the project to work reliably on free Hugging Face CPU hardware while expanding the number of models that could be tested. Rather than spending most of the project searching for a powerful enough image model, I could focus on analyzing why AI systems struggle with perspective transformation and how prompt structure and model design affect spatial reasoning performance.

### What the move cost
Shifting away from image editing meant giving up direct visual evidence of perspective transformation. The project no longer produces realistic alternate-angle images of the same scene, which was one of the original goals and one of the most visually interesting parts of the idea. By focusing on text-generation models instead, the research became less about visual realism and more about analyzing descriptive reasoning through language outputs.

The move also reduced the ability to test true image-based spatial understanding. Text-generation models can describe viewpoint changes, but they do not actually “see” or reconstruct 3D geometry the way advanced vision systems attempt to. As a result, the project now studies how AI models reason about perspective through text rather than whether they can genuinely generate accurate new visual viewpoints from an image.

### What I need a peer tester to try next week
To test one scene description across all the text-generation models, with different settings available on the sliders provided, as different approaches. This can help them better understand the relationships between different models: their actual limitations, their properties, and how they work in general. 
