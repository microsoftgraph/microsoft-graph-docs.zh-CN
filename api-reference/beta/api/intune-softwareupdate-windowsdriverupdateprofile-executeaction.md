---
title: executeAction 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fb4a283d2954e0e37828475635727f3fcd6ffe62
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61344650"
---
# <a name="executeaction-action"></a>executeAction 操作

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="prerequisites"></a>先决条件
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|DeviceManagementConfiguration.Read.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|DeviceManagementConfiguration.Read.All|

## <a name="http-request"></a>HTTP 请求
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/executeAction
```

## <a name="request-headers"></a>请求标头
|标头|值|
|:---|:---|
|Authorization|Bearer &lt;token&gt;。必需。|
|接受|application/json|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|属性|类型|说明|
|:---|:---|:---|
|actionName|[driverApprovalAction](../resources/intune-softwareupdate-driverapprovalaction.md)|尚未记录|
|driverIds|String collection|尚未记录|
|deploymentDate|DateTimeOffset|尚未记录|



## <a name="response"></a>响应
如果成功，此操作在响应正文中返回 响应代码和 `200 OK` [bulkDriverActionResult。](../resources/intune-softwareupdate-bulkdriveractionresult.md)

## <a name="example"></a>示例

### <a name="request"></a>请求
下面是一个请求示例。
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsDriverUpdateProfiles/{windowsDriverUpdateProfileId}/executeAction

Content-type: application/json
Content-length: 137

{
  "actionName": "decline",
  "driverIds": [
    "Driver Ids value"
  ],
  "deploymentDate": "2016-12-31T23:58:18.3419405-08:00"
}
```

### <a name="response"></a>响应
下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 298

{
  "value": {
    "@odata.type": "microsoft.graph.bulkDriverActionResult",
    "successfulDriverIds": [
      "Successful Driver Ids value"
    ],
    "failedDriverIds": [
      "Failed Driver Ids value"
    ],
    "notFoundDriverIds": [
      "Not Found Driver Ids value"
    ]
  }
}
```




