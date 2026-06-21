개인 Karabiner-Elements 구성입니다.
지극히 개인적인 구성이기 때문에 자세히 설명하지 않습니다.
미래의 나를 위해 작성했습니다.

## Prerequisites

- Karabiner-Elements
- macism: `/opt/macism/bin/macism`
- 설정 > 키보드 > 키보드 단축키... > 입력 소스 > 이전 입력 소스 선택: F19
- 입력 소스
  - ABC: `com.apple.keylayout.ABC`
  - 구름 두벌식: `org.youknowone.inputmethod.Gureum.han2`
  - ABC, Colemak, hisle 등 `"language": "en"` 인 입력 소스가 적어도 하나 있을 것
  - 두벌식, 세벌식 등 `"language": "en"` 이 아닌 입력 소스가 적어도 하나 있을 것

## Input Source Stuff

Right Command 단독 탭으로 입력 소스를 직접 선택한다.

- 현재 입력 소스가 `"language": "en"` 이면 구름 두벌식으로 전환한다.
- 현재 입력 소스가 `"language": "en"` 이 아니면 ABC로 전환한다.

Left Shift / Right Shift 단독 탭은 Karabiner에서 입력 소스 전환으로 쓰지
않는다. hisle가 물리적인 왼쪽/오른쪽 Shift를 직접 받아서 로마자/한글
모드를 선택하기 때문이다.

Karabiner의 `"language": "en"` 조건은 hisle 내부의 로마자/한글 모드를
구분하지 못한다. hisle 전용 조건이 필요하면 language 조건이 아니라 input
source id 조건을 써야 한다.

Caps Lock 단독 탭은 en 입력 소스에서는 Escape만 내보내고, non-en 입력
소스에서는 Escape 뒤에 F19를 내보낸다.

## MS RDC Stuff

원격으로 Windows PC 를 다룰 때 모든 키매핑을 원격 PC 에 위임하기 위해
ms_rdc, vmod, input_source, misc 룰에 조건을 적절히 설정함.
모든 나머지 룰은 vmod 룰에 의존함.

### Keypad_1

원격 PC 역시 Capslock 기반으로 소프트 레이어링을 하기 때문에 그러한 키가 전달되어야 하지만
순수 Capslock 행동이 macOS 에서 MS RDC 로 그대로 전달되지 않기 때문에
사용하지 않는 임의의 키(Keypad_1)를 그러한 키로 활용한다는 가정을 함.

## etc (UHK60v2 Stuff)

한 쪽 Spacebar 는 그냥 Spacebar, 다른 쪽 Spacebar 는 Keypad_0 로 구성해둔다는 가정을 함.

마찬가지로 Fn 키는 F20 으로 구성해둔다는 가정을 함.

### Keypad_0

| Tap      | Hold      |
| ---      | ---       |
| Spacebar | 2nd Layer |

### F20

애플 내장 fn 키로 단순 매핑
