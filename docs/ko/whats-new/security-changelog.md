---
toc_priority: 76
toc_title: Security Changelog
---

## ClickHouse 배포판 19.14.3.3 에서 수정된 것, 2019-09-10 {#fixed-in-clickhouse-release-19-14-3-3-2019-09-10}

### CVE-2019-15024 {#cve-2019-15024}

ZooKeeper 에 대한 쓰기 권한을 가진 공격자는 ClickHouse 가 실행되는 네트워크에서 사용 가능한 사용자 지정 서버를 실행하여 ClickHouse 복제본 역할을 하는 사용자 지정 악성 서버를 만들어 "ZooKeeper"에 등록할 수 있음. 

공헌: Yandex Information Security Team의 Eldar Zaitov

### CVE-2019-16535 {#cve-2019-16535}

Аn OOB read, OOB write and integer underflow in decompression algorithms can be used to achieve RCE or DoS via native protocol.

공헌: Yandex Information Security Team의 Eldar Zaitov

### CVE-2019-16536 {#cve-2019-16536}

Stack overflow leading to DoS can be triggered by a malicious authenticated client.

공헌: Yandex Information Security Team의 Eldar Zaitov

## ClickHouse 배포판 19.13.6.1 에서 수정된 것, 2019-09-20 {#fixed-in-clickhouse-release-19-13-6-1-2019-09-20}

### CVE-2019-18657 {#cve-2019-18657}

Table function `url` had the vulnerability allowed the attacker to inject arbitrary HTTP headers in the request.

공헌: [Nikita Tikhomirov](https://github.com/NSTikhomirov)

## ClickHouse 배포판 18.12.13 에서 수정된 것, 2018-09-10 {#fixed-in-clickhouse-release-18-12-13-2018-09-10}

### CVE-2018-14672 {#cve-2018-14672}

Functions for loading CatBoost models allowed path traversal and reading arbitrary files through error messages.

Credits: Andrey Krasichkov of Yandex Information Security Team

## ClickHouse 배포판 18.10.3 에서 수정된 것, 2018-08-13 {#fixed-in-clickhouse-release-18-10-3-2018-08-13}

### CVE-2018-14671 {#cve-2018-14671}

unixODBC allowed loading arbitrary shared objects from the file system which led to a Remote Code Execution vulnerability.

Credits: Andrey Krasichkov and Evgeny Sidorov of Yandex Information Security Team

## ClickHouse 배포판 1.1.54388 에서 수정된 것, 2018-06-28 {#fixed-in-clickhouse-release-1-1-54388-2018-06-28}

### CVE-2018-14668 {#cve-2018-14668}

“remote” table function allowed arbitrary symbols in “user”, “password” and “default_database” fields which led to Cross Protocol Request Forgery Attacks.

공헌: Yandex Information Security Team의 Andrey Krasichkov

## ClickHouse 배포판 1.1.54390 에서 수정된 것, 2018-07-06 {#fixed-in-clickhouse-release-1-1-54390-2018-07-06}

### CVE-2018-14669 {#cve-2018-14669}

ClickHouse MySQL client had “LOAD DATA LOCAL INFILE” functionality enabled that allowed a malicious MySQL database read arbitrary files from the connected ClickHouse server.

공헌: Yandex Information Security Team의 Andrey Krasichkov 와 Evgeny Sidorov

## ClickHouse 배포판 1.1.54131 에서 수정된 것, 2017-01-10 {#fixed-in-clickhouse-release-1-1-54131-2017-01-10}

### CVE-2018-14670 {#cve-2018-14670}

deb 패키지의 구성이 잘못되면 DB를 무단으로 사용할 수 있음.

공헌: 영국 국가 사이버 보안 센터 (NCSC)

{## [원문](https://clickhouse.tech/docs/en/security_changelog/) ##}
