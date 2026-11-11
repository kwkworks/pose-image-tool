# 테스트에 쓴 프롬프트 모음

노트 `pose_tool.ipynb` 가 자동으로 만든 기록입니다. 모든 생성은 시드 고정(재현 가능).

## 프롬프트 원문

### astronaut

> A single astronaut in a white spacesuit with a gold visor, holding a balanced pose. Full-body shot, eye level, 35mm lens. Harsh sunlight from the left casting a sharp shadow. Gray lunar surface with Earth rising on the black horizon. Photorealistic NASA-style documentary photography.

### ballerina

> A single ballerina in a pale pink tutu and satin pointe shoes, holding a balanced pose. Full-body shot, eye level, 50mm lens. Warm spotlight from above with a soft glow on the floor. Dark empty theater stage with velvet curtains. Photorealistic stage photography, shallow depth of field.

### knight

> A single medieval knight in polished silver plate armor and a red cape, holding a balanced pose. Full-body shot, low angle, 35mm lens. Golden hour backlight with rim light on the armor. Grassy hill in front of a stone castle. Cinematic fantasy film still, rich colors.

## 방식 B(klein)에서 프롬프트 앞에 붙인 포즈 지시문

> The reference image is a stick-figure pose skeleton. Draw a new photo where the subject matches that exact body pose, limb positions and framing. Do not draw the skeleton itself.

## 생성 기록

| 파일 | 실험 | 방식 | 포즈 | 프롬프트 | 시드 | 스텝 | cfg | 강도 | 크기 |
|---|---|---|---|---|---|---|---|---|---|
| exp1_pose01_astronaut_A.png | 1 | A | pose_01.png | astronaut | 42 | 25 | 7.0 | 1.0 | 640x512 |
| exp1_pose01_astronaut_klein.png | 1 | B | pose_01.png | astronaut | 42 | 4 | 4.0 | - | 1024x768 |
| exp1_pose01_ballerina_A.png | 1 | A | pose_01.png | ballerina | 42 | 25 | 7.0 | 1.0 | 640x512 |
| exp1_pose01_ballerina_klein.png | 1 | B | pose_01.png | ballerina | 42 | 4 | 4.0 | - | 1024x768 |
| exp1_pose01_knight_A.png | 1 | A | pose_01.png | knight | 42 | 25 | 7.0 | 1.0 | 640x512 |
| exp1_pose01_knight_klein.png | 1 | B | pose_01.png | knight | 42 | 4 | 4.0 | - | 1024x768 |
| exp3_pose02_strength0.3.png | 3 | A | pose_02.png | astronaut | 42 | 25 | 7.0 | 0.3 | 640x512 |
| exp3_pose02_strength0.6.png | 3 | A | pose_02.png | astronaut | 42 | 25 | 7.0 | 0.6 | 640x512 |
| exp3_pose02_strength1.0.png | 3 | A | pose_02.png | astronaut | 42 | 25 | 7.0 | 1.0 | 640x512 |
| exp3_pose02_strength1.4.png | 3 | A | pose_02.png | astronaut | 42 | 25 | 7.0 | 1.4 | 640x512 |
| output_01.png | 기본 | A | pose_01.png | astronaut | 42 | 25 | 7.0 | 1.0 | 640x512 |
| output_01_klein.png | 기본 | B | pose_01.png | astronaut | 42 | 4 | 4.0 | - | 1024x768 |
| output_02.png | 기본 | A | pose_02.png | astronaut | 42 | 25 | 7.0 | 1.0 | 640x512 |
| output_02_klein.png | 기본 | B | pose_02.png | astronaut | 42 | 4 | 4.0 | - | 1024x768 |
| output_03.png | 기본 | A | pose_03.png | astronaut | 42 | 25 | 7.0 | 1.0 | 640x448 |
| output_03_klein.png | 기본 | B | pose_03.png | astronaut | 42 | 4 | 4.0 | - | 1024x704 |
| exp2_knight_pose01_A.png | 2 | A | pose_01.png | knight | 42 | 25 | 7.0 | 1.0 | 640x512 |
| exp2_knight_pose01_klein.png | 2 | B | pose_01.png | knight | 42 | 4 | 4.0 | - | 1024x768 |
| exp2_knight_pose02_A.png | 2 | A | pose_02.png | knight | 42 | 25 | 7.0 | 1.0 | 640x512 |
| exp2_knight_pose02_klein.png | 2 | B | pose_02.png | knight | 42 | 4 | 4.0 | - | 1024x768 |
| exp2_knight_pose03_A.png | 2 | A | pose_03.png | knight | 42 | 25 | 7.0 | 1.0 | 640x448 |
| exp2_knight_pose03_klein.png | 2 | B | pose_03.png | knight | 42 | 4 | 4.0 | - | 1024x704 |
