---
title: 获取 teamworkDeviceActivity
description: 获取已启用Microsoft Teams的活动状态。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 39c67adc760d2e04668790621ed927cdacf80eca
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347420"
---
# <a name="get-teamworkdeviceactivity"></a>获取 teamworkDeviceActivity
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取[已启用Microsoft Teams](../resources/teamworkdeviceactivity.md)的活动[状态](../resources/teamworkdevice.md)。 

[!INCLUDE [teamworkdevice-api-disclaimer](../../includes/teamworkdevice-api-disclaimer.md)]

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|TeamworkDevice.Read.All、TeamworkDevice.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|TeamworkDevice.Read.All、TeamworkDevice.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /teamwork/devices/{teamworkDeviceId}/activity
```

## <a name="optional-query-parameters"></a>可选的查询参数
此操作支持 使用 `$select` 和 `$expand` [OData 查询参数](/graph/query-parameters) 自定义响应。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [teamworkDeviceActivity](../resources/teamworkdeviceactivity.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_teamworkdeviceactivity"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/1ae3fe60-fe60-1ae3-60fe-e31a60fee31a/activity
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-teamworkdeviceactivity-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-teamworkdeviceactivity-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-teamworkdeviceactivity-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-teamworkdeviceactivity-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/get-teamworkdeviceactivity-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/get-teamworkdeviceactivity-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDeviceActivity"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDeviceActivity",
    "id": "1ae3fe60-fe60-1ae3-60fe-e31a60fee31a",
    "activePeripherals": {
      "roomCamera": null,
      "contentCamera": null,
      "speaker": {
        "id": "Headset Earphone (Logitech SmartDock)",
        "displayName": "Headset Earphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
      "communicationSpeaker": {
        "id": "Headset Earphone (Logitech SmartDock)",
        "displayName": "Headset Earphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
      "microphone": {
        "id": "Headset Microphone (Logitech SmartDock)",
        "displayName": "Headset Microphone (Logitech SmartDock)",
        "vendorId": "VID_046D",
        "productId": "PID_0864"
      },
    },
    "createdDateTime": "2021-03-19T19:00:04.000Z",
    "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
    "createdBy": null,
    "lastModifiedBy": null
  }
}
```

