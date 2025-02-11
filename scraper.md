## Facebook 群组爬虫

我们目前使用这个JS爬虫：https://github.com/floriandiud/facebook-group-members-scraper
配合这个Chrome插件：https://chromewebstore.google.com/detail/autoscroll/occjjkgifpmdgodlplnacmkejpdionan
来爬取 Facebook 群组的成员列表

基本原理：模拟滚轮下滑，在下滑时读取API请求，从里面找到需要的字段 Profile Id,Full Name,Profile Link等等，并将以上信息存储到SessionStorage当中。

目前的需求和挑战：以上流程爬取一个16K成员的群组需要8小时。有哪些方法可以改进这个爬虫？

- 我们将提供可用的 Facebook 账号
- 可参考的开源爬虫项目：https://github.com/NanmiCoder/MediaCrawler