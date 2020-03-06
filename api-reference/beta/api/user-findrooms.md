---
title: 用户：findRooms
description: '获取用户租户中或特定房间列表中的所有会议室。 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c3621b59e619d9152519926525edacdc1086ccbf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42451966"
---
# <a name="user-findrooms"></a><span data-ttu-id="33653-103">用户：findRooms</span><span class="sxs-lookup"><span data-stu-id="33653-103">user: findRooms</span></span>

<span data-ttu-id="33653-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33653-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="33653-105">获取代表用户租户或特定会议室列表中的所有会议室的 [emailAddress](../resources/emailaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33653-105">Get the [emailAddress](../resources/emailaddress.md) objects that represent all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="33653-106">租户可以将会议室整理到会议室列表。</span><span class="sxs-lookup"><span data-stu-id="33653-106">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="33653-107">在此 API 中，每个会议室和会议室列表由 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="33653-107">In this API, each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="33653-108">可以获取租户租户中的[所有会议室列表](user-findroomlists.md)、获取租户中的所有会议室，或者获取特定会议室列表的所有会议室。</span><span class="sxs-lookup"><span data-stu-id="33653-108">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="33653-109">最多可以访问租户中的前 100 个会议室。</span><span class="sxs-lookup"><span data-stu-id="33653-109">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="33653-110">权限</span><span class="sxs-lookup"><span data-stu-id="33653-110">Permissions</span></span>
<span data-ttu-id="33653-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33653-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="33653-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="33653-113">Permission type</span></span>      | <span data-ttu-id="33653-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33653-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33653-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33653-115">Delegated (work or school account)</span></span> | <span data-ttu-id="33653-116">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="33653-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="33653-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33653-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33653-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="33653-118">Not supported.</span></span>    |
|<span data-ttu-id="33653-119">Application</span><span class="sxs-lookup"><span data-stu-id="33653-119">Application</span></span> | <span data-ttu-id="33653-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="33653-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33653-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33653-121">HTTP request</span></span>

<span data-ttu-id="33653-122">若要获取租户中的所有会议室：</span><span class="sxs-lookup"><span data-stu-id="33653-122">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/{id}/findRooms
```

<span data-ttu-id="33653-123">若要获取租户特定会议室列表中的所有会议室：</span><span class="sxs-lookup"><span data-stu-id="33653-123">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/{id}/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="33653-124">查询参数</span><span class="sxs-lookup"><span data-stu-id="33653-124">Query parameters</span></span>

| <span data-ttu-id="33653-125">查询参数</span><span class="sxs-lookup"><span data-stu-id="33653-125">Query parameter</span></span>       | <span data-ttu-id="33653-126">类型</span><span class="sxs-lookup"><span data-stu-id="33653-126">Type</span></span> | <span data-ttu-id="33653-127">说明</span><span class="sxs-lookup"><span data-stu-id="33653-127">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="33653-128">RoomList</span><span class="sxs-lookup"><span data-stu-id="33653-128">RoomList</span></span> | <span data-ttu-id="33653-129">string</span><span class="sxs-lookup"><span data-stu-id="33653-129">string</span></span> | <span data-ttu-id="33653-130">与会议室列表关联的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="33653-130">The SMTP address associated with the room list.</span></span> <span data-ttu-id="33653-131">每个会议室列表用包含 SMTP 地址的 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="33653-131">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="33653-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="33653-132">Request headers</span></span>
| <span data-ttu-id="33653-133">名称</span><span class="sxs-lookup"><span data-stu-id="33653-133">Name</span></span>       | <span data-ttu-id="33653-134">类型</span><span class="sxs-lookup"><span data-stu-id="33653-134">Type</span></span> | <span data-ttu-id="33653-135">说明</span><span class="sxs-lookup"><span data-stu-id="33653-135">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="33653-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="33653-136">Authorization</span></span>  | <span data-ttu-id="33653-137">string</span><span class="sxs-lookup"><span data-stu-id="33653-137">string</span></span>  | <span data-ttu-id="33653-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33653-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="33653-140">Content-Type</span><span class="sxs-lookup"><span data-stu-id="33653-140">Content-Type</span></span>  | <span data-ttu-id="33653-141">string</span><span class="sxs-lookup"><span data-stu-id="33653-141">string</span></span>  | <span data-ttu-id="33653-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="33653-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="33653-144">请求正文</span><span class="sxs-lookup"><span data-stu-id="33653-144">Request body</span></span>
<span data-ttu-id="33653-145">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33653-145">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33653-146">响应</span><span class="sxs-lookup"><span data-stu-id="33653-146">Response</span></span>

<span data-ttu-id="33653-147">如果成功，此方法将在响应主体中返回 `200 OK` 响应代码和 [emailAddress](../resources/emailaddress.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="33653-147">If successful, this method returns a `200 OK` response code and a collection of [emailAddress](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="33653-148">示例</span><span class="sxs-lookup"><span data-stu-id="33653-148">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="33653-149">请求 1</span><span class="sxs-lookup"><span data-stu-id="33653-149">Request 1</span></span>

<span data-ttu-id="33653-150">第一个示例将获取代表登录用户租户中定义的所有会议室的 [emailAddress](../resources/emailaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33653-150">The first example gets the [emailAddress](../resources/emailaddress.md) objects that represent all the rooms defined in the signed-in user's tenant.</span></span>


# <a name="http"></a>[<span data-ttu-id="33653-151">HTTP</span><span class="sxs-lookup"><span data-stu-id="33653-151">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms
```
# <a name="c"></a>[<span data-ttu-id="33653-152">C#</span><span class="sxs-lookup"><span data-stu-id="33653-152">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-in-tenant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33653-153">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33653-153">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-in-tenant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33653-154">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33653-154">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-in-tenant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-1"></a><span data-ttu-id="33653-155">响应 1</span><span class="sxs-lookup"><span data-stu-id="33653-155">Response 1</span></span>
<span data-ttu-id="33653-156">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="33653-156">Here is an example of the response.</span></span> 

<span data-ttu-id="33653-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33653-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

##### <a name="request-2"></a><span data-ttu-id="33653-159">请求 2</span><span class="sxs-lookup"><span data-stu-id="33653-159">Request 2</span></span>

<span data-ttu-id="33653-160">第二个示例将获取 [emailAddress](../resources/emailaddress.md) 对象，该对象代表由电子邮件地址 Building2Rooms@contoso.onmicrosoft.com 标识的特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="33653-160">The second example gets the [emailAddress](../resources/emailaddress.md) objects that represent the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>


# <a name="http"></a>[<span data-ttu-id="33653-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="33653-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```
# <a name="c"></a>[<span data-ttu-id="33653-162">C#</span><span class="sxs-lookup"><span data-stu-id="33653-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-rooms-from-specific-list-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33653-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33653-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-rooms-from-specific-list-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33653-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33653-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-rooms-from-specific-list-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response-2"></a><span data-ttu-id="33653-165">响应 2</span><span class="sxs-lookup"><span data-stu-id="33653-165">Response 2</span></span>
<span data-ttu-id="33653-166">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="33653-166">Here is an example of the response.</span></span> 

<span data-ttu-id="33653-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33653-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
