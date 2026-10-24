# NTE Guitar v1.4.3

기존 곡·설정을 보존하는 업데이트와 신규 설치용 파일을 함께 제공합니다. 이전 v1.0 릴리스와 다운로드는 유지합니다.

## 다운로드 선택

- **기존 사용자:** [NTE-Guitar-v1.4.3-Update-Windows.zip](https://github.com/kgp0907/NTE-Guitar-Macro/releases/download/v1.4.3/NTE-Guitar-v1.4.3-Update-Windows.zip)
- **신규 사용자:** [NTE-Guitar-v1.4.3-Windows.zip](https://github.com/kgp0907/NTE-Guitar-Macro/releases/download/v1.4.3/NTE-Guitar-v1.4.3-Windows.zip) — 기존 기본 29곡 포함
- **이전 버전:** [v1.0 릴리스](https://github.com/kgp0907/NTE-Guitar-Macro/releases/tag/v1.0)

기존 사용자는 프로그램을 완전히 종료하고 폴더를 백업한 뒤 업데이트 ZIP의 내용을 기존 폴더에 병합하세요. EXE와 `_internal`을 함께 교체하고 `songs`, `sources`, 설정 파일은 유지하세요. 기존 폴더를 삭제하거나 신규 설치용 기본 곡·설정을 덮어쓰지 마세요.

## 첫 배포 이후 주요 변경

- 허용된 공유곡 온라인 연주와 `.nteplay` 파일 추가·오프라인 단축키 연주. 원본 MIDI·편집용 파트 대신 최종 편곡 결과를 받습니다.
- 미니모드 재생/이어하기·일시정지·정지 버튼 분리. 일시정지는 위치를 유지하고, F8은 완전 정지입니다.
- 1.4.3: 상태 문구가 바뀌어도 세 버튼 크기와 위치가 움직이지 않도록 고정했습니다.
- 손상된 단축키 설정 복구, 중복 실행 잠금, 단축키 정렬, 공유창 미리 듣기·늦은 응답·중복 추가 처리 개선.

키 누름·연타 간격 보정과 짧은 처리 지연 회복은 v1.0의 Fix5에 이미 포함됐습니다. 이번 미니모드 수정에서 연주 엔진과 서버는 변경하지 않았습니다.

## 검증

소스·최종 EXE 각각 9종 검사, 네 언어 × 세 HUD 크기 배치, 최종 EXE와 소스 75개 모듈 일치, ZIP 무결성과 기존 사용자 파일 보존 검사를 통과했습니다. 실제 게임 입력·청음·디스플레이 DPI 변경은 자동 검사 범위에 포함하지 않습니다.

첨부된 `CHANGES-v1.4.3-KR.md`, `SHARED-SONGS-KR.md`, `VALIDATION-v1.4.3-KR.md`에서 자세한 내용을 확인하세요. `SHA256SUMS.txt`는 공개 첨부파일의 해시입니다. 실행에 Python은 필요하지 않습니다. GitHub의 자동 생성 Source code ZIP/TAR는 Windows 실행 배포본이 아닙니다.

## English

Choose **Update-Windows.zip** to keep an existing library and settings, or **Windows.zip** for a fresh installation with the same 29 default arrangements. Exit the player, back up the folder, and merge the update contents into the existing installation; keep your songs, sources and settings. v1.0 remains available.

This release adds permitted offline shared-song imports and a separate mini-player Pause button, with stable transport button widths in v1.4.3. Source and executable checks passed; actual in-game playback and audio still require user verification. Download the Windows asset rather than GitHub's automatic source archive.
