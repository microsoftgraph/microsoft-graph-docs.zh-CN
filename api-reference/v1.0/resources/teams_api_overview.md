# <a name="use-the-microsoft-graph-api-to-work-with-microsoft-teams"></a>将 Microsoft Graph API 与 Microsoft Teams 结合使用



Microsoft 团队是基于聊天提供内置访问特定于团队的日历、 文件、 OneNote 笔记、 计划程序计划和更多的 Office 365 中工作区。

## <a name="key-resources-in-microsoft-teams"></a>在 Microsoft 团队中的关键资源

| 资源 | 方法 |
|:---------------|:--------|
|[团队](../resources/team.md)| [列出您的团队](../api/user_list_joinedteams.md)、[列出所有团队](../../../concepts/teams_list_all_teams.md)、[创建](../api/team_put_teams.md)、[读取](../api/team_get.md)、[更新](../api/team_update.md)、[删除](../../v1.0/api/group_delete.md)、[克隆](../api/team_clone.md)、[存档](../api/team_archive.md)、 [unarchive](../api/team_unarchive.md) |
|[组](../resources/group.md)| [将成员添加](../api/group_post_members.md)、 [删除成员](../api/group_delete_members.md)、[添加所有者](../api/group_post_owners.md)、 [删除所有者](../api/group_delete_owners.md)，[获取文件](drive.md)、[获取笔记本](../../v1.0/resources/notebook.md)，[获取计划](plannergroup.md)、[获取日历](event.md) |
|[通道](../resources/channel.md)|[列表](../api/channel_list.md)、[创建](../api/channel_post.md)、[读取](../api/channel_get.md)、[更新](../api/channel_patch.md)、[删除](../api/channel_delete.md)|
|[teamsTab](../resources/teamstab.md) |[列表](../api/teamstab_list.md)、[创建](../api/teamstab_add.md)、[读取](../api/teamstab_get.md)、[更新](../api/teamstab_update.md)、[删除](../api/teamstab_delete.md) |
|[teamsApp](../resources/teamsapp.md)|[列表](../api/teamsapp_list.md)、[发布](../api/teamsapp_publish.md)、[更新](../api/teamsapp_update.md)、[删除](../api/teamsapp_delete.md)|
|[teamsAppInstallation](../resources/teamsappinstallation.md)| [列表](../api/teamsappinstallation_list.md)、[安装](../api/teamsappinstallation_add.md)、[升级](../api/teamsappinstallation_delete.md)、[删除](../api/teamsappinstallation_delete.md) |
| （预览）[chatMessage](../../beta/resources/chatmessage.md)和[chatThread](../../beta/resources/chatthread.md) | [列表](../../beta/api/channel_list_messages.md)、[创建](../../beta/api/channel_post_chatthreads.md)、[读取](../../beta/api/channel_get_message.md) |
| （预览）[呼叫](../../beta/resources/call.md) | [应答](../../beta/api/call_answer.md)、[拒绝](../../beta/api/call_reject.md)、[重定向](../../beta/api/call_redirect.md)、[设为静音](../../beta/api/call_mute.md)、[取消静音](../../beta/api/call_unmute.md)、[更新元数据](../../beta/api/call_updatemetadata.md)、[更改屏幕共享角色](../../beta/api/call_changescreensharingrole.md)，[列表参与者](../../beta/api/call_list_participants.md)，[邀请参与者](../../beta/api/participant_invite.md)，[将所有参与者设为都静音](../../beta/api/participant_muteall.md) |

## <a name="teams-and-groups"></a>团队和组

在 Microsoft Graph 中的 Microsoft 团队由此[group](../resources/group.md)资源。 Microsoft 团队和 Office 365 组通讯组协作的各种需求。 几乎所有的基于组的功能适用于 Microsoft 团队和 Office 365 组，例如组日历、 文件、 备注和照片，计划，等等。 [团队](team.md)和 Office 365 组的主要区别是通信的成员之间的模式。 通过特定的团队的上下文中的持久聊天，团队成员进行通信。 Office 365 的组成员的组对话，是在 Outlook 中的组的上下文中发生的电子邮件对话进行通信。

