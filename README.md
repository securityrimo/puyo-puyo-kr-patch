# 뿌요뿌요 시리즈 한글 번역 프로젝트

컴파일사의 대표작 뿌요뿌요(ぷよぷよ) 시리즈의 한글 번역 패치를 배포하는 프로젝트입니다.

Claude Code를 활용하여 리버싱/번역하고, 사람이 기초 검수를 진행한 프로젝트입니다.

더 많은 게임의 번역에 대한 기여를 위해, 모든 패치에 사용된 코드는 기기별로 공개됩니다.

> 자매 프로젝트 - [마도물어 시리즈 한글 번역 프로젝트](https://github.com/mcpads/madou-monogatari-kr-patch)

## 뿌요뿌욘 (드림캐스트)

드림캐스트 **뿌요뿌욘 (ぷよぷよ~ん, Puyo Puyo 4)** 한글 번역 패치입니다.

참고: [뿌요뿌욘 - 나무위키](https://namu.wiki/w/%EB%BF%8C%EC%9A%94%EB%BF%8C%EC%9A%98)

![dc-puyo-puyo-screenshot-1](/img/dc-puyo-puyo-screenshot-1.png)

![dc-puyo-puyo-screenshot-2](/img/dc-puyo-puyo-screenshot-2.png)

![dc-puyo-puyo-screenshot-3](/img/dc-puyo-puyo-screenshot-3.png)

### 적용 방법

1. **일본판 원본 GDI ROM**을 준비합니다
2. [Puyo Puyo 4 (Dreamcast) KR v0.2.0.dcp](https://raw.githubusercontent.com/mcpads/puyo-puyo-kr-patch/main/Puyo%20Puyo%204%20(Dreamcast)%20KR%20v0.2.0.dcp)를 다운로드합니다
3. [Universal Dreamcast Patcher](https://github.com/DerekPascarella/UniversalDreamcastPatcher)로 원본 GDI에 DCP 패치를 적용합니다

### 체크섬

#### 원본 ROM (GDI, 27트랙)

데이터 트랙 체크섬:

**track03.bin** (메인 데이터)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `a0fadb90f60aae1b5b5cd1d9ceffb018`                                 |
| SHA-1    | `6e5515fcc8e35e0c45083e9de9b9880d6c918420`                         |
| SHA-256  | `50f6f59f5a53a72e13bda9631d2ed86f31a1ac02907bd3e480e5d99c3fa16af9` |
| 크기     | 278,413,296 bytes                                                  |

**track27.bin** (파일 데이터)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `95694f7b0957660c165ef8b6b25fd579`                                 |
| SHA-1    | `27ee0d7ac17a917f5b0287c5d70ac7721e215ced`                         |
| SHA-256  | `fdcece61e384e865bcc1d5ee5af812b021bafb30009ebe35ba87a6b925e767ce` |
| 크기     | 205,661,232 bytes                                                  |

**track01.bin** (IP.BIN)

| 알고리즘 | 해시                                                               |
| -------- | ------------------------------------------------------------------ |
| MD5      | `6ef4f836257a40ef0d7480946d6f9bc4`                                 |
| SHA-1    | `40de748625a511e321d05f6f0feee0427a90924f`                         |
| SHA-256  | `ae8b5cad18af0670d811dffe978d0c608c52f80e46fb8249766abc21a3a5e5ff` |
| 크기     | 1,157,184 bytes                                                    |

### 수정 중인 문제

- **스케토우다라 만담**: 중간에 스케토우다라 캐릭터 포트레이트가 깨지는 현상이 있습니다 (게임 진행에는 영향 없음)
- **루루 만담**: 중간에 치코 캐릭터 포트레이트가 깨지는 현상이 있습니다 (게임 진행에는 영향 없음)
- 일부 대사의 대사창 크기/위치가 최적화되지 않은 부분이 있을 수 있습니다
- 현재 실기 동작 확인 중입니다 (스토리 모드 동작에 문제가 있다는 사례가 존재)

### 패치 정보

- 한글 폰트: [Maplestory Light/Bold](https://maplestory.nexon.com/Media/Font), [BMJUA](http://font.woowahan.com/jua/)
- [패쳐 코드베이스](https://github.com/mcpads/dc-puyo-puyon-kr-patcher)

### 크레딧

- **패치 제작자**: mcpads
- **리버싱**: mcpads (with Claude Code)
- **한글 번역**: Claude Code (Opus 4.6) 및 Codex (GPT 5.4)
- **이미지 번역**: Gemini Nano Banana 2
- **QA**: mcpads
- **원작**: Sega / Compile (1999)

---

## 번역 예정 작품

### 슈퍼 나조 뿌요 1 (SNES)

SFC **슈퍼 퍼즐뿌요 1 (す～ぱ～なぞぷよ ルルーのルー)** 한글 번역 패치 작업입니다. 진행 중입니다.

참고: [슈퍼 퍼즐뿌요 - 나무위키](https://namu.wiki/w/%ED%8D%BC%EC%A6%90%EB%BF%8C%EC%9A%94%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-6)

![sfc-nzao-puyo-screenshot-1](/img/sfc-nazo-puyo-screenshot-1.png)

- [x] 일본어 폰트 추출 및 테이블 완성
- [x] 시나리오 텍스트 추출
- [x] 시나리오 및 이벤트 대사 번역
- [x] 한글 폰트 통합 및 적용
- [ ] 시스템 UI
- [ ] 시스템 안정성
- [ ] 플레이 테스트 및 최종 검수

### 슈퍼 나조 뿌요 2 (SNES)

SFC **슈퍼 퍼즐뿌요 2 (すーぱーなぞぷよ通 ルルーの鉄腕繁盛記)** 한글 번역 패치 작업입니다. 진행 중입니다.

참고: [슈퍼 퍼즐뿌요 - 나무위키](https://namu.wiki/w/%ED%8D%BC%EC%A6%90%EB%BF%8C%EC%9A%94%20%EC%8B%9C%EB%A6%AC%EC%A6%88#s-6)

![sfc-nzao-puyo2-screenshot-1](/img/sfc-nazo-puyo2-screenshot-1.png)

![sfc-nzao-puyo2-screenshot-2](/img/sfc-nazo-puyo2-screenshot-2.png)

- [x] 일본어 폰트 추출 및 테이블 완성
- [x] 시나리오 텍스트 추출
- [x] 시나리오 및 이벤트 대사 번역
- [x] 한글 폰트 통합 및 적용
- [ ] 시스템 UI
- [ ] 시스템 안정성
- [ ] 플레이 테스트 및 최종 검수

## 이슈 제보 및 피드백

어색한 번역, 번역 오타, 심각한 그래픽 깨짐, 게임 멈춤 등의 문제는 아래 방법으로 제보해 주세요.

- **GitHub Issue**: [이슈 트래커 링크](https://github.com/mcpads/puyo-puyo-kr-patch/issues)에 새 이슈를 등록해 주세요.
- **제보 시 포함할 내용**:
  - 문제가 발생한 위치 (예: 아르르 스토리 3번째 만담)
  - 문제 현상 (예: 대사가 대사창 밖으로 넘침)
  - 사용 중인 에뮬레이터 및 버전
  - (가능하다면) 스크린샷

## 업데이트 기록

| 버전   | 날짜       | 대상                  | 내용                                                    |
| ------ | ---------- | --------------------- | ------------------------------------------------------- |
| v0.1.0 | 2026-03-28 | 뿌요뿌욘 (드림캐스트) | 베타 배포                                               |
| v0.2.0 | 2026-03-29 | 뿌요뿌욘 (드림캐스트) | 룰 설명 번역, 오프닝 자막 2번째부터 안나오는 문제 수정, 대사 타이밍 조정 |

## 라이선스

- 본 패치 파일은 개인적, 비상업적 용도로 제공됩니다. 원작 게임의 저작권은 해당 권리자에게 있습니다.
- 본 한글패치 파일 자체를 제작자에 허가없이 타 사이트에 재배포하지 말아 주시고, 재배포를 원하실 경우 패치원본 게시물의 링크를 공유해 주시기 바랍니다.
- 본 한글패치 파일을 이용하여 금전적 이득을 취하는 모든 행위를 일절 금합니다. 해당 행위로 발생하는 모든 책임은 이용 당사자에게 있으며, 패치 제작자는 어떠한 책임도 지지 않습니다.
