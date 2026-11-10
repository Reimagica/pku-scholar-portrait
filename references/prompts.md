# 分阶段提示词
先读取 SKILL.md，再使用对应模板。只填写当前阶段需要的字段；双花括号是替换变量，发送生图前必须替换。参考序号随实际传入图片排列同步调整。

## 共用画风块
Simple PERSONALIZED adult hand-drawn editorial cartoon in the approved series style. Express identity through 3–5 distinctive visible traits and the person's own expression, not through photographic tracing. A slightly enlarged head may be used independently of eye size. Preserve the person's particular eye opening, lids, eye spacing and gaze. The expression may be slightly more charming and cartoon-like: eyes can be modestly enlarged while retaining their individual elongated/almond shape and lid occlusion. No generic large round sparkling eyes. Confident slightly irregular black pen outlines; use a continuous flowing stroke for each shoulder, sleeve edge and lapel wherever natural, never deliberate dash-gap-dash contours; head, hair, nose, mouth and glasses described with few intentional strokes. Hair in a few shape masses; glasses freely drawn with the same pen rather than glossy plastic. Broad water-based felt-tip marker flat passes, mild darker overlaps, uneven stroke ends and ivory paper gaps, especially on clothing. Preserve the subject's complexion. For light complexions, use warm ivory light planes and sparse muted pale ochre facial shadows. Face line weight and shadows follow the bundled portrait-style.png: moderate tapered interior facial pen lines, slightly stronger outer contour, light grouped eyebrow strokes, flat shadow patches and open light planes appropriate to the subject. Avoid uniform heavy outlining, solid block brows or makeup-like eyelids. No photographic skin, dense strand rendering, artificial swirly grain, glossy shading or fine fabric texture. Keep the person's recognizable skin tone and characteristic accessories.

## P：新人物独立绘制
Use case: stylized-concept, character redesign.
Image 1 is the APPROVED SERIES DRAWING STYLE, not the subject identity.
Image 2 is the ACTUAL SUBJECT PHOTO: use for identity, expression, clothing and POSE. Preserve its torso orientation, shoulder line and arm placement while simplifying them into cartoon shapes. Auxiliary photos, if supplied, inform face recognition only.
{{OPTIONAL_COLOR_REFERENCE_ROLE}}
Draw only one waist-up adult cartoon character, no scenery, no words or icons.
IDENTITY ANCHORS: {{THREE_TO_FIVE_PERSON_SPECIFIC_ANCHORS}}
HEAD GEOMETRY: {{SUBJECT_PHOTO_ROLL_TURN_EYE_AXIS_NOSE_MOUTH_CHIN_AND_JAW}}. Preserve those relationships as one coherent three-dimensional head. Keep the original cheek asymmetry and hair occlusions.
EXPRESSION: {{EYE_SHAPE_LIDS_GAZE_BROWS_MOUTH_ASYMMETRY}}. Observe brow tension separately from smile; preserve closed-mouth versus tooth-showing expression. Do not standardize everyone into the same cheerful face.
HEAD/BODY: {{DESIRED_HEAD_PROPORTION}}, do not automatically enlarge the eyes.
CLOTHING/POSE: {{CLOTHING_AND_SIMPLE_POSE}}
COLOR CHECK: {{GARMENT_BASE_COLOR_AND_PATTERN_COLOR_SEPARATELY}}
POSE LOCK: {{MAIN_PHOTO_POSE_TO_KEEP}}. Do not borrow the style reference person’s gesture.
{{COMMON_STYLE_BLOCK}}
Background: {{TRUE_TRANSPARENCY_OR_CLEAN_IVORY}}. Keep deliberate ivory highlights inside skin/clothes opaque when using transparency. Keep complete head and necessary shoulders/arms within the asset. No background from the photograph, no borrowed facial traits from the style master.

