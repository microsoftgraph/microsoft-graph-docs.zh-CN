---
title: 发送设备命令
description: '此 API 支持 Project Rome 功能命令与 Microsoft 帐户关联的设备。 在执行 GET 呼叫后`me/devices`，向您的设备发出命令的设备 ID 中传递。 支持两种类型的命令： LaunchURI 和 AppServices。 如果您正在使用 LaunchURI，指定*类型*和*负载*参数。 对于 AppService 呼叫，指定 '
localization_priority: Normal
ms.openlocfilehash: 54349e2f43a776523614b0cd2abbc209e89305fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891985"
---
# <a name="send-device-command"></a>发送设备命令

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 不支持在生产应用程序中使用这些 API。

此 API 支持 Project Rome 功能命令与 Microsoft 帐户关联的设备。 在执行 GET 呼叫后`me/devices`，向您的设备发出命令的设备 ID 中传递。 支持两种类型的命令： LaunchURI 和 AppServices。 如果您正在使用 LaunchURI，指定*类型*和*负载*参数。 AppService 呼叫的指定*类型*、*负载*、 *packageFamilyName*和*appServiceName*参数。

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
|Accept | application/json |

## <a name="request-body"></a>请求正文

在请求正文中，提供的命令属性的 JSON 表示形式。

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
## <a name="command-properties"></a>Command 属性 

|**Name**|**类型**|**说明**|
|:----|:------|:------|
|payload | microsoft.graph.json| 负载以将发送到应用程序服务或启动在设备上的 URI。 |
|responsePayload | microsoft.graph.json| 返回从目标设备的负载。 |
|postBackURI | 字符串 | 回发 URI 发送更新的随后进行通知。 |
|packageFamilyName | 字符串 | Windows 应用程序包系列名称。 |
|appServiceName | 字符串 | 由目标应用程序定义的应用程序服务的名称。 所需如果启动应用程序服务。 |
|type| 字符串 | LaunchURI 或 AppService。 |
|id| 字符串 | 已向设备发送命令的 ID。 |
|actionStatus | 字符串 | 命令的[状态](get-device-command-status.md)。 |
|error| 字符串| 目标应用程序的请求相关联的任何错误。 |

## <a name="launch-uri-example"></a>启动 URI 示例

下面是 LaunchURI 请求; 的一个示例它将启动 URI 或目标设备上的应用程序。 要启动 URI 或应用程序，发出公告使用的设备 ID (从上执行 GET 呼叫获取`me/devices`)。 *类型*参数设置为*LaunchURI*和提供 URI 值，如https://bing.com。

#### <a name="request"></a>请求

下面展示了示例请求。

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

下面展示了示例响应。

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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


## <a name="app-service-example"></a>应用程序服务示例

下面是查询应用程序服务在设备上的一个示例。 若要使用的应用程序服务必须执行 POST 呼叫使用的设备 id (从上执行 GET 呼叫获取`me/devices`)。 若要使用下面的示例，您必须目标设备上安装[Rome 应用程序](https://aka.ms/romanapp)。

必须在调用设置多个其他属性。 *类型*必须设置为*AppService* *AppServiceName*必须设置为应用程序服务应用程序中定义的名称、 *PackageFamilyName*必须设置为应用程序清单和*负载*中定义的程序包系列名称包含的键和值您正在呼叫的目标应用程序中的服务。

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

下面展示了示例响应。

<!-- {
  "blockType": "ignored",
  "truncated": false,
  "@odata.type": "microsoft.graph.commandobject",
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
