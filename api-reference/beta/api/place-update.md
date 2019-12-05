---
title: 更新位置
description: 更新 place 对象的属性。
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 3e2e517d0a20384c8aaaa24e9f385cf5560c411e
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844188"
---
# <a name="update-place"></a><span data-ttu-id="b755b-103">更新位置</span><span class="sxs-lookup"><span data-stu-id="b755b-103">Update place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b755b-104">更新[place](../resources/place.md)对象的属性，该对象可以是一个[聊天室](../resources/room.md)或[roomList](../resources/roomlist.md)。</span><span class="sxs-lookup"><span data-stu-id="b755b-104">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="b755b-105">您可以通过指定**id**或**emailAddress**属性来标识**聊天室**或**roomList** 。</span><span class="sxs-lookup"><span data-stu-id="b755b-105">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b755b-106">权限</span><span class="sxs-lookup"><span data-stu-id="b755b-106">Permissions</span></span>

<span data-ttu-id="b755b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b755b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b755b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b755b-109">Permission type</span></span>                        | <span data-ttu-id="b755b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b755b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b755b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b755b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b755b-112">将读写全部。</span><span class="sxs-lookup"><span data-stu-id="b755b-112">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="b755b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b755b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b755b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b755b-114">Not supported.</span></span> |
| <span data-ttu-id="b755b-115">Application</span><span class="sxs-lookup"><span data-stu-id="b755b-115">Application</span></span>                            | <span data-ttu-id="b755b-116">不支持</span><span class="sxs-lookup"><span data-stu-id="b755b-116">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="b755b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b755b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="b755b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b755b-118">Request headers</span></span>

| <span data-ttu-id="b755b-119">名称</span><span class="sxs-lookup"><span data-stu-id="b755b-119">Name</span></span>       | <span data-ttu-id="b755b-120">值</span><span class="sxs-lookup"><span data-stu-id="b755b-120">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b755b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b755b-121">Authorization</span></span>  | <span data-ttu-id="b755b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b755b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b755b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b755b-124">Content-Type</span></span> | <span data-ttu-id="b755b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b755b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b755b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b755b-127">Request body</span></span>

