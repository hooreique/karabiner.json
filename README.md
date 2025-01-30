개인 Karabiner-Elements 구성입니다.
지극히 개인적인 구성이기 때문에 자세히 설명하지 않습니다.
미래의 나를 위해 작성했습니다.

## Prerequisites

- 설정 > 키보드 > 키보드 단축키... > 입력 소스 > 이전 입력 소스 선택: F19
- 설정 > 키보드 > 키보드 단축키... > 입력 소스 > 입력 메뉴에서 다음 소스 선택: F18
- 입력 소스
  - ABC, Colemak 등 `"language": "en"` 인 입력 소스가 적어도 하나 있을 것
  - 두벌식, 세벌식 등 `"language": "en"` 이 아닌 입력 소스가 적어도 하나 있을 것

## Input Source Stuff

Left Shift 는 항상 en 으로,
Right Shift 는 항상 non-en 으로 가도록 함

이때 주의할 점은 직전에 사용한 레이아웃을 반대 쪽으로 항상 유지해야 한다는 것.
그렇게 하고 싶지 않았으나 스크립트를 실행하는 방식으로는 반응이 느린 문제가 있어서 Ad-hoc 한 것임.
다시 말해, 평소에 en 과 non-en 단 두 개의 입력 소스만 사용한다는 가정을 함.

Windows + 날개셋 구성이 그리운 지점이다.

## MS RDC Stuff

원격으로 Windows PC 를 다룰 때 모든 키매핑을 원격 PC 에 위임하기 위해
ms_rdc, vkey, input_source, misc 룰에 조건을 적절히 설정함.
모든 나머지 룰은 vkey 룰에 의존함.

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
