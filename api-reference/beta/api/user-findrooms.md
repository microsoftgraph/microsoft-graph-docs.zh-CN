---
title: 用户：findRooms
description: '获取用户租户中或特定房间列表中的所有会议室。 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7f5a696ff3cb7876a672b665999165a5b4e80b9f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35450959"
---
# <a name="user-findrooms"></a><span data-ttu-id="5bd30-103">用户：findRooms</span><span class="sxs-lookup"><span data-stu-id="5bd30-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5bd30-104">获取代表用户租户或特定会议室列表中的所有会议室的 [emailAddress](../resources/emailaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5bd30-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="5bd30-105">租户可以将会议室整理到会议室列表。</span><span class="sxs-lookup"><span data-stu-id="5bd30-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="5bd30-106">在此 API 中，每个会议室和会议室列表由 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="5bd30-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="5bd30-107">可以获取租户租户中的[所有会议室列表](user-findroomlists.md)、获取租户中的所有会议室，或者获取特定会议室列表的所有会议室。</span><span class="sxs-lookup"><span data-stu-id="5bd30-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="5bd30-108">最多可以访问租户中的前 100 个会议室。</span><span class="sxs-lookup"><span data-stu-id="5bd30-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5bd30-109">权限</span><span class="sxs-lookup"><span data-stu-id="5bd30-109">Permissions</span></span>
<span data-ttu-id="5bd30-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5bd30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5bd30-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5bd30-112">Permission type</span></span>      | <span data-ttu-id="5bd30-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5bd30-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5bd30-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd30-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5bd30-115">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bd30-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="5bd30-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5bd30-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5bd30-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5bd30-117">Not supported.</span></span>    |
|<span data-ttu-id="5bd30-118">Application</span><span class="sxs-lookup"><span data-stu-id="5bd30-118">Application</span></span> | <span data-ttu-id="5bd30-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bd30-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5bd30-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5bd30-120">HTTP request</span></span>

<span data-ttu-id="5bd30-121">若要获取租户中的所有会议室：</span><span class="sxs-lookup"><span data-stu-id="5bd30-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="5bd30-122">若要获取租户特定会议室列表中的所有会议室：</span><span class="sxs-lookup"><span data-stu-id="5bd30-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/<id>/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="5bd30-123">查询参数</span><span class="sxs-lookup"><span data-stu-id="5bd30-123">Query parameters</span></span>

| <span data-ttu-id="5bd30-124">查询参数</span><span class="sxs-lookup"><span data-stu-id="5bd30-124">Query parameter</span></span>       | <span data-ttu-id="5bd30-125">类型</span><span class="sxs-lookup"><span data-stu-id="5bd30-125">Type</span></span> | <span data-ttu-id="5bd30-126">说明</span><span class="sxs-lookup"><span data-stu-id="5bd30-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="5bd30-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="5bd30-127">RoomList</span></span> | <span data-ttu-id="5bd30-128">string</span><span class="sxs-lookup"><span data-stu-id="5bd30-128">string</span></span> | <span data-ttu-id="5bd30-129">与会议室列表关联的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="5bd30-129">The SMTP address associated with the room list.</span></span> <span data-ttu-id="5bd30-130">每个会议室列表用包含 SMTP 地址的 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="5bd30-130">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="5bd30-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="5bd30-131">Request headers</span></span>
| <span data-ttu-id="5bd30-132">名称</span><span class="sxs-lookup"><span data-stu-id="5bd30-132">Name</span></span>       | <span data-ttu-id="5bd30-133">类型</span><span class="sxs-lookup"><span data-stu-id="5bd30-133">Type</span></span> | <span data-ttu-id="5bd30-134">说明</span><span class="sxs-lookup"><span data-stu-id="5bd30-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="5bd30-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bd30-135">Authorization</span></span>  | <span data-ttu-id="5bd30-136">string</span><span class="sxs-lookup"><span data-stu-id="5bd30-136">string</span></span>  | <span data-ttu-id="5bd30-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5bd30-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5bd30-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5bd30-139">Content-Type</span></span>  | <span data-ttu-id="5bd30-140">string</span><span class="sxs-lookup"><span data-stu-id="5bd30-140">string</span></span>  | <span data-ttu-id="5bd30-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5bd30-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="5bd30-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="5bd30-143">Request body</span></span>
<span data-ttu-id="5bd30-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5bd30-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bd30-145">响应</span><span class="sxs-lookup"><span data-stu-id="5bd30-145">Response</span></span>

<span data-ttu-id="5bd30-146">如果成功，此方法将在响应主体中返回 `200 OK` 响应代码和 [emailAddress](../resources/emailaddress.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5bd30-146">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="5bd30-147">示例</span><span class="sxs-lookup"><span data-stu-id="5bd30-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="5bd30-148">请求 1</span><span class="sxs-lookup"><span data-stu-id="5bd30-148">Request 1</span></span>

<span data-ttu-id="5bd30-149">第一个示例将获取代表登录用户租户中定义的所有会议室的 [emailAddress](../resources/emailaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5bd30-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5bd30-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bd30-150">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5bd30-151">C#</span><span class="sxs-lookup"><span data-stu-id="5bd30-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-in-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bd30-152">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bd30-152">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-in-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5bd30-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bd30-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-in-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="5bd30-154">响应 1</span><span class="sxs-lookup"><span data-stu-id="5bd30-154">Response 1</span></span>
<span data-ttu-id="5bd30-155">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5bd30-155">Here is an example of the response.</span></span> 

<span data-ttu-id="5bd30-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bd30-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_in_tenant",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Conf Room Adams",
            "address": "Adams@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Crystal",
            "address": "Crystal@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Stevens",
            "address": "Stevens@contoso.onmicrosoft.com"
        }
    ]
}
```

##### <a name="request-2"></a><span data-ttu-id="5bd30-158">请求 2</span><span class="sxs-lookup"><span data-stu-id="5bd30-158">Request 2</span></span>

<span data-ttu-id="5bd30-159">第二个示例将获取 [emailAddress](../resources/emailaddress.md) 对象，该对象代表由电子邮件地址 Building2Rooms@contoso.onmicrosoft.com 标识的特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="5bd30-159">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="5bd30-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="5bd30-160">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="5bd30-161">C#</span><span class="sxs-lookup"><span data-stu-id="5bd30-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-from-specific-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5bd30-162">Javascript</span><span class="sxs-lookup"><span data-stu-id="5bd30-162">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-from-specific-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5bd30-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5bd30-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-from-specific-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="5bd30-164">响应 2</span><span class="sxs-lookup"><span data-stu-id="5bd30-164">Response 2</span></span>
<span data-ttu-id="5bd30-165">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="5bd30-165">Here is an example of the response.</span></span> 

<span data-ttu-id="5bd30-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5bd30-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_rooms_from_specific_list",
  "truncated": true,
  "@odata.type": "microsoft.graph.emailAddress",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.emailAddress)",
    "value": [
        {
            "name": "Conf Room Baker",
            "address": "Baker@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Hood",
            "address": "Hood@contoso.onmicrosoft.com"
        },
        {
            "name": "Conf Room Rainier",
            "address": "Rainier@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRooms",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
