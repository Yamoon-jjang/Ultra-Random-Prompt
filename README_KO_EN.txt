Ultra Random Prompt v8.0.1
KO / EN Bilingual • Single-File Image Prompt Composer
Author: NiceMan (나이스맨)

============================================================
한국어
============================================================

Ultra Random Prompt는 여러 이미지 생성 워크플로에서 사용할 영어 프롬프트를 조합하고 관리하는 단일 HTML 앱입니다.
주 기능은 이미지가 아닌 프롬프트 텍스트 생성입니다. ComfyUI에서 다양한 이미지 모델을 사용할 때 활용할 수 있습니다.

주요 기능
- 상단 KO/EN 버튼으로 한글·영문 화면 전환 (출력 영어 프롬프트 원문 유지)
- 인물/외모/장면/스타일/성인 NSFW 카테고리와 36개 프리셋
- 일반 클릭 고정, Ctrl/⌘ 멀티선택, Shift 하위 카테고리 지정, 랜덤 POOL 선택
- 자연어형과 태그형; 자동·중립/실사/일러스트·애니 기본 방향
- 자연어 길이 간결/표준/상세, 프롬프트 1~100개 일괄 생성 및 중복 억제
- 수동 미리보기 편집, 복사, 번역, 한 줄당 한 프롬프트 TXT 저장(원래 역슬래시 보존, 실제 줄바꿈만 \n으로 표시)
- 설정 저장·복원, 아티스트 스타일 참고, 모바일·키보드 조작
- 선택적 이미지 분석(OpenAI/Gemini/Ollama Vision), 선택적 AI 이미지 미리보기(OpenAI/Gemini)

실행
1. 압축 파일을 풉니다.
2. `Ultra_random_prompt_v8.0.1.html`을 Chrome 등 현대적인 브라우저에서 엽니다.
3. 상단에서 KO 또는 EN을 선택하고, 왼쪽에서 항목을 고릅니다.
4. 오른쪽에서 자연어형/태그형, 방향, 길이, 생성 개수를 정해 생성합니다.
5. 프롬프트를 복사하거나 TXT로 저장해 원하는 이미지 생성 워크플로에 사용합니다.

주의
- 선택이 전혀 없으면 생성되지 않습니다. 항목을 선택하거나 전체 랜덤을 먼저 실행하세요.
- 직접 고정한 장면 조건은 유지합니다. 자동 이벤트는 배경 장소와의 명백한 불일치만 보수적으로 보정하고, 실내 종류별로 여러 후보를 유지합니다.
- 자동 조명과 시간대가 명백히 충돌할 때만 조명(또는 직접 고정한 조명에 대한 자동 시간대)을 정리합니다. 성인 NSFW 촛불도 같은 원칙이며, 두 값을 모두 직접 고정했다면 유지합니다.
- 「친구와 저녁 약속」은 자동 시간대에서 저녁에 적합한 시간을 고릅니다. 저녁 약속을 직접 고정하고 시간대를 자동으로 두어도 적용됩니다.
- 이벤트를 직접 고정하고 배경을 랜덤으로 두면 활성화한 배경 POOL 안에서 어울리는 장소를 찾습니다. 적합한 후보가 없으면 POOL·고정 선택을 우선하며 임의로 새 장소를 만들지 않습니다.
- 성인 NSFW 자동 달빛·명시적 야간 배경은 고정된 낮 시간대와의 충돌을 보정합니다. 정오 고정 시 자동 조명은 여러 호환 후보 사이에서 선택하여 과도한 편중을 줄입니다.
- 자동 조명은 기존에 뽑힌 값이 장면에 맞으면 우선 유지합니다. 부적합할 때는 위치·날씨·시간·스타일에 맞는 후보에서 가중 선택해 일반/NSFW 조명 한 종류로의 편중을 완화합니다.
- 이벤트 고정·자동 배경은 단어 일부만 같은 장소(서점 라운지·호텔 욕실·요가 스튜디오 등)를 적합하다고 간주하지 않습니다. 「비 내리는 저녁」의 자동 날씨도 비와 일치시킵니다. 두 조건을 모두 직접 고정한 경우에는 사용자 선택을 그대로 유지합니다.
- 1인 고정 프리셋은 성별을 자동 선택할 때 남녀 혼성 때문에 2인으로 바뀌지 않습니다. 직접 선택한 혼성 인원 규칙은 그대로 유지됩니다.
- 커스텀 적용 시 같은 그룹의 일반 선택은 보관되지만 출력에서는 대체됩니다. 화면에 적용 안내가 표시됩니다.
- 미선택 항목은 대부분 생략되지만, 자연스러운 문장을 위해 최소 피사체/표정/시선/배경 기본값이 들어갈 수 있습니다.
- 번역 시 프롬프트 원문(성인 문맥 포함)이 비공식 외부 Google 번역 서비스로 전송될 수 있습니다.
- 메인 생성 버튼은 이미지가 아닌 텍스트 프롬프트를 생성합니다.
- OpenAI/Gemini API 기능은 별도로 실행하는 선택 사항이며 사용 조건에 따라 과금됩니다.
- Ollama 이미지 분석에는 설치·실행된 Vision 지원 모델이 필요합니다.
- 저장한 공급자 API 키는 브라우저 localStorage에 보관되며 분석/이미지 미리보기에서 같은 공급자 키를 공유합니다.
- 공개용 HTML에 실제 API 키를 하드코딩하지 마십시오.
- 성인 NSFW 옵션은 성인 대상 텍스트 프롬프트용입니다. 직접 선택과 조합 기능은 화면 언어와 무관하게 유지됩니다.

