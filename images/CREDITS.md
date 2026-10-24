# 이미지 출처와 라이선스

## 표지와 배너

- `book-cover.png` — 뷰어 첫 화면에 쓰는 세로형 표지. 저자가 `git-wide.png`와 같은 계열로 직접 제공한 이미지로 교체됐다. 생성 경위와 라이선스는 이 저장소의 커밋 이력만으로는 확인할 수 없으니, 재배포 전에 저자에게 출처를 확인한다.
- `book-cover.svg` — 교체 전 처음 썼던 표지의 원본 소스. 지금은 쓰이지 않지만, 이 저장소를 위해 새로 만든 그래픽이라 저작권 문제가 없다는 점만 기록으로 남겨 둔다. 색상은 `.illust-gen/excalidraw-export/excal_lib.py`의 파스텔 팔레트를 그대로 썼다.
- `git-wide.png` — README 맨 위에 쓰는 가로형 배너(1440×576). 저자가 직접 제공한 파일이다. 생성 경위와 라이선스는 이 저장소의 커밋 이력만으로는 확인할 수 없으니, 재배포 전에 저자에게 출처를 확인한다.
- `timeline-2026h2.png`, `timeline-2026h2.svg` — [8부 2절](../part8/02-2026-second-half.md)에 쓰는 타임라인 그래픽. 이 저장소를 위해 새로 그린 그래픽이다. 저작권 문제가 없다.

## 인물 사진 (`people/`)

모두 위키미디어 커먼즈(Wikimedia Commons)에서 받았고, 커먼즈가 **퍼블릭 도메인(Public domain)**으로 표시한 것만 썼다. 저작권이 만료된 오래된 사진과 초상이라 사용에 제약이 없다.

| 파일 | 인물 | 원본 | 커먼즈 라이선스 |
|---|---|---|---|
| `riemann.jpg` | 베른하르트 리만 | [Georg Friedrich Bernhard Riemann.jpeg](https://commons.wikimedia.org/wiki/File:Georg_Friedrich_Bernhard_Riemann.jpeg) | Public domain |
| `poincare.jpg` | 앙리 푸앵카레 | [Henri Poincaré-2.jpg](https://commons.wikimedia.org/wiki/File:Henri_Poincar%C3%A9-2.jpg) | Public domain |
| `hilbert.jpg` | 다비트 힐베르트 | [David Hilbert, 1907.jpg](https://commons.wikimedia.org/wiki/File:David_Hilbert,_1907.jpg) | Public domain |
| `kepler.jpg` | 요하네스 케플러 | [Johannes Kepler1.jpg](https://commons.wikimedia.org/wiki/File:Johannes_Kepler1.jpg) | Public domain |
| `cantor.jpg` | 게오르크 칸토어 | [Georg Cantor3.jpg](https://commons.wikimedia.org/wiki/File:Georg_Cantor3.jpg) | Public domain |
| `godel.jpg` | 쿠르트 괴델 | [Kurt gödel.jpg](https://commons.wikimedia.org/wiki/File:Kurt_g%C3%B6del.jpg) | Public domain |
| `turing.jpg` | 앨런 튜링 | [Alan Turing (1951).jpg](https://commons.wikimedia.org/wiki/File:Alan_Turing_(1951).jpg) | Public domain |
| `einstein.jpg` | 알베르트 아인슈타인 | [Albert Einstein 1947.jpg](https://commons.wikimedia.org/wiki/File:Albert_Einstein_1947.jpg) | Public domain |
| `boltzmann.jpg` | 루트비히 볼츠만 | [Boltzmann2.jpg](https://commons.wikimedia.org/wiki/File:Boltzmann2.jpg) | Public domain |
| `darwin.jpg` | 찰스 다윈 | [Charles Darwin seated.jpg](https://commons.wikimedia.org/wiki/File:Charles_Darwin_seated.jpg) | Public domain |
| `descartes.jpg` | 르네 데카르트 (프란스 할스 作) | [Frans Hals - Portret van René Descartes.jpg](https://commons.wikimedia.org/wiki/File:Frans_Hals_-_Portret_van_Ren%C3%A9_Descartes.jpg) | Public domain |
| `hume.jpg` | 데이비드 흄 (앨런 램지 作) | [David Hume.jpg](https://commons.wikimedia.org/wiki/File:David_Hume.jpg) | Public domain |

원본 파일은 받은 그대로 두지 않고 웹에 싣기 좋게 가로와 세로 모두 360px 이하로 줄이고 JPEG 품질 85로 다시 저장했다. 원본 해상도가 필요하면 위 커먼즈 링크에서 받는다.

## 더 추가하려면

인물 사진을 더 넣고 싶으면, 커먼즈에서 검색한 뒤 다음으로 라이선스를 직접 확인하고 이 표에 한 줄을 추가한다.

```bash
curl -s "https://commons.wikimedia.org/w/api.php?action=query&titles=File:<파일명>&prop=imageinfo&iiprop=url|extmetadata&format=json" \
  | python3 -c "import json,sys; d=json.load(sys.stdin); p=list(d['query']['pages'].values())[0]['imageinfo'][0]; print(p['url']); print(p['extmetadata'].get('LicenseShortName',{}).get('value'))"
```

`LicenseShortName`이 `Public domain`이 아니면 쓰지 않는다. CC BY나 CC BY-SA 같은 저작자 표시 라이선스는 이 표에 저작자 이름까지 같이 적어야 한다.
