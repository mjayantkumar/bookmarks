Shell
=====
* [Full vim for readline (bash, gdb, python, etc)](https://github.com/ardagnir/athame)
* [Code Inflation](https://www.computer.org/cms/Computer.org/ComputingNow/issues/2015/04/mso2015020010.pdf)
* [joinc](http://www.joinc.co.kr/modules/moniwiki/wiki.php/Site/Bash)
* string

  ```
  ${VAR_NAME##*[delimeter]} cut after delimeter
  ${VAR_NAME%[delimeter]*} cut before delimeter
  ```
  * example

    ```
    $ TEST=some_string.ext
    $ echo ${TEST##*_}
    string.ext
    $ echo ${TEST%.*}
    some_string
    ```
* miscellaneous
  * `CUR_DIR=$(readlink -f $(dirname $(readlink -f ${BASH_SOURCE[0]}))) current directory`