---
title: 列出 windowsQualityUpdateProfiles
description: 列出 windowsQualityUpdateProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9d124e0db3cb13e529205f5cd939c16920c23b4b
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160241"
---
# <a name="list-windowsqualityupdateprofiles"></a>列出 windowsQualityUpdateProfiles

命名空间：microsoft.graph

> **重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象的属性和关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最高特权到最低特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsQualityUpdateProfiles
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 679

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
      "id": "76fc7b65-7b65-76fc-657b-fc76657bfc76",
      "displayName": "Display Name value",
      "description": "Description value",
      "expeditedUpdateSettings": {
        "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
        "qualityUpdateRelease": "Quality Update Release value",
        "daysUntilForcedReboot": 5
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```




