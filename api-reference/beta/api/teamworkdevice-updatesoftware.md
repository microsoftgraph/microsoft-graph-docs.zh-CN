---
title: teamworkDevice： updateSoftware
description: 更新启用了 Microsoft Teams 的设备的软件。
author: adsrivastava2
ms.localizationpriority: medium
ms.prod: teamwork
doc_type: apiPageType
ms.openlocfilehash: 9e2435dc52b88e836874ceae1b3e62bd09fdaec5
ms.sourcegitcommit: e4796212a2e8bbec61b6da8336f776c0305c49df
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/28/2022
ms.locfileid: "62262454"
---
# <a name="teamworkdevice-updatesoftware"></a>teamworkDevice： updateSoftware
命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新启用了 Microsoft Teams 的设备[的软件](../resources/teamworkdevice.md)。 此 API 将触发长时间运行的操作。

[!INCLUDE [teamworkdevice-api-disclaimer](../../includes/teamworkdevice-api-disclaimer.md)]

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型|权限（从最低特权到最高特权）|
|:---|:---|
|委派（工作或学校帐户）|TeamworkDevice.ReadWrite.All|
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|TeamworkDevice.ReadWrite.All|

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /teamwork/devices/{teamworkDeviceId}/updateSoftware
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

|参数|类型|说明|
|:---|:---|:---|
|softwareType|teamworkSoftwareType|要更新的软件类型。 有效类型为：、`adminAgent`、`operatingSystem`、`firmware``teamsClient`、`partnerAgent`、`companyPortal`。|
|softwareVersion|String|指定可供更新的软件版本。|



## <a name="response"></a>响应

如果成功，此方法返回 `202 Accepted` 响应代码。 响应还将包含标头 `Location` ，其中包含 [teamworkDeviceOperation 资源](../resources/teamworkdeviceoperation.md) 的位置。 可以通过对此位置进行 GET 请求来检查软件更新操作的状态，该位置将返回操作是 、 `queued``succeeded`或 `failed`。

如果操作已进入排队 `409 Conflict` 状态，此方法还会返回 响应代码。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "teamworkdevice_updatesoftware"
}
-->
``` http
POST https://graph.microsoft.com/beta/teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/updateSoftware
Content-Type: application/json
Content-length: 64

{
  "softwareType": "teamsClient",
  "softwareVersion": "1.0.96.22"
}
```


### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Location: /teamwork/devices/0f3ce432-e432-0f3c-32e4-3c0f32e43c0f/operations/119eb06d-0c4b-4fb3-a754-33dd0d6b618c
Content-Type: text/plain
Content-Length: 0
```

