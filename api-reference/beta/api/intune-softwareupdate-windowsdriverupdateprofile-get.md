---
title: 获取 windowsDriverUpdateProfile
description: 读取 windowsDriverUpdateProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad92ae756c73eae2349a5a39546745be8c93928b
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2022
ms.locfileid: "64630434"
---
# <a name="get-windowsdriverupdateprofile"></a>获取 windowsDriverUpdateProfile

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

读取 [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应 `200 OK` 代码和 [windowsDriverUpdateProfile](../resources/intune-softwareupdate-windowsdriverupdateprofile.md) 对象。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 782

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDriverUpdateProfile",
    "id": "55bcc52a-c52a-55bc-2ac5-bc552ac5bc55",
    "displayName": "Display Name value",
    "description": "Description value",
    "approvalType": "automatic",
    "deviceReporting": 15,
    "newUpdates": 10,
    "deploymentDeferralInDays": 8,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "inventorySyncStatus": {
      "@odata.type": "microsoft.graph.windowsDriverUpdateProfileInventorySyncStatus",
      "lastSuccessfulSyncDateTime": "2017-01-01T00:03:28.120883-08:00",
      "driverInventorySyncState": "success"
    }
  }
}
```




