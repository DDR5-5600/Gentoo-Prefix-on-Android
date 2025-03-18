# Gentoo-Prefix-on-Android
將Gentoo Prefix移植到Android的Termux環境的嘗試 <br>
目前進度卡死因為Android檔案系統不支持hardlink <br>
因此進入stage2就會直接被權限問題擋下 <br>
除非上游portage支援關閉hardlock，否則目前就止步於此 <br>

[emerge permission denied var/db/.pkg.portage_lockfile](https://forums.gentoo.org/viewtopic-t-1132047-start-0-postdays-0-postorder-asc-highlight-.html) <br>
[Bug 774384 - sys-apps/portage-prefix: Add option to disable locking or use symlinks for systems that do not support hardlinks](https://bugs.gentoo.org/774384)
