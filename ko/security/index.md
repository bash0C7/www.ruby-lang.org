---
layout: page
title: "보안이슈"
lang: ko
---

Ruby와 관련한 보안이슈에 대해 정보를 공유하는 곳입니다.
{: .summary}

### 보안 취약점 알리기

보안상 취약한 부분이나 심각한 문제를 야기할 수 있는 부분에 대해서는
security@ruby-lang.org ([the PGP public key](/security.asc))로 메일을 보내주십시오. 이는
비공개 메일링 리스트로 운영되고 있으며 보고된 문제에 대한 확인과 해결책이 이루어진 다음 일반에게 정보를 공개하고 있습니다.

### 알려진 취약점

다음과 같은 보안 취약점이 보고된 바 있습니다.

* [부동소수점 파싱할 때 힙 오버플로 발생
  (CVE-2013-4164)](/ko/news/2013/11/22/heap-overflow-in-floating-point-parsing-cve-2013-4164/)
  2013년 11월 22일 공개
* [Hostname check bypassing vulnerability in SSL client
  (CVE-2013-4073)](/en/news/2013/06/27/hostname-check-bypassing-vulnerability-in-openssl-client-cve-2013-4073/)
  2013년 6월 27일 공개
* [Object taint bypassing in DL and Fiddle in Ruby
  (CVE-2013-2065)](/en/news/2013/05/14/taint-bypass-dl-fiddle-cve-2013-2065/)
  2013년 5월 14일 공개
* [Entity expansion DoS vulnerability in REXML (XML bomb,
  CVE-2013-1821)][1]
  2013년 2월 22일 공개
* [Denial of Service and Unsafe Object Creation Vulnerability in JSON
  (CVE-2013-0269)][2]
  2013년 2월 22일 공개
* [XSS exploit of RDoc documentation generated by rdoc
  (CVE-2013-0256)][3]
  2013년 2월 6일 공개
* [Hash-flooding DoS vulnerability for ruby 1.9 (CVE-2012-5371)][4]
  2012년 10월 10일 공개
* [Unintentional file creation caused by inserting a illegal NUL
  character (CVE-2012-4522)][5]
  2012년 10월 12일 공개
* [$SAFE escaping vulnerability about Exception#to\_s / NameError#to\_s
  (CVE-2012-4464, CVE-2012-4466)][6]
  2012년 10월 12일 공개
* [Security Fix for RubyGems: SSL server verification failure for remote
  repository][7] 2012년 4월 20일 공개
* [Security Fix for Ruby OpenSSL module: Allow 0/n splitting as a
  prevention for the TLS BEAST attack][8]
  2012년 2월 16일 공개
* [Denial of service attack was found for Ruby\'s Hash algorithm
  (CVE-2011-4815)][9]
  2011년 12월 28일 공개
* [Exception methods can bypass $SAFE][10]
  2011년 2월 18일 공개
* [FileUtils is vulnerable to symlink race attacks][11]
  2011년 2월 18일 공개
* [WEBrick XSS취약점 (CVE-2010-0541)][12]
  2010년 8월 16일 공개
* [Buffer over-run in ARGF.inplace\_mode=][13]
  2010년 7월 2일 공개
* [WEBrick::이스케이프 시퀀스 취약점][14]
  2010년 1월 10일 공개
* [Heap overflow in String (CVE-2009-4124)][15]
  2009년 12월 7일 공개
* [DoS vulnerability in
  BigDecimal](/en/news/2009/06/09/dos-vulnerability-in-bigdecimal/)
  2009년 6월 9일 공개
* [DoS vulnerability in
  REXML](/en/news/2008/08/23/dos-vulnerability-in-rexml/)
  2008년 8월 23일 공개
* [Multiple vulnerabilities in
  Ruby](/en/news/2008/08/08/multiple-vulnerabilities-in-ruby/)
  2008년 8월 8일 공개
* [임의의 코드를 실행할 수 있는 보안
  취약성](/ko/news/2008/06/23/arbitrary-code-execution-vulnerabilities)
  2008년 6월 20일 공개
* [File access vulnerability of
  WEBrick](/en/news/2008/03/03/webrick-file-access-vulnerability/)
  2008년 5월 3일 공개
* [Net::HTTPS
  Vulnerability](/en/news/2007/10/04/net-https-vulnerability/)
  2007년 10월 4일 공개
* [Another DoS Vulnerability in CGI
  Library](/en/news/2006/12/04/another-dos-vulnerability-in-cgi-library/)
  2006년 11월 3일 공개
* [Ruby vulnerability in the safe level
  settings](/en/news/2005/10/03/ruby-vulnerability-in-the-safe-level-settings/)
  2005년 10월 2일 공개

좀 더 자세한 사항은 [영문 페이지](/en/security/)를 참조하시기 바랍니다.


[1]: /en/news/2013/02/22/rexml-dos-2013-02-22/
[2]: /en/news/2013/02/22/json-dos-cve-2013-0269/
[3]: /en/news/2013/02/06/rdoc-xss-cve-2013-0256/
[4]: /en/news/2012/11/09/ruby19-hashdos-cve-2012-5371/
[5]: /en/news/2012/10/12/poisoned-NUL-byte-vulnerability/
[6]: /en/news/2012/10/12/cve-2012-4464-cve-2012-4466/
[7]: /en/news/2012/04/20/ruby-1-9-3-p194-is-released/
[8]: /en/news/2012/02/16/security-fix-for-ruby-openssl-module-allow-0n-splitting-as-a-prevention-for-the-tls-beast-attack-/
[9]: /en/news/2011/12/28/denial-of-service-attack-was-found-for-rubys-hash-algorithm-cve-2011-4815/
[10]: /en/news/2011/02/18/exception-methods-can-bypass-safe/
[11]: /en/news/2011/02/18/fileutils-is-vulnerable-to-symlink-race-attacks/
[12]: /ko/news/2010/08/16/webrick-xss-cve-2010-0541/
[13]: /en/news/2010/07/02/ruby-1-9-1-p429-is-released/
[14]: /ko/news/2010/01/15/webrick-escape-sequence-injection/
[15]: /en/news/2009/12/07/heap-overflow-in-string/

