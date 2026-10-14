# DedicatedProject 소스 코드 사본

이 폴더는 게임 에셋을 제외하고 코드와 프로젝트 구조를 검토할 수 있도록 만든 `DedicatedProject` 사본입니다.

원본: `C:\Users\lsgls\Desktop\GitHub\DedicatedProject`

사본: `C:\Users\lsgls\Documents\GitHub\DedicatedProject_DelAsset`

## 포함한 내용

- `Source`: 게임 C++ 소스 및 헤더, Unreal 빌드·타깃 설정.
- `Config`: 프로젝트 기본 설정 파일.
- `DedicatedProject.uproject`: 프로젝트 및 엔진 플러그인 참조 정보.
- `.github`: Issue·Pull Request 문서 템플릿.
- `README.md`, `.gitattributes`, `.gitignore`.
- `DedicatedProject-Sequence-Diagrams.drawio`: 이미지 삽입 흔적이 없는 시퀀스 다이어그램 XML.

게임 소스는 원본의 바이트를 유지했습니다. 공개 사본의 Config/DefaultEngine.ini에서 Android 파일 서버 SecurityToken 값은 비웠습니다. `.gitignore`에는 에셋 및 외부 패키지의 재추가를 방지하기 위한 제외 규칙을 추가했습니다. 원본 파일은 수정하지 않았습니다.

## 제외한 내용

- `Content` 전체. 자체 제작 여부와 관계없이 Blueprint, 맵, DataTable을 포함한 모든 Unreal 에셋을 제외했습니다.
- `Fab`, `ParagonCrunch`, `ParagonWraith`, `Sci_Fi_Laboratory`, `StarterContent` 등 `Content` 내부의 외부 에셋 및 리소스 폴더.
- 루트의 `PolarFacility_UE51.png`를 비롯한 이미지, 모델, 사운드, 영상, 폰트 및 바이너리 파일.
- `Build`, `Binaries`, `DerivedDataCache`, `Intermediate`, `Saved`, `.vs`와 생성된 `.sln`, `.vsconfig`.
- `.git` 전체. 과거 커밋이나 Git LFS 저장소에 들어 있는 에셋이 사본에 따라오지 않도록 이력을 포함하지 않았습니다.
- 외부 `Plugins`, `ThirdParty`, `Vendor`, `External` 패키지. 원본 루트에서 별도 플러그인 패키지 폴더는 확인되지 않았습니다.

## 사용 범위와 확인 사항

에셋을 제외했으므로 이 사본만으로 원래 게임을 실행하거나 패키징할 수 없습니다. 코드와 설정에 남아 있는 `/Game/...` 등의 에셋 경로, 클래스명, `OnlineSubsystemSteam` 등 플러그인 참조는 해당 에셋이나 플러그인의 파일을 포함한다는 의미가 아닙니다.

Unreal 템플릿에서 생성된 소스의 기존 저작권 표시는 그대로 유지했습니다. 이 작업은 파일 유형과 디렉터리 구조를 기준으로 에셋 및 외부 패키지를 배제한 작업이며, 모든 소스 코드의 최초 작성자나 재배포 권한을 판정한 결과는 아닙니다.

`COPY_MANIFEST.csv`에는 복사한 원본 파일의 상대 경로, 크기, SHA-256 및 복사 직후 일치 확인 결과가 기록되어 있습니다. 해시는 공개 준비를 마친 사본의 현재 파일 기준입니다. `.gitignore`에는 에셋 제외 규칙을 추가했고 `Config/DefaultEngine.ini`의 `SecurityToken` 값은 비웠으므로 두 파일의 `CopyMatchesOriginal`은 False입니다. 원본 파일의 SHA-256은 `SourceSHA256`에 보존했습니다. 원본 파일의 해시와 최종 수정 시간이 복사 전후 동일한지도 확인했습니다.
