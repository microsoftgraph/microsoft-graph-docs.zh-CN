---
title: 获取位置
description: 检索 place 对象的属性和关系。
localization_priority: Normal
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 1b53f6b1cb89bb4c5b3d02d5b32154877a5de706
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/24/2019
ms.locfileid: "35841064"
---
# <a name="get-place"></a><span data-ttu-id="f0d06-103">获取位置</span><span class="sxs-lookup"><span data-stu-id="f0d06-103">Get place</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="f0d06-104">获取由其 ID 或电子邮件地址指定的[place](../resources/place.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f0d06-104">Get the properties and relationships of a [place](../resources/place.md) object specified by either its ID or email address.</span></span> 

<span data-ttu-id="f0d06-105">**Place**对象可以是下列类型之一:</span><span class="sxs-lookup"><span data-stu-id="f0d06-105">The **place** object can be one of the following types:</span></span>

* <span data-ttu-id="f0d06-106">包含丰富属性 (如聊天室的电子邮件地址、辅助功能、容量和设备支持) 的[会议室](../resources/room.md)。</span><span class="sxs-lookup"><span data-stu-id="f0d06-106">A [room](../resources/room.md) which includes rich properties such as an email address for the room, and accessibility, capacity, and device support.</span></span>
* <span data-ttu-id="f0d06-107">包含会议室列表的电子邮件地址的[会议室列表](../resources/roomlist.md), 以及用于获取该会议室列表中的**会议室**实例集合的导航属性。</span><span class="sxs-lookup"><span data-stu-id="f0d06-107">A [room list](../resources/roomlist.md) which includes an email address for the room list, and a navigation property to get the collection of **room** instances in that room list.</span></span>

<span data-ttu-id="f0d06-108">**聊天室**和**roomList**均派生自[place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f0d06-108">Both **room** and **roomList** are derived from the [place](../resources/place.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f0d06-109">权限</span><span class="sxs-lookup"><span data-stu-id="f0d06-109">Permissions</span></span>

<span data-ttu-id="f0d06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0d06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f0d06-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0d06-112">Permission type</span></span>                        | <span data-ttu-id="f0d06-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0d06-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f0d06-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0d06-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="f0d06-115">将. 所有</span><span class="sxs-lookup"><span data-stu-id="f0d06-115">Place.Read.All</span></span> |
| <span data-ttu-id="f0d06-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0d06-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0d06-117">不支持</span><span class="sxs-lookup"><span data-stu-id="f0d06-117">Not supported</span></span> |
| <span data-ttu-id="f0d06-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0d06-118">Application</span></span>                            | <span data-ttu-id="f0d06-119">将. 所有</span><span class="sxs-lookup"><span data-stu-id="f0d06-119">Place.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0d06-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0d06-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /places/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0d06-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f0d06-121">Optional query parameters</span></span>

<span data-ttu-id="f0d06-122">此方法支持以下查询参数来帮助自定义响应:</span><span class="sxs-lookup"><span data-stu-id="f0d06-122">This method supports the following query parameters to help customize the response:</span></span>
* <span data-ttu-id="f0d06-123">$filter</span><span class="sxs-lookup"><span data-stu-id="f0d06-123">$filter</span></span>
* <span data-ttu-id="f0d06-124">$select</span><span class="sxs-lookup"><span data-stu-id="f0d06-124">$select</span></span>
* <span data-ttu-id="f0d06-125">$top</span><span class="sxs-lookup"><span data-stu-id="f0d06-125">$top</span></span>

<span data-ttu-id="f0d06-126">有关一般信息, 请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f0d06-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0d06-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0d06-127">Request headers</span></span>

| <span data-ttu-id="f0d06-128">名称</span><span class="sxs-lookup"><span data-stu-id="f0d06-128">Name</span></span>          | <span data-ttu-id="f0d06-129">说明</span><span class="sxs-lookup"><span data-stu-id="f0d06-129">Description</span></span>               |
|:--------------|:--------------------------|
| <span data-ttu-id="f0d06-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0d06-130">Authorization</span></span> | <span data-ttu-id="f0d06-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0d06-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0d06-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0d06-133">Request body</span></span>

<span data-ttu-id="f0d06-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0d06-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0d06-135">响应</span><span class="sxs-lookup"><span data-stu-id="f0d06-135">Response</span></span>

<span data-ttu-id="f0d06-136">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[place](../resources/place.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f0d06-136">If successful, this method returns a `200 OK` response code and the requested [place](../resources/place.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f0d06-137">示例</span><span class="sxs-lookup"><span data-stu-id="f0d06-137">Examples</span></span>

### <a name="example-1-get-a-room"></a><span data-ttu-id="f0d06-138">示例 1: 获取聊天室</span><span class="sxs-lookup"><span data-stu-id="f0d06-138">Example 1: Get a room</span></span>
#### <a name="request"></a><span data-ttu-id="f0d06-139">请求</span><span class="sxs-lookup"><span data-stu-id="f0d06-139">Request</span></span>

<span data-ttu-id="f0d06-140">下面的示例指定用于获取其属性的**聊天室**的**id** 。</span><span class="sxs-lookup"><span data-stu-id="f0d06-140">The following example specifies the **id** of a **room** to get its properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_room"
}-->

```http
GET https://graph.microsoft.com/beta/places/3162F1E1-C4C0-604B-51D8-91DA78989EB1
```

#### <a name="response"></a><span data-ttu-id="f0d06-141">响应</span><span class="sxs-lookup"><span data-stu-id="f0d06-141">Response</span></span>

<span data-ttu-id="f0d06-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f0d06-142">The following is an example of the response.</span></span>

><span data-ttu-id="f0d06-143">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f0d06-143">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f0d06-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f0d06-144">All the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-a-room-list"></a><span data-ttu-id="f0d06-145">示例 2: 获取会议室列表</span><span class="sxs-lookup"><span data-stu-id="f0d06-145">Example 2: Get a room list</span></span>
#### <a name="request"></a><span data-ttu-id="f0d06-146">请求</span><span class="sxs-lookup"><span data-stu-id="f0d06-146">Request</span></span>

<span data-ttu-id="f0d06-147">下面的示例指定**roomList**的**emailAddress**以获取其属性。</span><span class="sxs-lookup"><span data-stu-id="f0d06-147">The following example specifies the **emailAddress** of a **roomList** to get its properties.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_roomlist"
}-->

```http
GET https://graph.microsoft.com/beta/places/bldg1@contoso.com
```

#### <a name="response"></a><span data-ttu-id="f0d06-148">响应</span><span class="sxs-lookup"><span data-stu-id="f0d06-148">Response</span></span>

<span data-ttu-id="f0d06-149">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f0d06-149">The following is an example of the response.</span></span>

><span data-ttu-id="f0d06-150">**注意**: 为了提高可读性, 可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f0d06-150">**Note**: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="f0d06-151">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f0d06-151">All the properties will be returned from an actual call.</span></span>

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
