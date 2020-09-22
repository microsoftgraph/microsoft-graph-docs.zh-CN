---
title: 更新位置
description: 更新 place 对象的属性。
localization_priority: Normal
author: vrod9429
ms.prod: Outlook
doc_type: apiPageType
ms.openlocfilehash: 6c62796c56c2e0af51b7a159dead20b51f21e87f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978802"
---
# <a name="update-place"></a><span data-ttu-id="15186-103">更新位置</span><span class="sxs-lookup"><span data-stu-id="15186-103">Update place</span></span>

<span data-ttu-id="15186-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15186-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="15186-105">更新 [place](../resources/place.md) 对象的属性，该对象可以是一个 [聊天室](../resources/room.md) 或 [roomList](../resources/roomlist.md)。</span><span class="sxs-lookup"><span data-stu-id="15186-105">Update the properties of [place](../resources/place.md) object, which can be a [room](../resources/room.md) or [roomList](../resources/roomlist.md).</span></span> <span data-ttu-id="15186-106">您可以通过指定**id**或**emailAddress**属性来标识**聊天室**或**roomList** 。</span><span class="sxs-lookup"><span data-stu-id="15186-106">You can identify the **room** or **roomList** by specifying the **id** or **emailAddress** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="15186-107">权限</span><span class="sxs-lookup"><span data-stu-id="15186-107">Permissions</span></span>

