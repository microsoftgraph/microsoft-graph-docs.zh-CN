# <a name="use-the-onenote-rest-api"></a>使用 OneNote REST API

Microsoft Graph 允许您的应用获取对用户的个人或组织帐户中的 OneNote 笔记本、节和页面的授权访问权限。 使用[适当的委派或应用程序权限](../../../concepts/permissions_reference.md#notes-permissions)，您的应用可以访问已登录用户或租户中的任何用户的 OneNote 数据。

## <a name="root-url"></a>根 URL
OneNote 服务根 URL 为 OneNote API 的所有调用使用以下格式。
```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```
URL 中的 `version` 段代表您希望使用的 Microsoft Graph 版本。

- `v1.0` 用于稳定生产代码。
- `beta` 用于试用正在开发的功能。 beta 端点中的功能可能会出现变动；我们不建议在生产代码中使用它。

位置可以是 Office 365 或消费者 OneDrive、团队笔记本 上的用户笔记本，也可以是 Office 365 上的 SharePoint 站点托管的团队笔记本。 

![OneNote API 开发堆栈](https://cdn.graph.office.net/prod/GraphDocuments/en-us/concepts/images/onenote-dev-diagram.png)

### <a name="user-notebooks"></a>用户笔记本
要访问消费者 OneDrive 或 OneDrive for Business 上的个人笔记本，请使用下列 URL 之一：

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

- `me` 用于为当前用户可以访问的 OneNote 内容（拥有和共享）。
- `users/{id}` 用于指定用户已与当前用户共享的 OneNote 内容（此 URL 中）。 使用[用户](users.md) API。
> **注意：** 可以通过在 `https://graph.microsoft.com/v1.0/users` 上发出 GET 请求来获取用户 ID。

### <a name="group-notebooks"></a>团队笔记本
要访问团队拥有的笔记本，请使用下列服务根 URL：

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
### <a name="sharepoint-site-notebooks"></a>SharePoint 网站笔记本

要访问 SharePoint 团队网站所有的笔记本，请使用下列服务根 URL：

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

