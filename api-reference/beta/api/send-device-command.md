---
title: 发送设备命令
description: '此 API 使 Project 罗马功能能够命令与 Microsoft 帐户关联的设备。 在`me/devices`执行 GET 呼叫后，传入设备的 ID 以向设备发出命令。 支持两种类型的命令： LaunchURI 和 AppServices。 如果使用的是 LaunchURI，请指定*type*和*载荷*参数。 对于 AppService 调用，请指定 '
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: f112c7d3253a0a0801b7542f492c6f3f1f675c81
ms.sourcegitcommit: 66ceeb5015ea4e92dc012cd48eee84b2bbe8e7b4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/20/2019
ms.locfileid: "37053940"
---
# <a name="send-device-command"></a>发送设备命令

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

此 API 使 Project 罗马功能能够命令与 Microsoft 帐户关联的设备。 在`me/devices`执行 GET 呼叫后，传入设备的 ID 以向设备发出命令。 支持两种类型的命令： LaunchURI 和 AppServices。 如果使用的是 LaunchURI，请指定*type*和*载荷*参数。 对于 AppService 调用，指定*type*、*载荷*、 *packageFamilyName*和*appServiceName*参数。

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
POST me/devices/{id}/commands
```

## <a name="request-headers"></a>请求标头


| 标头 |值
|:----|:------|
|Authorization| Bearer {token}。必需。 |
|接受 | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供命令属性的 JSON 表示形式。

```json
{
  "type": "appService",
  "payload": "payload-JSON",
  "packageFamilyName": "packageFamilyName",
  "appServiceName": "appServiceName",
  "postbackURI": "postbackURI"
}
```

## <a name="response"></a>响应

```http
HTTP/1.1 201 OK
```

```json
{
  "id": "0",
  "status": "requesting",
  "type": "appService",
  "appServiceName": "appServiceName",
  "packageFamilyName": "packageFamilyName",
  "error": "null",
  "responsePayload": "null",
  "payload": "payload-JSON",
  "permissionTicket": "null",
  "postBackUri": "postbackURI"
}
```
### <a name="command-properties"></a>命令属性 

|**名称**|**Type**|**说明**|
|:----|:------|:------|
|payload | microsoft. json| 要发送到应用程序服务或启动设备上的 URI 的有效负载。 |
|responsePayload | microsoft. json| 从目标设备返回的有效负载。 |
|postBackURI | String | 回发 URI 以发送后续的更新通知。 |
|packageFamilyName | String | Windows 程序包系列应用程序的名称。 |
|appServiceName | String | 由目标应用程序定义的应用服务的名称。 如果启动应用服务，则为必需。 |
|type| String | LaunchURI 或 AppService。 |
|id| String | 已发送到设备的命令的 ID。 |
|actionStatus | String | 命令的[状态](get-device-command-status.md)。 |
|error| String| 与目标应用程序中的请求关联的任何错误。 |

## <a name="examples"></a>示例

### <a name="example-1-launch-uri"></a>示例1：启动 URI 

以下是 LaunchURI 请求的示例;它会启动一个 URI 或目标设备上的应用程序。 若要启动 URI 或应用，请使用设备 ID 发出 POST （通过执行 GET 呼叫获取`me/devices`）。 将*类型*参数设置为*LaunchURI* ，并提供 URI 值（如https://bing.com）。

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "post_command"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{ "type" : "LaunchUri", "payload" : {"uri":"https://bing.com"}}

```
#### <a name="response"></a>响应 

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7337D1B...",
  "status": "requesting",
  "type": null,
  "appServiceName": null,
  "packageFamilyName": null,
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "uri": "https://bing.com"
  }
}

```


### <a name="example-2-app-service"></a>示例2： App service

下面的示例演示如何在设备上查询应用服务。 若要使用应用服务，必须使用设备 ID （通过执行 GET 呼叫获取`me/devices`）执行 POST 调用。 若要使用以下示例，必须在目标设备上安装[罗马应用程序](https://aka.ms/romanapp)。

必须在调用中设置多个附加属性。 *Type*必须设置为*AppService*， *AppServiceName*必须设置为应用程序中定义的应用服务的名称， *PackageFamilyName*必须设置为应用程序清单中定义的程序包系列名称和*有效负载*保留您在目标应用程序中调用的服务的键和值。

#### <a name="request"></a>请求

<!-- {
  "blockType": "ignored",
  "name": "post_command_2"
} -->

```http

POST me/devices/{id}/commands
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8

{
  "type" : "AppService",
  "appServiceName" : "com.microsoft.test.cdppingpongservice",
  "packageFamilyName" : "5085ShawnHenry.RomanTestApp_jsjw7knzsgcce",
  "payload" : {
    "Type":"Toast","Title":"Hello","Subtitle":"World!"}
  }
```

#### <a name="response"></a>响应

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.command",
  "isCollection": true
} -->

```http
HTTP/1.1 201 OK

{
  "id": "0158355AD4D680CC4E2994CC009EFFD7EADA8307E96FF1C8D19B..",
  "status": "requesting",
  "type": null,
  "appServiceName": "com.microsoft.randomnumbergenerator",
  "packageFamilyName": "Microsoft.SDKSamples.AppServicesProvider.CS_8wekyb3d8bbwe",
  "error": null,
  "permissionTicket": null,
  "postBackUri": null,
  "payload": {
    "Type": "Toast",
    "Title": "Hello",
    "Subtitle": "World!"
  }
}
```