有一个团队任何组具有**resourceProvisioningOptions**属性包含"团队"。 

>**注意：** 可以更改**Group.resourceProvisioningOptions**属性。
添加或移除集合;"团队"否则，您将获取错误的结果时您列出所有团队。

API 级别团队和组之间的差异如下：

- [列表加入团队](../api/user_list_joinedteams.md)方法仅适用于 Microsoft 团队。
- 另请参阅[已知问题](../../../concepts/known_issues.md)的这些 Api。

>**注意：** 如果您使用-例如作为选项卡或自动程序的 Microsoft 团队中运行的一部分-组 API[的 Microsoft 团队应用程序](https://docs.microsoft.com/en-us/microsoftteams/platform/#apps-in-microsoft-teams)中，而不是独立应用程序中按照[您的 Microsoft 团队的页面中使用 Microsoft Graph](https://docs.microsoft.com/en-us/microsoftteams/platform/resources/microsoft-graph)一文中的指南。

## <a name="membership-changes-in-microsoft-teams"></a>在 Microsoft 团队的成员身份更改

若要添加到团队成员和所有者，更改具有相同的 id。 的[组](../resources/group.md)的成员资格

| 用例      | Verb      | URL |
| ------------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| [Add member](../api/group_post_members.md)    | POST      | /groups/ {id} /members/ ref  |
| [删除成员](../api/group_delete_members.md)   | DELETE    | /groups/ {id} /members/ {userId} / $ref |
| [添加所有者](../api/group_post_owners.md)     | POST       | /groups/ {id} /owners/ ref |
| [删除所有者](../api/group_delete_owners.md) | DELETE    | /groups/ {id} /owners/ {userId} / $ref |
| [更新团队](../api/team_update.md)  | PATCH     | /teams/ {id} |

我们建议时添加所有者，您还添加用户作为成员。 如果团队都有一个所有者不是成员，所有权和成员身份更改可能不显示立即在 Microsoft 团队。 此外，不同的应用程序和 Api 将处理的以不同方式。 例如，Microsoft 团队将显示团队时的 Microsoft 团队 PowerShell cmdlet 和/我/joinedTeams API 将仅显示的团队用户是其成员的用户可为成员或的所有者。 若要避免混淆，添加到成员列表的所有所有者。 

已知问题： 当删除 /groups/ {id} / 所有者被调用时，用户也从 /groups/ {id} / 成员列表。 若要解决此问题，建议用户移除所有者和成员，然后等待 10 秒钟，然后将其添加回成员。

添加和删除成员和所有者，不要放置大括号内的 {} 周围 id。

| Speed | 语法 | 
| ------ | ----- |
| 快速 | https://graph.microsoft.com/v1.0/groups/02bd9fd6-8f93-4758-87c3-1fb73740a315/members/48d31887-5fad-4d73-a9f5-3c356e68a038/$ref | 
| 慢速 | https://graph.microsoft.com/v1.0/groups/{02bd9fd6-8f93-4758-87c3-1fb73740a315}/members/{48d31887-5fad-4d73-a9f5-3c356e68a038}/$ref | 

同样，如果`userId`中的 URL 或有效负载表示为 UPN 而不是为 GUID，性能会变慢。

| Speed | 语法 | 
| ------ | ----- |
| 快速 | 48d31887-5fad-4d73-a9f5-3c356e68a038 | 
| 慢速 | john@example.com | 

如果变为速度较慢的路径，如果当前工作组成员或所有者登录到 Microsoft 团队应用程序/网站时，更改将反映在一个小时内。
如果无这些用户已登录到 Microsoft 团队应用程序/网站，更改将不会反映之前小时后两者之一登录。

## <a name="see-also"></a>另请参阅

- [Microsoft 团队 API 概述](../../../concepts/teams-concept-overview.md)
- 示例代码： [Contoso 航空公司](https://github.com/microsoftgraph/contoso-airlines-teams-sample)、 [C# 浮动示例](https://github.com/microsoftgraph/csharp-teams-sample-graph)