<span data-ttu-id="b755b-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b755b-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b755b-129">一次只能更新一个位置资源（**会议室**或**roomList**）的实例。</span><span class="sxs-lookup"><span data-stu-id="b755b-129">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="b755b-130">在请求正文中，使用`@odata.type`指定位置的类型，并包含要更新的类型的属性。</span><span class="sxs-lookup"><span data-stu-id="b755b-130">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="b755b-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b755b-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b755b-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b755b-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b755b-133">属性</span><span class="sxs-lookup"><span data-stu-id="b755b-133">Property</span></span>               | <span data-ttu-id="b755b-134">类型</span><span class="sxs-lookup"><span data-stu-id="b755b-134">Type</span></span>                                              | <span data-ttu-id="b755b-135">说明</span><span class="sxs-lookup"><span data-stu-id="b755b-135">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="b755b-136">address</span><span class="sxs-lookup"><span data-stu-id="b755b-136">address</span></span>                | [<span data-ttu-id="b755b-137">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b755b-137">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="b755b-138">会议室或 roomlist 的街道地址。</span><span class="sxs-lookup"><span data-stu-id="b755b-138">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="b755b-139">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="b755b-139">audioDeviceName</span></span>        | <span data-ttu-id="b755b-140">String</span><span class="sxs-lookup"><span data-stu-id="b755b-140">String</span></span>                                            | <span data-ttu-id="b755b-141">指定会议室中音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="b755b-141">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="b755b-142">bookingType</span><span class="sxs-lookup"><span data-stu-id="b755b-142">bookingType</span></span>            | [<span data-ttu-id="b755b-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="b755b-143">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="b755b-144">会议室的类型。</span><span class="sxs-lookup"><span data-stu-id="b755b-144">Type of room.</span></span> <span data-ttu-id="b755b-145">可能的值为 `Standard` 和 `Reserved`。</span><span class="sxs-lookup"><span data-stu-id="b755b-145">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="b755b-146">幢</span><span class="sxs-lookup"><span data-stu-id="b755b-146">building</span></span>               | <span data-ttu-id="b755b-147">String</span><span class="sxs-lookup"><span data-stu-id="b755b-147">String</span></span>                                            | <span data-ttu-id="b755b-148">指定聊天室所在的建筑物名称或楼号。</span><span class="sxs-lookup"><span data-stu-id="b755b-148">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="b755b-149">能够</span><span class="sxs-lookup"><span data-stu-id="b755b-149">capacity</span></span>               | <span data-ttu-id="b755b-150">String</span><span class="sxs-lookup"><span data-stu-id="b755b-150">String</span></span>                                            | <span data-ttu-id="b755b-151">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="b755b-151">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="b755b-152">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="b755b-152">displayDeviceName</span></span>      | <span data-ttu-id="b755b-153">String</span><span class="sxs-lookup"><span data-stu-id="b755b-153">String</span></span>                                            | <span data-ttu-id="b755b-154">指定聊天室中显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="b755b-154">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="b755b-155">floorLabel</span><span class="sxs-lookup"><span data-stu-id="b755b-155">floorLabel</span></span>             | <span data-ttu-id="b755b-156">String</span><span class="sxs-lookup"><span data-stu-id="b755b-156">String</span></span>                                            | <span data-ttu-id="b755b-157">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="b755b-157">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="b755b-158">floorNumber</span><span class="sxs-lookup"><span data-stu-id="b755b-158">floorNumber</span></span>            | <span data-ttu-id="b755b-159">Int32</span><span class="sxs-lookup"><span data-stu-id="b755b-159">Int32</span></span>                                             | <span data-ttu-id="b755b-160">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="b755b-160">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="b755b-161">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b755b-161">geoCoordinates</span></span>         | [<span data-ttu-id="b755b-162">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b755b-162">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="b755b-163">指定纬度、经度和海拔高度坐标（可选）中的会议室或 roomlist 位置。</span><span class="sxs-lookup"><span data-stu-id="b755b-163">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="b755b-164">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="b755b-164">isWheelchairAccessible</span></span> | <span data-ttu-id="b755b-165">布尔</span><span class="sxs-lookup"><span data-stu-id="b755b-165">Boolean</span></span>                                           | <span data-ttu-id="b755b-166">指定会议室是否 wheelchair 可访问。</span><span class="sxs-lookup"><span data-stu-id="b755b-166">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="b755b-167">label</span><span class="sxs-lookup"><span data-stu-id="b755b-167">label</span></span>                  | <span data-ttu-id="b755b-168">String</span><span class="sxs-lookup"><span data-stu-id="b755b-168">String</span></span>                                            | <span data-ttu-id="b755b-169">指定聊天室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="b755b-169">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="b755b-170">昵称</span><span class="sxs-lookup"><span data-stu-id="b755b-170">nickname</span></span>               | <span data-ttu-id="b755b-171">String</span><span class="sxs-lookup"><span data-stu-id="b755b-171">String</span></span>                                            | <span data-ttu-id="b755b-172">指定聊天室的昵称，例如 "会议室"。</span><span class="sxs-lookup"><span data-stu-id="b755b-172">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="b755b-173">phone</span><span class="sxs-lookup"><span data-stu-id="b755b-173">phone</span></span>                  | <span data-ttu-id="b755b-174">String</span><span class="sxs-lookup"><span data-stu-id="b755b-174">String</span></span>                                            | <span data-ttu-id="b755b-175">会议室或 roomlist 的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b755b-175">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="b755b-176">标记</span><span class="sxs-lookup"><span data-stu-id="b755b-176">tags</span></span>                   | <span data-ttu-id="b755b-177">String 集合</span><span class="sxs-lookup"><span data-stu-id="b755b-177">String collection</span></span>                                 | <span data-ttu-id="b755b-178">指定会议室的其他功能，例如，视图类型或家具类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="b755b-178">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="b755b-179">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="b755b-179">videoDeviceName</span></span>        | <span data-ttu-id="b755b-180">String</span><span class="sxs-lookup"><span data-stu-id="b755b-180">String</span></span>                                            | <span data-ttu-id="b755b-181">指定聊天室中视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="b755b-181">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="b755b-182">响应</span><span class="sxs-lookup"><span data-stu-id="b755b-182">Response</span></span>

<span data-ttu-id="b755b-183">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b755b-183">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b755b-184">示例</span><span class="sxs-lookup"><span data-stu-id="b755b-184">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="b755b-185">示例1：更新聊天室</span><span class="sxs-lookup"><span data-stu-id="b755b-185">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="b755b-186">请求</span><span class="sxs-lookup"><span data-stu-id="b755b-186">Request</span></span>

<span data-ttu-id="b755b-187">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b755b-187">The following is an example of the request.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="b755b-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="b755b-188">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="b755b-189">C#</span><span class="sxs-lookup"><span data-stu-id="b755b-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b755b-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b755b-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b755b-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b755b-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b755b-192">响应</span><span class="sxs-lookup"><span data-stu-id="b755b-192">Response</span></span>

<span data-ttu-id="b755b-193">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b755b-193">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b755b-194">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b755b-194">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b755b-195">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b755b-195">All the properties will be returned from an actual call.</span></span>

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
      "latitude": 47.0,
      "longitude": -122.0
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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="b755b-196">示例2：更新 roomlist</span><span class="sxs-lookup"><span data-stu-id="b755b-196">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="b755b-197">请求</span><span class="sxs-lookup"><span data-stu-id="b755b-197">Request</span></span>

<span data-ttu-id="b755b-198">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b755b-198">The following is an example of the request.</span></span>



# <a name="httptabhttp"></a>[<span data-ttu-id="b755b-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="b755b-199">HTTP</span></span>](#tab/http)
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
  "phone":"555-555-0100",
  "address": {
    "street": "4567 Main Street",
    "city": "Buffalo",
    "state": "NY",
    "postalCode": "98052",
    "countryOrRegion": "USA"
  },
  "geoCoordinates": {
    "altitude": null,
    "latitude": 47.0,
    "longitude": -122.0,
    "accuracy": null,
    "altitudeAccuracy": null
 }
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b755b-200">C#</span><span class="sxs-lookup"><span data-stu-id="b755b-200">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b755b-201">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b755b-201">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b755b-202">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b755b-202">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b755b-203">响应</span><span class="sxs-lookup"><span data-stu-id="b755b-203">Response</span></span>

<span data-ttu-id="b755b-204">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b755b-204">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b755b-205">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b755b-205">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b755b-206">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b755b-206">All the properties will be returned from an actual call.</span></span>

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
  "geoCoordinates": {
    "altitude": null,
    "latitude": 47.0,
    "longitude": -122.0,
    "accuracy": null,
    "altitudeAccuracy": null
 },
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
