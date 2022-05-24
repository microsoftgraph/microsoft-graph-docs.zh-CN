---
title: 更新设置
description: 更新SharePoint和OneDrive的一个或多个租户级别设置。
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 07abcd226649c175fe6906a3b15e14971d8e9cf7
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653612"
---
# <a name="update-settings"></a>更新设置
命名空间：microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新SharePoint和OneDrive的一个或多个租户级别[设置](../resources/tenantadmin-settings.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|SharePointTenantSettings.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|SharePointTenantSettings.ReadWrite.All|

代表用户调用时，用户需要属于以下管理员角色之一。 若要详细了解管理员角色，请参阅[Microsoft 365 管理中心中的管理员角色](/microsoft-365/admin/add-users/about-admin-roles)：
* 全局管理员
* SharePoint 管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /admin/sharepoint/settings
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
[!INCLUDE [table-intro](../../includes/update-property-table-intro.md)]
下表显示了可为设置对象编辑 [的](../resources/tenantadmin-settings.md) 属性。

|属性|类型|说明|
|:---|:---|:---|
| allowedDomainGuidsForSyncApp                       | GUID 集合              | OneDrive 同步应用的受信任域 GUID 的集合。                                                                                                                                                  |
| deletedUserPersonalSiteRetentionPeriodInDays       | Int32                        | 保留已删除用户OneDrive的天数。                                                                                                                                                   |
| excludedFileExtensionsForSyncApp                   | String collection            | OneDrive 同步应用未上传的文件扩展名的集合。                                                                                                                                           |
| imageTaggingOption                                 | imageTaggingChoice           | 指定租户的图像标记选项。 可取值为：`disabled`、`basic`、`enhanced`。                                                                                                       |
| isCommentingOnSitePagesEnabled                     | Boolean                      | 指示是否允许在SharePoint的新式网站页面上使用注释。                                                                                                                                          |
| isFileActivityNotificationEnabled                  | Boolean                      | 指示是否为OneDrive事件启用推送通知。                                                                                                                                               |
| isLoopEnabled                                      | Boolean                      | 指示是否允许在SharePoint网站上Fluid Framework。                                                                                                                                                   |
| isMacSyncAppEnabled                                | Boolean                      | 指示是否可以使用适用于 Mac 的OneDrive 同步应用同步文件。                                                                                                                                          |
| isResharingByExternalUsersEnabled                  | Boolean                      | 指示是否允许来宾重新共享他们不拥有的文件、文件夹和网站。                                                                                                                           |
| isSharePointMobileNotificationEnabled              | Boolean                      | 指示是否为SharePoint启用了移动推送通知。                                                                                                                                             |
| isSharePointNewsfeedEnabled                        | Boolean                      | 指示是否允许在SharePoint的新式网站页面上使用新闻源。                                                                                                                                   |
| isSiteCreationEnabled                              | Boolean                      | 指示是否允许用户创建网站。                                                                                                                                                           |
| isSiteCreationUIEnabled                            | Boolean                      | 指示是否显示用于创建网站的 UI 命令。                                                                                                                                                     |
| isSitePagesCreationEnabled                         | Boolean                      | 指示是否允许在SharePoint网站上创建新的新式页面。                                                                                                                                         |
| isSitesStorageLimitAutomatic                       | Boolean                      | 指示站点存储空间是自动管理的还是每个站点是否设置了特定的存储限制。                                                                                                       |
| isSyncButtonHiddenOnPersonalSite                   | Boolean                      | 指示是否隐藏OneDrive中的同步按钮。                                                                                                                                                            |
| isUnmanagedSyncAppForTenantRestricted              | Boolean                      | 指示是否允许用户仅在已加入特定域的电脑上同步文件。                                                                                                                           |
| personalSiteDefaultStorageLimitInMB                | Int64                        | 为所有分配了限定许可证的新用户和现有用户的默认OneDrive存储限制。 以兆字节为单位 (MB) 。                                                                           |
| sharingAllowedDomainList                           | String collection            | 允许在组织外部共享的电子邮件域的集合。                                                                                                                              |
| sharingBlockedDomainList                           | String collection            | 阻止在组织外部共享的电子邮件域的集合。                                                                                                                              |
| sharingCapability                                  | sharingCapabilities          | 租户的共享功能。 可能的值是：`disabled`、`externalUserSharingOnly`、`externalUserAndGuestSharing`、`existingExternalUserSharingOnly`。                                                |
| sharingDomainRestrictionMode                       | sharingDomainRestrictionMode | 指定域的外部共享模式。 可取值为：`none`、`allowList`、`blockList`。                                                                                                        |
| siteCreationDefaultManagedPath                     | String                       | 团队网站托管路径的值。 这是创建新团队网站的路径。                                                                                                          |
| siteCreationDefaultStorageLimitInMB                | Int32                        | 创建新站点时的默认存储配额。 以兆字节为单位 (MB) 。                                                                                                                            |
| tenantDefaultTimezone                              | String                       | 新创建的站点的租户的默认时区。                                                                                                                                                      |




## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [设置](../resources/tenantadmin-settings.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "update_tenant_settings"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/admin/sharepoint/settings
Content-Type: application/json
Content-length: 1323

{
    "deletedUserPersonalSiteRetentionPeriodInDays": 365,
    "excludedFileExtensionsForSyncApp": [".mp3"],
    "imageTaggingOption": "enhanced",
    "isSitesStorageLimitAutomatic": false,
    "isSyncButtonHiddenOnPersonalSite": false,
    "isUnmanagedSyncAppForTenantRestricted": false,
    "personalSiteDefaultStorageLimitInMB": 120000
}
```


### <a name="response"></a>响应

下面展示了示例响应。

>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tenantAdmin.settings"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.tenantAdmin.settings",
    "id": "e79403fa-abdf-af49-56c5-f7119d8b1948",
    "allowedDomainGuidsForSyncApp": [
        "bdd1ab9b-3fd0-4def-a761-ec8d7471732c", 
        "ad31vb6b-5zd0-7tyg-m231-kj8d6578432c"
    ],
    "availableManagedPathsForSiteCreation": [
        "/sites/",
        "/teams/"
    ],
    "deletedUserPersonalSiteRetentionPeriodInDays": 365,
    "excludedFileExtensionsForSyncApp": [
        ".mp3"
    ],
    "imageTaggingOption": "basic",
    "isCommentingOnSitePagesEnabled": true,
    "isFileActivityNotificationEnabled": true,
    "isLoopEnabled": true,
    "isMacSyncAppEnabled": false,
    "isResharingByExternalUsersEnabled": true,
    "isSharePointMobileNotificationEnabled": true,
    "isSharePointNewsfeedEnabled": true,
    "isSiteCreationEnabled": true,
    "isSiteCreationUIEnabled": true,
    "isSitePagesCreationEnabled": true,
    "isSitesStorageLimitAutomatic": false,
    "isSyncButtonHiddenOnPersonalSite": false,
    "isUnmanagedSyncAppForTenantRestricted": false,
    "personalSiteDefaultStorageLimitInMB": 120000,
    "sharingAllowedDomainList" : [
        "contoso.com",
        "fabrikam.com"
    ],
    "sharingBlockedDomainList" : [
        "contoso.com",
        "fabrikam.com"
    ],
    "sharingCapability": "externalUserAndGuestSharing",
    "sharingDomainRestrictionMode": "allowList",
    "siteCreationDefaultManagedPath": "/sites/",
    "siteCreationDefaultStorageLimitInMB": 808034,
    "tenantDefaultTimezone": "(UTC-05:00) Eastern Time (US and Canada)"
}
```
