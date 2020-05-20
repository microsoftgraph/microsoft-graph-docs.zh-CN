---
title: 列表位置
description: 检索 place 对象的列表。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 5344d1ffda70a9b2e9dd23d950319acbacc5482a
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290270"
---
# <a name="list-places"></a><span data-ttu-id="86f0f-103">列表位置</span><span class="sxs-lookup"><span data-stu-id="86f0f-103">List places</span></span>

<span data-ttu-id="86f0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86f0f-104">Namespace: microsoft.graph</span></span>


<span data-ttu-id="86f0f-105">获取在租户中定义的指定类型的[位置](../resources/place.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="86f0f-105">Get a collection of the specified type of [place](../resources/place.md) objects defined in the tenant.</span></span> <span data-ttu-id="86f0f-106">例如，您可以获取租户中的所有会议室、所有会议室列表或特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="86f0f-106">For example, you can get all the rooms, all the room lists, or the rooms in a specific room list in the tenant.</span></span>

<span data-ttu-id="86f0f-107">**Place**对象可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="86f0f-107">A **place** object can be one of the following types:</span></span>

* <span data-ttu-id="86f0f-108">包含丰富属性（如聊天室的电子邮件地址、辅助功能、容量和设备支持）的[会议室](../resources/room.md)。</span><span class="sxs-lookup"><span data-stu-id="86f0f-108">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span> 
* <span data-ttu-id="86f0f-109">包含会议室列表的电子邮件地址的[会议室列表](../resources/roomlist.md)，以及用于获取会议室列表中的会议室实例集合的导航属性。</span><span class="sxs-lookup"><span data-stu-id="86f0f-109">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of room instances in the room list.</span></span> 

<span data-ttu-id="86f0f-110">**聊天室**和**roomList**均派生自**place**对象。</span><span class="sxs-lookup"><span data-stu-id="86f0f-110">Both **room** and **roomList** are derived from the **place** object.</span></span>

<span data-ttu-id="86f0f-111">默认情况下，此操作返回每页100个位置。</span><span class="sxs-lookup"><span data-stu-id="86f0f-111">By default, this operation returns 100 places per page.</span></span> 

<span data-ttu-id="86f0f-112">与[findRooms](https://docs.microsoft.com/graph/api/user-findrooms?view=graph-rest-beta&tabs=http)和[findRoomLists](https://docs.microsoft.com/graph/api/user-findroomlists?view=graph-rest-beta)函数相比，此操作为聊天室和会议室列表返回更丰富的有效负载。</span><span class="sxs-lookup"><span data-stu-id="86f0f-112">Compared with the [findRooms](https://docs.microsoft.com/graph/api/user-findrooms?view=graph-rest-beta&tabs=http) and [findRoomLists](https://docs.microsoft.com/graph/api/user-findroomlists?view=graph-rest-beta) functions, this operation returns a richer payload for rooms and room lists.</span></span> <span data-ttu-id="86f0f-113">有关比较的详细信息，请参阅[详细信息](../resources/place.md#using-the-places-api)。</span><span class="sxs-lookup"><span data-stu-id="86f0f-113">See [details](../resources/place.md#using-the-places-api) for how they compare.</span></span>

## <a name="permissions"></a><span data-ttu-id="86f0f-114">Permissions</span><span class="sxs-lookup"><span data-stu-id="86f0f-114">Permissions</span></span>

<span data-ttu-id="86f0f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="86f0f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="86f0f-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="86f0f-117">Permission type</span></span>                        | <span data-ttu-id="86f0f-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="86f0f-118">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="86f0f-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="86f0f-119">Delegated (work or school account)</span></span>     | <span data-ttu-id="86f0f-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="86f0f-120">Place.Read.All</span></span> |
| <span data-ttu-id="86f0f-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="86f0f-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86f0f-122">不支持</span><span class="sxs-lookup"><span data-stu-id="86f0f-122">Not supported</span></span> |
| <span data-ttu-id="86f0f-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="86f0f-123">Application</span></span>                            | <span data-ttu-id="86f0f-124">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="86f0f-124">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="86f0f-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="86f0f-125">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="86f0f-126">若要获取租户中的所有聊天室，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="86f0f-126">To get all the rooms in a tenant:</span></span>

```http
GET /places/microsoft.graph.room
```

<span data-ttu-id="86f0f-127">若要获取租户中的所有会议室列表，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="86f0f-127">To get all the room lists in a tenant:</span></span>

```http
GET /places/microsoft.graph.roomlist
```

<span data-ttu-id="86f0f-128">若要获取指定会议室列表中的所有会议室，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="86f0f-128">To get all the rooms in the specified room list:</span></span>

```http
GET /places/{room-list-emailaddress}/microsoft.graph.roomlist/rooms
```

><span data-ttu-id="86f0f-129">**注意**：若要获取会议室列表中的聊天室，必须按其**emailAddress**属性（而不是**id**）指定会议室列表。</span><span class="sxs-lookup"><span data-stu-id="86f0f-129">**Note**: To get rooms in a room list, you must specify the room list by its **emailAddress** property, not by its **id**.</span></span> 

## <a name="optional-query-parameters"></a><span data-ttu-id="86f0f-130">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="86f0f-130">Optional query parameters</span></span>
<span data-ttu-id="86f0f-131">此方法支持以下查询参数来帮助自定义响应：</span><span class="sxs-lookup"><span data-stu-id="86f0f-131">This method supports the following query parameters to help customize the response:</span></span>
- `$filter`
- `$select`
- `$top`
- `$skip`
- `$count=true`

<span data-ttu-id="86f0f-132">使用 `$top` 自定义页面大小。</span><span class="sxs-lookup"><span data-stu-id="86f0f-132">Use `$top` to customize the page size.</span></span> <span data-ttu-id="86f0f-133">默认页面大小是 100。</span><span class="sxs-lookup"><span data-stu-id="86f0f-133">The default page size is 100.</span></span>

<span data-ttu-id="86f0f-134">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="86f0f-134">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="86f0f-135">请求标头</span><span class="sxs-lookup"><span data-stu-id="86f0f-135">Request headers</span></span>

| <span data-ttu-id="86f0f-136">名称</span><span class="sxs-lookup"><span data-stu-id="86f0f-136">Name</span></span>          | <span data-ttu-id="86f0f-137">说明</span><span class="sxs-lookup"><span data-stu-id="86f0f-137">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="86f0f-138">Authorization</span><span class="sxs-lookup"><span data-stu-id="86f0f-138">Authorization</span></span> | <span data-ttu-id="86f0f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="86f0f-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="86f0f-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="86f0f-141">Request body</span></span>

<span data-ttu-id="86f0f-142">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="86f0f-142">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="86f0f-143">响应</span><span class="sxs-lookup"><span data-stu-id="86f0f-143">Response</span></span>

<span data-ttu-id="86f0f-144">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[place](../resources/place.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="86f0f-144">If successful, this method returns a `200 OK` response code and a collection of [place](../resources/place.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="86f0f-145">示例</span><span class="sxs-lookup"><span data-stu-id="86f0f-145">Examples</span></span>

### <a name="example-1-list-all-the-rooms-defined-in-the-tenant"></a><span data-ttu-id="86f0f-146">示例1：列出租户中定义的所有聊天室</span><span class="sxs-lookup"><span data-stu-id="86f0f-146">Example 1: List all the rooms defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="86f0f-147">请求</span><span class="sxs-lookup"><span data-stu-id="86f0f-147">Request</span></span>

<span data-ttu-id="86f0f-148">下面的示例演示如何获取租户中的所有[聊天室](../resources/room.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86f0f-148">The following example shows how to get all the [room](../resources/room.md) objects in the tenant.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_all_rooms"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.room
```

#### <a name="response"></a><span data-ttu-id="86f0f-149">响应</span><span class="sxs-lookup"><span data-stu-id="86f0f-149">Response</span></span>

<span data-ttu-id="86f0f-150">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86f0f-150">The following is an example of the response.</span></span>

><span data-ttu-id="86f0f-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="86f0f-151">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="86f0f-152">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86f0f-152">All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/microsoft.graph.room",
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
      "capacity": "50",
      "building": "1",
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
      "capacity": "40",
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelchairAccessible": false,
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

### <a name="example-2-list-all-the-room-lists-defined-in-the-tenant"></a><span data-ttu-id="86f0f-153">示例2：列出租户中定义的所有会议室列表</span><span class="sxs-lookup"><span data-stu-id="86f0f-153">Example 2: List all the room lists defined in the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="86f0f-154">请求</span><span class="sxs-lookup"><span data-stu-id="86f0f-154">Request</span></span>

<span data-ttu-id="86f0f-155">下面的示例演示如何获取租户中的所有[roomList](../resources/roomlist.md)对象。</span><span class="sxs-lookup"><span data-stu-id="86f0f-155">The following example shows how to get all the [roomList](../resources/roomlist.md) objects in the tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_all_roomlists"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/microsoft.graph.roomlist
```

#### <a name="response"></a><span data-ttu-id="86f0f-156">响应</span><span class="sxs-lookup"><span data-stu-id="86f0f-156">Response</span></span>

<span data-ttu-id="86f0f-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86f0f-157">The following is an example of the response.</span></span>

><span data-ttu-id="86f0f-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="86f0f-158">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="86f0f-159">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86f0f-159">All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places/microsoft.graph.roomList",
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

### <a name="example-3-list-rooms-contained-in-a-room-list"></a><span data-ttu-id="86f0f-160">示例3：会议室列表中包含的会议室</span><span class="sxs-lookup"><span data-stu-id="86f0f-160">Example 3: List rooms contained in a room list</span></span>

#### <a name="request"></a><span data-ttu-id="86f0f-161">请求</span><span class="sxs-lookup"><span data-stu-id="86f0f-161">Request</span></span>

<span data-ttu-id="86f0f-162">下面的示例演示如何获取**roomList**中包含的[聊天室](../resources/room.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="86f0f-162">The following example shows how to get a list of [room](../resources/room.md) objects contained in a **roomList**.</span></span> 

<!-- {
  "blockType": "request",
  "name": "get_rooms_in_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg2@contoso.com/microsoft.graph.roomlist/rooms
```

#### <a name="response"></a><span data-ttu-id="86f0f-163">响应</span><span class="sxs-lookup"><span data-stu-id="86f0f-163">Response</span></span>

<span data-ttu-id="86f0f-164">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="86f0f-164">The following is an example of the response.</span></span>

><span data-ttu-id="86f0f-165">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="86f0f-165">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="86f0f-166">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="86f0f-166">All the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#places('bldg2%40contoso.com')/microsoft.graph.roomList/rooms",
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
      "capacity": "40",
      "building": "2",
      "floorNumber": 2,
      "isManaged": true,
      "isWheelchairAccessible": false,
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
    "Error: Malformed function params 'id-of-roomlist'"
  ]
}-->
