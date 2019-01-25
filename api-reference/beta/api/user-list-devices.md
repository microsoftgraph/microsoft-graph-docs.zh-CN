---
title: 列出用户设备
description: 获取支持 Project Rome 功能的用户设备的列表。 这包括以启动应用程序，或者邮件或将数据发送到应用程序的能力。 在您之后执行 GET 呼叫我/设备，传递中要向您的设备发送命令的设备 ID。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 891f66691149106d4ff5a2951170524203eb2ea7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509523"
---
# <a name="list-user-devices"></a>列出用户设备

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

获取支持 Project Rome 功能的用户设备的列表。 这包括以启动应用程序，或者邮件或将数据发送到应用程序的能力。 在您之后执行 GET 呼叫我/设备中的设备 ID 传递到向设备[发送命令](send-device-command.md)。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。


|权限类型      | 权限（从最低特权到最高特权）              |
|:--------------------|:---------------------------------------------------------|
|委派（工作或学校帐户） | 不支持。    |
|委派（个人 Microsoft 帐户） | Device.Read    |
|应用程序 | 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
GET me/devices
```

## <a name="request-headers"></a>请求标头

| 标头 |值
|:----|:------|
|Authorization| Bearer {token}。必需。 |
|Accept | application/json |

## <a name="request-body"></a>请求正文
请勿提供此方法的请求正文。

## <a name="response"></a>响应

如果成功，此方法将在响应正文中返回一个 200 响应代码以及用户设备属性。

<!-- { "blockType": "ignored" } -->

```http
HTTP/1.1 200 OK
```

<!-- { "blockType": "ignored" } -->

```json
{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#devices",
  "value": [
    {
      "name": "name",
      "id": "id",
      "status": "status",
      "platform": "platform",
      "kind": "formFactor",
      "model": "model",
      "manufacturer": "manufacturer",
    }
  ]
}
```

## <a name="example"></a>示例
本示例将返回用户的设备的列表。 若要命令设备使用`me/devices/{id}/command`，您将需要获取的设备，则返回的 ID。

#### <a name="request"></a>请求

下面展示了示例请求。

<!-- {
  "blockType": "ignored",
  "name": "list_devices"
}-->

```http
GET me/devices
Authorization: Bearer Eaeou....
Content-Type: application/json; charset=utf-8
```

#### <a name="response"></a>响应

下面是一个响应示例。 注意：为简洁起见，可能会截断此处显示的响应对象。 将从实际调用中返回所有属性。

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 140

{
  "value": [
    {
      "Name": "JimSurface",
      "id": "6841b3db-2b55-467b-ad84-79a41a4ef665",
      "Manufacturer": "Microsoft Corporation",
      "Model": "Surface Book",
      "Kind": "Tablet",
      "Status": "Unknown",
      "Platform": "Windows"
    }
  ]
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-devices.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
