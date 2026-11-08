# GitHub Pages 첫 배포 안내

배포할 사이트: **눈길 — 우리의 일본 스키여행**

- 저장소 이름: `japan-ski-trip`
- 배포 방식: `main` 브랜치의 `/(root)` 폴더
- 구성: HTML 한 파일, 사진 내장, 별도 빌드 없음
- 저장소: [kanghuij-hash/japan-ski-trip](https://github.com/kanghuij-hash/japan-ski-trip)

## 1. GitHub 계정 만들기

[GitHub 가입](https://github.com/signup)에서 사용자 이름, 이메일, 비밀번호를 등록하고 이메일 인증을 완료하세요. 비밀번호와 인증 코드는 이 채팅에 보내지 않아도 됩니다.

계정을 준비한 뒤 저장소 생성과 업로드를 진행합니다. GitHub 연동을 사용한다면 가입한 계정으로 연결합니다.

## 2. 프로젝트 저장소 만들기

로그인 후 [새 저장소 만들기](https://github.com/new)에서 다음처럼 설정합니다.

| 항목 | 설정 |
|---|---|
| Owner | 본인의 계정 |
| Repository name | `japan-ski-trip` |
| Description | 일본 스키여행 지역 후보 비교 페이지 |
| Visibility | Public |
| README 자동 생성 | 해제 — 준비한 README를 업로드합니다. |

무료 GitHub Pages를 쓰는 이 계획에서는 저장소와 사이트가 공개됩니다. 배포용 폴더에는 여행 페이지와 출처·안내 파일만 포함되어 있습니다.

## 3. 완성된 파일 올리기

처음에는 GitHub 웹사이트에서 파일을 업로드하면 됩니다. 터미널 명령어를 입력할 필요는 없습니다.

1. 새 저장소의 **uploading an existing file** 링크 또는 **Add file → Upload files**를 선택합니다.
2. 배포 준비 ZIP을 압축 해제한 뒤 아래 파일들을 저장소의 가장 바깥에 올립니다.
   - `index.html`: 사이트 본문과 지역별 실제 사진
   - `PHOTO-CREDITS.md`: 사진 저작자·출처·라이선스
   - `README.md`: 프로젝트 설명
   - `.nojekyll`: 정적 파일을 그대로 배포하는 설정
   - `.gitignore`, `.gitattributes`, `DEPLOY.md`: 함께 업로드해도 되는 관리·안내 파일
3. **Commit changes**를 눌러 저장합니다. 저장할 브랜치는 `main`입니다.

`index.html`을 `japan-ski/`라는 하위 폴더 안에 올리지 않도록 주의하세요. 저장소 첫 화면의 파일 목록에 `index.html`이 바로 보여야 합니다.

원본 MD, 작업용 스크립트, 미리보기 스크린샷, `.git` 폴더는 업로드할 필요가 없습니다. 준비한 ZIP에는 이 항목들이 포함되어 있지 않습니다.

## 4. 홈페이지 주소 발급하기

1. 저장소에서 **Settings → Pages**를 엽니다.
2. **Build and deployment → Source**에서 **Deploy from a branch**를 선택합니다.
3. **Branch**는 `main`, 폴더는 **/(root)**로 설정합니다.
4. **Save**를 누릅니다.
5. 배포가 끝나면 Pages 화면에서 실제 발급된 주소를 확인합니다.

일반적인 주소 형식은 `https://사용자이름.github.io/japan-ski-trip/`입니다. 실제 Pages 화면에 표시된 주소를 사용합니다. 별도 도메인 구매는 필요하지 않습니다.

## 5. 톡방 공유 전 확인하기

- 실제 휴대폰과 카카오톡 내장 브라우저에서 첫 화면과 지역 사진이 보이는지
- 스키장 상세 정보와 비교함이 열리는지
- 후보 문구 복사에 배포된 페이지 주소가 포함되는지
- 사진 출처와 공식 자료 링크가 열리는지

톡방 안내 문구 예:

> 일본 스키여행 후보 정리했어요 ⛷️
> 링크에서 지역별 가격·이동·스키장을 비교해 보고, 마음에 드는 지역을 골라주세요.
> 투표는 톡방에서 진행할게요!
> [발급된 홈페이지 주소]

## 이후 수정할 때

수정한 `index.html`을 같은 저장소·같은 위치에 다시 올리고 **Commit changes**를 누르면 설정한 배포 경로로 반영됩니다. 사진 라이선스나 원본 출처가 바뀌면 PHOTO-CREDITS.md와 페이지 내부 출처도 함께 수정합니다.

## Git 용어 세 가지만

- **Repository(저장소)**: 프로젝트 파일과 변경 기록을 모아두는 곳
- **Commit**: 변경한 파일을 한 번의 기록으로 저장하기
- **Push**: 로컬 컴퓨터의 기록을 GitHub에 올리기 — 웹사이트 업로드에서는 직접 입력하지 않아도 됩니다.

로컬 Git으로 수정할 때는 이 저장소를 복제한 폴더에서 작업하고, 본인의 Git 작성자 정보를 설정한 뒤 commit과 push를 진행합니다. 웹 업로드 방식과 로컬 Git 방식 모두 같은 저장소를 갱신합니다.

공식 문서: [GitHub Pages 소개](https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages), [배포 브랜치 설정](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site)
