---
title: 获取设备命令状态
description: 获取设备上命令的状态。 有关状态代码的完整列表, 请参阅 actionStatus 的列表。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 74104859b0621e51c0af9eced15912632fe5b9fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35954303"
---
# <a name="get-device-command-status"></a>获取设备命令状态

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取设备上命令的状态。 有关状态代码的完整列表, 请参阅[actionStatus 的列表](#list-of-actionstatus)。

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

## <a name="list-of-actionstatus"></a>ActionStatus 列表

- 请求、//命令已创建, 正在等待处理
- 已将 sentToTarget、//命令发送到目标设备
- 正在执行、//目标设备确认了命令的接收并正在执行该命令
- 已完成,//命令执行已完成
- failedToSend,//服务无法将命令发送到目标设备
- executionFailed,//命令执行失败
- commandDropped、//设备处于 ConnectedStandby 状态时由客户端丢弃的命令
- 取消、//取消命令
- 取消、//取消命令
- 已取消,//命令已取消
- 重试,//服务正在重试将命令发送到目标
- 已过期,//命令处理超过了过期时间
- 处理命令时出现错误,//内部错误
- 自定义//自定义状态

## <a name="example"></a>示例

在此示例中, 将需要设备的 ID 以及已颁发给设备的命令的 ID。 在发出对`/me/devices`的 GET 呼叫时, 将返回设备 ID, 并且在对`/me/devices/{id}/command`进行开机自检呼叫时返回命令 id。

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

获取设备上特定操作的响应负载。 在查询应用程序服务以传送数据时, 将使用响应负载。


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

在此示例中, 将需要设备的 ID 以及已颁发给设备的命令的 ID。 在`/me/devices`发出 GET 呼叫时, 将返回设备 ID, 并在对`/me/devices/{id}/command`进行开机自检呼叫时返回命令 id。

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
