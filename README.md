# STM32 Nucleo-F446RE 연습 프로젝트 🔧

> 드론 자작 프로젝트를 위한 STM32 임베디드 개발 학습 저장소

## 프로젝트 목적

본 저장소는 [drone-DIY-STM32](../drone-DIY-STM32) 본 프로젝트에
앞서 STM32 개발 환경과 기본 기능을 학습하기 위한 연습 공간입니다.

Nucleo-F446RE 교육용 보드를 활용하여 GPIO, 통신, 타이머,
인터럽트, RTOS 등 임베디드 개발의 핵심 요소를 단계별로 학습합니다.

## 사용 하드웨어

- **보드**: STM32 Nucleo-F446RE
  - MCU: STM32F446RE (ARM Cortex-M4, 180MHz)
  - Flash: 512KB / SRAM: 128KB
  - 온보드 ST-Link 디버거 내장
- **개발 환경**: STM32CubeIDE
- **라이브러리**: HAL (Hardware Abstraction Layer)

## 학습 로드맵

### Phase 1: 기본기
- [ ] 01. LED 깜빡이기 (GPIO 출력)
- [ ] 02. 버튼 입력 받기 (GPIO 입력)
- [ ] 03. UART 통신 (PC와 시리얼 통신)
- [ ] 04. 타이머 인터럽트
- [ ] 05. 외부 인터럽트 (EXTI)

### Phase 2: 통신 프로토콜
- [ ] 06. I2C 통신 (센서 연결)
- [ ] 07. SPI 통신
- [ ] 08. PWM 신호 생성 (모터 제어 준비)
- [ ] 09. ADC (아날로그 신호 읽기)

### Phase 3: 센서 실습
- [ ] 10. MPU6050 IMU 센서 (가속도/자이로)
- [ ] 11. GPS 모듈 데이터 파싱
- [ ] 12. 초음파 거리 센서

### Phase 4: RTOS
- [ ] 13. FreeRTOS 태스크 생성
- [ ] 14. Queue를 이용한 태스크 간 통신
- [ ] 15. Mutex, Semaphore
- [ ] 16. 다중 태스크 통합 예제

### Phase 5: 통합 응용
- [ ] 17. 센서 데이터 UART 전송 시스템
- [ ] 18. FreeRTOS 기반 다중 센서 처리

## 폴더 구조

​​## 폴더 구조

```
STM32-nucleo-practice/
│
├── README.md
├── docs/
│   ├── setup-guide.md
│   ├── pin-reference.md
│   └── troubleshooting.md
│
├── 01_led_blink/
├── 02_button_input/
├── 03_uart_hello/
├── 04_timer_interrupt/
├── 05_external_interrupt/
├── 06_i2c_communication/
├── 07_spi_communication/
├── 08_pwm_motor/
├── 09_adc_analog/
├── 10_mpu6050_imu/
├── 11_gps_parser/
├── 12_ultrasonic/
├── 13_freertos_task/
├── 14_freertos_queue/
├── 15_freertos_sync/
├── 16_freertos_multi/
├── 17_sensor_uart_system/
└── 18_freertos_integration/
```

## 각 예제 문서화 규칙

모든 예제 폴더는 다음 구조를 따릅니다.

```
예제폴더/
├── README.md          (해당 예제 설명)
├── src/               (소스 코드)
├── inc/               (헤더 파일)
├── ioc/               (STM32CubeMX 설정 파일)
└── media/             (시연 영상/사진)
```

### 각 README.md 포함 사항
- 학습 목표
- 사용 페리페럴
- 회로 연결 방법
- 핵심 코드 설명
- 실행 결과 (사진/GIF)
- 배운 점 / 삽질한 점

## 개발 환경

- **IDE**: STM32CubeIDE 1.14+
- **OS**: Windows 11
- **라이브러리**: STM32 HAL
- **RTOS**: FreeRTOS (CMSIS-RTOS v2)
- **디버거**: ST-Link V2 (온보드)

## 학습 참고 자료

- [STM32F446RE 데이터시트](https://www.st.com/en/microcontrollers-microprocessors/stm32f446re.html)
- [Nucleo-F446RE User Manual](https://www.st.com/resource/en/user_manual/dm00105823.pdf)
- STM32CubeIDE 공식 튜토리얼
- 유튜브 채널: (참고한 채널 기록)

## 진행 일지

학습 진행 상황은 [docs/study-log.md](docs/study-log.md)에 주간 단위로
기록합니다.

## 다음 단계

본 연습 저장소의 학습 완료 후, 습득한 기술을 활용하여
[drone-DIY-STM32](../drone-DIY-STM32) 본 프로젝트에서
자작 드론의 비행 제어 펌웨어를 개발합니다.

---

## 프로젝트 정보

- **작성자**: 태경 (@your-github-id)
- **소속**: 한양대학교 ERICA 융합시스템공학과
- **시작일**: 2026년 8월
- **목적**: 방산 임베디드 SW 직무 취업 준비
