然后执行  composer install 即可。


如何更新包裹？
GitHub Hook
启用Packagist服务挂钩可确保在您推送到GitHub时，您的包将始终立即更新。

为此，您可以：

确保您通过GitHub登录（如果您已经有一个未连接到GitHub的帐户，您可以在您的个人资料上连接它）。如果您已经登录，请先退出，然后再次通过GitHub登录，以确保您授予我们所需的权限。
确保Packagist应用程序可以访问您发布包所需的所有GitHub组织。
检查您的包裹清单，看看是否有任何关于不自动同步的警告。
如果您仍需要在某些软件包上设置同步，请尝试触发手动帐户同步，让Packagist再次尝试在您的帐户上设置挂钩。请注意，归档存储库无法设置，因为它们只是在GitHub的API中只读。
不想通过GitHub登录并授予我们webhook配置访问权限？
您可以使用以下值手动配置GitHub webhook：

有效载荷URL： https://packagist.org/api/github?username=goalwaybe
内容类型： application/json
秘密：你的Packagist API令牌
哪些事件？只是push活动就足够了。



测试webhook函数是否自动更新,

测试webhook函数第二次是否自动更新,