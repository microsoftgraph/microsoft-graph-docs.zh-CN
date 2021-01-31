---
title: 更新位置
description: 更新 place 对象的属性。
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 3ce93b0d170c0aca27c6814d319a2161cacc1050
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059618"
---
# <a name="update-place"></a><span data-ttu-id="352c8-103">更新位置</span><span class="sxs-lookup"><span data-stu-id="352c8-103">Update place</span></span>

<span data-ttu-id="352c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="352c8-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="352c8-105">更新 place[对象的属性](../resources/place.md)，可以是聊天室[或](../resources/room.md) [roomList。](../resources/roomlist.md)</span><span class="sxs-lookup"><span data-stu-id="352c8-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="352c8-106">可以通过指定 id **或** **emailAddress** 属性来标识会议室或 **roomList。**</span><span class="sxs-lookup"><span data-stu-id="352c8-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="352c8-107">权限</span><span class="sxs-lookup"><span data-stu-id="352c8-107">Permissions</span></span>

<span data-ttu-id="352c8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="352c8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="352c8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="352c8-110">Permission type</span></span>                        | <span data-ttu-id="352c8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="352c8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="352c8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="352c8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="352c8-113">Place.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="352c8-113">Place.ReadWrite.All</span></span> |
| <span data-ttu-id="352c8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="352c8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="352c8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="352c8-115">Not supported.</span></span> |
| <span data-ttu-id="352c8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="352c8-116">Application</span></span>                            | <span data-ttu-id="352c8-117">不支持</span><span class="sxs-lookup"><span data-stu-id="352c8-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="352c8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="352c8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="352c8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="352c8-119">Request headers</span></span>

| <span data-ttu-id="352c8-120">名称</span><span class="sxs-lookup"><span data-stu-id="352c8-120">Name</span></span>       | <span data-ttu-id="352c8-121">值</span><span class="sxs-lookup"><span data-stu-id="352c8-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="352c8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="352c8-122">Authorization</span></span>  | <span data-ttu-id="352c8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="352c8-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="352c8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="352c8-125">Content-Type</span></span> | <span data-ttu-id="352c8-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="352c8-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="352c8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="352c8-128">Request body</span></span>

