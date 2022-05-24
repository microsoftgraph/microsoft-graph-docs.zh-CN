---
title: 获取设置
description: 获取SharePoint和OneDrive的租户级别设置。
author: liamfernandez
ms.localizationpriority: medium
ms.prod: files
doc_type: apiPageType
ms.openlocfilehash: 2111ff6b45149a133de0022d50dd92042c0c3d60
ms.sourcegitcommit: 10b45b3e666bf6b438803885128bc2f0fa2fa994
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/24/2022
ms.locfileid: "65653600"
---
# <a name="get-settings"></a>获取设置
命名空间：microsoft.graph.tenantAdmin

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取SharePoint和OneDrive的租户级别[设置](../resources/tenantadmin-settings.md)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|SharePointTenantSettings.Read.All、SharePointTenantSettings.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|SharePointTenantSettings.Read.All、SharePointTenantSettings.ReadWrite.All|

代表用户调用时，用户需要属于以下管理员角色之一。 若要详细了解管理员角色，请参阅[Microsoft 365 管理中心中的管理员角色](/microsoft-365/admin/add-users/about-admin-roles)：
* 全局管理员
* 全局读取者
* SharePoint 管理员

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /admin/sharepoint/settings
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持一些 OData 查询参数来帮助自定义响应。 若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [设置](../resources/tenantadmin-settings.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

请求示例如下所示。

<!-- {
  "blockType": "request",
  "name": "get_settings"
}
-->
``` http
GET https://graph.microsoft.com/beta/admin/sharepoint/settings
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
    "value": {
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
        "deletedUserPersonalSiteRetentionPeriodInDays": 344,
        "excludedFileExtensionsForSyncApp": [
            ".md", 
            ".git"
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
        "isSitesStorageLimitAutomatic": true,
        "isSyncButtonHiddenOnPersonalSite": true,
        "isUnmanagedSyncAppForTenantRestricted": true,
        "personalSiteDefaultStorageLimitInMB": 113664,
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
}
```