## L：独立风景适配
Image 1 is the selected approved landscape asset {{A_B_OR_C}}.
{{OPTIONAL_PHOTO_ROLE}}
Adapt only {{SPECIFIC_LAYOUT_OR_BRANCH_CHANGE}} for placement on {{SIDE}} of a portrait poster. Preserve landmark silhouette, physical structure and sparse hand-drawn character.
Loose broken black pen outlines, large empty gaps in tree crowns, scattered olive/yellow marker dabs. No realistic foliage texture or green filled wall.
{{MAPLE_OR_REFLECTION_OR_STONE_CONSTRAINT}}
True transparent surroundings, no person, no portrait lettering, no name strip. Local ivory inside objects is allowed.
枫叶：每叶独立叶柄，连接主枝/侧枝清楚，叶形大小和朝向不重复；橙黄笔触集中在中部，叶尖留白。
未名湖石：高窄直立，红字从上到下“未”“名”“湖”。
水面按任务指定“少量淡色波纹”或“疏落断续倒影”，不要自行加长塔影。

## A：组合认可人物、风景和姓名条
Image 1 is the approved person asset. Image 2 is the approved landscape. {{OPTIONAL_LAYOUT_REFERENCE}}
Create a vertical 127:178 composition on warm ivory paper.
Place the person on {{SIDE}}, landscape on opposite side beside lower torso. Preserve the approved person's exact drawn identity, eye direction, head/body proportions, contour language and marker coloring. Do not reinterpret or beautify the face.
Landscape remains subordinate and is only scaled/positioned with {{APPROVED_ADAPTATION}}.
Reserve 2–3 staggered empty zones near/above the head and above the landscape; no keywords, icons, placeholder text or boxes.
Bottom approximately 10–12%: medium grey hand-painted strip with clear white bold hand-lettered name exactly:
"{{EXACT_NAME_AND_LINE_BREAKS}}"
Keep entire name inside safe margins. No other text besides existing landmark inscription if used.
Only layout and the name strip are new; do not regenerate a different portrait.
姓名未提供时删去姓名条指令，并将主画面延伸到底。优先独立摆放素材、文字和图标；组版后对照人物锁定项。

## K1：关键词与图标独立素材
Create a small hand-drawn keyword group on true transparent background for an existing scholar poster.
Exact wording: "{{KEYWORD_WITH_CASE_AND_LINEBREAKS}}".
Casual clear black handwriting with an optional loose, pale-gold underline, matching the supplied layout reference. {{ICON_DESCRIPTION_OR_TEXT_ONLY}}
When an icon is requested, use a few simple black pen marks with tiny pale ochre accents, adjacent to the phrase; no dense diagram.
No extra words or symbols. Keep this group separate from any person or scenery.
每幅用本次确定的2–3组关键词，选择1–2项适合的图标，其余纯文字。参照[关键词示意](../assets/keyword-technique.png)的线条与点染，词义和文字以本次输入为准。

## K2：加到已有底稿的空白区
Edit only the reserved empty areas of the supplied approved base.
Add these exact keyword groups at {{POSITIONS}}:
{{EXACT_KEYWORDS_AND_OPTIONAL_ICON_MAPPING}}
Keep portrait, gaze, head proportion, clothing marker texture, scenery and name strip unchanged. Do not fill every gap with decorative marks. Typography remains legible at 7-inch size.
若有已制作的独立关键词组，则将其作为插入素材。后续修改词语也只处理文字/图标层。

## R：单目标修订
Edit ONLY {{TARGET_REGION}} in the current approved base.
CHANGE: {{EXPLICIT_USER_REQUESTED_LOCAL_CHANGES}}. Each change must name its own target region; preserve other regions.
LOCK: {{EXPLICIT_ALREADY_APPROVED_ELEMENTS}}.
REFERENCE ROLES: {{ONLY_NEEDED_REFERENCE_ROLES}}.
No new elements or changed text outside the target region.
输出后逐项对照LOCK，而不把这段提示词当成已锁定的证据。

## 眼珠局部修订
Use IMAGE coordinates. Keep eyelids, eye opening, frame, face and all other areas.
Viewer-left eye = subject's anatomical RIGHT eye; viewer-right eye = subject's anatomical LEFT eye.
Move viewer-left iris/pupil {{DIRECTION_AND_AMOUNT}}.
Move viewer-right iris/pupil {{DIRECTION_AND_AMOUNT}}.
Retain pupil size and natural lid occlusion. Preserve explicitly requested unequal offsets. Do not equalize both eyes automatically.
只按本次人物的明确特征和改动要求填写移动方向与幅度。
