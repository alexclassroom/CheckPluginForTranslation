# CheckPluginForTranslation
這個檢查程式能夠檢查託管於 WordPress.org 外掛目錄的外掛，是否已完成國際化的整備。

原開發者 [ePascalC](https://github.com/ePascalC) 撰寫了這份指令碼，並在[開發者自己的網站](https://wp-info.org/tools/checkplugini18n.php) **(目前已停止服務)** 上執行，輔助他自己快速檢查其他外掛開發者會發生的問題：
- 無法建立語言套件
- 外掛沒有做好介面字串國際化的整備
- 外掛僅有 dev，沒有 stable
- 其他問題

檢查結果範例：點擊[這裡](https://github.com/ePascalC/CheckPluginForTranslation/blob/master/v0.2.5%20examples.pdf)以查看

Checks that will be performed:
* Plugin slug and base folder are reachable
* Readme in /trunk or /tags
  * Filesize not over 10k
  * Find the 'Required at least' and 'Stable Tag'
  * Make sure 'Tested up to' is not over 'Required at least'
  * Tags (not over 5)
* Versions under /tags
* Find the main php file
  * Find Text Domain
  * _function load_plugin_textdomain (if needed) (still to be done)_
* Existing language packs
* _Translation status (still to be done)_
* Translation editors - PTE
* Revision log
* _Translation warning (as in #polyglots-warnings on slack) (still to be done)_
* _Language pack status (as in #meta-language-packs on slack) (still to be done)_
* _Waiting strings (still to be done)_
* List with useful links
* Summary table

All help is appreaciated!

Pascal.
