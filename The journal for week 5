## Week 5 — Add Controls 

### What I Built
I built a spce called The Scene Describer, and it generates cinematic scene descriptions from chosen viewpoints of a described image referring to the inputs. The model used for text generation id distil gpt-2, which is fast and simpler, but it's less instruction following than the other ones. Also, the the viewpoint-dropdowns are very limited, since the only inputs distilled gpt-2 understands are: close up, wide shot, birds' eye view, low angle, and over the shoulder. These 5 are the only inputs that you can let the AI execute and not cause a chao in the output. 

### What I Tried
I tested the sliders st their extremes. I put each slider at it's max when every other one is at the default. The prompt is "From a bird's eye view, the night city looked: "
- Case 1: The temperature was at its max. The paragraph was 50 - 60 words long, and it tried to describe a reporter drving around the city and talking to herself. At the start of the paragraph it was all normal, but as we approach the end, more and more random combonations of numbers and letters started to appear, like "11AM", "2:00", and "6.oan". 
- Case 2: The Top - p was at its max. The paragraph was 60 - 70 words long, as it tried to describe a part time worker telling his story, which is completly off from the intention of the prompt. It tried it's best to make the paragraph about a city and make the sentences rational, which it did accomplish, but the sentences do not have actual connection, and they often ended in an unexpected way due to the reason that the Top - p is connected to the possibility of what the next word in a sentence could be. 
- Case 3: The Max New Tokens is at its max. The paragraph was bout 120 - 130 words long, as the content being meaningless and made up with sentences that have no connection. The ending wasn't a complete sentence too. 
- Case 4: The Repetition Penalty was at it's max. The paragraph was about 20 - 30 words long, as it tried to describe the literal view of a bird instead of the city sceneries, so I can say that it misunderstood the prompt. Something weird is that at the start of this paragraph, it says "The city looked like it was in its final days", which is completly off from the rest of the paragraph. 

### What Suprised Me 
When the Repetition Penalty was at its max, the paragraph in the output was exceptionally short. This was not supposed to happen since the Max New Tokens was at the default (which means the paragraph should be 60 - 70 words long). I tried a few more times, but I end up getting the same length as the first one. 

### What I Want to Try Next
A fair upgrade to add to this space would be HuggingFaceTB/SmolLM2-135M-Instruct. this model aquires the fastest responses for lightweight text generation, and also is better at following the descriptive prompts when generating texts. 
