# Assignment - A Comparative Study of Prompt Adherence in ChatGPT and Gemini Image Generation: The Effects of Constraint Complexity on Object Counting, Spatial Relationships, and Text Accuracy

- This study is to compare the image generation capabilities of ChatGPT and Gemini using text prompt. We will test if the model able to generate image correctly according to our prompt description

## Selected Tools

- The web interface can help to generate image but it cannot provide a specific model for comparison, therefore we use API instead.

Tool-1: ChatGPT
Model: gpt-image-2.5-sunburst
Interface: Python code with OpenAI API

Tool-2: Gemini
Model: gemini-3-pro-image
Interface: Python code with Gemini API


## Test Objectives
The evaluation examines whether the model can:
- generate image with the correct shape, color and count
- generate image with the correct spatial location describe in the prompt
- generate image with the correct text and/or symbol
- generate complex image using all of the elements above and present a photo realistic image.


## Test Cases and Success Criteria
Test 1:
- Capability: Object counting, shape and color generation
- Input: Prompt to generate image according to the shape, color and count
- Evaluation: Can the model generate the correct number of object, with the correct shape and color
- Success Criteria: 9 objects with correct shape, color and count


Test 2:
- Capability: Placing object is the position according to the prompt although it is physically impossible
- Input: Prompt to generate image according to spatial description
- Evaluation: Can the model generate the image with the correct position even though it is physically impossible. As a bonus qualitative check, see if the reflection on the metallic sphere can reflect other objective according to spatial position.
- Success Criteria: Spatial position of the 4 object is correct.

Test 3:
- Capability: Generating text in the image settings
- Input: Prompt to generate image that contains text information
- Evaluation: Can the model generate the image that contains text according to our prompt requirement
- Success Criteria: Text in the image is generated with the correct information

Test 4 - generate complex image according to the describing in the prompt
- Capability: Generating complex image
- Input: Prompt to generate complex image that involves multiple objects and lighting
- Evaluation: Can the model generate complex image according to the prompt
- Success Criteria: Able to generate image according to the prompt


## Rationale for Test Case Design
- This test case is design to check if the model is able to generate image based on user text prompt.
- Test 1 is design to test the ability to count and draw shape with the correct color.
- Test 2 is design to test the model able to place object in physically impossible position and at the same time adhere to the spatial requirement.
- Test 3 is design


## Test Methodology
### Text Environment

The following controls were used to reduce contextual influence between trials:
- Image generation was test via API for better control and selection of a model.
- The same prompt were reused for all three trials of a test case.
- We use human as a judge to evaluation the accuracy of the image.
- Each test was repeated three times to assess consistency.




### scoring approach
### Test Result Summary


### Test 1 - Evaluate if the model can count object by its color and shape

Prompt
```text
Generate image using only instruction in this prompt. Do not use search or any external tools. Specify which model is used to generate this response.

Image Generate Instruction: Generate an image with 3 silver sphere with metallic surface, 2 pyramid in green color and 4 square in yellow color all cluster together.
```

### Test 2 -


## Observations and Discussion


## Strengths and Weaknesses

## Suggestions for Effective Use

## Limitations of This Evaluation

## Conclusion


## Appendix
