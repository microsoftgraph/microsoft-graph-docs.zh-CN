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
# <a name="update-place"></a><span data-ttu-id="79c84-103">更新位置</span><span class="sxs-lookup"><span data-stu-id="79c84-103">Update place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79c84-104">更新[place](../resources/place.md)对象的属性，该对象可以是一个[聊天室](../resources/room.md)或[roomList](../resources/roomlist.md)。</span><span class="sxs-lookup"><span data-stu-id="79c84-104">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="79c84-105">您可以通过指定**id**或**emailAddress**属性来标识**聊天室**或**roomList** 。</span><span class="sxs-lookup"><span data-stu-id="79c84-105">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="79c84-106">权限</span><span class="sxs-lookup"><span data-stu-id="79c84-106">Permissions</span></span>

<span data-ttu-id="79c84-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79c84-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="79c84-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="79c84-109">Permission type</span></span>                        | <span data-ttu-id="79c84-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="79c84-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="79c84-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79c84-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="79c84-112">将读写全部。</span><span class="sxs-lookup"><span data-stu-id="79c84-112">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="79c84-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79c84-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="79c84-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="79c84-114">Not supported.</span></span> |
| <span data-ttu-id="79c84-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="79c84-115">Application</span></span>                            | <span data-ttu-id="79c84-116">不支持</span><span class="sxs-lookup"><span data-stu-id="79c84-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="79c84-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79c84-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id}
```

## <a name="request-headers"></a><span data-ttu-id="79c84-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="79c84-118">Request headers</span></span>

| <span data-ttu-id="79c84-119">名称</span><span class="sxs-lookup"><span data-stu-id="79c84-119">Name</span></span>       | <span data-ttu-id="79c84-120">类型</span><span class="sxs-lookup"><span data-stu-id="79c84-120">Type</span></span> | <span data-ttu-id="79c84-121">描述</span><span class="sxs-lookup"><span data-stu-id="79c84-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="79c84-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="79c84-122">Authorization</span></span>  | <span data-ttu-id="79c84-123">string</span><span class="sxs-lookup"><span data-stu-id="79c84-123">string</span></span>  | <span data-ttu-id="79c84-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="79c84-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="79c84-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="79c84-126">Request body</span></span>

<span data-ttu-id="79c84-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="79c84-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="79c84-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="79c84-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="79c84-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="79c84-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="79c84-130">属性</span><span class="sxs-lookup"><span data-stu-id="79c84-130">Property</span></span>               | <span data-ttu-id="79c84-131">类型</span><span class="sxs-lookup"><span data-stu-id="79c84-131">Type</span></span>                                              | <span data-ttu-id="79c84-132">说明</span><span class="sxs-lookup"><span data-stu-id="79c84-132">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="79c84-133">address</span><span class="sxs-lookup"><span data-stu-id="79c84-133">address</span></span>                | [<span data-ttu-id="79c84-134">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="79c84-134">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="79c84-135">会议室或 roomlist 的街道地址。</span><span class="sxs-lookup"><span data-stu-id="79c84-135">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="79c84-136">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="79c84-136">audioDeviceName</span></span>        | <span data-ttu-id="79c84-137">String</span><span class="sxs-lookup"><span data-stu-id="79c84-137">String</span></span>                                            | <span data-ttu-id="79c84-138">指定会议室中音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="79c84-138">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="79c84-139">bookingType</span><span class="sxs-lookup"><span data-stu-id="79c84-139">bookingType</span></span>            | [<span data-ttu-id="79c84-140">bookingType</span><span class="sxs-lookup"><span data-stu-id="79c84-140">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="79c84-141">会议室的类型。</span><span class="sxs-lookup"><span data-stu-id="79c84-141">Type of room.</span></span> <span data-ttu-id="79c84-142">可能的值为 `Standard` 和 `Reserved`。</span><span class="sxs-lookup"><span data-stu-id="79c84-142">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="79c84-143">幢</span><span class="sxs-lookup"><span data-stu-id="79c84-143">building</span></span>               | <span data-ttu-id="79c84-144">String</span><span class="sxs-lookup"><span data-stu-id="79c84-144">String</span></span>                                            | <span data-ttu-id="79c84-145">指定聊天室所在的建筑物名称或楼号。</span><span class="sxs-lookup"><span data-stu-id="79c84-145">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="79c84-146">能够</span><span class="sxs-lookup"><span data-stu-id="79c84-146">capacity</span></span>               | <span data-ttu-id="79c84-147">String</span><span class="sxs-lookup"><span data-stu-id="79c84-147">String</span></span>                                            | <span data-ttu-id="79c84-148">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="79c84-148">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="79c84-149">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="79c84-149">displayDeviceName</span></span>      | <span data-ttu-id="79c84-150">String</span><span class="sxs-lookup"><span data-stu-id="79c84-150">String</span></span>                                            | <span data-ttu-id="79c84-151">指定聊天室中显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="79c84-151">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="79c84-152">floorLabel</span><span class="sxs-lookup"><span data-stu-id="79c84-152">floorLabel</span></span>             | <span data-ttu-id="79c84-153">String</span><span class="sxs-lookup"><span data-stu-id="79c84-153">String</span></span>                                            | <span data-ttu-id="79c84-154">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="79c84-154">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="79c84-155">floorNumber</span><span class="sxs-lookup"><span data-stu-id="79c84-155">floorNumber</span></span>            | <span data-ttu-id="79c84-156">Int32</span><span class="sxs-lookup"><span data-stu-id="79c84-156">Int32</span></span>                                             | <span data-ttu-id="79c84-157">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="79c84-157">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="79c84-158">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="79c84-158">geoCoordinates</span></span>         | [<span data-ttu-id="79c84-159">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="79c84-159">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="79c84-160">指定纬度、经度和海拔高度坐标（可选）中的会议室或 roomlist 位置。</span><span class="sxs-lookup"><span data-stu-id="79c84-160">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="79c84-161">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="79c84-161">isWheelchairAccessible</span></span> | <span data-ttu-id="79c84-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="79c84-162">Boolean</span></span>                                           | <span data-ttu-id="79c84-163">指定会议室是否 wheelchair 可访问。</span><span class="sxs-lookup"><span data-stu-id="79c84-163">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="79c84-164">label</span><span class="sxs-lookup"><span data-stu-id="79c84-164">label</span></span>                  | <span data-ttu-id="79c84-165">String</span><span class="sxs-lookup"><span data-stu-id="79c84-165">String</span></span>                                            | <span data-ttu-id="79c84-166">指定聊天室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="79c84-166">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="79c84-167">昵称</span><span class="sxs-lookup"><span data-stu-id="79c84-167">nickname</span></span>               | <span data-ttu-id="79c84-168">String</span><span class="sxs-lookup"><span data-stu-id="79c84-168">String</span></span>                                            | <span data-ttu-id="79c84-169">指定聊天室的昵称，例如 "会议室"。</span><span class="sxs-lookup"><span data-stu-id="79c84-169">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="79c84-170">phone</span><span class="sxs-lookup"><span data-stu-id="79c84-170">phone</span></span>                  | <span data-ttu-id="79c84-171">String</span><span class="sxs-lookup"><span data-stu-id="79c84-171">String</span></span>                                            | <span data-ttu-id="79c84-172">会议室或 roomlist 的电话号码。</span><span class="sxs-lookup"><span data-stu-id="79c84-172">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="79c84-173">标记</span><span class="sxs-lookup"><span data-stu-id="79c84-173">tags</span></span>                   | <span data-ttu-id="79c84-174">String collection</span><span class="sxs-lookup"><span data-stu-id="79c84-174">String collection</span></span>                                 | <span data-ttu-id="79c84-175">指定会议室的其他功能，例如，视图类型或家具类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="79c84-175">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="79c84-176">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="79c84-176">videoDeviceName</span></span>        | <span data-ttu-id="79c84-177">String</span><span class="sxs-lookup"><span data-stu-id="79c84-177">String</span></span>                                            | <span data-ttu-id="79c84-178">指定聊天室中视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="79c84-178">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="79c84-179">响应</span><span class="sxs-lookup"><span data-stu-id="79c84-179">Response</span></span>

<span data-ttu-id="79c84-180">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79c84-180">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="79c84-181">示例</span><span class="sxs-lookup"><span data-stu-id="79c84-181">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="79c84-182">示例1：更新聊天室</span><span class="sxs-lookup"><span data-stu-id="79c84-182">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="79c84-183">请求</span><span class="sxs-lookup"><span data-stu-id="79c84-183">Request</span></span>

<span data-ttu-id="79c84-184">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79c84-184">The following is an example of the request.</span></span>


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

### <a name="response"></a><span data-ttu-id="79c84-185">响应</span><span class="sxs-lookup"><span data-stu-id="79c84-185">Response</span></span>

<span data-ttu-id="79c84-186">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="79c84-186">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="79c84-187">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79c84-187">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="79c84-188">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="79c84-188">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="79c84-189">示例2：更新 roomlist</span><span class="sxs-lookup"><span data-stu-id="79c84-189">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="79c84-190">请求</span><span class="sxs-lookup"><span data-stu-id="79c84-190">Request</span></span>

<span data-ttu-id="79c84-191">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="79c84-191">The following is an example of the request.</span></span>


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

### <a name="response"></a><span data-ttu-id="79c84-192">响应</span><span class="sxs-lookup"><span data-stu-id="79c84-192">Response</span></span>

<span data-ttu-id="79c84-193">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="79c84-193">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="79c84-194">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="79c84-194">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="79c84-195">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="79c84-195">All the properties will be returned from an actual call.</span></span>

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
