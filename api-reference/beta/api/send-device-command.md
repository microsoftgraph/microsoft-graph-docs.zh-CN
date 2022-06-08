---
title: 已弃用)  (发送设备命令
description: '此 API 使 Project Rome 功能能够命令与 Microsoft 帐户关联的设备。 执行 GET 调用 `me/devices`后，传入设备的 ID，向设备发出命令。 支持两种类型的命令：LaunchURI 和 AppServices。 如果使用的是 LaunchURI，请指定 *类型* 和 *有效负载* 参数。 对于 AppService 调用，请指定 '
ms.localizationpriority: medium
doc_type: apiPageType
ms.prod: project-rome
author: ailae
ms.openlocfilehash: db99f797b234b96d83487765218d49c78d434c5f
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65944144"
---
# <a name="send-device-command-deprecated"></a>已弃用)  (发送设备命令

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

> [!CAUTION]
> 此 API 已弃用，并在 2020 年 9 月 30 日停止返回数据。

此 API 使 Project Rome 功能能够命令与 Microsoft 帐户关联的设备。 执行 GET 调用 `me/devices`后，传入设备的 ID，向设备发出命令。 支持两种类型的命令：LaunchURI 和 AppServices。 如果使用的是 LaunchURI，请指定 *类型* 和 *有效负载* 参数。 对于 AppService 调用，请指定 *类型*、 *有效负载*、 *packageFamilyName* 和 *appServiceName* 参数。

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
|payload | microsoft.graph.json| 要发送到应用服务或在设备上启动 URI 的有效负载。 |
|responsePayload | microsoft.graph.json| 从目标设备返回的有效负载。 |
|postBackURI | 字符串 | 发回 URI 以发送更新的后续通知。 |
|packageFamilyName | String | 应用程序的 Windows 包系列名称。 |
|appServiceName | String | 由目标应用程序定义的应用服务的名称。 如果启动应用服务，则为必需。 |
|type| String | LaunchURI 或 AppService。 |
|id| String | 已发送到设备的命令的 ID。 |
|actionStatus | 字符串 | 命令的 [状态](get-device-command-status.md) 。 |
|error| String| 与来自目标应用程序的请求关联的任何错误。 |

## <a name="examples"></a>示例

### <a name="example-1-launch-uri"></a>示例 1：启动 URI

下面是 LaunchURI 请求的示例;它将在目标设备上启动 URI 或应用程序。 若要启动 URI 或应用，请使用在) 执行 `me/devices` GET 调用 (获取的设备 ID 发出 POST。 将 *Type* 参数设置为 *LaunchURI* 并提供 URI 值，例如 https://bing.com。

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

以下示例演示如何查询设备上的应用服务。 若要使用应用服务，必须使用在) 执行 `me/devices` GET 调用 (获取的设备 ID 执行 POST 调用。 若要使用以下示例，必须在目标设备上安装 [Rome 应用](https://aka.ms/romanapp) 。

必须在调用中设置其他几个属性。 *类型* 必须设置为 *AppService*， *AppServiceName* 必须设置为应用程序中定义的应用服务的名称， *必须将 PackageFamilyName* 设置为应用清单中定义的包系列名称， *有效负载* 保存在目标应用程序中调用的服务的密钥和值。

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


