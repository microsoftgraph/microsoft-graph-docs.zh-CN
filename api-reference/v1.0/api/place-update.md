---
title: 更新位置
description: 更新 place 对象的属性。
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 1b009f51fc095c5832ea7638f2ee4edd1ff21110
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053970"
---
# <a name="update-place"></a><span data-ttu-id="b164b-103">更新位置</span><span class="sxs-lookup"><span data-stu-id="b164b-103">Update place</span></span>

<span data-ttu-id="b164b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b164b-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="b164b-105">更新 place [对象](../resources/place.md) 的属性，可以是 room [或](../resources/room.md) [roomList](../resources/roomlist.md)。</span><span class="sxs-lookup"><span data-stu-id="b164b-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="b164b-106">可以通过指定 **id** **或** **emailAddress** 属性来标识 room 或 **roomList。**</span><span class="sxs-lookup"><span data-stu-id="b164b-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b164b-107">权限</span><span class="sxs-lookup"><span data-stu-id="b164b-107">Permissions</span></span>

<span data-ttu-id="b164b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b164b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b164b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b164b-110">Permission type</span></span>                        | <span data-ttu-id="b164b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b164b-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b164b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b164b-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="b164b-113">Place.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b164b-113">Place.ReadWrite.All</span></span> |
| <span data-ttu-id="b164b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b164b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b164b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b164b-115">Not supported.</span></span> |
| <span data-ttu-id="b164b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b164b-116">Application</span></span>                            | <span data-ttu-id="b164b-117">不支持</span><span class="sxs-lookup"><span data-stu-id="b164b-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="b164b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b164b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="b164b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b164b-119">Request headers</span></span>

| <span data-ttu-id="b164b-120">名称</span><span class="sxs-lookup"><span data-stu-id="b164b-120">Name</span></span>       | <span data-ttu-id="b164b-121">值</span><span class="sxs-lookup"><span data-stu-id="b164b-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="b164b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b164b-122">Authorization</span></span>  | <span data-ttu-id="b164b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b164b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b164b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b164b-125">Content-Type</span></span> | <span data-ttu-id="b164b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b164b-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b164b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b164b-128">Request body</span></span>

