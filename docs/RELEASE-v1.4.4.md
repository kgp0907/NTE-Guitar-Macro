# NTE Guitar v1.4.4 · 첫 실행 설정 저장 오류 수정

빈 폴더에서 공유곡 또는 MIDI를 처음 추가한 뒤 다시 실행하면 단축키 설정과 정상 백업이 없다는 경고가 뜨던 문제를 수정했습니다. 첫 실행 때 설정이 메모리에만 있고 파일로 저장되지 않았던 것이 원인이었습니다.

- 첫 실행 시 설정 파일과 정상 백업을 생성합니다.
- 공유곡·MIDI 추가 후 재실행과 단축키 지정 후 재실행 검사를 추가했습니다.
- 실제 설정 손상 복구와 기존 곡·설정 보호는 유지합니다.

## 다운로드

- **기존 사용자:** [업데이트 ZIP](https://github.com/kgp0907/NTE-Guitar-Macro/releases/download/v1.4.4/NTE-Guitar-v1.4.4-Update-Windows.zip)
- **처음 설치:** [신규 설치 ZIP · 기본 29곡 포함](https://github.com/kgp0907/NTE-Guitar-Macro/releases/download/v1.4.4/NTE-Guitar-v1.4.4-Windows.zip)

기존 사용자는 프로그램을 완전히 종료하고 폴더를 백업한 다음 업데이트 ZIP을 기존 폴더에 병합하세요. 기존 곡·원본 MIDI·설정 파일을 삭제하지 마세요.

**이미 경고가 난 테스트 폴더는:** 이전 버전에서 설정 파일 자체를 만들지 못했을 수 있으므로, 수정본 적용 후 단축키 설정에서 사용할 키를 한 번 저장하세요. 곡 파일은 유지됩니다. 수정본이 과거 단축키를 임의로 추측해 덮어쓰지는 않습니다.

소스·EXE 각각 9종 검사와 기존 사용자 파일 18종 보존 검사를 통과했습니다. 실제 게임 입력·청음은 별도 확인 대상입니다. 자세한 결과는 첨부 문서와 VALIDATION-v1.4.4.json에 있습니다.

[v1.4.3](https://github.com/kgp0907/NTE-Guitar-Macro/releases/tag/v1.4.3)과 [v1.0](https://github.com/kgp0907/NTE-Guitar-Macro/releases/tag/v1.0) 다운로드도 유지합니다.

## English

Fixes missing initial shortcut settings after adding a first shared song or MIDI arrangement in an empty folder and restarting. Initial settings and a valid backup are now saved on first launch. Existing songs and settings remain protected. Use Update-Windows.zip for an existing installation and Windows.zip for a fresh installation. A folder already affected by the old bug may need one explicit shortcut save. Previous releases remain available.
