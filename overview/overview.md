# <a name="overview-of-microsoft-graph"></a>Microsoft Graph 概述

Microsoft Graph通过一个终结点从 Office 365 和其他 Microsoft 云服务公开了多个 API：**https://graph.microsoft.com**。Microsoft Graph 简化了本来会更加复杂的查询。 
 
可以使用 Microsoft Graph 执行以下操作：

- 访问多个 Microsoft 云服务中的数据，包括 Azure Active Directory、作为 Office 365 一部分的 Exchange Online、SharePoint、OneDrive、OneNote 和 Planner。
- 在实体和关系之间导航。
- 访问 Microsoft 云中的情报和见解（针对商业用户）。

**Microsoft Graph 开发堆栈**

![显示 Microsoft Graph 开发堆栈层的关系图。底部是数据层，包括用户、组、文件、邮件、日历、个人联系人、任务、组织联系人、人员、Excel 和注释。下一层是身份验证和授权。接下来是所选的开发环境，包括 Android，iOS 和 Visual Studio Microsoft Graph API SDK。最后一层是解决方案，它使用包括 .NET、JS、HTML 和 Ruby 在内的所选技术，并且被托管在 Microsoft Azure 或其他托管平台中。](./images/MicrosoftGraph_DevStack.png)

<!--<a name="msg_queries"> </a>-->

##<a name="common-microsoft-graph-queries"></a>常见的 Microsoft Graph 查询

Microsoft Graph 公开了两个终结点：/v1.0 和 /beta。/V1.0 终结点包括可在生产应用中访问的资源。 [/beta](http://developer.microsoft.com/en-us/graph/docs/api-reference/beta/beta-overview) 终结点包含当前处于预览状态的 API。下表列出了一些可用于访问 Microsoft Graph API 的常见查询。

| **操作**    | **服务终结点** |
|:--------------------------|:----------------------------------------|
|   获取我的个人资料 |    [`https://graph.microsoft.com/v1.0/me`](https://graph.microsoft.io/en-us/graph-explorer/?request=me&version=v1.0) |
|   获取我的文件 | [`https://graph.microsoft.com/v1.0/me/drive/root/children`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren&version=v1.0) |
|   获取我的照片	     | [`https://graph.microsoft.com/v1.0/me/photo/$value`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fphoto%2F%24value&version=v1.0) |
|   获取我的邮件 |    [`https://graph.microsoft.com/v1.0/me/messages`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fmessages&version=v1.0) |
|   获取我的高重要性的邮件 | [`https://graph.microsoft.com/v1.0/me/messages?$filter=importance%20eq%20'high'`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fmessages%3F%24filter%3Dimportance%2520eq%2520'high'&version=v1.0) |
|   获取我的日历 |    [`https://graph.microsoft.com/v1.0/me/calendar`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fcalendar&version=v1.0) |
|   获取我的经理	    | [`https://graph.microsoft.com/v1.0/me/manager`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fmanager&version=v1.0) |
|   获取上一个修改文件 foo.txt 的用户 |    [`https://graph.microsoft.com/v1.0/me/drive/root/children/foo.txt/lastModifiedByUser`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fdrive%2Froot%2Fchildren%2Ffoo.txt%2FlastModifiedByUser&version=v1.0) |
|   获取我隶属于的统一组|    [`https://graph.microsoft.com/v1.0/me/memberOf/$/microsoft.graph.group?$filter=groupTypes/any(a:a%20eq%20'unified')`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2FmemberOf%2F%24%2Fmicrosoft.graph.group%3F%24filter%3DgroupTypes%2Fany(a%3Aa%2520eq%2520'unified')&version=v1.0) |
|   获取我组织中的用户	     | [`https://graph.microsoft.com/v1.0/users`](https://graph.microsoft.io/en-us/graph-explorer/?request=users&version=v1.0) |
|   获取群组聊天 |    `https://graph.microsoft.com/v1.0/groups/{id}/conversations`|
|   获取与我相关的人员    | [`https://graph.microsoft.com/beta/me/people`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fpeople&version=beta)  |
|   获取我常用的项目 |    [`https://graph.microsoft.com/beta/me/insights/trending`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Finsights%2Ftrending&version=beta) |
|   获取我的任务    | [`https://graph.microsoft.com/beta/me/tasks`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Ftasks&version=beta) |
|   获取我的注释 |    [`https://graph.microsoft.com/beta/me/notes/notebooks`](https://graph.microsoft.io/en-us/graph-explorer/?request=me%2Fnotes%2Fnotebooks&version=beta) |


>**注意：**beta 终结点中的 API 可能会发生更改。建议不要在生产应用中使用它们。 

<!-- <a name="msg_roof"> </a> -->

## <a name="explore-microsoft-graph"></a>浏览 Microsoft Graph

- 使用 Microsoft Graph 和所选的平台 [入门](https://developer.microsoft.com/en-us/graph/docs/get-started/get-started)。
- 通过浏览 TOC，发现可在生产应用中使用的资源和操作。
- 预览新的 [/beta API](https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/beta-overview)。
- 访问 [Microsoft Graph 浏览器](https://graph.microsoft.io/graph-explorer)。
- 请查看我们的 [Microsoft Graph 代码片段示例](https://github.com/search?q=org%3Amicrosoftgraph+snippets-sample)。

 >  我们非常重视你的反馈。请在 [Stack Overflow](http://stackoverflow.com/questions/tagged/office365+or+microsoftgraph) 上与我们联系。使用 {MicrosoftGraph} 和 {office365} 标记出你的问题。



