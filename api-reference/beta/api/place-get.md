---
title: 获取位置
description: 检索 place 对象的属性和关系。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2a5c259d05b88a6195a76420e573d6bbff155065
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055398"
---
# <a name="get-place"></a><span data-ttu-id="354f6-103">获取位置</span><span class="sxs-lookup"><span data-stu-id="354f6-103">Get place</span></span>

<span data-ttu-id="354f6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="354f6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="354f6-105">获取由其 ID 或电子邮件地址 [指定的 place](../resources/place.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="354f6-105">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="354f6-106">**place** 对象可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="354f6-106">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="354f6-107">[包含](../resources/room.md)丰富属性（如会议室的电子邮件地址）以及辅助功能、容量和设备支持的聊天室。</span><span class="sxs-lookup"><span data-stu-id="354f6-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="354f6-108">[包含会议室](../resources/roomlist.md)列表的电子邮件地址的会议室列表，以及用于获取该会议室列表中的会议室实例集合的导航属性。 </span><span class="sxs-lookup"><span data-stu-id="354f6-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="354f6-109">**room 和** **roomList** 均派生自 [place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="354f6-109">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="354f6-110">权限</span><span class="sxs-lookup"><span data-stu-id="354f6-110">Permissions</span></span>

<span data-ttu-id="354f6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="354f6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="354f6-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="354f6-113">Permission type</span></span>                        | <span data-ttu-id="354f6-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="354f6-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="354f6-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="354f6-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="354f6-116">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="354f6-116">Place.Read.All</span></span> |
| <span data-ttu-id="354f6-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="354f6-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="354f6-118">不支持</span><span class="sxs-lookup"><span data-stu-id="354f6-118">Not supported</span></span> |
| <span data-ttu-id="354f6-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="354f6-119">Application</span></span>                            | <span data-ttu-id="354f6-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="354f6-120">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="354f6-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="354f6-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="354f6-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="354f6-122">Optional query parameters</span></span>
<span data-ttu-id="354f6-123">使用 $select 获取特定 **位置** 属性。</span><span class="sxs-lookup"><span data-stu-id="354f6-123">Use $select to get specific **place** properties.</span></span>

<span data-ttu-id="354f6-124">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="354f6-124">For more information on OData query options, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="354f6-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="354f6-125">Request headers</span></span>

| <span data-ttu-id="354f6-126">名称</span><span class="sxs-lookup"><span data-stu-id="354f6-126">Name</span></span>          | <span data-ttu-id="354f6-127">说明</span><span class="sxs-lookup"><span data-stu-id="354f6-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="354f6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="354f6-128">Authorization</span></span> | <span data-ttu-id="354f6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="354f6-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="354f6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="354f6-131">Request body</span></span>

<span data-ttu-id="354f6-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="354f6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="354f6-133">响应</span><span class="sxs-lookup"><span data-stu-id="354f6-133">Response</span></span>

<span data-ttu-id="354f6-134">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` 请求的 [place](../resources/place.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="354f6-134">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="354f6-135">示例</span><span class="sxs-lookup"><span data-stu-id="354f6-135">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="354f6-136">示例 1：获取聊天室</span><span class="sxs-lookup"><span data-stu-id="354f6-136">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="354f6-137">请求</span><span class="sxs-lookup"><span data-stu-id="354f6-137">Request</span></span>

<span data-ttu-id="354f6-138">以下示例指定要 **获取** 其 **属性的聊天室** 的 ID。</span><span class="sxs-lookup"><span data-stu-id="354f6-138">The following example specifies the **id** of a **room** to get its properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="354f6-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="354f6-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="c"></a>[<span data-ttu-id="354f6-140">C#</span><span class="sxs-lookup"><span data-stu-id="354f6-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="354f6-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="354f6-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="354f6-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="354f6-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="354f6-143">Java</span><span class="sxs-lookup"><span data-stu-id="354f6-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="354f6-144">响应</span><span class="sxs-lookup"><span data-stu-id="354f6-144">Response</span></span>

<span data-ttu-id="354f6-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="354f6-145">The following is an example of the response.</span></span>

><span data-ttu-id="354f6-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="354f6-146">**Note**: The response object shown here might be shortened for readability.</span></span>

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
}
```

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="354f6-147">示例 2：获取会议室列表</span><span class="sxs-lookup"><span data-stu-id="354f6-147">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="354f6-148">请求</span><span class="sxs-lookup"><span data-stu-id="354f6-148">Request</span></span>

<span data-ttu-id="354f6-149">以下示例指定 **roomList** **的 emailAddress，** 以获取其属性。</span><span class="sxs-lookup"><span data-stu-id="354f6-149">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>

# <a name="http"></a>[<span data-ttu-id="354f6-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="354f6-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```
# <a name="c"></a>[<span data-ttu-id="354f6-151">C#</span><span class="sxs-lookup"><span data-stu-id="354f6-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="354f6-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="354f6-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="354f6-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="354f6-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="354f6-154">Java</span><span class="sxs-lookup"><span data-stu-id="354f6-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="354f6-155">响应</span><span class="sxs-lookup"><span data-stu-id="354f6-155">Response</span></span>

<span data-ttu-id="354f6-156">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="354f6-156">The following is an example of the response.</span></span>

><span data-ttu-id="354f6-157">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="354f6-157">**Note**: The response object shown here might be shortened for readability.</span></span>

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


