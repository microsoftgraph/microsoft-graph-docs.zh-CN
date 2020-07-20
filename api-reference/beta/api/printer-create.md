---
title: 打印机：创建
description: 创建（注册）具有通用打印服务的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a0b64166b6d7c95f3ad4995321b50b2c4aaadda9
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081060"
---
# <a name="printer-create"></a>打印机：创建

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

创建（注册）具有通用打印服务的打印机。 这是一个长时间运行的操作，因此它返回可用于跟踪和验证打印机注册的[printerCreateOperation](../resources/printercreateoperation.md) 。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| User.Read.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序|不支持。|

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

| 参数      | 类型    |说明| 是否必需？ |
|:---------------|:--------|:----------|:----------|
|displayName|String|要分配给打印机的显示名称。|是|
|manufacturer|String|打印机的制造商。|是|
|model|String|打印机的型号。|是|
|physicalDeviceId|String|打印机的物理设备 UUID。 如果属性为 true，则为必需 `hasPhysicalDevice` 。|否|
|hasPhysicalDevice|Boolean|如果打印机具有物理输出设备，则为 True，否则为 false。 如果省略，则默认值为 true。|否|
|certificateSigningRequest|[printCertificateSigningRequest](../resources/printcertificatesigningrequest.md)|打印机创建并使用的证书的 x.509 证书签名请求（CSR），用于标识自己。|是|
|connectorId|String|充当打印机代理的连接器的 Id。|否|

## <a name="response"></a>响应
如果成功，此方法将 `202 Accepted` 在标头中返回响应代码和关联的[printerCreateOperation](../resources/printercreateoperation.md)的链接 `Operation-Location` 。

向链接的 URL 发出 GET 请求可用于获取正在进行的打印机注册的状态。 成功完成打印机注册后，对链接的 URL 的 GET 请求将包含创建的打印机对象和已注册的证书。

## <a name="example"></a>示例
### <a name="request"></a>请求
下面展示了示例请求。 若要获取有关创建所需证书签名请求（CSR）的帮助，请参阅[CSR 生成代码示例](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request)。


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json
Content-length: 319

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
