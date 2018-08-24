# <a name="use-the-microsoft-graph-api-to-work-with-project-rome"></a>使用 Microsoft Graph API 来处理 Project Rome

[Project Rome](https://developer.microsoft.com/en-us/windows/project-rome) 是用以构建一个跨设备体验平台的 Microsoft 计划。 当用户使用登录客户端设备时使用的同一 Microsoft 帐户登录，Project Rome 让本地客户端或服务上的应用程序与远程主机上的应用程序和服务进行交互。 这将允许您围绕用户任务而不是设备来构建跨设备和跨平台的体验。

通过 Microsoft Graph 启用这些体验的关键要素是活动。

## <a name="activities"></a>活动

Microsoft Graph 中的活动使您的应用程序能够让用户跨设备和平台参与互动。 活动是用户互动的单位，它包括三个组件：

- 深层链接
- 直观表示形式
- 使用 [http://schema.org/](http://schema.org/) 共享词汇描述该活动的内容元数据

应用程序创建会话时, 历史记录项会添加到活动中，以反映用户互动的时期。 每次用户继续参与活动时，新的历史记录项会添加到活动中，以累计用户的互动。

当应用程序发布用户活动对象时，该对象将在 Windows 的某些新 UI 中显示；例如，Cortana 通知和日程表。 活动对象中可以指定丰富的元数据 （以允许活动在适当的上下文中呈现）和丰富的视觉效果 （使用[自适应卡片](http://adaptivecards.io/)标记）。

以下 Microsoft Graph API 可用于创建和检索用户活动：

- [创建或替换活动](../api/projectrome_put_activity.md)
- [获取活动](../api/projectrome_get_activities.md)
- [获取最近的活动](../api/projectrome_get_recent_activities.md)
- [删除活动](../api/projectrome_delete_activity.md)
- [创建或替换历史记录项](../api/projectrome_put_historyitem.md)
- [删除历史记录项](../api/projectrome_delete_historyitem.md)