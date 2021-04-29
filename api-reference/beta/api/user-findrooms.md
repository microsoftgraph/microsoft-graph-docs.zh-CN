---
title: 用户：findRooms
description: '获取用户租户中或特定房间列表中的所有会议室。 '
localization_priority: Priority
author: vrod9429
ms.prod: outlook
doc_type: apiPageType
ms.openlocfilehash: 9007795bfb04f8484be61d13a5da17602df80337
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52052640"
---
# <a name="user-findrooms"></a><span data-ttu-id="88e2c-103">用户：findRooms</span><span class="sxs-lookup"><span data-stu-id="88e2c-103">user: findRooms</span></span>

<span data-ttu-id="88e2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88e2c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88e2c-105">获取代表用户租户或特定会议室列表中的所有会议室的 [emailAddress](../resources/emailaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88e2c-105">Get the [emailAddress](../resources/emailaddress.md) objects that represent all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="88e2c-106">租户可以将会议室整理到会议室列表。</span><span class="sxs-lookup"><span data-stu-id="88e2c-106">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="88e2c-107">在此 API 中，每个会议室和会议室列表由 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="88e2c-107">In this API, each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="88e2c-108">可以获取租户租户中的[所有会议室列表](user-findroomlists.md)、获取租户中的所有会议室，或者获取特定会议室列表的所有会议室。</span><span class="sxs-lookup"><span data-stu-id="88e2c-108">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="88e2c-109">最多可以访问租户中的前 100 个会议室。</span><span class="sxs-lookup"><span data-stu-id="88e2c-109">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="88e2c-110">权限</span><span class="sxs-lookup"><span data-stu-id="88e2c-110">Permissions</span></span>
<span data-ttu-id="88e2c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88e2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="88e2c-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="88e2c-113">Permission type</span></span>      | <span data-ttu-id="88e2c-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88e2c-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88e2c-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88e2c-115">Delegated (work or school account)</span></span> | <span data-ttu-id="88e2c-116">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="88e2c-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="88e2c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88e2c-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88e2c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="88e2c-118">Not supported.</span></span>    |
|<span data-ttu-id="88e2c-119">Application</span><span class="sxs-lookup"><span data-stu-id="88e2c-119">Application</span></span> | <span data-ttu-id="88e2c-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="88e2c-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88e2c-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88e2c-121">HTTP request</span></span>

<span data-ttu-id="88e2c-122">若要获取租户中的所有会议室：</span><span class="sxs-lookup"><span data-stu-id="88e2c-122">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/{id}/findRooms
```

<span data-ttu-id="88e2c-123">若要获取租户特定会议室列表中的所有会议室：</span><span class="sxs-lookup"><span data-stu-id="88e2c-123">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/{id}/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="88e2c-124">查询参数</span><span class="sxs-lookup"><span data-stu-id="88e2c-124">Query parameters</span></span>

| <span data-ttu-id="88e2c-125">查询参数</span><span class="sxs-lookup"><span data-stu-id="88e2c-125">Query parameter</span></span>       | <span data-ttu-id="88e2c-126">类型</span><span class="sxs-lookup"><span data-stu-id="88e2c-126">Type</span></span> | <span data-ttu-id="88e2c-127">说明</span><span class="sxs-lookup"><span data-stu-id="88e2c-127">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="88e2c-128">RoomList</span><span class="sxs-lookup"><span data-stu-id="88e2c-128">RoomList</span></span> | <span data-ttu-id="88e2c-129">string</span><span class="sxs-lookup"><span data-stu-id="88e2c-129">string</span></span> | <span data-ttu-id="88e2c-130">与会议室列表关联的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="88e2c-130">The SMTP address associated with the room list.</span></span> <span data-ttu-id="88e2c-131">每个会议室列表用包含 SMTP 地址的 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="88e2c-131">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="88e2c-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="88e2c-132">Request headers</span></span>
| <span data-ttu-id="88e2c-133">名称</span><span class="sxs-lookup"><span data-stu-id="88e2c-133">Name</span></span>       | <span data-ttu-id="88e2c-134">类型</span><span class="sxs-lookup"><span data-stu-id="88e2c-134">Type</span></span> | <span data-ttu-id="88e2c-135">说明</span><span class="sxs-lookup"><span data-stu-id="88e2c-135">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="88e2c-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="88e2c-136">Authorization</span></span>  | <span data-ttu-id="88e2c-137">string</span><span class="sxs-lookup"><span data-stu-id="88e2c-137">string</span></span>  | <span data-ttu-id="88e2c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88e2c-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="88e2c-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88e2c-140">Content-Type</span></span>  | <span data-ttu-id="88e2c-141">string</span><span class="sxs-lookup"><span data-stu-id="88e2c-141">string</span></span>  | <span data-ttu-id="88e2c-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="88e2c-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="88e2c-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="88e2c-144">Request body</span></span>
<span data-ttu-id="88e2c-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88e2c-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88e2c-146">响应</span><span class="sxs-lookup"><span data-stu-id="88e2c-146">Response</span></span>

<span data-ttu-id="88e2c-147">如果成功，此方法将在响应主体中返回 `200 OK` 响应代码和 [emailAddress](../resources/emailaddress.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="88e2c-147">If successful, this method returns a `200 OK` response code and a collection of [emailAddress](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="88e2c-148">示例</span><span class="sxs-lookup"><span data-stu-id="88e2c-148">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="88e2c-149">请求 1</span><span class="sxs-lookup"><span data-stu-id="88e2c-149">Request 1</span></span>

<span data-ttu-id="88e2c-150">第一个示例将获取代表登录用户租户中定义的所有会议室的 [emailAddress](../resources/emailaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88e2c-150">The first example gets the [emailAddress](../resources/emailaddress.md) objects that represent all the rooms defined in the signed-in user's tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="88e2c-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="88e2c-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms
```
# <a name="c"></a>[<span data-ttu-id="88e2c-152">C#</span><span class="sxs-lookup"><span data-stu-id="88e2c-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-in-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88e2c-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88e2c-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-in-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88e2c-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88e2c-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-in-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88e2c-155">Java</span><span class="sxs-lookup"><span data-stu-id="88e2c-155">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-rooms-in-tenant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="88e2c-156">响应 1</span><span class="sxs-lookup"><span data-stu-id="88e2c-156">Response 1</span></span>
<span data-ttu-id="88e2c-157">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="88e2c-157">Here is an example of the response.</span></span> 

<span data-ttu-id="88e2c-158">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="88e2c-158">Note: The response object shown here might be shortened for readability.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="88e2c-159">请求 2</span><span class="sxs-lookup"><span data-stu-id="88e2c-159">Request 2</span></span>

<span data-ttu-id="88e2c-160">第二个示例将获取 [emailAddress](../resources/emailaddress.md) 对象，该对象代表由电子邮件地址 Building2Rooms@contoso.onmicrosoft.com 标识的特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="88e2c-160">The second example gets the [emailAddress](../resources/emailaddress.md) objects that represent the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>


# <a name="http"></a>[<span data-ttu-id="88e2c-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="88e2c-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```
# <a name="c"></a>[<span data-ttu-id="88e2c-162">C#</span><span class="sxs-lookup"><span data-stu-id="88e2c-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-from-specific-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88e2c-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88e2c-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-from-specific-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88e2c-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88e2c-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-from-specific-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="88e2c-165">Java</span><span class="sxs-lookup"><span data-stu-id="88e2c-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-rooms-from-specific-list-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="88e2c-166">响应 2</span><span class="sxs-lookup"><span data-stu-id="88e2c-166">Response 2</span></span>
<span data-ttu-id="88e2c-167">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="88e2c-167">Here is an example of the response.</span></span> 

<span data-ttu-id="88e2c-168">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="88e2c-168">Note: The response object shown here might be shortened for readability.</span></span>
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