전체 설명: `Ultra_random_prompt_v8.0.1_사용자메뉴얼_KO.txt`

============================================================
ENGLISH
============================================================

Ultra Random Prompt is a single-file HTML composer for English image-generation prompts, designed for varied image-model workflows including ComfyUI. The primary Generate command creates TEXT, not an image.

Features
- KO/EN interface toggle with source prompt text and selection state preserved
- Subject, Appearance, Scene, Style, and adult NSFW categories; 36 thematic presets
- Fixed choices, Ctrl/Command multi-selection, Shift subcategory selection, weighted random pools
- Natural Language and Tags; Neutral, Photorealistic, or Illustration/Anime direction
- Concise, Standard, and Detailed natural-language output; 1–100 prompts per batch
- Random variation within presets with duplicate-reduction attempts
- Manual preview editing, copy, translation, and one-prompt-per-line TXT export (literal backslashes preserved; physical newlines encoded as \n)
- Saved settings, artist references, mobile and keyboard controls
- Optional Image Analysis through OpenAI, Gemini, or Ollama Vision
- Optional AI Image Preview through OpenAI or Gemini image-generation APIs

Quick start
1. Extract the ZIP archive.
2. Open `Ultra_random_prompt_v8.0.1.html` in a modern browser.
3. Choose KO or EN, then select prompt ingredients from the left panel.
4. Set output format, visual direction, length (for Natural Language), and result count.
5. Generate, review, copy, or export the prompt text into your preferred workflow.

Important notes
- With nothing selected, choose an item or click Full Random before generating.
- Explicit scene choices are preserved. Automatic events are checked for clear venue contradictions while retaining multiple activity choices for different indoor locations.
- Clear automatic light/time conflicts are reconciled; an explicitly chosen light is kept when the time is automatic. The same rule applies to adult candlelight, while two directly fixed axes remain unchanged.
- A dinner appointment with automatic time uses varied late-afternoon/evening slots rather than morning or noon.
- A fixed event with a random background favors compatible venues **within the enabled background pool only**. If none is available, fixed choices and pool boundaries take priority.
- Automatic adult moonlight and explicitly night-named venues are reconciled with a fixed daytime; noon lighting is sampled from more compatible options instead of being dominated by a single default.
- Automatically sampled ordinary/adult lighting remains unchanged when consistent with scene, time, weather, and style. Incompatible lighting is chosen from a wider, weighted compatible set instead of collapsing to the first suggestion.
- Venue matching does not treat a bookstore lounge as a nightclub, a hotel bathroom as a shopping venue, or a yoga studio as backstage. Automatic weather follows an explicitly rainy evening; two directly selected conflicting choices are not overwritten.
- Solo-fixed presets do not silently become groups when the gender is randomized. The intentional manual mixed-gender group rules remain unchanged.
- Applying a Custom entry retains other choices in that group, but replaces them in the current output; a visible notice explains this.
- Unselected fields are usually omitted, but minimal subject, expression, gaze, or scene defaults may still appear for readable sentences.
- Translation can send the source prompt (including adult-context text) to an unofficial external Google translation endpoint.
- The app itself does not run ComfyUI or guarantee any particular image model's output quality.
- Optional external API calls may incur charges; account/model availability varies by provider.
- Ollama analysis requires an installed local model with actual Vision capabilities.
- OpenAI/Gemini keys, when stored, reside in browser localStorage; the same provider key is shared by Analysis and Preview.
- Never distribute an HTML copy containing a hardcoded private API key.
- Adult text-prompt data and explicit selections remain available regardless of the chosen UI language.

Complete guide: `Ultra_random_prompt_v8.0.1_User_Manual_EN.txt`

============================================================
PACKAGE CONTENTS
============================================================
Ultra_random_prompt_v8.0.1.html
Ultra_random_prompt_v8.0.1_사용자메뉴얼_KO.txt
Ultra_random_prompt_v8.0.1_User_Manual_EN.txt
README_KO_EN.txt
SHA256SUMS.txt

A SHA256SUMS file is included to verify release file integrity.
