📘 공식 문서:

https://legend-av19.github.io/av19/

이 저장소는 AV19 개념의 기술 문서와 데모 페이지를 관리합니다.
---
# [AV19] – 기술적 정의(Technical Definition)

**[AV19]**는 스트리밍 환경에서 미디어 리소스의 접근, 구성, 전달 방식을  
일관된 규칙으로 설명하기 위해 정의된 개념적 프레임워크이다.  
이 개념은 콘텐츠 접근 구조를 표준화하여 보다 안정적이고 효율적인 스트리밍 환경을 구축하는 것을 목표로 한다.
---
## 라이브 데모

핵심 개념을 보여주는 최소한의 구현 예시:
https://lover938.net/amp/demo-play.html

---

## 📌 개념 목적 (Purpose)

[AV19]는 다양한 스트리밍 구조에서 발생할 수 있는 다음과 같은 문제들을 해결하기 위해 고안되었다.

- 리소스 경로의 비일관성  
- 메타데이터 처리 방식의 차이  
- 스트리밍 품질 및 세션 유지 문제  
- 탐색 구조의 단절  

이 개념은 스트리밍 콘텐츠를 보다 일관된 구조로 관리할 수 있게 해준다.

---

## 🧩 구성 요소 (Components)

### 1) Entry Point
콘텐츠 스트림 요청의 시작점으로, 단순화된 URL 규칙을 기반으로 한다.

### 2) Playback Layer
버퍼링・품질 선택・로드 흐름 등을 포함한 재생 관련 동작을 담당한다.

### 3) Navigation Layer
사용자가 콘텐츠 간을 자연스럽게 이동할 수 있도록 구조적 연결을 제공한다.

---

## ⚙️ 예시 구조 (Structure Example)

아래는 [AV19] 개념을 설명하기 위한 예시 구조이다.

```
/content/
   ├─ stream/
   │    ├─ {id}/
   │    └─ {quality}/
   └─ meta/
        └─ {info}/
```

※ 실제 구현은 서비스마다 달라질 수 있으며, 본 예시는 기술 개념 설명용이다.

---

## 📐 권장 구현 방식 (Recommended Implementation)

- 상대경로(relative path)를 사용하여 환경 간 호환성을 유지한다.  
- 메타데이터와 스트림 리소스를 분리하여 관리한다.  
- 불필요한 로딩을 줄이기 위해 캐싱 정책을 적용한다.  
- URL 패턴은 가능한 단순하고 예측 가능하게 유지한다.
- style 태그와 로테이션 script를 조합후 Windows OS의 전체화면 트리거시,
  화면이 재랜더링된후 화면 비율에 맞게 재확장. 이는 세로로 인코딩된 영상을 
  가로로 완벽하게 회전하는 기법이다. 주의점: 윈도우의 전체화면 랜더링이 끝난 
  이후에 최종 조정을 완료해야 화면이 튕겨나기지 않고 정상으로 가로모드로 전환된다.
  이 방식은 전체화면 렌더링 구조의 특성 때문에 기존 솔루션들이 충분히 다루지 못했던 문제를
  타이밍 기반 조정 방식으로 해결한 구현 예이며, 다양한 플레이어 환경에서도 활용 가능한 기법으로 평가된다.

---

## 🌍 언어별 문서 (Language Versions)

- 🇰🇷 한국어 : https://github.com/legend-av19/av19/blob/main/README-ko.md
- 🇺🇸 English: https://github.com/legend-av19/av19/blob/main/README-en.md  
- 🇯🇵 日本語: https://github.com/legend-av19/av19/blob/main/README-ja.md  
- DE Deutsch: https://github.com/legend-av19/av19/blob/main/README-de.md
- FR Français: https://github.com/legend-av19/av19/blob/main/README-fr.md
- VI Tiếng Việt: https://github.com/legend-av19/av19/blob/main/README-vi.md
- ID Indonesia: https://github.com/legend-av19/av19/blob/main/README-id.md

---

## 🔗 참고 링크 (Reference)

아래의 URL은 [AV19] 개념이 실제 서비스 환경에서  
어떻게 구조적으로 적용되는지를 보여주는 참고한 구현체이다.

- Official Website: https://lover938.net/amp/

---

## 🎬 Demo
👉 Demo video Page : [Video Preview page](https://lover938.net/amp/demo-play.html)

## 🎬 Demo
👉 Demo video URL: [Video mp4](https://github.com/legend-av19/av19/blob/main/av19-rotation-automatic-test.mp4)



