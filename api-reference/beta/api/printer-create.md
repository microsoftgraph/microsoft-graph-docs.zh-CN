---
title: printer： create
description: 创建 (通用) 在打印机上注册。
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 01aea7fbcd4c4723f7d2253fc9591bd0c75d85e8
ms.sourcegitcommit: 0759717104292bda6012dd2e9e3a362567aa2b64
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/12/2021
ms.locfileid: "60939336"
---
# <a name="printer-create"></a>printer： create

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建 (通用) 在打印机上注册。 这是一个长时间运行的操作，因此它将返回一个 [printerCreateOperation，](../resources/printercreateoperation.md) 该打印机可用于跟踪和验证打印机的注册。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。 登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| Printer.Create、Printer.ReadWrite.All、Printer.FullControl.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization | Bearer {token}。必需。 |
| Content-type  | application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供具有以下属性的 JSON 对象。

| 参数      | 类型    |Description| 是否必需？ |
|:---------------|:--------|:----------|:----------|
|displayName|String|要显示名称打印机的打印机。|是|
|manufacturer|String|打印机的制造商。|是|
|model|String|打印机的模型。|是|
|physicalDeviceId|String|打印机的物理设备 UUID。 如果属性为 `hasPhysicalDevice` true，则必需。|否|
|hasPhysicalDevice|Boolean|如果打印机具有物理输出设备，则其为 True，否则为 false。 如果省略，则默认值为 true。|否|
|certificateSigningRequest|[printCertificateSigningRequest](../resources/printcertificatesigningrequest.md)|X.509 证书签名 (CSR) 由打印机创建和用于标识自身的证书。|是|
|connectorId|String|充当打印机代理的连接器的 ID。|否|

## <a name="response"></a>响应
如果成功，此方法在标头中返回 响应代码和关联 `202 Accepted` [printerCreateOperation](../resources/printercreateoperation.md) `Operation-Location` 的链接。

对链接 URL 进行 GET 请求可用于获取正在进行的打印机注册的状态。 成功完成打印机注册后，对链接 URL 的 GET 请求将包含创建的打印机对象和注册的证书。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>响应
下面展示了示例响应。

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/beta/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printers: create",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
