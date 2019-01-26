---
title: 在 Microsoft Graph 中使用 Office 365 使用情况报表
description: 通过 Microsoft Graph，可以访问 Office 365 使用情况报表资源，了解企业用户的 Office 365 服务使用情况。 例如，可以发现大量使用服务且要达到配额的用户，也可以发现可能完全不需要 Office 365 许可证的用户。
localization_priority: Priority
ms.prod: reports
ms.openlocfilehash: 3f389aa241d463bc906408e965a01482824a7084
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509152"
---
# <a name="working-with-office-365-usage-reports-in-microsoft-graph"></a>在 Microsoft Graph 中使用 Office 365 使用情况报表

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过 Microsoft Graph，可以访问 Office 365 使用情况报表资源，了解企业用户的 Office 365 服务使用情况。 例如，可以发现大量使用服务且要达到配额的用户，也可以发现可能完全不需要 Office 365 许可证的用户。

## <a name="authorization"></a>授权

Microsoft Graph 通过权限控制对资源的访问。 必须指定访问报表资源所需的权限。 通常是在 Azure Active Directory (Azure AD) 门户中指定权限。 有关详细信息，请参阅 [Microsoft Graph 权限参考](/graph/permissions-reference)和[报表权限](/graph/permissions-reference#reports-permissions)。

## <a name="changes-to-the-reports-apis"></a>对报告 API 所做的更改

已更新原始报告 API，因此你可以为所需的特定视图调用 API，而不是传递视图参数。 我们建议你尽快开始在应用程序中使用新 API。 下表列出了已删除的 API 以及替换它们的新 API。

| 原始 API            | 新 API                                  |
| :---------------------- | :--------------------------------------- |
| EmailActivity           | <ul><li>[getEmailActivityUserDetail](../api/reportroot-getemailactivityuserdetail.md)</li><li>[getEmailActivityCounts](../api/reportroot-getemailactivitycounts.md)</li><li>[getEmailActivityUserCounts](../api/reportroot-getemailactivityusercounts.md)</li></ul> |
| EmailAppUsage           | <ul><li>[getEmailAppUsageUserDetail](../api/reportroot-getemailappusageuserdetail.md)</li><li>[getEmailAppUsageAppsUserCounts](../api/reportroot-getemailappusageappsusercounts.md)</li><li>[getEmailAppUsageUserCounts](../api/reportroot-getemailappusageusercounts.md)</li><li>[getEmailAppUsageVersionsUserCounts](../api/reportroot-getemailappusageversionsusercounts.md)</li></ul> |
| MailboxUsage            | <ul><li>[getMailboxUsageDetail](../api/reportroot-getmailboxusagedetail.md)</li><li>[getMailboxUsageMailboxCounts](../api/reportroot-getmailboxusagemailboxcounts.md)</li><li>[getMailboxUsageQuotaStatusMailboxCounts](../api/reportroot-getmailboxusagequotastatusmailboxcounts.md)</li><li>[getMailboxUsageStorage](../api/reportroot-getmailboxusagestorage.md)</li></ul> |
| Office365Activations    | <ul><li>[getOffice365ActivationsUserDetail](../api/reportroot-getoffice365activationsuserdetail.md)</li><li>[getOffice365ActivationCounts](../api/reportroot-getoffice365activationcounts.md)</li><li>[getOffice365ActivationsUserCounts](../api/reportroot-getoffice365activationsusercounts.md)</li></ul> |
| Office365ActiveUser     | <ul><li>[getOffice365ActiveUserDetail](../api/reportroot-getoffice365activeuserdetail.md)</li><li>[getOffice365ActiveUserCounts](../api/reportroot-getoffice365activeusercounts.md)</li><li>[getOffice365ServicesUserCounts](../api/reportroot-getoffice365servicesusercounts.md)</li></ul> |
| Office365GroupsActivity | <ul><li>[getOffice365GroupsActivityDetail](../api/reportroot-getoffice365groupsactivitydetail.md)</li><li>[getOffice365GroupsActivityCounts](../api/reportroot-getoffice365groupsactivitycounts.md)</li><li>[getOffice365GroupsActivityGroupCounts](../api/reportroot-getoffice365groupsactivitygroupcounts.md)</li><li>[getOffice365GroupsActivityStorage](../api/reportroot-getoffice365groupsactivitystorage.md)</li><li>[getOffice365GroupsActivityFileCounts](../api/reportroot-getoffice365groupsactivityfilecounts.md)</li></ul> |
| OneDriveActivity        | <ul><li>[getOneDriveActivityUserDetail](../api/reportroot-getonedriveactivityuserdetail.md)</li><li>[getOneDriveActivityUserCounts](../api/reportroot-getonedriveactivityusercounts.md)</li><li>[getOneDriveActivityFileCounts](../api/reportroot-getonedriveactivityfilecounts.md)</li></ul> |
| OneDriveUsage           | <ul><li>[getOneDriveUsageAccountDetail](../api/reportroot-getonedriveusageaccountdetail.md)</li><li>[getOneDriveUsageAccountCounts](../api/reportroot-getonedriveusageaccountcounts.md)</li><li>[getOneDriveUsageFileCounts](../api/reportroot-getonedriveusagefilecounts.md)</li><li>[getOneDriveUsageStorage](../api/reportroot-getonedriveusagestorage.md)</li></ul> |
| SharePointActivity      | <ul><li>[getSharePointActivityUserDetail](../api/reportroot-getsharepointactivityuserdetail.md)</li><li>[getSharePointActivityFileCounts](../api/reportroot-getsharepointactivityfilecounts.md)</li><li>[getSharePointActivityUserCounts](../api/reportroot-getsharepointactivityusercounts.md)</li><li>[getSharePointActivityPages](../api/reportroot-getsharepointactivitypages.md)</li></ul> |
| SharePointSiteUsage     | <ul><li>[getSharePointSiteUsageDetail](../api/reportroot-getsharepointsiteusagedetail.md)</li><li>[getSharePointSiteUsageFileCounts](../api/reportroot-getsharepointsiteusagefilecounts.md)</li><li>[getSharePointSiteUsageSiteCounts](../api/reportroot-getsharepointsiteusagesitecounts.md)</li><li>[getSharePointSiteUsageStorage](../api/reportroot-getsharepointsiteusagestorage.md)</li><li>[getSharePointSiteUsagePages](../api/reportroot-getsharepointsiteusagepages.md)</li></ul> |
| SfbActivity             | <ul><li>[getSkypeForBusinessActivityUserDetail](../api/reportroot-getskypeforbusinessactivityuserdetail.md)</li><li>[getSkypeForBusinessActivityCounts](../api/reportroot-getskypeforbusinessactivitycounts.md)</li><li>[getSkypeForBusinessActivityUserCounts](../api/reportroot-getskypeforbusinessactivityusercounts.md)</li></ul> |
| SfbDeviceUsage          | <ul><li>[getSkypeForBusinessDeviceUsageUserDetail](../api/reportroot-getskypeforbusinessdeviceusageuserdetail.md)</li><li>[getSkypeForBusinessDeviceUsageDistributionUserCounts](../api/reportroot-getskypeforbusinessdeviceusagedistributionusercounts.md)</li><li>[getSkypeForBusinessDeviceUsageUserCounts](../api/reportroot-getskypeforbusinessdeviceusageusercounts.md)</li></ul> |
| SfbOrganizerActivity    | <ul><li>[getSkypeForBusinessOrganizerActivityCounts](../api/reportroot-getskypeforbusinessorganizeractivitycounts.md)</li><li>[getSkypeForBusinessOrganizerActivityUserCounts](../api/reportroot-getskypeforbusinessorganizeractivityusercounts.md)</li><li>[getSkypeForBusinessOrganizerActivityMinuteCounts](../api/reportroot-getskypeforbusinessorganizeractivityminutecounts.md)</li></ul> |
| SfbParticipantActivity  | <ul><li>[getSkypeForBusinessParticipantActivityCounts](../api/reportroot-getskypeforbusinessparticipantactivitycounts.md)</li><li>[getSkypeForBusinessParticipantActivityUserCounts](../api/reportroot-getskypeforbusinessparticipantactivityusercounts.md)</li><li>[getSkypeForBusinessParticipantActivityMinuteCounts](../api/reportroot-getskypeforbusinessparticipantactivityminutecounts.md)</li></ul> |
| SfbP2PActivity          | <ul><li>[getSkypeForBusinessPeerToPeerActivityCounts](../api/reportroot-getskypeforbusinesspeertopeeractivitycounts.md)</li><li>[getSkypeForBusinessPeerToPeerActivityUserCounts](../api/reportroot-getskypeforbusinesspeertopeeractivityusercounts.md)</li><li>[getSkypeForBusinessPeerToPeerActivityMinuteCounts](../api/reportroot-getskypeforbusinesspeertopeeractivityminutecounts.md)</li></ul> |
| YammerActivity          | <ul><li>[getYammerActivityUserDetail](../api/reportroot-getyammeractivityuserdetail.md)</li><li>[getYammerActivityCounts](../api/reportroot-getyammeractivitycounts.md)</li><li>[getYammerActivityUserCounts](../api/reportroot-getyammeractivityusercounts.md)</li></ul> |
| YammerDeviceUsage       | <ul><li>[getYammerDeviceUsageUserDetail](../api/reportroot-getyammerdeviceusageuserdetail.md)</li><li>[getYammerDeviceUsageDistributionUserCounts](../api/reportroot-getyammerdeviceusagedistributionusercounts.md)</li><li>[getYammerDeviceUsageUserCounts](../api/reportroot-getyammerdeviceusageusercounts.md)</li></ul> |
| YammerGroupsActivity    | <ul><li>[getYammerGroupsActivityDetail](../api/reportroot-getyammergroupsactivitydetail.md)</li><li>[getYammerGroupsActivityGroupCounts](../api/reportroot-getyammergroupsactivitygroupcounts.md)</li><li>[getYammerGroupsActivityCounts](../api/reportroot-getyammergroupsactivitycounts.md)</li></ul> |

## <a name="next-steps"></a>后续步骤

借助报表资源和 API，可以通过新方式使用 Microsoft Graph 与用户进行交互，并管理他们的用户体验。 若要了解详细信息：

- 深入了解对方案最有帮助的资源的方法和属性。
- 尝试在 [Graph 浏览器](https://developer.microsoft.com/graph/graph-explorer)中调用 API。

需要更多灵感？请参阅[我们的一些合作伙伴如何使用 Microsoft Graph](https://developer.microsoft.com/graph/graph/examples#partners)。
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/report.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
