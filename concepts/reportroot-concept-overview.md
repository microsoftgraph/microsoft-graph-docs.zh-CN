# <a name="microsoft-graph-reports-api-overview"></a>Microsoft Graph 报告 API 概述

借助 Microsoft 365 管理中心中的使用情况报告，管理员可以了解其公司各 Office 365 服务的使用情况。 Microsoft Graph 中的报告 API 可用于与 Office 365 使用情况报告集成。

## <a name="why-use-the-reports-api"></a>为什么使用报告 API？

### <a name="integrate-office-365-usage-reporting-into-your-organizations-existing-reporting-solution"></a>将 Office 365 使用情况报告集成到组织的现有报告解决方案中
很多公司都有使用报告应用程序或 Web 门户的现有报告解决方案。 你可以使用报告 API 将 Office 365 使用情况数据并入组织的现有报告解决方案中，以便所有 IT 服务报告均位于统一位置。  

### <a name="retain-usage-reports-for-historical-analysis"></a>保留使用情况报告以供历史分析
你可以使用报告 API 获取所有使用情况报告中可用的数据，包括每个服务的组织级别的摘要、过去 7/30/90/180 天的实体级别（用户、网站和帐户）的使用情况信息和每日活动聚合。 这样，可以根据需要保留历史使用情况信息。

## <a name="what-data-can-i-access-by-using-the-reports-api"></a>使用报告 API 可以访问哪些数据？

你可以使用报告 API 访问下表中列出的数据集。

|Office 365 应用|数据集|
|:--------|:--------|
|Microsoft Teams|[设备使用情况](../api-reference/v1.0/resources/microsoft_teams_device_usage_reports.md)<br/>|[用户活动](../api-reference/v1.0/resources/microsoft_teams_user_activity_reports.md)|
|Office 365（常规） |[激活](../api-reference/v1.0/resources/office_365_activations_reports.md)<br/>[活动用户](../api-reference/v1.0/resources/office_365_active_users_reports.md)<br/>[组活动](../api-reference/v1.0/resources/office_365_groups_activity_reports.md)|
|OneDrive |[活动](../api-reference/v1.0/resources/onedrive_activity_reports.md)<br/>[使用情况](../api-reference/v1.0/resources/onedrive_usage_reports.md)|
|Outlook|[活动](../api-reference/v1.0/resources/email_activity_reports.md)<br/>[应用使用情况](../api-reference/v1.0/resources/email_app_usage_reports.md)<br/>[邮箱使用情况](../api-reference/v1.0/resources/mailbox_usage_reports.md)|
|SharePoint |[活动](../api-reference/v1.0/resources/sharepoint_activity_reports.md)<br/>[网站使用情况](../api-reference/v1.0/resources/sharepoint_site_usage_reports.md)|
|Skype for Business |[活动](../api-reference/v1.0/resources/skype_for_business_activity_reports.md)<br/>[设备使用情况](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[设备使用情况](../api-reference/v1.0/resources/skype_for_business_device_usage_reports.md)<br/>[参与者活动](../api-reference/v1.0/resources/skype_for_business_participant_activity_reports.md)<br/>[对等活动](../api-reference/v1.0/resources/skype_for_business_peer_to_peer_activity.md)|
|Yammer |[活动](../api-reference/v1.0/resources/yammer_activity_reports.md)<br/>[设备使用情况](../api-reference/v1.0/resources/yammer_device_usage_reports.md)<br/>[组活动](../api-reference/v1.0/resources/yammer_groups_activity_reports.md)|

## <a name="next-steps"></a>后续步骤

* 请在 [Graph 浏览器](https://developer.microsoft.com/zh-CN/graph/graph-explorer)中探索 API。
* 了解有关如何[使用报告 REST API](../api-reference/v1.0/resources/report.md) 的详细信息。
