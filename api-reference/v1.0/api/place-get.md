---
title: 获取位置
description: 检索 place 对象的属性和关系。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 3934a6cbb683e6bd6591e2dfcc33f8361bc4d0e5
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290481"
---
# <a name="get-place"></a><span data-ttu-id="c87ff-103">获取位置</span><span class="sxs-lookup"><span data-stu-id="c87ff-103">Get place</span></span>

<span data-ttu-id="c87ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c87ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c87ff-105">获取由其 ID 或电子邮件地址指定的[place](../resources/place.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c87ff-105">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="c87ff-106">**Place**对象可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="c87ff-106">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="c87ff-107">包含丰富属性（如聊天室的电子邮件地址、辅助功能、容量和设备支持）的[会议室](../resources/room.md)。</span><span class="sxs-lookup"><span data-stu-id="c87ff-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="c87ff-108">包含会议室列表的电子邮件地址的[会议室列表](../resources/roomlist.md)，以及用于获取该会议室列表中的**会议室**实例集合的导航属性。</span><span class="sxs-lookup"><span data-stu-id="c87ff-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="c87ff-109">**聊天室**和**roomList**均派生自[place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c87ff-109">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="c87ff-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="c87ff-110">Permissions</span></span>

<span data-ttu-id="c87ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c87ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c87ff-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c87ff-113">Permission type</span></span>                        | <span data-ttu-id="c87ff-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c87ff-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c87ff-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c87ff-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="c87ff-116">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="c87ff-116">Place.Read.All</span></span> |
| <span data-ttu-id="c87ff-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c87ff-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c87ff-118">不支持</span><span class="sxs-lookup"><span data-stu-id="c87ff-118">Not supported</span></span> |
| <span data-ttu-id="c87ff-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c87ff-119">Application</span></span>                            | <span data-ttu-id="c87ff-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="c87ff-120">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c87ff-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c87ff-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c87ff-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c87ff-122">Optional query parameters</span></span>
<span data-ttu-id="c87ff-123">用于 `$select` 获取特定的**位置**属性。</span><span class="sxs-lookup"><span data-stu-id="c87ff-123">Use `$select` to get specific **place** properties.</span></span>

<span data-ttu-id="c87ff-124">有关详细信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c87ff-124">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c87ff-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="c87ff-125">Request headers</span></span>

| <span data-ttu-id="c87ff-126">名称</span><span class="sxs-lookup"><span data-stu-id="c87ff-126">Name</span></span>          | <span data-ttu-id="c87ff-127">说明</span><span class="sxs-lookup"><span data-stu-id="c87ff-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="c87ff-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="c87ff-128">Authorization</span></span> | <span data-ttu-id="c87ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c87ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c87ff-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c87ff-131">Request body</span></span>

<span data-ttu-id="c87ff-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c87ff-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c87ff-133">响应</span><span class="sxs-lookup"><span data-stu-id="c87ff-133">Response</span></span>

<span data-ttu-id="c87ff-134">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和请求的[place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c87ff-134">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c87ff-135">示例</span><span class="sxs-lookup"><span data-stu-id="c87ff-135">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="c87ff-136">示例1：获取聊天室</span><span class="sxs-lookup"><span data-stu-id="c87ff-136">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="c87ff-137">请求</span><span class="sxs-lookup"><span data-stu-id="c87ff-137">Request</span></span>

<span data-ttu-id="c87ff-138">下面的示例指定用于获取其属性的**聊天室**的**id** 。</span><span class="sxs-lookup"><span data-stu-id="c87ff-138">The following example specifies the **id** of a **room** to get its properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```

#### <a name="response"></a><span data-ttu-id="c87ff-139">响应</span><span class="sxs-lookup"><span data-stu-id="c87ff-139">Response</span></span>

<span data-ttu-id="c87ff-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c87ff-140">The following is an example of the response.</span></span>

><span data-ttu-id="c87ff-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c87ff-141">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c87ff-142">所有属性都是从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c87ff-142">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_room",
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
}
```

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="c87ff-143">示例2：获取会议室列表</span><span class="sxs-lookup"><span data-stu-id="c87ff-143">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="c87ff-144">请求</span><span class="sxs-lookup"><span data-stu-id="c87ff-144">Request</span></span>

<span data-ttu-id="c87ff-145">下面的示例指定**roomList**的**emailAddress**以获取其属性。</span><span class="sxs-lookup"><span data-stu-id="c87ff-145">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg1@contoso.com
```


#### <a name="response"></a><span data-ttu-id="c87ff-146">响应</span><span class="sxs-lookup"><span data-stu-id="c87ff-146">Response</span></span>

<span data-ttu-id="c87ff-147">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c87ff-147">The following is an example of the response.</span></span>

><span data-ttu-id="c87ff-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c87ff-148">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c87ff-149">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c87ff-149">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "name": "get_roomlist",
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
  "geocoordinates": null,
  "phone": null,
  "emailAddress": "bldg1@contoso.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get place",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