<span data-ttu-id="352c8-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="352c8-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="352c8-130">一次只能更新 (**聊天室** 或 **roomList**) 资源实例。</span><span class="sxs-lookup"><span data-stu-id="352c8-130">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="352c8-131">在请求正文中，用于指定位置的类型，并包括要 `@odata.type` 更新的类型的属性。</span><span class="sxs-lookup"><span data-stu-id="352c8-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="352c8-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="352c8-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="352c8-133">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="352c8-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="352c8-134">属性</span><span class="sxs-lookup"><span data-stu-id="352c8-134">Property</span></span>               | <span data-ttu-id="352c8-135">类型</span><span class="sxs-lookup"><span data-stu-id="352c8-135">Type</span></span>                                              | <span data-ttu-id="352c8-136">说明</span><span class="sxs-lookup"><span data-stu-id="352c8-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="352c8-137">address</span><span class="sxs-lookup"><span data-stu-id="352c8-137">address</span></span>                | [<span data-ttu-id="352c8-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="352c8-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="352c8-139">会议室或会议室列表的街道地址。</span><span class="sxs-lookup"><span data-stu-id="352c8-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="352c8-140">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="352c8-140">audioDeviceName</span></span>        | <span data-ttu-id="352c8-141">String</span><span class="sxs-lookup"><span data-stu-id="352c8-141">String</span></span>                                            | <span data-ttu-id="352c8-142">指定会议室中的音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="352c8-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="352c8-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="352c8-143">bookingType</span></span>            | [<span data-ttu-id="352c8-144">bookingType</span><span class="sxs-lookup"><span data-stu-id="352c8-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="352c8-145">聊天室的类型。</span><span class="sxs-lookup"><span data-stu-id="352c8-145">Type of room.</span></span> <span data-ttu-id="352c8-146">可能的值为 `Standard` 和 `Reserved`。</span><span class="sxs-lookup"><span data-stu-id="352c8-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="352c8-147">building</span><span class="sxs-lookup"><span data-stu-id="352c8-147">building</span></span>               | <span data-ttu-id="352c8-148">String</span><span class="sxs-lookup"><span data-stu-id="352c8-148">String</span></span>                                            | <span data-ttu-id="352c8-149">指定房间的大楼名称或建筑物编号。</span><span class="sxs-lookup"><span data-stu-id="352c8-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="352c8-150">capacity</span><span class="sxs-lookup"><span data-stu-id="352c8-150">capacity</span></span>               | <span data-ttu-id="352c8-151">Int32</span><span class="sxs-lookup"><span data-stu-id="352c8-151">Int32</span></span>                                             | <span data-ttu-id="352c8-152">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="352c8-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="352c8-153">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="352c8-153">displayDeviceName</span></span>      | <span data-ttu-id="352c8-154">String</span><span class="sxs-lookup"><span data-stu-id="352c8-154">String</span></span>                                            | <span data-ttu-id="352c8-155">指定会议室中的显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="352c8-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="352c8-156">floorLabel</span><span class="sxs-lookup"><span data-stu-id="352c8-156">floorLabel</span></span>             | <span data-ttu-id="352c8-157">String</span><span class="sxs-lookup"><span data-stu-id="352c8-157">String</span></span>                                            | <span data-ttu-id="352c8-158">指定房间的楼层字母。</span><span class="sxs-lookup"><span data-stu-id="352c8-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="352c8-159">floorNumber</span><span class="sxs-lookup"><span data-stu-id="352c8-159">floorNumber</span></span>            | <span data-ttu-id="352c8-160">Int32</span><span class="sxs-lookup"><span data-stu-id="352c8-160">Int32</span></span>                                             | <span data-ttu-id="352c8-161">指定房间的楼层。</span><span class="sxs-lookup"><span data-stu-id="352c8-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="352c8-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="352c8-162">geoCoordinates</span></span>         | [<span data-ttu-id="352c8-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="352c8-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="352c8-164">指定以纬度、经度和（可选）高度坐标表示的会议室或会议室列表位置。</span><span class="sxs-lookup"><span data-stu-id="352c8-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="352c8-165">isWheelChairAccessible</span><span class="sxs-lookup"><span data-stu-id="352c8-165">isWheelChairAccessible</span></span> | <span data-ttu-id="352c8-166">布尔</span><span class="sxs-lookup"><span data-stu-id="352c8-166">Boolean</span></span>                                           | <span data-ttu-id="352c8-167">指定会议室是否可供访问。</span><span class="sxs-lookup"><span data-stu-id="352c8-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="352c8-168">label</span><span class="sxs-lookup"><span data-stu-id="352c8-168">label</span></span>                  | <span data-ttu-id="352c8-169">String</span><span class="sxs-lookup"><span data-stu-id="352c8-169">String</span></span>                                            | <span data-ttu-id="352c8-170">指定会议室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="352c8-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="352c8-171">nickname</span><span class="sxs-lookup"><span data-stu-id="352c8-171">nickname</span></span>               | <span data-ttu-id="352c8-172">String</span><span class="sxs-lookup"><span data-stu-id="352c8-172">String</span></span>                                            | <span data-ttu-id="352c8-173">指定会议室的昵称，例如"conf room"。</span><span class="sxs-lookup"><span data-stu-id="352c8-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="352c8-174">phone</span><span class="sxs-lookup"><span data-stu-id="352c8-174">phone</span></span>                  | <span data-ttu-id="352c8-175">String</span><span class="sxs-lookup"><span data-stu-id="352c8-175">String</span></span>                                            | <span data-ttu-id="352c8-176">会议室或会议室列表的电话号码。</span><span class="sxs-lookup"><span data-stu-id="352c8-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="352c8-177">tags</span><span class="sxs-lookup"><span data-stu-id="352c8-177">tags</span></span>                   | <span data-ttu-id="352c8-178">字符串集合</span><span class="sxs-lookup"><span data-stu-id="352c8-178">String collection</span></span>                                 | <span data-ttu-id="352c8-179">指定会议室的其他功能，例如，视图类型或费用类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="352c8-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="352c8-180">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="352c8-180">videoDeviceName</span></span>        | <span data-ttu-id="352c8-181">String</span><span class="sxs-lookup"><span data-stu-id="352c8-181">String</span></span>                                            | <span data-ttu-id="352c8-182">指定会议室中的视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="352c8-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="352c8-183">响应</span><span class="sxs-lookup"><span data-stu-id="352c8-183">Response</span></span>

<span data-ttu-id="352c8-184">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和更新的 [place](../resources/place.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="352c8-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="352c8-185">示例</span><span class="sxs-lookup"><span data-stu-id="352c8-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="352c8-186">示例 1：更新聊天室</span><span class="sxs-lookup"><span data-stu-id="352c8-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="352c8-187">请求</span><span class="sxs-lookup"><span data-stu-id="352c8-187">Request</span></span>

<span data-ttu-id="352c8-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="352c8-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="352c8-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="352c8-189">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="352c8-190">C#</span><span class="sxs-lookup"><span data-stu-id="352c8-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="352c8-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="352c8-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="352c8-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="352c8-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="352c8-193">Java</span><span class="sxs-lookup"><span data-stu-id="352c8-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="352c8-194">响应</span><span class="sxs-lookup"><span data-stu-id="352c8-194">Response</span></span>

<span data-ttu-id="352c8-195">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="352c8-195">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="352c8-196">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="352c8-196">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="352c8-197">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="352c8-197">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="352c8-198">示例 2：更新会议室列表</span><span class="sxs-lookup"><span data-stu-id="352c8-198">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="352c8-199">请求</span><span class="sxs-lookup"><span data-stu-id="352c8-199">Request</span></span>

<span data-ttu-id="352c8-200">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="352c8-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="352c8-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="352c8-201">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="352c8-202">C#</span><span class="sxs-lookup"><span data-stu-id="352c8-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="352c8-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="352c8-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="352c8-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="352c8-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="352c8-205">Java</span><span class="sxs-lookup"><span data-stu-id="352c8-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="352c8-206">响应</span><span class="sxs-lookup"><span data-stu-id="352c8-206">Response</span></span>

<span data-ttu-id="352c8-207">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="352c8-207">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="352c8-208">为了可读性，可能会缩短此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="352c8-208">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="352c8-209">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="352c8-209">All the properties will be returned from an actual call.</span></span>

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

