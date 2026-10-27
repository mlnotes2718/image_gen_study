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
- Test 3 is design to test if the image can include textual information in the image according to the prompt request
- Test 4 is design to test if the image can generate image according to the complex requirement.


## Test Methodology
### Test Environment

The following controls were used to reduce contextual influence between trials:
- Image generation was test via API for better control and selection of a model.
- The same prompt were reused for all three trials of a test case.
- We use human as a judge to evaluation the accuracy of the image.
- Each test was repeated three times to assess consistency.


### Test Prompt

#### Test 1 - Evaluate if the model can count object by its color and shape

**Prompt**
```text
Generate an image containing exactly the following objects:

- 3 silver spheres with metallic surfaces.
- 2 green pyramids.
- 4 yellow cubes.

Arrange all 9 objects on a plain white table.
All objects must be fully visible, clearly separated,
and not overlapping.

Do not include any additional objects or text.
```

### Test 2 - Evaluate if the model place object according to the prompt's spatial requirement

**Prompt**
```text
Generate a photorealistic image showing the following
arrangement of objects:

- A large red cube balancing directly on the sharp tip
  of a green pyramid.
- The green pyramid is standing upright on a flat white table.
- A metallic sphere is floating in mid-air to the right
  of the pyramid, without any visible support.
- A yellow cylinder is positioned horizontally underneath
  the floating metallic sphere, without touching it.

All objects must be clearly visible.
Do not include any supporting structures, strings,
or additional objects.

Use a slightly elevated camera angle and a plain
white background.
```

### Test 3 - Evaluate if the model can place text information into an image in a realistic manner

```text
Generate a photorealistic image of a large electronic
flight departure board inside a modern international airport.

The board must display exactly six flights in a table
with four columns labelled:
FLIGHT, DESTINATION, TIME, and STATUS.

Display the following information exactly:

FLIGHT | DESTINATION | TIME | STATUS
SQ318  | LONDON      | 09:45 | BOARDING
JL712  | TOKYO       | 10:20 | ON TIME
EK355  | DUBAI       | 11:05 | DELAYED
QF082  | SYDNEY      | 12:30 | GATE OPEN
CX650  | HONG KONG   | 13:15 | ON TIME
TG402  | BANGKOK     | 14:50 | CANCELLED

All six rows must be present in the specified order.
Every flight number, destination, time, and status
must match exactly.

Mount the departure board high above the airport floor.
Position the camera at a standing adult's eye level,
approximately 1.6 metres above the floor, looking
upward at the board at a 15-degree angle.

Use a natural passenger viewpoint with realistic
perspective distortion.

The entire board must remain visible within the frame.
All text must be sharp, clearly readable, and correctly
aligned in four columns despite the viewing angle.

Use realistic electronic display lighting.

Do not add extra flights, columns, or information
to the board.
```


### Test 4 - Evaluate if the model can generate a realistic image according to the prompt requirements

```text
Generate a photorealistic image of a modern minimalist
living room with the following furniture arrangement:

- One beige three-seater sofa positioned against the back wall.
- One rectangular wooden coffee table directly in front
  of the sofa.
- Two identical blue armchairs, one on each side of the
  coffee table, facing inward.
- One black floor lamp positioned to the right of the sofa.
- One green potted plant positioned to the left of the sofa.
- One large ceiling to floor sliding door on the left wall with the door open.

Soft morning sunlight enters through the glass from
the left, illuminating the furniture and casting
realistic, consistent shadows toward the right.

The background outside the sliding glass door should show a clear blue sky with ocean waves and a sandy beach.

Use a wide-angle, eye-level camera perspective.

The room should have natural materials, realistic
fabric textures, accurate furniture proportions,
and a warm, inviting atmosphere.

All furniture must be clearly visible.
Do not include people, additional furniture, or text.
```

### Scoring Approach
### Test Result Summary





## Observations and Discussion


## Strengths and Weaknesses

## Suggestions for Effective Use

## Limitations of This Evaluation

## Conclusion


## Appendix A - Detailed Test Result
