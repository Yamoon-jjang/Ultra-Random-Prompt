Ultra Random Prompt v8.0.0
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
2. `Ultra_random_prompt_v8.0.0.html`을 Chrome 등 현대적인 브라우저에서 엽니다.
3. 상단에서 KO 또는 EN을 선택하고, 왼쪽에서 항목을 고릅니다.
4. 오른쪽에서 자연어형/태그형, 방향, 길이, 생성 개수를 정해 생성합니다.
5. 프롬프트를 복사하거나 TXT로 저장해 원하는 이미지 생성 워크플로에 사용합니다.

주의
- 선택이 전혀 없으면 생성되지 않습니다. 항목을 선택하거나 전체 랜덤을 먼저 실행하세요.
- 직접 고정한 계절은 유지하며, 일반 장면의 자동 선택에서 명백한 반대 계절 문구만 제한적으로 보정합니다.
- 메인 생성 버튼은 이미지가 아닌 텍스트 프롬프트를 생성합니다.
- OpenAI/Gemini API 기능은 별도로 실행하는 선택 사항이며 사용 조건에 따라 과금됩니다.
- Ollama 이미지 분석에는 설치·실행된 Vision 지원 모델이 필요합니다.
- 저장한 공급자 API 키는 브라우저 localStorage에 보관되며 분석/이미지 미리보기에서 같은 공급자 키를 공유합니다.
- 공개용 HTML에 실제 API 키를 하드코딩하지 마십시오.
- 성인 NSFW 옵션은 성인 대상 텍스트 프롬프트용입니다. 직접 선택과 조합 기능은 화면 언어와 무관하게 유지됩니다.

전체 설명: `Ultra_random_prompt_v8.0.0_사용자메뉴얼_KO.txt`

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
2. Open `Ultra_random_prompt_v8.0.0.html` in a modern browser.
3. Choose KO or EN, then select prompt ingredients from the left panel.
4. Set output format, visual direction, length (for Natural Language), and result count.
5. Generate, review, copy, or export the prompt text into your preferred workflow.

Important notes
- With nothing selected, choose an item or click Full Random before generating.
- Explicitly chosen seasons are preserved; only clear opposite-season cues from automatic ordinary-scene selections are conservatively corrected.
- The app itself does not run ComfyUI or guarantee any particular image model's output quality.
- Optional external API calls may incur charges; account/model availability varies by provider.
- Ollama analysis requires an installed local model with actual Vision capabilities.
- OpenAI/Gemini keys, when stored, reside in browser localStorage; the same provider key is shared by Analysis and Preview.
- Never distribute an HTML copy containing a hardcoded private API key.
- Adult text-prompt data and explicit selections remain available regardless of the chosen UI language.

Complete guide: `Ultra_random_prompt_v8.0.0_User_Manual_EN.txt`

============================================================
PACKAGE CONTENTS
============================================================
Ultra_random_prompt_v8.0.0.html
Ultra_random_prompt_v8.0.0_사용자메뉴얼_KO.txt
Ultra_random_prompt_v8.0.0_User_Manual_EN.txt
README_KO_EN.txt
SHA256SUMS.txt

A SHA256SUMS file is included to verify release file integrity.
