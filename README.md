# LBC Lab 홈페이지 — GitHub Pages 배포 안내

Wix 사이트(supia0525.wixsite.com/yunju)를 정적 HTML로 옮긴 버전입니다.
GitHub Pages에 무료로 호스팅하고 lbclab.hanyang.ac.kr 도메인을 연결할 수 있습니다.

## 1. 이미지·파일 준비 (배포 전 필수)

아래 파일들을 기존 Wix 사이트에서 저장해 지정된 이름으로 폴더에 넣어주세요.
(브라우저에서 이미지 우클릭 → "이미지를 다른 이름으로 저장")

### images/ 폴더
| 저장할 파일명 | 원본 (Wix 사이트 위치) |
|---|---|
| yunju-nam.jpg | About Us — PI 프로필 사진 |
| member-gun-kim.jpg | About Us — Gun Kim |
| member-sumin-cho.jpg | About Us — Sumin Cho |
| member-gaun-im.jpg | About Us — Gaun Im |
| member-hyunjeong-lim.jpg | About Us — Hyunjeong Lim |
| poster-2023-hsp.jpg | Conferences — 2023 HSP 포스터 |
| poster-2019-cogsci.jpg | Conferences — 2019 Cognitive Science 포스터 |
| poster-2019-ecem.jpg | Conferences — 2019 ECEM 포스터 |
| poster-2018-cuny.jpg | Conferences — 2018 CUNY 포스터 |
| event-2025-psycholing.jpg | Events — 2025 심리언어학회 표지 |
| event-2023-colloquium.png | Events — 콜로키움 포스터 |

### files/ 폴더
| 저장할 파일명 | 원본 |
|---|---|
| cv-yunju-nam.pdf | About Us — CV (docx라면 PDF로 변환 권장) |
| ai-speaker-dataset.xlsx | Publications — AI speaker Data set |
| 2025-proceedings.pdf | Events — 2025 학술대회 Proceedings |
| 2023-colloquium-materials.pdf | Events — 콜로키움 Materials |

이미지가 아직 없어도 사이트는 열립니다(해당 자리만 비어 보임).

## 2. GitHub Pages 배포

1. github.com 에서 계정 생성 후 새 저장소(repository) 생성 — 예: `lbclab-website`, Public
2. 이 폴더의 전체 파일을 저장소에 업로드 (웹에서 "Add file → Upload files"로 드래그하면 됩니다)
3. 저장소 Settings → Pages → Branch를 `main`, 폴더 `/ (root)`로 설정 → Save
4. 몇 분 후 `https://계정명.github.io/lbclab-website/` 에서 사이트 확인

## 3. 한양대 도메인 연결

1. 저장소 Settings → Pages → Custom domain에 `lbclab.hanyang.ac.kr` 입력 → Save
   (이 폴더의 CNAME 파일이 같은 역할을 하므로 이미 준비되어 있습니다)
2. 한양대 도메인 신청서의 CNAME 레코드 값에 **`계정명.github.io`** 입력
   (예: GitHub 계정이 `lbclab`이면 `lbclab.github.io` — 저장소 이름은 붙이지 않습니다)
3. 학교 승인 및 DNS 반영(최대 48시간) 후 Settings → Pages에서
   "Enforce HTTPS" 체크 → https://lbclab.hanyang.ac.kr 로 접속 가능

## 4. 이후 수정 방법

HTML 파일을 직접 수정해 저장소에 다시 업로드하면 몇 분 내 반영됩니다.
논문 추가 등 수정이 필요할 때 Claude에게 파일을 주고 요청하시면 됩니다.
