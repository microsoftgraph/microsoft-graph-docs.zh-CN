---
title: 获取设备命令状态
description: 获取设备上的命令的状态。 状态代码的完整列表，请参阅 actionStatus 的列表。
localization_priority: Normal
ms.openlocfilehash: 9dca743a50f248abee76fb4d54352df3d400ada1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883130"
---
# <a name="get-device-command-status"></a>获取设备命令状态

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

获取设备上的命令的状态。 状态代码的完整列表，请参阅[actionStatus 的列表](#list-of-actionstatus)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。    |
|委派（个人 Microsoft 帐户） | Device.Command    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/commands/{id}
```

## <a name="request-headers"></a>请求标头

| 标头 |值
|:----|:------|
|Authorization| Bearer {token}。必需。 |
|Accept | application/json |

## <a name="response"></a>响应
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
  {
    "id": "0",
    "status": "requesting",
    "type": "null",
    "appServiceName": "null",
    "packageFamilyName": "null",
    "error": "null",
    "responsepayload": "null",
    "payload": "null",
    "permissionTicket": "null",
    "postBackUri": "null"
  }
```

## <a name="list-of-actionstatus"></a>ActionStatus 的列表

- 请求，/ / 命令已创建并正在等待处理
- sentToTarget，/ / 命令已发送到目标设备
- 执行 / / 目标设备确认收到该命令，并且正在执行它
- 完成，/ / 命令执行完毕
- failedToSend，/ / 服务未能发送到目标设备命令
- executionFailed，/ / 命令执行失败
- commandDropped，/ / 命令而丢弃客户端设备是否处于 ConnectedStandby 状态
- 取消，/ / 取消命令
- 正在取消，/ / 取消该命令
- canceled、 / / 命令已被取消
- 重试，/ / 服务正在重试发送到目标的命令
- 过期，/ / 命令处理超过到期时间
- 错误: / / 内部处理命令时的错误
- 自定义 / / 自定义状态

## <a name="example"></a>示例

本示例中，您需要的设备 ID 和的命令的已颁发的设备 ID。 对的设备时发出 GET 返回 ID 调用`/me/devices`，并执行 POST 时，则返回 ID 的命令对调用`/me/devices/{id}/command`。

#### <a name="request"></a>请求

下面为请求示例。

<!-- {
  "blockType": "ignored",
  "name": "get_command"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>响应

以下示例显示了相应的响应。
<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "value":
  {
    "id": "0158355AD4D680CC4E2994CC009EFFD7337D1335FCA6ED266…",
    "status": "completed",
    "type": null,
    "appServiceName": null,
    "packageFamilyName": null,
    "error": null,
    "permissionTicket": null,
    "postBackUri": null,
    "payload": null
  }
}
```


## <a name="get-command-payload"></a>获取命令负载

获取响应负载设备上的特定操作。 响应负载用于查询应用程序服务时返回带数据。


### <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。    |
|委派（个人 Microsoft 帐户） | Device.Command    |
|应用程序 | 不支持。 |

### <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET me/devices/{id}/command/{id}/responsePayload
```

### <a name="request-headers"></a>请求标头

| 标头 |值
|:----|:------|
|Authorization| Bearer {token}。必需。 |
|Accept | application/json |

### <a name="response"></a>响应
<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```
<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"date-time",
  "Type":"Ok"
}
```

### <a name="example"></a>示例

本示例中，您需要的设备 ID 和的命令的已颁发的设备 ID。 在呼叫的设备时发出 GET 返回 ID `/me/devices`，并执行 POST 时，则返回 ID 的命令对调用`/me/devices/{id}/command`。

#### <a name="request"></a>请求

下面为请求示例。

<!-- { 
  "blockType": "ignored",
  "name": "get_command_payload"
} -->
```http
GET me/devices/{id}/commands/{id}
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>响应

以下示例显示了相应的响应。

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK

{
  "@odata.context": "https://graph.microsoft.com/devices/$metadata#microsoft.graph.PayloadResponse",
  "MsIgnoredParameter":0,
  "CreationDate":"04/27/2017",
  "Type":"Ok"
}
```
