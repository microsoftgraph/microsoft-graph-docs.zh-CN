---
title: 更新位置
description: 更新 place 对象的属性。
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 5e89dc031802ea420079bbbbbf5dd46f4fe181fc
ms.sourcegitcommit: dd94c3a0f7663699825b6dbc119cdcef494cd130
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2019
ms.locfileid: "37949501"
---
# <a name="update-place"></a>更新位置

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

更新[place](../resources/place.md)对象的属性，该对象可以是一个[聊天室](../resources/room.md)或[roomList](../resources/roomlist.md)。 您可以通过指定**id**或**emailAddress**属性来标识**聊天室**或**roomList** 。

## <a name="permissions"></a>权限

要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。

| 权限类型                        | 权限（从最低特权到最高特权） |
|:---------------------------------------|:--------------------------------------------|
| 委派（工作或学校帐户）     | 将读写全部。 |
| 委派（个人 Microsoft 帐户） | 不支持。 |
| 应用程序                            | 不支持 |

## <a name="http-request"></a>HTTP 请求

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id}
```

## <a name="request-headers"></a>请求标头

| 名称       | 类型 | 描述|
|:-----------|:------|:----------|
| Authorization  | string  | Bearer {token}。必需。 |

## <a name="request-body"></a>请求正文

在请求正文中，提供应更新的相关字段的值。 请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。 为了获得最佳性能，请勿加入尚未更改的现有值。

| 属性               | 类型                                              | 说明 |
|:-----------------------|:--------------------------------------------------|:--|
| address                | [physicalAddress](../resources/physicaladdress.md)             | 会议室或 roomlist 的街道地址。 |
| audioDeviceName        | String                                            | 指定会议室中音频设备的名称。 |
| bookingType            | [bookingType](../resources/room.md)                            | 会议室的类型。 可能的值为 `Standard` 和 `Reserved`。 |
| 幢               | String                                            | 指定聊天室所在的建筑物名称或楼号。 |
| 能够               | String                                            | 指定会议室的容量。 |
| displayDeviceName      | String                                            | 指定聊天室中显示设备的名称。 |
| floorLabel             | String                                            | 指定会议室所在的楼层号。 |
| floorNumber            | Int32                                             | 指定会议室所在的楼层号。 |
| geoCoordinates         | [outlookGeoCoordinates](../resources/outlookgeocoordinates.md) | 指定纬度、经度和海拔高度坐标（可选）中的会议室或 roomlist 位置。 |
| isWheelchairAccessible | Boolean                                           | 指定会议室是否 wheelchair 可访问。 |
| label                  | String                                            | 指定聊天室的描述性标签，例如数字或名称。 |
| 昵称               | String                                            | 指定聊天室的昵称，例如 "会议室"。 |
| phone                  | String                                            | 会议室或 roomlist 的电话号码。 |
| 标记                   | String collection                                 | 指定会议室的其他功能，例如，视图类型或家具类型等详细信息。 |
| videoDeviceName        | String                                            | 指定聊天室中视频设备的名称。 |

## <a name="response"></a>响应

如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[place](../resources/place.md)对象。

## <a name="examples"></a>示例

### <a name="example-1-update-a-room"></a>示例1：更新聊天室

### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "request",
  "name": "update_room"
}-->
```http
PATCH https://graph.microsoft.com/beta/places/cf100@contoso.com
Content-type: application/json
Content-length: 285

{
  "@odata.type": "microsoft.graph.room",
  "nickname": "Conf Room",
  "building": "1",
  "label": "100",
  "capacity": "50",
  "isWheelchairAccessible": false
}
```

### <a name="response"></a>响应

下面展示了示例响应。

> [!NOTE]
> 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
    "@odata.type": "#microsoft.graph.room",
    "id": "3162F1E1-C4C0-604B-51D8-91DA78989EB1",
    "emailAddress": "cf100@contoso.com",
    "displayName": "Conf Room 100",
    "address": {
      "street": "4567 Main Street",
      "city": "Buffalo",
      "state": "NY",
      "postalCode": "98052",
      "countryOrRegion": "USA"
    },
    "geoCoordinates": {
      "latitude": 47.640568390488626,
      "longitude": -122.1293731033803
    },
    "phone": "555-555-0100",
    "nickname": "Conf Room",
    "label": "100",
    "capacity": "50",
    "building": "1",
    "floorLabel": "1P",
    "floorNumber": 1,
    "isManaged": true,
    "isWheelchairAccessible": false,
    "bookingType": "standard",
    "tags": [
      "bean bags"
    ],
    "audioDeviceName": null,
    "videoDeviceName": null,
    "displayDevice": "surface hub"
}
```

### <a name="example-2-update-a-roomlist"></a>示例2：更新 roomlist

### <a name="request"></a>请求

下面展示了示例请求。


<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/beta/places/Building1RroomList@contoso.onmicrosoft.com
Content-type: application/json

{
  "@odata.type": "microsoft.graph.roomlist",
  "displayName": "Building 1",
  "phone":"555-555-0100"
}
```

### <a name="response"></a>响应

下面展示了示例响应。

> [!NOTE]
> 为了提高可读性，可能缩短了此处显示的响应对象。 所有属性都将通过实际调用返回。

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/$entity",
  "@odata.type": "#microsoft.graph.roomList",
  "id": "DC404124-302A-92AA-F98D-7B4DEB0C1705",
  "displayName": "Building 1",
  "address": {
    "street": "4567 Main Street",
    "city": "Buffalo",
    "state": "NY",
    "postalCode": "98052",
    "countryOrRegion": "USA"
  },
  "geocoordinates": null,
  "phone": "555-555-0100",
  "emailAddress": "bldg1@contoso.com"
}
```


<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
