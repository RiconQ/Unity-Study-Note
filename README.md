# Unity 강연 영상 공부 방법

> Unite Seoul, Unite, GDC, Unity Korea 같은 Unity 강연 영상을 단순 시청으로 끝내지 않고, 실제 개발 역량과 프로젝트 적용으로 연결하기 위한 공부 방식

---

# 1. 공부 목적

강연 영상은 다음 목적을 위해 본다.

1. Unity 기능과 기술 흐름 파악
2. 실제 프로젝트의 문제 해결 방식 분석
3. 내 프로젝트에 적용할 수 있는 아이디어 확보
4. 나중에 다시 참고할 수 있는 기술 문서화
5. 작은 실험을 통해 기술 자산으로 전환

핵심 기준은 다음과 같다.

> 영상을 보고 “알게 된 것”보다,
> Unity 프로젝트 안에서 “작게라도 실험해본 것”이 더 중요하다.

---

# 2. 영상 유형 분류

| 유형         | 목적                                       | 공부 방식            |
| ---------- | ---------------------------------------- | ---------------- |
| 기술 개념형     | URP, Shader, DOTS, Addressables 같은 개념 이해 | 핵심 개념 정리         |
| 사례 분석형     | 실제 게임 제작 방식, 문제 해결 과정 분석                 | 내 프로젝트 적용 가능성 판단 |
| 툴 사용형      | Unity 기능, 패키지, 워크플로우 학습                  | 직접 따라 해보기        |
| 아트 / 테크아트형 | 셰이더, 렌더링, VFX, NPR 표현 학습                 | 샘플 씬 제작          |
| 최적화형       | Profiler, Draw Call, 메모리, 빌드 최적화 학습      | 비교 실험            |
| 파이프라인형     | 팀 협업, 에셋 관리, 빌드 자동화 학습                   | 지금 필요한 부분만 요약    |

---

# 3. 시청 우선순위

## 1순위: 현재 프로젝트에 바로 연결되는 영상

예시:

* Player Controller
* Camera / Cinemachine
* Input System
* Interaction System
* Inventory
* UI
* Save / Load
* Scene Management
* ScriptableObject 구조
* Animation
* Physics
* AI / Navigation

이 유형은 본 뒤 바로 코드, 씬, 시스템 구조에 적용할 수 있는지 판단한다.

---

## 2순위: 프로젝트 품질을 올리는 기술

예시:

* URP
* Shader Graph
* Lighting
* Post Processing
* Outline
* Toon Shading
* NPR Rendering
* VFX Graph
* Animation Rigging
* Audio System
* UI Polish

이 유형은 바로 본 프로젝트에 넣기보다, 작은 샘플 씬에서 먼저 실험하는 것이 좋다.

---

## 3순위: 프로젝트 규모가 커질 때 필요한 기술

예시:

* Addressables
* Asset Bundle
* Scene Streaming
* Asset Management
* Build Pipeline
* Memory Profiling
* Performance Optimization
* Localization
* Platform Build Workflow

이 유형은 당장 깊게 파기보다, 나중에 다시 볼 수 있게 요약해둔다.

---

## 4순위: 현재는 참고만 할 기술

예시:

* DOTS
* ECS
* Multiplayer
* Dedicated Server
* Large Open World
* LiveOps
* Console Optimization
* Mobile Advanced Optimization
* 대규모 팀 파이프라인

---

# 4. 3단계 시청법

## 1단계: 빠르게 훑기

목적은 전체 구조 파악이다.

* 1.25배속 또는 1.5배속으로 시청
* 모든 내용을 필기하지 않음
* 쓸모 있어 보이는 구간만 타임스탬프 저장
* 모르는 용어는 따로 적고 넘어감
* 현재 내 프로젝트와 관련 있는지 판단

이 단계의 목표는 다음 질문에 답하는 것이다.

> 이 영상을 지금 깊게 볼 가치가 있는가?

---

## 2단계: 핵심 구간만 정독

1단계에서 표시한 구간만 다시 본다.