<span data-ttu-id="15186-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15186-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="15186-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="15186-110">Permission type</span></span>                        | <span data-ttu-id="15186-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15186-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="15186-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15186-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="15186-113">将读写全部。</span><span class="sxs-lookup"><span data-stu-id="15186-113">Place.ReadWrite.All.</span></span> |
| <span data-ttu-id="15186-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="15186-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="15186-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="15186-115">Not supported.</span></span> |
| <span data-ttu-id="15186-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="15186-116">Application</span></span>                            | <span data-ttu-id="15186-117">不支持</span><span class="sxs-lookup"><span data-stu-id="15186-117">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="15186-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15186-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /places/{id | emailAddress}
```

## <a name="request-headers"></a><span data-ttu-id="15186-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="15186-119">Request headers</span></span>

| <span data-ttu-id="15186-120">名称</span><span class="sxs-lookup"><span data-stu-id="15186-120">Name</span></span>       | <span data-ttu-id="15186-121">值</span><span class="sxs-lookup"><span data-stu-id="15186-121">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="15186-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="15186-122">Authorization</span></span>  | <span data-ttu-id="15186-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15186-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="15186-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="15186-125">Content-Type</span></span> | <span data-ttu-id="15186-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="15186-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="15186-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="15186-128">Request body</span></span>

<span data-ttu-id="15186-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="15186-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="15186-130">一次只能更新一个位置资源 (**会议室** 或 **roomList**) 的实例。</span><span class="sxs-lookup"><span data-stu-id="15186-130">Only one instance of a place resource (**room** or **roomList**) can be updated at a time.</span></span> <span data-ttu-id="15186-131">在请求正文中，使用 `@odata.type` 指定位置的类型，并包含要更新的类型的属性。</span><span class="sxs-lookup"><span data-stu-id="15186-131">In the request body, use `@odata.type` to specify the type of place, and include the properties of that type to update.</span></span> <span data-ttu-id="15186-132">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="15186-132">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="15186-133">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="15186-133">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="15186-134">属性</span><span class="sxs-lookup"><span data-stu-id="15186-134">Property</span></span>               | <span data-ttu-id="15186-135">类型</span><span class="sxs-lookup"><span data-stu-id="15186-135">Type</span></span>                                              | <span data-ttu-id="15186-136">说明</span><span class="sxs-lookup"><span data-stu-id="15186-136">Description</span></span> |
|:-----------------------|:--------------------------------------------------|:--|
| <span data-ttu-id="15186-137">address</span><span class="sxs-lookup"><span data-stu-id="15186-137">address</span></span>                | [<span data-ttu-id="15186-138">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="15186-138">physicalAddress</span></span>](../resources/physicaladdress.md)             | <span data-ttu-id="15186-139">会议室或 roomlist 的街道地址。</span><span class="sxs-lookup"><span data-stu-id="15186-139">The street address of the room or roomlist.</span></span> |
| <span data-ttu-id="15186-140">audioDeviceName</span><span class="sxs-lookup"><span data-stu-id="15186-140">audioDeviceName</span></span>        | <span data-ttu-id="15186-141">String</span><span class="sxs-lookup"><span data-stu-id="15186-141">String</span></span>                                            | <span data-ttu-id="15186-142">指定会议室中音频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="15186-142">Specifies the name of the audio device in the room.</span></span> |
| <span data-ttu-id="15186-143">bookingType</span><span class="sxs-lookup"><span data-stu-id="15186-143">bookingType</span></span>            | [<span data-ttu-id="15186-144">bookingType</span><span class="sxs-lookup"><span data-stu-id="15186-144">bookingType</span></span>](../resources/room.md)                            | <span data-ttu-id="15186-145">会议室的类型。</span><span class="sxs-lookup"><span data-stu-id="15186-145">Type of room.</span></span> <span data-ttu-id="15186-146">可能的值为 `Standard` 和 `Reserved`。</span><span class="sxs-lookup"><span data-stu-id="15186-146">Possible values are `Standard` and `Reserved`.</span></span> |
| <span data-ttu-id="15186-147">幢</span><span class="sxs-lookup"><span data-stu-id="15186-147">building</span></span>               | <span data-ttu-id="15186-148">String</span><span class="sxs-lookup"><span data-stu-id="15186-148">String</span></span>                                            | <span data-ttu-id="15186-149">指定聊天室所在的建筑物名称或楼号。</span><span class="sxs-lookup"><span data-stu-id="15186-149">Specifies the building name or building number that the room is in.</span></span> |
| <span data-ttu-id="15186-150">能够</span><span class="sxs-lookup"><span data-stu-id="15186-150">capacity</span></span>               | <span data-ttu-id="15186-151">String</span><span class="sxs-lookup"><span data-stu-id="15186-151">String</span></span>                                            | <span data-ttu-id="15186-152">指定会议室的容量。</span><span class="sxs-lookup"><span data-stu-id="15186-152">Specifies the capacity of the room.</span></span> |
| <span data-ttu-id="15186-153">displayDeviceName</span><span class="sxs-lookup"><span data-stu-id="15186-153">displayDeviceName</span></span>      | <span data-ttu-id="15186-154">String</span><span class="sxs-lookup"><span data-stu-id="15186-154">String</span></span>                                            | <span data-ttu-id="15186-155">指定聊天室中显示设备的名称。</span><span class="sxs-lookup"><span data-stu-id="15186-155">Specifies the name of the display device in the room.</span></span> |
| <span data-ttu-id="15186-156">floorLabel</span><span class="sxs-lookup"><span data-stu-id="15186-156">floorLabel</span></span>             | <span data-ttu-id="15186-157">String</span><span class="sxs-lookup"><span data-stu-id="15186-157">String</span></span>                                            | <span data-ttu-id="15186-158">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="15186-158">Specifies the floor letter that the room is on.</span></span> |
| <span data-ttu-id="15186-159">floorNumber</span><span class="sxs-lookup"><span data-stu-id="15186-159">floorNumber</span></span>            | <span data-ttu-id="15186-160">Int32</span><span class="sxs-lookup"><span data-stu-id="15186-160">Int32</span></span>                                             | <span data-ttu-id="15186-161">指定会议室所在的楼层号。</span><span class="sxs-lookup"><span data-stu-id="15186-161">Specifies the floor number that the room is on.</span></span> |
| <span data-ttu-id="15186-162">geoCoordinates</span><span class="sxs-lookup"><span data-stu-id="15186-162">geoCoordinates</span></span>         | [<span data-ttu-id="15186-163">outlookGeoCoordinates</span><span class="sxs-lookup"><span data-stu-id="15186-163">outlookGeoCoordinates</span></span>](../resources/outlookgeocoordinates.md) | <span data-ttu-id="15186-164">指定纬度、经度和海拔高度坐标（可选）中的会议室或 roomlist 位置。</span><span class="sxs-lookup"><span data-stu-id="15186-164">Specifies the room or roomlist location in latitude, longitude and optionally, altitude coordinates.</span></span> |
| <span data-ttu-id="15186-165">isWheelchairAccessible</span><span class="sxs-lookup"><span data-stu-id="15186-165">isWheelchairAccessible</span></span> | <span data-ttu-id="15186-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="15186-166">Boolean</span></span>                                           | <span data-ttu-id="15186-167">指定会议室是否 wheelchair 可访问。</span><span class="sxs-lookup"><span data-stu-id="15186-167">Specifies whether the room is wheelchair accessible.</span></span> |
| <span data-ttu-id="15186-168">label</span><span class="sxs-lookup"><span data-stu-id="15186-168">label</span></span>                  | <span data-ttu-id="15186-169">String</span><span class="sxs-lookup"><span data-stu-id="15186-169">String</span></span>                                            | <span data-ttu-id="15186-170">指定聊天室的描述性标签，例如数字或名称。</span><span class="sxs-lookup"><span data-stu-id="15186-170">Specifies a descriptive label for the room, for example, a number or name.</span></span> |
| <span data-ttu-id="15186-171">昵称</span><span class="sxs-lookup"><span data-stu-id="15186-171">nickname</span></span>               | <span data-ttu-id="15186-172">String</span><span class="sxs-lookup"><span data-stu-id="15186-172">String</span></span>                                            | <span data-ttu-id="15186-173">指定聊天室的昵称，例如 "会议室"。</span><span class="sxs-lookup"><span data-stu-id="15186-173">Specifies a nickname for the room, for example, "conf room".</span></span> |
| <span data-ttu-id="15186-174">phone</span><span class="sxs-lookup"><span data-stu-id="15186-174">phone</span></span>                  | <span data-ttu-id="15186-175">String</span><span class="sxs-lookup"><span data-stu-id="15186-175">String</span></span>                                            | <span data-ttu-id="15186-176">会议室或 roomlist 的电话号码。</span><span class="sxs-lookup"><span data-stu-id="15186-176">The phone number of the room or roomlist.</span></span> |
| <span data-ttu-id="15186-177">tags</span><span class="sxs-lookup"><span data-stu-id="15186-177">tags</span></span>                   | <span data-ttu-id="15186-178">String collection</span><span class="sxs-lookup"><span data-stu-id="15186-178">String collection</span></span>                                 | <span data-ttu-id="15186-179">指定会议室的其他功能，例如，视图类型或家具类型等详细信息。</span><span class="sxs-lookup"><span data-stu-id="15186-179">Specifies additional features of the room, for example, details like the type of view or furniture type.</span></span> |
| <span data-ttu-id="15186-180">videoDeviceName</span><span class="sxs-lookup"><span data-stu-id="15186-180">videoDeviceName</span></span>        | <span data-ttu-id="15186-181">String</span><span class="sxs-lookup"><span data-stu-id="15186-181">String</span></span>                                            | <span data-ttu-id="15186-182">指定聊天室中视频设备的名称。</span><span class="sxs-lookup"><span data-stu-id="15186-182">Specifies the name of the video device in the room.</span></span> |

## <a name="response"></a><span data-ttu-id="15186-183">响应</span><span class="sxs-lookup"><span data-stu-id="15186-183">Response</span></span>

<span data-ttu-id="15186-184">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [place](../resources/place.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="15186-184">If successful, this method returns a `200 OK` response code and an updated [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="15186-185">示例</span><span class="sxs-lookup"><span data-stu-id="15186-185">Examples</span></span>

### <a name="example-1-update-a-room"></a><span data-ttu-id="15186-186">示例1：更新聊天室</span><span class="sxs-lookup"><span data-stu-id="15186-186">Example 1: Update a room</span></span>

### <a name="request"></a><span data-ttu-id="15186-187">请求</span><span class="sxs-lookup"><span data-stu-id="15186-187">Request</span></span>

<span data-ttu-id="15186-188">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15186-188">The following is an example of the request.</span></span>



# <a name="http"></a>[<span data-ttu-id="15186-189">HTTP</span><span class="sxs-lookup"><span data-stu-id="15186-189">HTTP</span></span>](#tab/http)
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
  "capacity": "50",
  "isWheelchairAccessible": false
}
```
# <a name="c"></a>[<span data-ttu-id="15186-190">C#</span><span class="sxs-lookup"><span data-stu-id="15186-190">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15186-191">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15186-191">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15186-192">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15186-192">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15186-193">Java</span><span class="sxs-lookup"><span data-stu-id="15186-193">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="15186-194">响应</span><span class="sxs-lookup"><span data-stu-id="15186-194">Response</span></span>

