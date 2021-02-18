---
title: 列出位置
description: 检索 place 对象的列表。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 81447b77efb0ee518aaaf33ecb8e1b4262660163
ms.sourcegitcommit: b0194231721c68053a0be6d8eb46687574eb8d71
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/18/2021
ms.locfileid: "50292145"
---
# <a name="list-places"></a><span data-ttu-id="aaff1-103">列出位置</span><span class="sxs-lookup"><span data-stu-id="aaff1-103">List places</span></span>

<span data-ttu-id="aaff1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aaff1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aaff1-105">获取租户中定义的指定 [类型的 place](../resources/place.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="aaff1-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="aaff1-106">例如，可以获取租户中特定会议室列表中的所有会议室、所有会议室列表或会议室。</span><span class="sxs-lookup"><span data-stu-id="aaff1-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="aaff1-107">**place** 对象可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="aaff1-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="aaff1-108">[包含](../resources/room.md)丰富属性（如会议室的电子邮件地址）以及辅助功能、容量和设备支持的聊天室。</span><span class="sxs-lookup"><span data-stu-id="aaff1-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="aaff1-109">会议室 [列表](../resources/roomlist.md) ，其中包括会议室列表的电子邮件地址，以及用于获取会议室列表中会议室实例集合的导航属性。</span><span class="sxs-lookup"><span data-stu-id="aaff1-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="aaff1-110">**room 和** **roomList** 均派生自 **place** 对象。</span><span class="sxs-lookup"><span data-stu-id="aaff1-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="aaff1-111">默认情况下，此操作返回每页 100 个位置。</span><span class="sxs-lookup"><span data-stu-id="aaff1-111">By default, this operation returns 100 places per page.</span></span> 

<span data-ttu-id="aaff1-112">与 [findRooms](../api/user-findrooms.md) 和 [findRoomLists](../api/user-findroomlists.md) 函数相比，此操作为会议室和会议室列表返回更丰富的有效负载。</span><span class="sxs-lookup"><span data-stu-id="aaff1-112">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="aaff1-113">请参阅 [其](../resources/place.md#using-the-places-api) 比较情况的详细信息。</span><span class="sxs-lookup"><span data-stu-id="aaff1-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="aaff1-114">权限</span><span class="sxs-lookup"><span data-stu-id="aaff1-114">Permissions</span></span>

<span data-ttu-id="aaff1-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aaff1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="aaff1-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="aaff1-117">Permission type</span></span>                        | <span data-ttu-id="aaff1-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aaff1-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="aaff1-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aaff1-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="aaff1-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaff1-120">Place.Read.All</span></span> |
| <span data-ttu-id="aaff1-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aaff1-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aaff1-122">不支持</span><span class="sxs-lookup"><span data-stu-id="aaff1-122">Not supported</span></span> |
| <span data-ttu-id="aaff1-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="aaff1-123">Application</span></span>                            | <span data-ttu-id="aaff1-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="aaff1-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="aaff1-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aaff1-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="aaff1-126">若要获取租户中的所有会议室，请进行以下选择：</span><span class="sxs-lookup"><span data-stu-id="aaff1-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="aaff1-127">若要获取租户中所有会议室列表，请：</span><span class="sxs-lookup"><span data-stu-id="aaff1-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="aaff1-128">若要获取指定会议室列表中的所有会议室，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="aaff1-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="aaff1-129">**注意**：若要获取会议室列表中的会议室，必须按 **其 emailAddress** 属性（而不是其 **ID）** 指定会议室列表。</span><span class="sxs-lookup"><span data-stu-id="aaff1-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="aaff1-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="aaff1-130">Optional query parameters</span></span>
<span data-ttu-id="aaff1-131">此方法支持以下查询参数来帮助自定义响应：</span><span class="sxs-lookup"><span data-stu-id="aaff1-131">This method supports the following query parameters to help customize the response:</span></span>
- <span data-ttu-id="aaff1-132">$filter</span><span class="sxs-lookup"><span data-stu-id="aaff1-132">$filter</span></span>
- <span data-ttu-id="aaff1-133">$select</span><span class="sxs-lookup"><span data-stu-id="aaff1-133">$select</span></span>
- <span data-ttu-id="aaff1-134">$top</span><span class="sxs-lookup"><span data-stu-id="aaff1-134">$top</span></span>
- <span data-ttu-id="aaff1-135">$skip</span><span class="sxs-lookup"><span data-stu-id="aaff1-135">$skip</span></span>
- <span data-ttu-id="aaff1-136">$count=true</span><span class="sxs-lookup"><span data-stu-id="aaff1-136">$count=true</span></span>

<span data-ttu-id="aaff1-137">使用$top自定义页面大小。</span><span class="sxs-lookup"><span data-stu-id="aaff1-137">Use $top to customize the page size.</span></span> <span data-ttu-id="aaff1-138">默认页面大小是 100。</span><span class="sxs-lookup"><span data-stu-id="aaff1-138">The default page size is 100.</span></span>

<span data-ttu-id="aaff1-139">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="aaff1-139">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="aaff1-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="aaff1-140">Request headers</span></span>

| <span data-ttu-id="aaff1-141">名称</span><span class="sxs-lookup"><span data-stu-id="aaff1-141">Name</span></span>          | <span data-ttu-id="aaff1-142">说明</span><span class="sxs-lookup"><span data-stu-id="aaff1-142">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="aaff1-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="aaff1-143">Authorization</span></span> | <span data-ttu-id="aaff1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aaff1-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aaff1-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="aaff1-146">Request body</span></span>

<span data-ttu-id="aaff1-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aaff1-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aaff1-148">响应</span><span class="sxs-lookup"><span data-stu-id="aaff1-148">Response</span></span>

<span data-ttu-id="aaff1-149">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [place](../resources/place.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="aaff1-149">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="aaff1-150">示例</span><span class="sxs-lookup"><span data-stu-id="aaff1-150">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="aaff1-151">示例 1：列出租户中定义的所有会议室</span><span class="sxs-lookup"><span data-stu-id="aaff1-151">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="aaff1-152">请求</span><span class="sxs-lookup"><span data-stu-id="aaff1-152">Request</span></span>

<span data-ttu-id="aaff1-153">以下示例演示如何获取租户 [中所有](../resources/room.md) 会议室对象。</span><span class="sxs-lookup"><span data-stu-id="aaff1-153">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="aaff1-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaff1-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```
# <a name="c"></a>[<span data-ttu-id="aaff1-155">C#</span><span class="sxs-lookup"><span data-stu-id="aaff1-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaff1-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaff1-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaff1-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaff1-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaff1-158">Java</span><span class="sxs-lookup"><span data-stu-id="aaff1-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aaff1-159">响应</span><span class="sxs-lookup"><span data-stu-id="aaff1-159">Response</span></span>

<span data-ttu-id="aaff1-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aaff1-160">The following is an example of the response.</span></span>

><span data-ttu-id="aaff1-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aaff1-161">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aaff1-162">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aaff1-162">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_all_rooms",
  "truncated": true,
  "@odata.type": "microsoft.graph.room",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/microsoft.graph.room",
  "value": [
    {
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
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "100",
      "capacity": 50,
      "building": "1",
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
    },
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78970B97",
      "emailAddress": "cf200@contoso.com",
      "displayName": "Conf Room 200",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488625,
        "longitude": -122.1293731033802
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "200",
      "capacity": 40,
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelChairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "benches",
        "nice view"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    }
  ]
}
```

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="aaff1-163">示例 2：列出租户中定义的所有会议室列表</span><span class="sxs-lookup"><span data-stu-id="aaff1-163">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="aaff1-164">请求</span><span class="sxs-lookup"><span data-stu-id="aaff1-164">Request</span></span>

<span data-ttu-id="aaff1-165">以下示例演示如何获取租户 [中所有 roomList](../resources/roomlist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aaff1-165">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="aaff1-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaff1-166">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```
# <a name="c"></a>[<span data-ttu-id="aaff1-167">C#</span><span class="sxs-lookup"><span data-stu-id="aaff1-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaff1-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaff1-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaff1-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaff1-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaff1-170">Java</span><span class="sxs-lookup"><span data-stu-id="aaff1-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aaff1-171">响应</span><span class="sxs-lookup"><span data-stu-id="aaff1-171">Response</span></span>

<span data-ttu-id="aaff1-172">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aaff1-172">The following is an example of the response.</span></span>

><span data-ttu-id="aaff1-173">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aaff1-173">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aaff1-174">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aaff1-174">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_all_roomlists",
  "truncated": true,
  "@odata.type": "microsoft.graph.roomList",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places/microsoft.graph.roomList",
  "value": [
    {
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
      "phone": null,
      "emailAddress": "bldg1@contoso.com"
    },
    {
      "id": "DC404124-302A-92AA-F98D-7B4DEB0C1706",
      "displayName": "Building 2",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geocoordinates": null,
      "phone": null,
      "emailAddress": "bldg2@contoso.com"
    }
  ]
}
```

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="aaff1-175">示例 3：包含在会议室列表中的列表聊天室</span><span class="sxs-lookup"><span data-stu-id="aaff1-175">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="aaff1-176">请求</span><span class="sxs-lookup"><span data-stu-id="aaff1-176">Request</span></span>

<span data-ttu-id="aaff1-177">下面的示例演示如何获取 **roomList** 中包含的会议室对象 [](../resources/room.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="aaff1-177">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="aaff1-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="aaff1-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="c"></a>[<span data-ttu-id="aaff1-179">C#</span><span class="sxs-lookup"><span data-stu-id="aaff1-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="aaff1-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="aaff1-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="aaff1-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="aaff1-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="aaff1-182">Java</span><span class="sxs-lookup"><span data-stu-id="aaff1-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="aaff1-183">响应</span><span class="sxs-lookup"><span data-stu-id="aaff1-183">Response</span></span>

<span data-ttu-id="aaff1-184">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="aaff1-184">The following is an example of the response.</span></span>

><span data-ttu-id="aaff1-185">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="aaff1-185">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="aaff1-186">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="aaff1-186">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_rooms_in_roomlist",
  "truncated": true,
  "@odata.type": "microsoft.graph.room",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#places('bldg2%40contoso.com')/microsoft.graph.roomList/rooms",
  "value": [
    {
      "id": "3162F1E1-C4C0-604B-51D8-91DA78970B97",
      "emailAddress": "cf200@contoso.com",
      "displayName": "Conf Room 200",
      "address": {
        "street": "4567 Main Street",
        "city": "Buffalo",
        "state": "NY",
        "postalCode": "98052",
        "countryOrRegion": "USA"
      },
      "geoCoordinates": {
        "latitude": 47.640568390488625,
        "longitude": -122.1293731033802
      },
      "phone": "000-000-0000",
      "nickname": "Conf Room",
      "label": "200",
      "capacity": 40,
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelChairAccessible": false,
      "bookingType": "standard",
      "tags": [
        "benches",
        "nice view"
      ],
      "audioDeviceName": null,
      "videoDeviceName": null,
      "displayDevice": "surface hub"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List places",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


