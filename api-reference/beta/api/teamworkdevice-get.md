---
title: 获取 teamworkDevice
description: 获取启用Microsoft Teams设备的属性，包括设备类型、硬件详细信息、活动状态和运行状况状态信息。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 2c77cf72923593ef42f36280046809453c20f305
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262430"
---
# <a name="get-teamworkdevice"></a>获取 teamworkDevice
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取启用Microsoft Teams的设备[的属性](../resources/teamworkdevice.md)。 例如，可以使用此方法获取为设备启用的设备的设备类型、硬件详细信息、活动状态和运行状况Teams。

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
GET /teamwork/devices/{teamworkDeviceId}
```

## <a name="optional-query-parameters"></a>可选的查询参数
此操作支持使用 `$select` [OData 查询参数](/graph/query-parameters) 自定义响应。

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [teamworkDevice](../resources/teamworkdevice.md) 对象。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "get_teamworkdevice"
}
-->
``` http
GET https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f
```


### <a name="response"></a>响应
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkDevice"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.teamworkDevice",
    "id": "0f3ce432-e432-0f3c-32e4-3c0f32e43c0f",
    "deviceType": "CollaborationBar",
    "hardwareDetail": {
      "serialNumber": "0189",
      "uniqueId": "5abcdefgh",
      "macAddresses": [],
      "manufacturer": "yealink",
      "model": "vc210"
    },
    "notes": "CollaborationBar device.",
    "companyAssetTag": "Tag1",
    "healthStatus": "Healthy",
    "activityState": "Idle",
    "createdDateTime": "2021-06-19T19:01:04.185Z",
    "createdBy": null,
    "lastModifiedDateTime": "2021-06-19T19:01:04.185Z",
    "lastModifiedBy": null,
    "currentUser": {
      "id": "2a610f6f-adf6-4205",
      "displayName": "Evan Lewis",
      "userIdentityType": "aadUser"
    }
  }
}
```

