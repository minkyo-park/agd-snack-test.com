# 아고다 할인코드 사이트

아고다 할인코드 정보 사이트 - GitHub Pages 배포용

## 사이트 구조

```
agoda-discount/
├── index.html              # 메인 페이지
├── discount-codes.html     # 할인코드 종류 총정리
├── how-to-use.html         # 할인코드 적용 방법
├── troubleshoot.html       # 오류 해결 가이드
├── card-promotions.html    # 카드사 할인 총정리
├── easy-pay.html           # 카카오페이·네이버페이
├── flights.html            # 항공권 할인
├── domestic.html           # 국내 숙소 할인
├── japan.html              # 일본 호텔 할인
├── southeast-asia.html     # 동남아 할인
├── europe.html             # 유럽 할인
├── vip.html                # VIP 혜택
├── promotions.html         # 프로모션
├── tips.html               # 할인 극대화 꿀팁
├── cancel-refund.html      # 취소·환불 가이드
├── faq.html                # FAQ
├── sitemap.xml             # 검색엔진 사이트맵
├── robots.txt              # 검색엔진 크롤링 설정
├── css/
│   └── style.css           # 공통 스타일시트
├── js/
│   ├── main.js             # 공통 JavaScript
│   └── components.js       # 헤더/푸터 컴포넌트
└── images/                 # 이미지 파일 (66개)
```

## GitHub Pages 배포 방법

### 방법 1: GitHub 웹사이트에서 직접 업로드

1. GitHub에서 새 저장소(repository) 생성
   - 저장소 이름: `agoda-discount` (또는 원하는 이름)
   - Public으로 설정
   
2. 이 폴더의 모든 파일을 저장소에 업로드
   - "Add file" > "Upload files" 클릭
   - 모든 파일과 폴더를 드래그 앤 드롭
   
3. GitHub Pages 활성화
   - 저장소 Settings > Pages
   - Source: "Deploy from a branch"
   - Branch: main, / (root)
   - Save 클릭
   
4. 배포 완료 후 URL 확인
   - `https://[사용자명].github.io/agoda-discount/`

### 방법 2: Git 명령어로 배포

```bash
git init
git add .
git commit -m "Initial commit: 아고다 할인코드 사이트"
git remote add origin https://github.com/[사용자명]/agoda-discount.git
git push -u origin main
```

## 어필리에이트 링크 설정 방법

각 HTML 파일에서 `href="#"` 또는 `href="#affiliate-link"`로 되어있는 링크를 실제 어필리에이트 링크로 교체하세요.

예시:
```html
<!-- 변경 전 -->
<a href="#" class="btn btn-primary">🔗 할인코드 적용하고 예약하기</a>

<!-- 변경 후 -->
<a href="https://www.agoda.com/[어필리에이트코드]" class="btn btn-primary">🔗 할인코드 적용하고 예약하기</a>
```

## sitemap.xml 도메인 업데이트

`sitemap.xml` 파일에서 `https://yourdomain.github.io/agoda-discount/`를 실제 배포 URL로 변경하세요.

## robots.txt 도메인 업데이트

`robots.txt` 파일에서 `Sitemap:` URL을 실제 배포 URL로 변경하세요.
