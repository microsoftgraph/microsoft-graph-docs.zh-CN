---
title: '发送设备命令 (已弃) '
description: '此 API Project Rome 功能来命令与 Microsoft 帐户关联的设备。 在 上执行 GET 调用后 `me/devices` ，请传递设备的 ID 以向设备发出命令。 支持两种类型的命令：LaunchURI 和 AppServices。 如果使用的是 LaunchURI，请 *指定类型和**有效负载* 参数。 对于 AppService 调用，指定 '
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: ''
author: ailae
ms.openlocfilehash: 76b6edf47492d5a04e554e3f70834b3aed24d6a2
ms.sourcegitcommit: 9adf70c5da7c5b65f7d20f571d101ee06f023bc3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/25/2022
ms.locfileid: "62201602"
---
# <a name="send-device-command-deprecated"></a>发送设备命令 (已弃) 

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!CAUTION]
> 此 API 已弃用，在 2020 年 9 月 30 日停止返回数据。

此 API Project Rome 功能来命令与 Microsoft 帐户关联的设备。 在 上执行 GET 调用后 `me/devices` ，请传递设备的 ID 以向设备发出命令。 支持两种类型的命令：LaunchURI 和 AppServices。 如果使用的是 LaunchURI，请 *指定类型和**有效负载* 参数。 对于 AppService 调用，请指定 *类型* *、payload* *、packageFamilyName* 和 *appServiceName* 参数。

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

|**名称**|**类型**|**说明**|
|:----|:------|:------|
|payload | microsoft.graph.json| 发送到应用服务或在设备上启动 URI 的有效负载。 |
|responsePayload | microsoft.graph.json| 从目标设备返回的有效负载。 |
|postBackURI | 字符串 | 回发 URI 以发送更新的后续通知。 |
|packageFamilyName | 字符串 | Windows程序包系列名称的应用程序。 |
|appServiceName | 字符串 | 由目标应用程序定义的应用服务的名称。 如果启动应用服务，此为必需项。 |
|type| 字符串 | LaunchURI 或 AppService。 |
|id| 字符串 | 已发送到设备的命令的 ID。 |
|actionStatus | 字符串 | [命令](get-device-command-status.md)的状态。 |
|error| 字符串| 与来自目标应用程序的请求关联的任何错误。 |

## <a name="examples"></a>示例

### <a name="example-1-launch-uri"></a>示例 1：启动 URI

下面是 LaunchURI 请求的一个示例;它将在目标设备上启动 URI 或应用程序。 若要启动 URI 或应用，请通过使用设备 ID (GET 调用获取的 POST `me/devices`) 。 将 *Type* 参数设置为 *LaunchURI* 并提供 URI 值，如 https://bing.com 。

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


### <a name="example-2-app-service"></a>示例 2：应用服务

以下示例演示如何在设备上查询应用服务。 若要使用应用服务，你必须使用设备 ID 执行 POST (通过对应用服务执行 GET `me/devices`) 。 若要使用以下示例，必须在目标 [设备上安装 Rome](https://aka.ms/romanapp) 应用。

必须在调用中设置其他几个属性。  Type 必须设置为 *AppService，AppServiceName* 必须设置为应用程序中定义的应用服务的名称 *，PackageFamilyName* 必须设置为应用清单中定义的程序包系列名称 *，Payload* 将保留目标应用程序中调用的服务的键和值。 

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


