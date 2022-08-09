## 운영체제란?
컴퓨터 하드웨어가 컴퓨터 소프트웨어와 통신하고 작동하도록 하는 소프트웨어 프로그램이다.



## 교착상태(DeadLock)

두개 이상의 프로세스나 스레드가 자원을 점유한 상태에서 더 필요한 자원을 얻지 못해 서로의 작업의 끝을 기다리다 무한히 다음 처리를 하지 못하는 상태.

* #### 교착상태를 처리하는 방법

예방, 회피가 있습니다.

* 은행원 알고리즘
    * 은행에서 모든 고객의 요구가 충족되도록 현금을 할당하는데서 유래함
    * 프로세스가 자원을 요구할 때, 시스템은 자원을 할당한 후에도 안정 상태로 남아있게 되는지 사전에 검사하여 교착 상태 회피
    * 안정 상태면 자원 할당, 아니면 다른 프로세스들이 자원 해지까지 대기

## CPU Scheduling
CPU를 잘 사용하기 위해 프로세스를 배정하는 작업

종류는 선점/비선점 Scheduling으로 나뉜다.
* 선점 - OS가 CPU의 사용권을 선점할 수 있는 경우, 강제 회수하는 경우
* 비선점 - 프로세스 종료 or I/O 등의 이벤트가 있을 때까지 실행 보장

대표적인 비선점 스케쥴링은 FCFS, 선점 스케쥴링은 Round Robin이 있습니다.

## 메모리
메모리는 컴퓨터에서 작업을 수행하기 위해 처리 대상이나 결과등을 저장하기 위한 공간입니다. 프로그램을 실행하기 위한 정보들은 메모리에 저장되어 처리됩니다.