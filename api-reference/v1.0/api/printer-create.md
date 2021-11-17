---
title: printer： create
description: 创建 (通用) 在打印机上注册。
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 65f3bc7ee802de4be6a96a30f885045eb2f997a4
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023041"
---
# <a name="printer-create"></a>printer： create
命名空间：microsoft.graph

创建 (通用) 在打印机上注册。 这是一个长时间运行的操作，因此它将返回一个 [printerCreateOperation，](../resources/printercreateoperation.md) 该打印机可用于跟踪和验证打印机的注册。

有关使用 CSR (创建打印机) 证书签名请求的帮助，请参阅 [CSR 生成代码示例](/universal-print/hardware/universal-print-oem-certificate-signing-request)。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。 登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| Printer.Create、Printer.ReadWrite.All、Printer.FullControl.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| 不支持。 |

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/create
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文
在请求正文中，提供参数的 JSON 表示形式。

下表显示了可用于此操作的参数。

| 参数      | 类型    |说明| 是否必需？ |
|:---------------|:--------|:----------|:----------|
|displayName|String|要显示名称打印机的打印机。|是|
|manufacturer|String|打印机的制造商。|是|
|model|String|打印机的模型。|是|
|physicalDeviceId|String|打印机的物理设备 UUID。 如果属性为 `hasPhysicalDevice` true，则必需。|否|
|hasPhysicalDevice|布尔|如果打印机具有物理输出设备，则其为 True，否则为 false。 如果省略，则默认值为 true。|否|
|certificateSigningRequest|[printCertificateSigningRequest](../resources/printcertificatesigningrequest.md)|X.509 证书签名请求 (CSR) 由打印机创建和用于标识自身的证书。|是|
|connectorId|String|充当打印机代理的连接器的 ID。|否|

## <a name="response"></a>响应
如果成功，此方法在标头中返回 响应代码和关联 `202 Accepted` [printerCreateOperation](../resources/printercreateoperation.md) `Operation-Location` 的链接。

对链接的 URL 进行 GET 请求，获取正在进行的打印机注册的状态。 成功完成打印机注册后，对链接 URL 的 GET 请求将包含创建的打印机对象和注册的证书。

## <a name="examples"></a>示例

### <a name="request"></a>请求

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer_create"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/create
Content-Type: application/json

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
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-create-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-create-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-create-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-create-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[转到](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/printer-create-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>响应

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/v1.0/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

