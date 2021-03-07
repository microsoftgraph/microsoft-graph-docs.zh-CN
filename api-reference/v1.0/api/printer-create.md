---
title: printer： create
description: 创建 (通用) 打印服务在打印机上注册。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 58285c3c6908812edce8ad80915f44f4df08fcb8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516993"
---
# <a name="printer-create"></a>printer： create
命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

创建 (通用) 打印服务在打印机上注册。 这是一项长时间运行的操作，因此它将返回 [一个 printerCreateOperation，](../resources/printercreateoperation.md) 该打印机可用于跟踪和验证打印机的注册。

有关创建用于创建打印机的 CSR (证书签名请求) ，请参阅 [CSR 生成代码示例](/universal-print/hardware/universal-print-oem-certificate-signing-request)。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。 登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。

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

| 参数      | 类型    |Description| 是否必需？ |
|:---------------|:--------|:----------|:----------|
|displayName|String|要显示名称打印机的打印机。|是|
|manufacturer|String|打印机的制造商。|是|
|model|String|打印机的模型。|是|
|physicalDeviceId|String|打印机的物理设备 UUID。 如果该属性为 `hasPhysicalDevice` true，则必需。|否|
|hasPhysicalDevice|Boolean|如果打印机具有物理输出设备，则其为 True，否则为 false。 如果省略，则默认值为 true。|否|
|certificateSigningRequest|[printCertificateSigningRequest](../resources/printcertificatesigningrequest.md)|X.509 证书签名请求 (CSR) ，用于打印机创建和用于标识自己的证书。|是|
|connectorId|String|充当打印机代理的连接器的 ID。|否|

## <a name="response"></a>响应
如果成功，此方法在标头中返回响应代码和指向关联的 `202 Accepted` [printerCreateOperation](../resources/printercreateoperation.md) `Operation-Location` 的链接。

您可以对链接的 URL 进行 GET 请求，获取正在进行的打印机注册的状态。 成功完成打印机注册后，对链接 URL 的 GET 请求将包含创建的打印机对象和注册的证书。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "printer_create"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/create
Content-Type: application/json
Content-length: 287

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