<span data-ttu-id="b164b-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b164b-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b164b-130">一次只能更新 (**或** **roomList**) 一个实例。</span><span class="sxs-lookup"><span data-stu-id="b164b-130">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="b164b-131">在请求正文中，使用 指定位置的类型，并包括要 `@odata.type` 更新的类型的属性。</span><span class="sxs-lookup"><span data-stu-id="b164b-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="b164b-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b164b-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b164b-133">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b164b-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b164b-134">属性</span><span class="sxs-lookup"><span data-stu-id="b164b-134">Property</span></span>               | <span data-ttu-id="b164b-135">类型</span><span class="sxs-lookup"><span data-stu-id="b164b-135">Type</span></span>                                              | <span data-ttu-id="b164b-136">说明</span><span class="sxs-lookup"><span data-stu-id="b164b-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="b164b-137">address</span><span class="sxs-lookup"><span data-stu-id="b164b-137">address</span></span>                | [<span data-ttu-id="b164b-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="b164b-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="b164b-139">会议室或会议室列表的街道地址。</span><span class="sxs-lookup"><span data-stu-id="b164b-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="b164b-140">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="b164b-140">audioDeviceName</span></span>        | <span data-ttu-id="b164b-141">String</span><span class="sxs-lookup"><span data-stu-id="b164b-141">String</span></span>                                            | <span data-ttu-id="b164b-142">指定会议室中的音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="b164b-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="b164b-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="b164b-143">bookingType</span></span>            | [<span data-ttu-id="b164b-144">bookingType</span><span class="sxs-lookup"><span data-stu-id="b164b-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="b164b-145">聊天室的类型。</span><span class="sxs-lookup"><span data-stu-id="b164b-145">Type of room.</span></span> <span data-ttu-id="b164b-146">可能的值为 `Standard` 和 `Reserved`。</span><span class="sxs-lookup"><span data-stu-id="b164b-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="b164b-147">building</span><span class="sxs-lookup"><span data-stu-id="b164b-147">building</span></span>               | <span data-ttu-id="b164b-148">String</span><span class="sxs-lookup"><span data-stu-id="b164b-148">String</span></span>                                            | <span data-ttu-id="b164b-149">指定会议室的大楼名称或建筑物编号。</span><span class="sxs-lookup"><span data-stu-id="b164b-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="b164b-150">capacity</span><span class="sxs-lookup"><span data-stu-id="b164b-150">capacity</span></span>               | <span data-ttu-id="b164b-151">Int32</span><span class="sxs-lookup"><span data-stu-id="b164b-151">Int32</span></span>                                             | <span data-ttu-id="b164b-152">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="b164b-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="b164b-153">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="b164b-153">displayDeviceName</span></span>      | <span data-ttu-id="b164b-154">String</span><span class="sxs-lookup"><span data-stu-id="b164b-154">String</span></span>                                            | <span data-ttu-id="b164b-155">指定会议室中显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="b164b-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="b164b-156">floorLabel</span><span class="sxs-lookup"><span data-stu-id="b164b-156">floorLabel</span></span>             | <span data-ttu-id="b164b-157">String</span><span class="sxs-lookup"><span data-stu-id="b164b-157">String</span></span>                                            | <span data-ttu-id="b164b-158">指定房间的楼层号。</span><span class="sxs-lookup"><span data-stu-id="b164b-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="b164b-159">floorNumber</span><span class="sxs-lookup"><span data-stu-id="b164b-159">floorNumber</span></span>            | <span data-ttu-id="b164b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="b164b-160">Int32</span></span>                                             | <span data-ttu-id="b164b-161">指定房间的楼层。</span><span class="sxs-lookup"><span data-stu-id="b164b-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="b164b-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b164b-162">geoCoordinates</span></span>         | [<span data-ttu-id="b164b-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="b164b-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="b164b-164">以纬度、经度和（可选）海拔坐标指定房间或房间列表位置。</span><span class="sxs-lookup"><span data-stu-id="b164b-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="b164b-165">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="b164b-165">isWheelChairAccessible</span></span> | <span data-ttu-id="b164b-166">布尔值</span><span class="sxs-lookup"><span data-stu-id="b164b-166">Boolean</span></span>                                           | <span data-ttu-id="b164b-167">指定会议室是否可供访问。</span><span class="sxs-lookup"><span data-stu-id="b164b-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="b164b-168">label</span><span class="sxs-lookup"><span data-stu-id="b164b-168">label</span></span>                  | <span data-ttu-id="b164b-169">String</span><span class="sxs-lookup"><span data-stu-id="b164b-169">String</span></span>                                            | <span data-ttu-id="b164b-170">指定会议室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="b164b-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="b164b-171">nickname</span><span class="sxs-lookup"><span data-stu-id="b164b-171">nickname</span></span>               | <span data-ttu-id="b164b-172">String</span><span class="sxs-lookup"><span data-stu-id="b164b-172">String</span></span>                                            | <span data-ttu-id="b164b-173">指定会议室的昵称，例如"conf room"。</span><span class="sxs-lookup"><span data-stu-id="b164b-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="b164b-174">phone</span><span class="sxs-lookup"><span data-stu-id="b164b-174">phone</span></span>                  | <span data-ttu-id="b164b-175">String</span><span class="sxs-lookup"><span data-stu-id="b164b-175">String</span></span>                                            | <span data-ttu-id="b164b-176">会议室或会议室列表的电话号码。</span><span class="sxs-lookup"><span data-stu-id="b164b-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="b164b-177">tags</span><span class="sxs-lookup"><span data-stu-id="b164b-177">tags</span></span>                   | <span data-ttu-id="b164b-178">字符串集合</span><span class="sxs-lookup"><span data-stu-id="b164b-178">String collection</span></span>                                 | <span data-ttu-id="b164b-179">指定会议室的其他功能，例如，视图类型或装饰类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="b164b-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="b164b-180">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="b164b-180">videoDeviceName</span></span>        | <span data-ttu-id="b164b-181">String</span><span class="sxs-lookup"><span data-stu-id="b164b-181">String</span></span>                                            | <span data-ttu-id="b164b-182">指定会议室中的视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="b164b-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="b164b-183">响应</span><span class="sxs-lookup"><span data-stu-id="b164b-183">Response</span></span>

<span data-ttu-id="b164b-184">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [place](../resources/place.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b164b-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b164b-185">示例</span><span class="sxs-lookup"><span data-stu-id="b164b-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="b164b-186">示例 1：更新聊天室</span><span class="sxs-lookup"><span data-stu-id="b164b-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="b164b-187">请求</span><span class="sxs-lookup"><span data-stu-id="b164b-187">Request</span></span>

<span data-ttu-id="b164b-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b164b-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="b164b-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="b164b-189">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_room"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/cf100@contoso.com
Content-type: application/json
Content-length: 285

{
  "@odata.type": "microsoft.graph.room",
  "nickname": "Conf Room",
  "building": "1",
  "label": "100",
  "capacity": 50,
  "isWheelChairAccessible": false
}
```
# <a name="c"></a>[<span data-ttu-id="b164b-190">C#</span><span class="sxs-lookup"><span data-stu-id="b164b-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b164b-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b164b-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b164b-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b164b-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b164b-193">Java</span><span class="sxs-lookup"><span data-stu-id="b164b-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b164b-194">响应</span><span class="sxs-lookup"><span data-stu-id="b164b-194">Response</span></span>

<span data-ttu-id="b164b-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b164b-195">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b164b-196">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b164b-196">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.room"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/$entity",
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
    "capacity": 50,
    "building": "1",
    "floorLabel": "1P",
    "floorNumber": 1,
    "isManaged": true,
    "isWheelChairAccessible": false,
    "bookingType": "standard",
    "tags": [
      "bean bags"
    ],
    "audioDeviceName": null,
    "videoDeviceName": null,
    "displayDevice": "surface hub"
}
```

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="b164b-197">示例 2：更新会议室列表</span><span class="sxs-lookup"><span data-stu-id="b164b-197">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="b164b-198">请求</span><span class="sxs-lookup"><span data-stu-id="b164b-198">Request</span></span>

<span data-ttu-id="b164b-199">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b164b-199">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b164b-200">HTTP</span><span class="sxs-lookup"><span data-stu-id="b164b-200">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/Building1RroomList@contoso.onmicrosoft.com
Content-type: application/json

{
  "@odata.type": "microsoft.graph.roomList",
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
# <a name="c"></a>[<span data-ttu-id="b164b-201">C#</span><span class="sxs-lookup"><span data-stu-id="b164b-201">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b164b-202">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b164b-202">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b164b-203">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b164b-203">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b164b-204">Java</span><span class="sxs-lookup"><span data-stu-id="b164b-204">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="b164b-205">响应</span><span class="sxs-lookup"><span data-stu-id="b164b-205">Response</span></span>

<span data-ttu-id="b164b-206">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b164b-206">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="b164b-207">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b164b-207">The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/$entity",
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

