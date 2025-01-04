### 주요 설정

| **설명**                   | **조건**                                                                                                                                         | **입력**                        | **출력**                                           |
|----------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------|--------------------------------------------------|
| **Right Control**           | 없음                                                                                                                                             | `right_control`                 | - 혼자 눌렀을 때: `delete_forward`               |
| **Left Shift**              | `com.microsoft.rdc.macos`가 활성화되지 않은 경우                                                                                                | `left_shift`                    | - 혼자 눌렀을 때: `im-select`로 Colemak 레이아웃 전환 |
| **Right Shift**             | `com.microsoft.rdc.macos`가 활성화되지 않은 경우                                                                                                | `right_shift`                   | - 혼자 눌렀을 때: `im-select`로 한글 레이아웃 전환   |
| **Right Command**           | `com.microsoft.rdc.macos`가 활성화되지 않은 경우                                                                                                | `right_command`                 | - 혼자 눌렀을 때: `/Users/song/.config/karabiner/im-select-toggle` |
| **Caps Lock**               | 없음                                                                                                                                             | `caps_lock`                     | - 혼자 눌렀을 때: `escape`<br> - 키 누름 상태 저장: `is_caps_lock_down` 변수 설정 |
| **Left Command**            | `com.microsoft.rdc.macos`가 활성화된 경우                                                                                                        | `left_command`                  | `left_option`                                   |
| **Left Option**             | `com.microsoft.rdc.macos`가 활성화된 경우                                                                                                        | `left_option`                   | `left_command`                                  |
| **Right Command**           | `com.microsoft.rdc.macos`가 활성화된 경우                                                                                                        | `right_command`                 | `right_option`                                  |
| **Right Option**            | `com.microsoft.rdc.macos`가 활성화된 경우                                                                                                        | `right_option`                  | `right_command`                                 |

### Caps Lock 조합 설정

| **설명**                 | **조건**                             | **입력**               | **출력**             |
|--------------------------|--------------------------------------|-----------------------|--------------------|
| **커서 이동**             | `is_caps_lock_down = 1`              | `j`                   | `left_arrow`       |
|                          |                                      | `k`                   | `down_arrow`       |
|                          |                                      | `i`                   | `up_arrow`         |
|                          |                                      | `l`                   | `right_arrow`      |
| **Delete/Backspace**      | `is_caps_lock_down = 1`              | `delete_or_backspace` | `delete_forward`   |
| **Home/End**              | `is_caps_lock_down = 1`              | `h`                   | `home`             |
|                          |                                      | `semicolon`           | `end`              |
| **스크롤**                | `is_caps_lock_down = 1`              | `e`                   | 위로 스크롤 (-64)   |
|                          |                                      | `d`                   | 아래로 스크롤 (64)  |
|                          |                                      | `s`                   | 오른쪽 스크롤 (64) |
|                          |                                      | `f`                   | 왼쪽 스크롤 (-64)  |
| **특정 애플리케이션 동작** | `is_caps_lock_down = 1` + Chrome 활성 | `/`                   | `Cmd + Shift + H`  |
|                          | `is_caps_lock_down = 1` + Firefox 활성 | `/`                   | `Option + Home`    |

### 디바이스 별 설정

| **디바이스**                     | **설명**                                                                                                                                     |
|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| **Apple Keyboard (Vendor ID: 1452, Product ID: 594)** | 키보드와 마우스 동시 입력 허용                                                                                                               |
| **Logitech Mouse (Vendor ID: 1133, Product ID: 45105)** | 마우스 수직 휠 방향 반전                                                                                                                     |
| **Apple Keyboard (Vendor ID: 1452, Product ID: 591)** | `escape` 키를 `~`로 맵핑                                                                                                                   |