<span data-ttu-id="15186-195">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="15186-195">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="15186-196">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="15186-196">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="15186-197">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="15186-197">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-update-a-roomlist"></a><span data-ttu-id="15186-198">示例2：更新 roomlist</span><span class="sxs-lookup"><span data-stu-id="15186-198">Example 2: Update a roomlist</span></span>

### <a name="request"></a><span data-ttu-id="15186-199">请求</span><span class="sxs-lookup"><span data-stu-id="15186-199">Request</span></span>

<span data-ttu-id="15186-200">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15186-200">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="15186-201">HTTP</span><span class="sxs-lookup"><span data-stu-id="15186-201">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_roomlist"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/places/Building1RroomList@contoso.onmicrosoft.com
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
# <a name="c"></a>[<span data-ttu-id="15186-202">C#</span><span class="sxs-lookup"><span data-stu-id="15186-202">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="15186-203">JavaScript</span><span class="sxs-lookup"><span data-stu-id="15186-203">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="15186-204">Objective-C</span><span class="sxs-lookup"><span data-stu-id="15186-204">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="15186-205">Java</span><span class="sxs-lookup"><span data-stu-id="15186-205">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="15186-206">响应</span><span class="sxs-lookup"><span data-stu-id="15186-206">Response</span></span>

<span data-ttu-id="15186-207">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="15186-207">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="15186-208">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="15186-208">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="15186-209">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="15186-209">All the properties will be returned from an actual call.</span></span>

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

