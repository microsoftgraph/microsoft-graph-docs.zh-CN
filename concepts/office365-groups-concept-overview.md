# <a name="overview-of-office-365-groups-in-microsoft-graph"></a>Microsoft Graph 中的 Office 365 组概述

Office 365 组为用户提供了基础成员身份服务，可用于共享会话、文件、备注、日历、计划和许多其他资产。 

## <a name="why-integrate-with-office-365-groups"></a>为何要与 Office 365 组集成？   

各个组会形成一个基础，让用户能够跨服务进行协作和集成，以支持任务计划、团队合作、教育等丰富的应用场景。 当你与 Office 365 组集成后，随着数百万用户在 Office 365 套件及更高版本中跨各种体验进行转换，你的应用程序即可为他们提供支持。  
 
### <a name="create-groups-to-facilitate-teamwork-across-services"></a>创建组以促进跨服务的团队合作 
 
你可以使用 Microsoft Graph API 在整个协作生命周期中创建、管理或删除组。 例如，可以执行以下操作：  
 
- 使用[创建组](../api-reference/v1.0/api/group_post_groups.md) API 预配一个新组。 然后，该组可用于一系列应用程序，例如 Outlook、SharePoint、Microsoft Teams、Planner，甚至 Microsoft Stream。 Microsoft Graph 可跨这些连接的服务进行同步，以对所有组成员无缝提供访问权限。  
 
    **每个 Office 365 组都与一组默认的 Office 365 服务集成**

    ![图表显示 Office 365 组与文件、备注、任务、站点、对话和日历的集成](images/office365-groups-concept-overview-related-services-infographic.png)  

- 允许成员指示某个组是他们的[收藏夹](../api-reference/v1.0/api/group_addfavorite.md)之一，或者在他们选择时[将其从收藏夹中删除](../api-reference/v1.0/api/group_removefavorite.md)。 
- 从自定义应用程序中[创建](../api-reference/v1.0/api/group_post_conversations.md)、[获取](../api-reference/v1.0/api/group_get_conversation.md)或[删除](../api-reference/v1.0/api/group_delete_conversation.md)组对话。 
- 在组日历上计划日历[事件](../api-reference/v1.0/resources/event.md)。 
- 获取与组关联的 [SharePoint 网站](../api-reference/v1.0/resources/site.md)的相关信息，如文档库[列表](../api-reference/v1.0/api/list_list.md)或[子网站](../api-reference/v1.0/api/site_list_subsites.md)。 
- 在 Planner 中[创建一个属于组的计划](../api-reference/v1.0/api/planner_post_buckets.md)。 该计划通过允许[创建任务](../api-reference/v1.0/api/planner_post_tasks.md)（可以[跨存储桶进行组织](../api-reference/v1.0/api/planner_post_buckets.md)），提供了一种直观的方式来跟踪团队合作。 
- 访问与组关联的 [OneNote](../api-reference/v1.0/resources/onenote.md) 笔记本，这可用于收集会议记录和整理想法。 
  
    **Outlook 网页中的 Office 365 组和对话**

    ![Outlook 网页版在“组”文件夹中列出组的屏幕截图](images/office365-groups-concept-overview-groups-in-outlook.png) 

- [为 Microsoft Teams 启用组](../api-reference/beta/api/team_put_teams.md)（预览版），以允许组成员参与持久聊天。  
- [删除组](../api-reference/v1.0/api/group_delete.md)。 删除组时，所有关联的内容也会一并删除，从而防止孤立的站点、对话或计划。 
 
### <a name="manage-group-membership-seamlessly"></a>无缝管理组成员身份 
 
Office 365 组是共享 Microsoft 服务或你的应用中资源访问权限的用户集合。 由于组成员身份是集中管理的，因此，对成员身份的任何更改都会影响与该组关联的所有服务。 你可使用 Microsoft Graph 执行以下组成员身份任务：
 
- 从现有组中[添加](../api-reference/v1.0/api/group_post_members.md)和[删除](../api-reference/v1.0/api/group_delete_members.md)成员。 
- 获取组的[所有者列表](../api-reference/v1.0/api/group_list_owners.md)或[成员列表](../api-reference/v1.0/api/group_list_members.md)。 这有助于传达哪些人员可以访问组内容，或者哪些人员可能需要执行管理职责，如续订组或批准加入请求。 
- 通过[更新组](../api-reference/v1.0/api/group_update.md)操作，可将组指定为**公开**（其中组内容对同一组织中的任何人都可见），或者**私人**（其中组内容仅对成员可见）。 
- 从组所有者列表中[删除不再参与特定组所有权职责的所有者](../api-reference/v1.0/api/group_delete_owners.md)。 
 
### <a name="establish-and-maintain-group-policy-settings"></a>建立和维护组策略设置 
 
随着组织内创建的组数量开始增长，Microsoft Graph 支持管理组的使用情况和生命周期的能力。 你可以跨组织中的所有组强制执行组策略。 可以使用 Microsoft Graph API 执行以下操作：

- 配置广泛的[组策略设置](../api-reference/v1.0/resources/groupsetting.md)，从而帮助定义行为，例如，除非所有者续订组并对 Office 365 组强制执行命名策略，否则会自动删除组。 
- [续订](../api-reference/v1.0/api/group_renew.md)即将到期的组，以让团队成员继续协作和访问内容。 如果未根据已建立的过期策略续订组，则会自动删除该组。 
- [恢复](../api-reference/v1.0/api/directory_deleteditems_restore.md)已删除的组。
 
## <a name="next-steps"></a>后续步骤

- 在 [Graph Explorer](https://developer.microsoft.com/zh-CN/graph/graph-explorer) 中尝试一些示例 API 请求。 
- 详细了解如何在 Microsoft Graph 中[使用组 API](../api-reference/v1.0/resources/groups-overview.md)。
