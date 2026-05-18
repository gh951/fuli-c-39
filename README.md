# 🛡️ CGo-Fuli-Scalp-DB

CGO-FULI C-39 두피 케어 모듈의 **Few-shot Learning 골드 데이터셋**

## 📋 구조

```
CGo-Fuli-Scalp-DB/
├── metadata.json          ← 메인 인덱스 (필수)
├── examples/              ← Few-shot 예시 (10-50장)
│   ├── basp-o0-normal.jpeg
│   ├── basp-m1-mild.jpeg
│   ├── basp-m2-mid.jpeg
│   ├── basp-v1-vertex.jpeg
│   ├── basp-v2-vertex-mid.jpeg
│   └── tongue-bai-thick.jpeg
├── golden-1000/           ← 골드 데이터셋 (점진 확장)
│   ├── normal/            (200장)
│   ├── m-shape/           (200장)
│   ├── vertex/            (200장)
│   ├── diffuse/           (200장)
│   └── tongue/            (200장)
└── README.md
```

## 🔗 사용

본진 `/api/vision-analyze.js`에서 자동 fetch:
```
https://gh951.github.io/CGo-Fuli-Scalp-DB/metadata.json
```

## 🏛️ 헌법

- **ZERO STORAGE**: 사용자 사진 절대 저장 X (이 DB는 예시 사진만)
- **무료 무한**: GitHub Pages 무료 호스팅
- **점진적 확장**: 0장 → 10장 → 1,000장 자동 정확도 상승

## 📊 진행 단계

| 단계 | 사진 수 | 예상 정확도 |
|---|---|---|
| Phase 0 | 0장 | Vision API 기본 |
| Phase 1 | 10장 | +30% |
| Phase 2 | 100장 | +60% |
| Phase 3 | 1,000장 | 룰루랩 80% 수준 ⭐ |

---

✦ Built by Lee Ju One × C-39 × Google AI × Claude ✦  
🛡️ CGO-FULI Constitution v2.0
