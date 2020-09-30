---
title: 更新打印机
description: 更新 printer 对象的属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 5ddbd41aa7e51434fb6e6d07a90bac090a0266d6
ms.sourcegitcommit: a9f0fde9924ad184d315bb2de43c2610002409f3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/30/2020
ms.locfileid: "48314958"
---
# <a name="update-printer"></a>更新打印机

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新 [printer](../resources/printer.md) 对象的属性。

## <a name="permissions"></a>权限
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。 登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。

仅允许注册打印机的应用程序使用应用程序权限更新打印机。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| 完全控制和所有打印机。 |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| Printer.ReadWrite.All |

## <a name="http-request"></a>HTTP 请求
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a>请求标头
| 名称       | 说明|
|:-----------|:-----------|
| Authorization | Bearer {token}。必需。 |
| Content-type  | `application/json` 使用委派权限时， `application/ipp` 使用应用程序权限时。 必需。|

## <a name="request-body"></a>请求正文

### <a name="delegated-permissions-and-json-payload"></a>委派权限和 JSON 有效负载

如果使用委派权限，则在请求正文中，提供应更新的相关 [打印机](../resources/printer.md) 字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性     | 类型        | 说明 |
|:-------------|:------------|:------------|
|location|[printerLocation](../resources/printerlocation.md)|打印机的物理和/或组织位置。|
|name|字符串|打印机的名称。|

### <a name="application-permissions-and-ipp-payload"></a>应用程序权限和 IPP 有效负载

如果使用应用程序权限，则请求正文包含一个二进制流，表示 [IPP 编码](https://tools.ietf.org/html/rfc8010)中的打印机属性组。

客户端必须提供一组包含一个或多个值 (的打印机属性，包括在 [RFC8011 节 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) 作业模板 ( 属性中定义的显式允许的带外值) 如 "xxx-默认"、"支持 xxx" 和 "xxx-ready" 属性) 、 [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) 打印机说明属性和打印机支持的任何属性扩展。 提供的每个打印机属性 (s) 的值将替换目标打印机对象上对应的打印机属性) 的值 (s。 对于可以具有多个值 (1setOf) 的属性，客户端提供的所有值都将替换相应的打印机对象属性的所有值。

## <a name="response"></a>响应

### <a name="delegated-permissions-and-json-payload"></a>委派权限和 JSON 有效负载

如果使用委派权限，如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [printer](../resources/printer.md) 对象。

### <a name="application-permissions-and-ipp-payload"></a>应用程序权限和 IPP 有效负载

如果使用应用程序权限，如果成功，此方法将返回 `204 No content` 响应代码。 它不在响应正文中返回任何内容。

## <a name="example"></a>示例

### <a name="request"></a>请求
下面展示了示例请求。

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/{id}
Content-type: application/json
Content-length: 124

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a>响应
下面展示了示例响应。
>**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "status": {
    "processingState": "idle",
    "processingStateReasons": [],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->