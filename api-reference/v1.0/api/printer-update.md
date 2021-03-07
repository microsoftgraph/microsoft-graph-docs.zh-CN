---
title: 更新打印机
description: 更新打印机对象的属性。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: e29335cab6d88c736825684b2ab46e65db64d563
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516964"
---
# <a name="update-printer"></a>更新打印机
命名空间：microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

更新 [打印机对象的属性](../resources/printer.md) 。

## <a name="permissions"></a>Permissions
要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。 登录用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。

>**注意：** 仅允许注册打印机的应用使用应用程序权限更新打印机。

|权限类型 | 权限（从最低特权到最高特权） |
|:---------------|:--------------------------------------------|
|委派（工作或学校帐户）| Printer.ReadWrite.All、Printer.FullControl.All |
|委派（个人 Microsoft 帐户）|不支持。|
|应用程序| Printer.ReadWrite.All |

>**注意：** 目前，只有没有物理设备的打印机可以使用应用程序权限进行更新。

## <a name="http-request"></a>HTTP 请求

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}
```

## <a name="request-headers"></a>请求标头
|名称|说明|
|:---|:---|
|Authorization|Bearer {token}。必需。|
|Content-Type|application/json. Required.|

## <a name="request-body"></a>请求正文

### <a name="delegated-permissions-and-json-payload"></a>委派的权限和 JSON 负载

如果使用委派权限，在请求正文中， [提供应更新](../resources/printer.md) 的相关打印机字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。 

可以使用委派权限更新以下属性。

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|defaults|[printerDefaults](../resources/printerdefaults.md)|打印机的默认打印设置。|
|位置|[printerLocation](../resources/printerlocation.md)|打印机的物理和/或组织位置。|
|displayName|String|打印机的名称。|

### <a name="application-permissions-and-json-payload"></a>应用程序权限和 JSON 负载
在请求正文中， [提供应更新](../resources/printer.md) 的相关打印机字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。 

可以使用应用程序权限更新以下属性。

| 属性     | 类型        | Description |
|:-------------|:------------|:------------|
|defaults|[printerDefaults](../resources/printerdefaults.md)|打印机的默认打印设置。|
|capabilities|[printerCapabilities](../resources/printerCapabilities.md)|与此打印机共享关联的打印机的功能。|
|displayName|String|打印机的名称。|
|manufacturer|String|打印机的制造商。|
|model|String|打印机的模型名称。|
|状态|[printerStatus](../resources/printerstatus.md)|打印机的处理状态，包括任何错误。|
|isAcceptingJobs|Boolean|打印机当前是否接受新的打印作业。|

### <a name="application-permissions-and-ipp-payload"></a>应用程序权限和 IPP 有效负载

使用应用程序权限，还可使用 Internet 打印协议或 IPP (更新) 负载。 在这种情况下，请求正文包含一个二进制流，该流代表 [IPP](https://tools.ietf.org/html/rfc8010)编码中的 Printer Attributes 组。

客户端必须为一组打印机属性提供一个或多个值 (包括 [RFC8011 第 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) 节"作业模板属性" ("xxx-default"、"xxx-supported"和"xxx-ready"属性) 、 [第 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) 节打印机说明属性以及打印机支持的任何属性扩展中定义的显式允许的带外值) 。 每个 (打印机) 的值将替换 (打印机) 打印机属性的值。 对于可以在 1setOf (多个值) ，客户端提供的所有值将替换相应的 Printer 对象属性的所有值。

## <a name="response"></a>响应

### <a name="delegated-permissions-and-json-payload"></a>委派的权限和 JSON 负载

如果使用委派权限，如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新的打印机对象[](../resources/printer.md)。

### <a name="application-permissions-and-json-payload"></a>应用程序权限和 JSON 负载

如果使用委派权限，如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新的打印机对象[](../resources/printer.md)。

### <a name="application-permissions-and-ipp-payload"></a>应用程序权限和 IPP 有效负载

如果使用应用程序权限，如果成功，此方法将返回 `204 No content` 响应代码。 它不会在响应正文中返回任何内容。

## <a name="examples"></a>示例

### <a name="request"></a>请求
<!-- {
  "blockType": "request",
  "name": "update_printer"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}
Content-Type: application/json
Content-length: 581

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```


### <a name="response"></a>响应
**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "status": {
    "state": "idle",
    "details": [],
    "description": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "contentType": "application/oxps",
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
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
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