이때는 아래 내용을 정리한다.

* 발표자가 다룬 문제
* 문제의 원인
* 해결 방식
* 사용한 Unity 기능
* 적용 시 장점
* 적용 시 단점
* 내 프로젝트 적용 가능성

모든 내용을 받아쓰지 않는다.
핵심은 “문제 → 해결 → 적용 가능성”이다.

---

## 3단계: 직접 실험

영상 공부의 핵심 단계다.

강연에서 나온 내용을 작은 Unity 테스트 씬으로 만들어본다.

| 영상 주제                | 실험 과제                                          |
| -------------------- | ---------------------------------------------- |
| URP Renderer Feature | 특정 오브젝트에 Outline 효과 적용 테스트                     |
| Shader Graph         | 보호막, 스캔라인, 물, 디졸브 셰이더 제작                       |
| Addressables         | 아이콘, 프리팹, 데이터 로딩 테스트                           |
| Optimization         | Profiler로 Batches, SetPass Calls, Draw Call 비교 |
| Cinemachine          | 카메라 충돌, FOV 보간, Shake 테스트                      |
| Input System         | 키 리바인딩 구조 테스트                                  |
| UI System            | Tooltip, Popup, Inventory UI 구조 테스트            |
| Save / Load          | JSON, ScriptableObject, Binary 방식 비교           |
| Placement System     | 그리드 배치 / 자유 배치 비교                              |
| Animation Rigging    | 캐릭터 손 위치 보정 테스트                                |

---

# 5. 필기 원칙

## 정리해야 하는 것

* 핵심 문제
* 해결 방식
* 사용 기술
* 프로젝트 적용 가능성
* 실험할 것
* 다시 볼 타임스탬프

## 정리하지 않아도 되는 것

* 발표자의 모든 문장
* 이미 아는 기초 설명
* 현재 프로젝트와 무관한 대규모 파이프라인
* 너무 고급이어서 당장 실험 불가능한 내용
* 홍보성 기능 소개

---

# 6. 모르는 개념 처리 방식

영상을 보다가 모르는 용어가 나와도 바로 멈추지 않는다.

먼저 아래처럼 기록한다.

| 용어             | 영상 맥락                   | 나중에 볼 우선순위 |
| -------------- | ----------------------- | ---------- |
| SRP Batcher    | URP 최적화 설명 중 등장         | 높음         |
| Shader Variant | 빌드 크기 / 성능 관련           | 높음         |
| GPU Instancing | 반복 오브젝트 렌더링 최적화         | 보통         |
| Render Pass    | URP Renderer Feature 관련 | 높음         |
| Addressables   | 에셋 로딩 구조                | 보통         |

모르는 개념을 모두 즉시 파고들면 영상 흐름이 끊긴다.
먼저 끝까지 보고, 현재 필요한 개념만 따로 학습한다.

---

# 7. 공부 루틴

## 평일 루틴

목표: 영상 하나에서 실험 Todo 하나 뽑기

```md
1. 영상 30~60분 시청
2. 핵심 내용 5줄 요약
3. 내 프로젝트 적용 가능성 판단
4. 실험 Todo 1개 작성
```

평일에는 완벽한 이해보다 “쓸만한 아이디어 수집”이 중요하다.

---

## 주말 루틴

목표: 영상 내용을 Unity에서 직접 검증하기

```md
1. 평일에 본 영상 중 하나 선택
2. 작은 테스트 씬 제작
3. 구현 난이도 확인
4. 장단점 정리
5. 현재 프로젝트 적용 여부 판단
6. 결과를 Markdown으로 정리
```

---

# 8. 공부 결과물 관리 방식

영상 공부 결과는 아래 3종류로 분리한다.

## 1. 영상 노트

영상별 요약 문서.

예시:

```text
Unite_URP_Optimization.md
Unite_Addressables_Workflow.md
GDC_TechArt_Shader.md
Unity_InputSystem_Workflow.md
```

---

## 2. 실험 씬

Unity 프로젝트 내부 테스트 씬.

