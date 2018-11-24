# <a name="use-the-microsoft-graph-api-to-get-change-notifications"></a>使用 Microsoft Graph API 获取更改通知

Microsoft Graph REST API 使用 webhook 机制来将通知传递到客户端。 客户端是配置其自己的 URL，以接收通知的 web 服务。 客户端应用程序使用通知更新时更改其状态。 有关详细信息，包括如何订阅和处理传入通知，请参阅[设置通知用户数据中的更改](../../../concepts/webhooks.md)。

使用 Microsoft Graph API，应用可以订阅以下资源的更改：

- 邮件
- 事件
- 联系人
- 用户
- 组
- 组对话
- 在 OneDrive，包括与 SharePoint 网站关联的驱动器上共享的内容
- 用户的个人 OneDrive 文件夹
- 安全警报

## <a name="permissions"></a>Permissions

通常订阅操作需要拥有对资源的读取权限。例如，若要获取邮件通知，应用需要 `Mail.Read` 权限。[创建订阅](../api/subscription_post_subscriptions.md)一文列出了各个资源类型所需的权限。下表列出了将 webhook 用于特定资源类型时应用可以请求的权限类型。

| 权限类型                        | v1.0 中支持的资源类型                                 |
| :------------------------------------- | :--------------------------------------------------------------- |
| 委派 - 工作或学校帐户     | [联系人][]、[对话][]、[驱动器][]、[事件][]、[邮件][]、[通知][] |
| 委派 - 个人 Microsoft 帐户 | 无                                                             |
| 应用程序                            | [联系人][]、[对话][]、[事件][]、[消息][]、[警报][]           |

## <a name="see-also"></a>另请参阅

- [订阅资源类型](./subscription.md)
- [获取订阅](../api/subscription_get.md)
- [创建订阅](../api/subscription_post_subscriptions.md)
- [更新订阅](../api/subscription_update.md)
- [删除订阅](../api/subscription_delete.md)

[联系人]: ./contact.md
[对话]: ./conversation.md
[驱动器]: ./drive.md
[事件]: ./event.md
[邮件]: ./message.md
[通知]: ./alert.md