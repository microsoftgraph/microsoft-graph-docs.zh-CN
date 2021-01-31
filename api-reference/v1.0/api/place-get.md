---
title: 获取位置
description: 检索 place 对象的属性和关系。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 2579bac8f3e9b9a3cd951ea5c533541edacb1308
ms.sourcegitcommit: 1138d6e84f64f3727e180da10f89b89021855c3e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2021
ms.locfileid: "50059649"
---
# <a name="get-place"></a><span data-ttu-id="cc024-103">获取位置</span><span class="sxs-lookup"><span data-stu-id="cc024-103">Get place</span></span>

<span data-ttu-id="cc024-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc024-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc024-105">获取由位置对象 ID[](../resources/place.md)或电子邮件地址指定的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cc024-105">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span>

<span data-ttu-id="cc024-106">**place** 对象可以是下列类型之一：</span><span class="sxs-lookup"><span data-stu-id="cc024-106">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="cc024-107">[包含](../resources/room.md)丰富的属性（如会议室的电子邮件地址）以及辅助功能、容量和设备支持的聊天室。</span><span class="sxs-lookup"><span data-stu-id="cc024-107">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="cc024-108">包含 [会议室](../resources/roomlist.md) 列表的电子邮件地址的会议室列表，以及用于获取该会议室列表中的 **会议室实例集合** 的导航属性。</span><span class="sxs-lookup"><span data-stu-id="cc024-108">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="cc024-109">**room** 和 **roomList** 都派生自 [place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cc024-109">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="cc024-110">权限</span><span class="sxs-lookup"><span data-stu-id="cc024-110">Permissions</span></span>

<span data-ttu-id="cc024-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc024-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="cc024-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc024-113">Permission type</span></span>                        | <span data-ttu-id="cc024-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc024-114">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="cc024-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc024-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="cc024-116">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc024-116">Place.Read.All</span></span> |
| <span data-ttu-id="cc024-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc024-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc024-118">不支持</span><span class="sxs-lookup"><span data-stu-id="cc024-118">Not supported</span></span> |
| <span data-ttu-id="cc024-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc024-119">Application</span></span>                            | <span data-ttu-id="cc024-120">Place.Read.All</span><span class="sxs-lookup"><span data-stu-id="cc024-120">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cc024-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc024-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cc024-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cc024-122">Optional query parameters</span></span>
<span data-ttu-id="cc024-123">用于 `$select` 获取特定 **位置** 属性。</span><span class="sxs-lookup"><span data-stu-id="cc024-123">Use `$select` to get specific **place** properties.</span></span>

<span data-ttu-id="cc024-124">有关详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="cc024-124">For more information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cc024-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc024-125">Request headers</span></span>

| <span data-ttu-id="cc024-126">名称</span><span class="sxs-lookup"><span data-stu-id="cc024-126">Name</span></span>          | <span data-ttu-id="cc024-127">说明</span><span class="sxs-lookup"><span data-stu-id="cc024-127">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="cc024-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc024-128">Authorization</span></span> | <span data-ttu-id="cc024-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cc024-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cc024-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc024-131">Request body</span></span>

<span data-ttu-id="cc024-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cc024-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc024-133">响应</span><span class="sxs-lookup"><span data-stu-id="cc024-133">Response</span></span>

<span data-ttu-id="cc024-134">如果成功，此方法在响应正文中返回响应代码和 `200 OK` 请求的 [place](../resources/place.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc024-134">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cc024-135">示例</span><span class="sxs-lookup"><span data-stu-id="cc024-135">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="cc024-136">示例 1：获取聊天室</span><span class="sxs-lookup"><span data-stu-id="cc024-136">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="cc024-137">请求</span><span class="sxs-lookup"><span data-stu-id="cc024-137">Request</span></span>

<span data-ttu-id="cc024-138">以下示例指定要 **获取** 其属性 **的** 聊天室的 ID。</span><span class="sxs-lookup"><span data-stu-id="cc024-138">The following example specifies the **id** of a **room** to get its properties.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc024-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc024-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="c"></a>[<span data-ttu-id="cc024-140">C#</span><span class="sxs-lookup"><span data-stu-id="cc024-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc024-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc024-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc024-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc024-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc024-143">Java</span><span class="sxs-lookup"><span data-stu-id="cc024-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-room-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="cc024-144">响应</span><span class="sxs-lookup"><span data-stu-id="cc024-144">Response</span></span>

<span data-ttu-id="cc024-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cc024-145">The following is an example of the response.</span></span>

><span data-ttu-id="cc024-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cc024-146">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cc024-147">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cc024-147">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="cc024-148">示例 2：获取会议室列表</span><span class="sxs-lookup"><span data-stu-id="cc024-148">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="cc024-149">请求</span><span class="sxs-lookup"><span data-stu-id="cc024-149">Request</span></span>

<span data-ttu-id="cc024-150">以下示例指定 **roomList** **的 emailAddress，** 以获取其属性。</span><span class="sxs-lookup"><span data-stu-id="cc024-150">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>


# <a name="http"></a>[<span data-ttu-id="cc024-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc024-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/places/bldg1@contoso.com
```
# <a name="c"></a>[<span data-ttu-id="cc024-152">C#</span><span class="sxs-lookup"><span data-stu-id="cc024-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cc024-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc024-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cc024-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cc024-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cc024-155">Java</span><span class="sxs-lookup"><span data-stu-id="cc024-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-roomlist-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="cc024-156">响应</span><span class="sxs-lookup"><span data-stu-id="cc024-156">Response</span></span>

<span data-ttu-id="cc024-157">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cc024-157">The following is an example of the response.</span></span>

><span data-ttu-id="cc024-158">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cc024-158">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cc024-159">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cc024-159">All the properties will be returned from an actual call.</span></span>

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

