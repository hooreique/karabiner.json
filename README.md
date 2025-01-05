### 주요 설정: 키 리매핑 및 조건
| **설명**                     | **입력 키**               | **출력 키/명령**                                       | **조건**                                                                                       |
|-------------------------------|---------------------------|-------------------------------------------------------|-----------------------------------------------------------------------------------------------|
| `right_control` 리매핑        | `right_control`           | `right_control`                                       | 단독 입력 시 `delete_forward`                                                                 |
| `left_shift` 리매핑           | `left_shift`              | `left_shift`                                          | 단독 입력 시 `im-select`로 Colemak 키보드 레이아웃 전환 (RDC 앱 제외)                          |
| `right_shift` 리매핑          | `right_shift`             | `right_shift`                                         | 단독 입력 시 `im-select`로 한글 3벌식 전환 (RDC 앱 제외)                                       |
| `right_command` 리매핑        | `right_command`           | `right_command`                                       | 단독 입력 시 사용자 정의 `im-select-toggle` 실행 (RDC 앱 제외)                                 |
| `caps_lock` 리매핑            | `caps_lock`               | `escape` (단독 입력 시) / CapsLock 키 눌림 상태 변수 설정 |                                                                                               |
| `left_command` ↔ `left_option`| `left_command`            | `left_option`                                         | RDC 앱 활성화 시                                                                               |
| `right_command` ↔ `right_option`| `right_command`           | `right_option`                                        | RDC 앱 활성화 시                                                                               |

### CapsLock + 조합 키 리매핑
| **조합 키**        | **출력 키/명령**      |
|---------------------|-----------------------|
| `CapsLock + J`      | `←` (Left Arrow)     |
| `CapsLock + K`      | `↓` (Down Arrow)     |
| `CapsLock + I`      | `↑` (Up Arrow)       |
| `CapsLock + L`      | `→` (Right Arrow)    |
| `CapsLock + H`      | `Home`               |
| `CapsLock + ;`      | `End`                |
| `CapsLock + E`      | 화면 위로 스크롤 (마우스 휠 -64) |
| `CapsLock + D`      | 화면 아래로 스크롤 (마우스 휠 64) |
| `CapsLock + S`      | 오른쪽으로 스크롤 (마우스 휠 64) |
| `CapsLock + F`      | 왼쪽으로 스크롤 (마우스 휠 -64) |

### CapsLock + 숫자 키 -> Function Key
| **CapsLock + 숫자 키** | **출력 키** |
|-------------------------|-------------|
| `CapsLock + 1`         | `F1`        |
| `CapsLock + 2`         | `F2`        |
| `CapsLock + 3`         | `F3`        |
| `CapsLock + 4`         | `F4`        |
| `CapsLock + 5`         | `F5`        |
| `CapsLock + 6`         | `F6`        |
| `CapsLock + 7`         | `F7`        |
| `CapsLock + 8`         | `F8`        |
| `CapsLock + 9`         | `F9`        |
| `CapsLock + 0`         | `F10`       |
| `CapsLock + -`         | `F11`       |
| `CapsLock + =`         | `F12`       |

### 특정 디바이스 설정
| **디바이스**       | **설정**                                                                                  |
|--------------------|-------------------------------------------------------------------------------------------|
| 키보드 (Vendor: 1452, Product: 594) | 기본값                                                                                 |
| 마우스 (Vendor: 1133, Product: 45105) | 마우스 세로 휠 반전                                                                    |
| 키보드 (Vendor: 1452, Product: 591) | `escape` 키를 `~ (틸드)`로 리매핑                                                      |
