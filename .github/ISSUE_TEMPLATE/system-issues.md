---
name: Bug trong máy của bạn
about: Chỉ các lỗi trong việc thiết lập OpenCore và Lilu được hỗ trợ.
title: ''
labels: ''
assignees: ''
labels: 'error'
---

Vui lòng dừng lại và đọc kỹ điều này. Nếu không, vấn đề của bạn sẽ được để **không được trả lời** và **bị đóng**.

* Chỉ có phiên bản mới nhất của OpenCore, Lilu, và các KEXTs được hỗ trợ.
* Không chấp nhận các bug reports liên quan đến Chameleon, Clover, Ozmozis hoặc các bootloader tương tự.
* Bao gồm thư mục `EFI` của bạn với OpenCore.
* Bao OpenCore DEBUG log (tham khảo cách cài đặt `Target` ở [Configuration.pdf](https://github.com/acidanthera/OpenCorePkg/blob/master/Docs/Configuration.pdf) hoặc ở đây: [OpenCore Debugging](https://viopencore.github.io/OpenCore-Desktop-Guide/troubleshooting/debug.html)).
* Bao gồm Lilu DEBUG log (thêm `-liludbgall liludump=60` vào boot arguments của Lilu's [README](https://github.com/acidanthera/Lilu/blob/master/README.md)).

Khi nào bạn cầnsử dụng [Issue tracker của Acidanthera](https://github.com/acidanthera/bugtracker):

* Bạn có tài nguyên hoặc patch mới để thêm nhưng không thể thực hiện yêu cầu kéo
* Bạn có kernel panics, crashes, bị treo và tin rằng đó không phải là vấn đề trong việc thiết lập OpenCore
* Bạn muốn thảo luận về các vấn đề kỹ thuật hoặc pháp lý

_Nếu bạn gặp kernel panic, hãy đảm bảo rằng bạn có phiên bản DEBUG của extension và bạn đã thêm boot arguments `-v keepyms = 1 debug = 0x100`. Từ macOS 10.13 hoặc cao hơn để tránh các tên kext cuộn qua panic log, bạn cũng nên đặt `PanicNoKextDump = YES` trong OpenCore. Sử dụng `ApplePanic = YES` để ghi kernel panic log vào tệp._
