---
title: 列出位置
description: 检索 place 对象的列表。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 019198d0173155c673e12a266bcf41922e040f81
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055391"
---
# <a name="list-places"></a><span data-ttu-id="b5e19-103">列出位置</span><span class="sxs-lookup"><span data-stu-id="b5e19-103">List places</span></span>

<span data-ttu-id="b5e19-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5e19-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5e19-105">获取租户中定义的指定 [类型 place](../resources/place.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="b5e19-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="b5e19-106">例如，可以获取租户中所有会议室、所有会议室列表或特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="b5e19-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="b5e19-107">**place** 对象可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="b5e19-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="b5e19-108">[包含](../resources/room.md)丰富属性（如会议室的电子邮件地址）以及辅助功能、容量和设备支持的聊天室。</span><span class="sxs-lookup"><span data-stu-id="b5e19-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="b5e19-109">[包含会议室](../resources/roomlist.md)列表的电子邮件地址的会议室列表，以及用于获取会议室列表中会议室实例集合的导航属性。</span><span class="sxs-lookup"><span data-stu-id="b5e19-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="b5e19-110">**room 和** **roomList** 均派生自 **place** 对象。</span><span class="sxs-lookup"><span data-stu-id="b5e19-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="b5e19-111">默认情况下，此操作返回每页 100 个位置。</span><span class="sxs-lookup"><span data-stu-id="b5e19-111">By default, this operation returns 100 places per page.</span></span> 

<span data-ttu-id="b5e19-112">与 [findRooms 和](../api/user-findrooms.md) [findRoomLists](../api/user-findroomlists.md) 函数相比，此操作为会议室和会议室列表返回更丰富的有效负载。</span><span class="sxs-lookup"><span data-stu-id="b5e19-112">Compared with the [findRooms](../api/user-findrooms.md) and [findRoomLists](../api/user-findroomlists.md) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="b5e19-113">请参阅 [有关](../resources/place.md#using-the-places-api) 它们如何比较的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b5e19-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5e19-114">权限</span><span class="sxs-lookup"><span data-stu-id="b5e19-114">Permissions</span></span>

<span data-ttu-id="b5e19-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5e19-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b5e19-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5e19-117">Permission type</span></span>                        | <span data-ttu-id="b5e19-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5e19-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b5e19-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5e19-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="b5e19-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5e19-120">Place.Read.All</span></span> |
| <span data-ttu-id="b5e19-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5e19-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5e19-122">不支持</span><span class="sxs-lookup"><span data-stu-id="b5e19-122">Not supported</span></span> |
| <span data-ttu-id="b5e19-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5e19-123">Application</span></span>                            | <span data-ttu-id="b5e19-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="b5e19-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5e19-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5e19-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="b5e19-126">若要获取租户中所有会议室，</span><span class="sxs-lookup"><span data-stu-id="b5e19-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="b5e19-127">若要获取租户中所有会议室列表，请进行以下设置：</span><span class="sxs-lookup"><span data-stu-id="b5e19-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="b5e19-128">若要获取指定会议室列表中的所有会议室，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="b5e19-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="b5e19-129">**注意**：若要获取会议室列表中的会议室，必须按 **其 emailAddress** 属性指定会议室列表，而不是按 **其 id 指定**。</span><span class="sxs-lookup"><span data-stu-id="b5e19-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="b5e19-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b5e19-130">Optional query parameters</span></span>
<span data-ttu-id="b5e19-131">此方法支持以下查询参数来帮助自定义响应：</span><span class="sxs-lookup"><span data-stu-id="b5e19-131">This method supports the following query parameters to help customize the response:</span></span>
- <span data-ttu-id="b5e19-132">$filter</span><span class="sxs-lookup"><span data-stu-id="b5e19-132">$filter</span></span>
- <span data-ttu-id="b5e19-133">$select</span><span class="sxs-lookup"><span data-stu-id="b5e19-133">$select</span></span>
- <span data-ttu-id="b5e19-134">$top</span><span class="sxs-lookup"><span data-stu-id="b5e19-134">$top</span></span>
- <span data-ttu-id="b5e19-135">$skip</span><span class="sxs-lookup"><span data-stu-id="b5e19-135">$skip</span></span>
- <span data-ttu-id="b5e19-136">$count=true</span><span class="sxs-lookup"><span data-stu-id="b5e19-136">$count=true</span></span>

<span data-ttu-id="b5e19-137">使用$top自定义页面大小。</span><span class="sxs-lookup"><span data-stu-id="b5e19-137">Use $top to customize the page size.</span></span> <span data-ttu-id="b5e19-138">默认页面大小是 100。</span><span class="sxs-lookup"><span data-stu-id="b5e19-138">The default page size is 100.</span></span>

<span data-ttu-id="b5e19-139">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="b5e19-139">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5e19-140">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5e19-140">Request headers</span></span>

| <span data-ttu-id="b5e19-141">名称</span><span class="sxs-lookup"><span data-stu-id="b5e19-141">Name</span></span>          | <span data-ttu-id="b5e19-142">说明</span><span class="sxs-lookup"><span data-stu-id="b5e19-142">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="b5e19-143">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5e19-143">Authorization</span></span> | <span data-ttu-id="b5e19-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5e19-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5e19-146">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5e19-146">Request body</span></span>

<span data-ttu-id="b5e19-147">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5e19-147">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5e19-148">响应</span><span class="sxs-lookup"><span data-stu-id="b5e19-148">Response</span></span>

<span data-ttu-id="b5e19-149">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [place](../resources/place.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b5e19-149">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b5e19-150">示例</span><span class="sxs-lookup"><span data-stu-id="b5e19-150">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="b5e19-151">示例 1：列出租户中定义的所有会议室</span><span class="sxs-lookup"><span data-stu-id="b5e19-151">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="b5e19-152">请求</span><span class="sxs-lookup"><span data-stu-id="b5e19-152">Request</span></span>

<span data-ttu-id="b5e19-153">以下示例演示如何获取租户 [中所有](../resources/room.md) 会议室对象。</span><span class="sxs-lookup"><span data-stu-id="b5e19-153">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5e19-154">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e19-154">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.room
```
# <a name="c"></a>[<span data-ttu-id="b5e19-155">C#</span><span class="sxs-lookup"><span data-stu-id="b5e19-155">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-rooms-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5e19-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5e19-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-rooms-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5e19-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5e19-157">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-rooms-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5e19-158">Java</span><span class="sxs-lookup"><span data-stu-id="b5e19-158">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-rooms-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5e19-159">响应</span><span class="sxs-lookup"><span data-stu-id="b5e19-159">Response</span></span>

<span data-ttu-id="b5e19-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b5e19-160">The following is an example of the response.</span></span>

><span data-ttu-id="b5e19-161">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b5e19-161">**Note**: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="b5e19-162">示例 2：列出租户中定义的所有会议室列表</span><span class="sxs-lookup"><span data-stu-id="b5e19-162">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="b5e19-163">请求</span><span class="sxs-lookup"><span data-stu-id="b5e19-163">Request</span></span>

<span data-ttu-id="b5e19-164">以下示例演示如何获取租户中 [所有 roomList](../resources/roomlist.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5e19-164">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

# <a name="http"></a>[<span data-ttu-id="b5e19-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e19-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/microsoft.graph.roomlist
```
# <a name="c"></a>[<span data-ttu-id="b5e19-166">C#</span><span class="sxs-lookup"><span data-stu-id="b5e19-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-all-roomlists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5e19-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5e19-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-all-roomlists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5e19-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5e19-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-all-roomlists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5e19-169">Java</span><span class="sxs-lookup"><span data-stu-id="b5e19-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-all-roomlists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5e19-170">响应</span><span class="sxs-lookup"><span data-stu-id="b5e19-170">Response</span></span>

<span data-ttu-id="b5e19-171">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b5e19-171">The following is an example of the response.</span></span>

><span data-ttu-id="b5e19-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b5e19-172">**Note**: The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="b5e19-173">示例 3：列出包含在会议室列表中的聊天室</span><span class="sxs-lookup"><span data-stu-id="b5e19-173">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="b5e19-174">请求</span><span class="sxs-lookup"><span data-stu-id="b5e19-174">Request</span></span>

<span data-ttu-id="b5e19-175">以下示例演示如何获取 **roomList** 中包含的 [会议室](../resources/room.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="b5e19-175">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

# <a name="http"></a>[<span data-ttu-id="b5e19-176">HTTP</span><span class="sxs-lookup"><span data-stu-id="b5e19-176">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```
# <a name="c"></a>[<span data-ttu-id="b5e19-177">C#</span><span class="sxs-lookup"><span data-stu-id="b5e19-177">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-rooms-in-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="b5e19-178">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5e19-178">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-rooms-in-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="b5e19-179">Objective-C</span><span class="sxs-lookup"><span data-stu-id="b5e19-179">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-rooms-in-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="b5e19-180">Java</span><span class="sxs-lookup"><span data-stu-id="b5e19-180">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-rooms-in-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="b5e19-181">响应</span><span class="sxs-lookup"><span data-stu-id="b5e19-181">Response</span></span>

<span data-ttu-id="b5e19-182">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b5e19-182">The following is an example of the response.</span></span>

><span data-ttu-id="b5e19-183">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b5e19-183">**Note**: The response object shown here might be shortened for readability.</span></span>

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


