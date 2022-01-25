---
title: '获取设备命令状态 (已弃) '
description: 获取设备上命令的状态。 有关状态代码的完整列表，请参阅 actionStatus 列表。
ms.localizationpriority: medium
doc_type: apiPageType
author: ailae
ms.prod: ''
ms.openlocfilehash: bbe26243c9779e7917e4014038b26473a7cd17f7
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201311"
---
# <a name="get-device-command-status-deprecated"></a>获取设备命令状态 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取设备上命令的状态。 有关状态代码的完整列表，请参阅 [list of actionStatus](#list-of-actionstatus)。

> [!CAUTION]
> 此 API 已弃用，在 2020 年 9 月 30 日停止返回数据。

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
|接受 | application/json |

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

## <a name="list-of-actionstatus"></a>actionStatus 列表

- requesting， // Command has been created and is waiting to be processed
- sentToTarget，// 命令已发送到目标设备
- 执行， // 目标设备确认收到命令并正在执行该命令
- 已完成，// 命令执行已完成
- failedToSend，// 服务无法将命令发送到目标设备
- executionFailed，// 命令执行失败
- commandDropped，// 如果设备位于 ConnectedStandby 状态，客户端丢弃的命令
- cancel、// Cancel the command
- cancelling，// Cancelling the command
- 已取消，// 命令已取消
- retry，// 服务正在重试向目标发送命令
- expired， // Command processing exceeded expiry time
- 错误，// 处理命令时出现内部错误
- 自定义 // 自定义状态

## <a name="example"></a>示例

在此例中，你将需要设备的 ID 和已颁发给设备的命令的 ID。 发出 GET 调用时，将返回设备 ID，对 执行 POST 调用时将 `/me/devices` 返回命令 `/me/devices/{id}/command` ID。

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
  "@odata.type": "microsoft.graph.command",
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


## <a name="get-command-payload"></a>获取命令有效负载

获取设备上特定操作的响应有效负载。 查询应用服务以返回数据时，会使用响应有效负载。


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
GET me/devices/{id}/commands/{id}/responsePayload
```

### <a name="request-headers"></a>请求标头

| 标头 |值
|:----|:------|
|Authorization| Bearer {token}。必需。 |
|接受 | application/json |

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

在此例中，你将需要设备的 ID 和已颁发给设备的命令的 ID。 在 上发出 GET 调用时，将返回设备 ID，对 执行 POST 调用时将 `/me/devices` 返回命令 `/me/devices/{id}/command` ID。

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
  "@odata.type": "microsoft.graph.command",
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


