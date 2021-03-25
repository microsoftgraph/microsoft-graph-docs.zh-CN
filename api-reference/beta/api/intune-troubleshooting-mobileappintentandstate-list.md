---
title: 列出 mobileAppIntentAndStates
description: 列出 mobileAppIntentAndState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9102dc877103e2965f0f99f3ad974e5e3dfd4b73
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51151842"
---
# <a name="list-mobileappintentandstates"></a>列出 mobileAppIntentAndStates

命名空间：microsoft.graph

> **重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

列出 [mobileAppIntentAndState 对象的属性和](../resources/intune-troubleshooting-mobileappintentandstate.md) 关系。

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应
如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) 对象集合。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1001

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
      "id": "45a775d6-75d6-45a7-d675-a745d675a745",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "mobileAppList": [
        {
          "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
          "applicationId": "Application Id value",
          "displayName": "Display Name value",
          "mobileAppIntent": "notAvailable",
          "displayVersion": "Display Version value",
          "installState": "failed",
          "supportedDeviceTypes": [
            {
              "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
              "type": "windowsRT",
              "minimumOperatingSystemVersion": "Minimum Operating System Version value",
              "maximumOperatingSystemVersion": "Maximum Operating System Version value"
            }
          ]
        }
      ]
    }
  ]
}
```