예시:

```text
Assets/_StudyLab/Scenes/OutlineTest.unity
Assets/_StudyLab/Scenes/AddressablesTest.unity
Assets/_StudyLab/Scenes/ShaderGraphTest.unity
Assets/_StudyLab/Scenes/CinemachineTest.unity
```

---

## 3. 기술 메모

나중에 다시 참고할 수 있는 정리 문서.

예시:

```text
URP_RendererFeature_Notes.md
Addressables_Basic_Workflow.md
ShaderGraph_NPR_Notes.md
Cinemachine_Camera_Notes.md
InputSystem_Rebinding_Notes.md
SaveLoad_Architecture_Notes.md
```

---

# 9. 추천 학습 주제 분류

## 현재 프로젝트에 바로 필요한 주제

현재 만들고 있는 게임이나 앱에 직접 연결되는 기능을 우선한다.

예시:

* 캐릭터 조작
* 카메라
* 입력 시스템
* 상호작용
* UI
* 인벤토리
* 저장 / 불러오기
* 씬 전환
* 오브젝트 배치
* 애니메이션
* 기본 최적화

---

## 곧 필요해질 수 있는 주제

프로젝트의 완성도와 확장성을 높이는 기술이다.

예시:

* URP 기초
* Shader Graph
* Lighting
* Post Processing
* Addressables
* Profiler 기초
* ScriptableObject Architecture
* Animation Rigging
* Localization
* Build Pipeline

---

## 나중에 볼 주제

프로젝트 규모가 커졌을 때 필요한 고급 주제다.

예시:

* DOTS
* ECS
* Multiplayer
* Dedicated Server
* Large World Streaming
* Advanced Build Pipeline
* Console Optimization
* Mobile Advanced Optimization
* LiveOps

---

# 10. 영상 공부 체크리스트

영상을 다 본 뒤 아래 항목을 확인한다.

* [ ] 이 영상의 핵심 문제를 설명할 수 있는가?
* [ ] 사용된 Unity 기능을 적어두었는가?
* [ ] 내 프로젝트에 적용 가능한 부분을 분리했는가?
* [ ] 지금은 불필요한 부분을 보류했는가?
* [ ] 실험 Todo를 최소 1개 만들었는가?
* [ ] 다시 볼 타임스탬프를 기록했는가?
* [ ] 모르는 용어를 따로 정리했는가?
* [ ] 실제 Unity에서 테스트할 수 있는 형태로 바꿨는가?

---

# 11. 피해야 할 공부 방식

## 모든 내용을 필기하기

강연 전체를 받아쓰면 나중에 다시 읽기 어렵다.
핵심은 전체 기록이 아니라 재사용 가능한 요약이다.

---

## 모르는 개념마다 멈추기

영상 하나를 보는 데 너무 오래 걸린다.
모르는 용어는 따로 기록하고, 중요한 것만 나중에 찾아본다.

---

## 지금 필요 없는 고급 기술에 빠지기

초기 프로토타입 단계에서 아래 주제에 깊게 빠지는 것은 비효율적일 수 있다.

* DOTS
* ECS
* 대규모 월드 스트리밍
* 커스텀 렌더 파이프라인
* 고급 GPU 최적화
* 멀티플레이 서버 구조
* 대규모 빌드 자동화
* 라이브 서비스 운영 구조

현재 목표는 지식 수집 자체가 아니라 프로젝트 진척이다.

---

# 12. 최종 원칙

강연 영상을 볼 때 항상 마지막에 이 질문을 남긴다.

> 그래서 내 프로젝트에서 뭘 바꿀 건가?

답이 없으면 참고 영상이다.
답이 있으면 실험 Todo로 바꾼다.
실험까지 끝났다면 그때부터 실제 기술 자산이 된다.

강연 영상 공부의 목표는 영상을 많이 보는 것이 아니다.
목표는 다음 흐름을 만드는 것이다.

```text
강연 시청 → 핵심 정리 → 작은 실험 → 결과 기록 → 프로젝트 적용 판단
```
