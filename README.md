# 서버 운영 가이드

## 소개 및 기본 규칙

#### 1. 본 문서는 서버 셋팅관련 방법에 대해서 정의합니다.

#### 2. 기본 OS는 CentOS 7.X 버젼을 사용하며, 일부 필요에따라 6.X버젼 관련 설명이 포함되어있을 수 있습니다.

#### 3. OS 설치는 일반적으로 서버 호스팅 업체에서 대행하므로 해당 과정은 생략합니다.

#### 4. 서버의 용도는 기본 웹서비스(Webservice) 를 위한 설정이며, 필요에 따라 다른 기능이 추가될 수 있습니다.

#### 5. 기본적으로 패키지 설치는 Yum 을 사용하며, Yum에서 제공하지 않는 패키지의 경우 소스설치를 진행합니다.

#### 6. 작업파일의 위치는 가능한한 전체경로(Full Path)로 명시합니다.
    예)
    (X) my.cnf
    (O) /etc/my.cnf

#### 7. 기본 설치/사용 서비스 패키지는 아래와 같습니다.
    7-1. Webserver : NginX 1.X
    7-2. Database : MariaDB 5.X
    7-3. Server side script : PHP 7.X

###### 패키지 버젼은 설치 시기에 따라 달라질 수 있습니다.

## Index
#### 1. 서버 일반
    1-1. 웹서버 + PHP 설치 및 기본 셋팅        
    1-2. DB 설치 및 기본 셋팅  
    1-3. 방화벽 설정  
    1-4. 시작 서비스 관리
  
##### 2. 보안
    2-1. 방화벽 설정  
    2-2. 사용자 격리  
  
##### 3. 관리 규칙  
    3-1 사용자 관리 규칙  
    3-2 웹로그 관리 규칙

##### 99. 서비스/운영 이슈
    99-1. 웹서버 이슈    
    99-2. Database 이슈    
    99-3. 기타 이슈

