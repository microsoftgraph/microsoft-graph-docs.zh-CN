---
title: 获取位置
description: 检索 place 对象的属性和关系。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 30a2b2c0f85019ac5e11b5b22850be2722b94de4
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36413599"
---
# <a name="get-place"></a><span data-ttu-id="9ceb9-103">获取位置</span><span class="sxs-lookup"><span data-stu-id="9ceb9-103">Get place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="9ceb9-104">获取由其 ID 或电子邮件地址指定的[place](../resources/place.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-104">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="9ceb9-105">**Place**对象可以是下列类型之一:</span><span class="sxs-lookup"><span data-stu-id="9ceb9-105">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="9ceb9-106">包含丰富属性 (如聊天室的电子邮件地址、辅助功能、容量和设备支持) 的[会议室](../resources/room.md)。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-106">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="9ceb9-107">包含会议室列表的电子邮件地址的[会议室列表](../resources/roomlist.md), 以及用于获取该会议室列表中的**会议室**实例集合的导航属性。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-107">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="9ceb9-108">**聊天室**和**roomList**均派生自[place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-108">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="9ceb9-109">权限</span><span class="sxs-lookup"><span data-stu-id="9ceb9-109">Permissions</span></span>

<span data-ttu-id="9ceb9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9ceb9-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ceb9-112">Permission type</span></span>                        | <span data-ttu-id="9ceb9-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ceb9-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9ceb9-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ceb9-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="9ceb9-115">将. 所有</span><span class="sxs-lookup"><span data-stu-id="9ceb9-115">Place.Read.All</span></span> |
| <span data-ttu-id="9ceb9-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ceb9-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ceb9-117">不支持</span><span class="sxs-lookup"><span data-stu-id="9ceb9-117">Not supported</span></span> |
| <span data-ttu-id="9ceb9-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ceb9-118">Application</span></span>                            | <span data-ttu-id="9ceb9-119">将. 所有</span><span class="sxs-lookup"><span data-stu-id="9ceb9-119">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ceb9-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ceb9-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9ceb9-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9ceb9-121">Optional query parameters</span></span>

<span data-ttu-id="9ceb9-122">此方法支持以下查询参数来帮助自定义响应:</span><span class="sxs-lookup"><span data-stu-id="9ceb9-122">This method supports the following query parameters to help customize the response:</span></span>
* <span data-ttu-id="9ceb9-123">$filter</span><span class="sxs-lookup"><span data-stu-id="9ceb9-123">$filter</span></span>
* <span data-ttu-id="9ceb9-124">$select</span><span class="sxs-lookup"><span data-stu-id="9ceb9-124">$select</span></span>
* <span data-ttu-id="9ceb9-125">$top</span><span class="sxs-lookup"><span data-stu-id="9ceb9-125">$top</span></span>

<span data-ttu-id="9ceb9-126">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9ceb9-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ceb9-127">Request headers</span></span>

| <span data-ttu-id="9ceb9-128">名称</span><span class="sxs-lookup"><span data-stu-id="9ceb9-128">Name</span></span>          | <span data-ttu-id="9ceb9-129">说明</span><span class="sxs-lookup"><span data-stu-id="9ceb9-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="9ceb9-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ceb9-130">Authorization</span></span> | <span data-ttu-id="9ceb9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ceb9-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ceb9-133">Request body</span></span>

<span data-ttu-id="9ceb9-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ceb9-135">响应</span><span class="sxs-lookup"><span data-stu-id="9ceb9-135">Response</span></span>

<span data-ttu-id="9ceb9-136">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-136">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9ceb9-137">示例</span><span class="sxs-lookup"><span data-stu-id="9ceb9-137">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="9ceb9-138">示例 1: 获取聊天室</span><span class="sxs-lookup"><span data-stu-id="9ceb9-138">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="9ceb9-139">请求</span><span class="sxs-lookup"><span data-stu-id="9ceb9-139">Request</span></span>

<span data-ttu-id="9ceb9-140">下面的示例指定用于获取其属性的**聊天室**的**id** 。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-140">The following example specifies the **id** of a **room** to get its properties.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ceb9-141">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9ceb9-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```http
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ceb9-142">C#</span><span class="sxs-lookup"><span data-stu-id="9ceb9-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-room-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ceb9-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ceb9-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-room-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ceb9-144">目标-C</span><span class="sxs-lookup"><span data-stu-id="9ceb9-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-room-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ceb9-145">响应</span><span class="sxs-lookup"><span data-stu-id="9ceb9-145">Response</span></span>

<span data-ttu-id="9ceb9-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-146">The following is an example of the response.</span></span>

><span data-ttu-id="9ceb9-147">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-147">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ceb9-148">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-148">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="9ceb9-149">示例 2: 获取会议室列表</span><span class="sxs-lookup"><span data-stu-id="9ceb9-149">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="9ceb9-150">请求</span><span class="sxs-lookup"><span data-stu-id="9ceb9-150">Request</span></span>

<span data-ttu-id="9ceb9-151">下面的示例指定**roomList**的**emailAddress**以获取其属性。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-151">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9ceb9-152">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9ceb9-152">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="9ceb9-153">C#</span><span class="sxs-lookup"><span data-stu-id="9ceb9-153">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-roomlist-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9ceb9-154">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ceb9-154">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-roomlist-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9ceb9-155">目标-C</span><span class="sxs-lookup"><span data-stu-id="9ceb9-155">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-roomlist-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9ceb9-156">响应</span><span class="sxs-lookup"><span data-stu-id="9ceb9-156">Response</span></span>

<span data-ttu-id="9ceb9-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-157">The following is an example of the response.</span></span>

><span data-ttu-id="9ceb9-158">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-158">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="9ceb9-159">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9ceb9-159">All the properties will be returned from an actual call.</span></span>

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
