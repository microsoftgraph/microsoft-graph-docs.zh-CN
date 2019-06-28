---
title: 用户：findRooms
description: '获取用户租户中或特定房间列表中的所有会议室。 '
localization_priority: Priority
author: angelgolfer-ms
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a7e4db27796a50b17819c1858e1d18e3dd7746f1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35270334"
---
# <a name="user-findrooms"></a><span data-ttu-id="c88f5-103">用户：findRooms</span><span class="sxs-lookup"><span data-stu-id="c88f5-103">user: findRooms</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c88f5-104">获取代表用户租户或特定会议室列表中的所有会议室的 [emailAddress](../resources/emailaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c88f5-104">Get all the meeting rooms in the user's tenant or in a specific room list.</span></span> 

<span data-ttu-id="c88f5-105">租户可以将会议室整理到会议室列表。</span><span class="sxs-lookup"><span data-stu-id="c88f5-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="c88f5-106">在此 API 中，每个会议室和会议室列表由 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="c88f5-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span> <span data-ttu-id="c88f5-107">可以获取租户租户中的[所有会议室列表](user-findroomlists.md)、获取租户中的所有会议室，或者获取特定会议室列表的所有会议室。</span><span class="sxs-lookup"><span data-stu-id="c88f5-107">You can [get all the room lists](user-findroomlists.md) in the tenant, get all the rooms in the tenant, or get all the rooms in a specific room list.</span></span> <span data-ttu-id="c88f5-108">最多可以访问租户中的前 100 个会议室。</span><span class="sxs-lookup"><span data-stu-id="c88f5-108">You can get up to the first 100 rooms in the tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="c88f5-109">权限</span><span class="sxs-lookup"><span data-stu-id="c88f5-109">Permissions</span></span>
<span data-ttu-id="c88f5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c88f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c88f5-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="c88f5-112">Permission type</span></span>      | <span data-ttu-id="c88f5-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c88f5-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c88f5-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c88f5-114">Delegated (work or school account)</span></span> | <span data-ttu-id="c88f5-115">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88f5-115">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="c88f5-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c88f5-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c88f5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c88f5-117">Not supported.</span></span>    |
|<span data-ttu-id="c88f5-118">Application</span><span class="sxs-lookup"><span data-stu-id="c88f5-118">Application</span></span> | <span data-ttu-id="c88f5-119">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c88f5-119">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c88f5-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c88f5-120">HTTP request</span></span>

<span data-ttu-id="c88f5-121">若要获取租户中的所有会议室：</span><span class="sxs-lookup"><span data-stu-id="c88f5-121">To get all the rooms in the tenant:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms
GET /users/<id>/findRooms
```

<span data-ttu-id="c88f5-122">若要获取租户特定会议室列表中的所有会议室：</span><span class="sxs-lookup"><span data-stu-id="c88f5-122">To get all the rooms in a specific room list of the tenant's:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/findRooms(RoomList='{room_list_emailAddress}')
GET /users/<id>/findRooms(RoomList='{room_list_emailAddress}')
```

## <a name="query-parameters"></a><span data-ttu-id="c88f5-123">查询参数</span><span class="sxs-lookup"><span data-stu-id="c88f5-123">Query parameters</span></span>

| <span data-ttu-id="c88f5-124">查询参数</span><span class="sxs-lookup"><span data-stu-id="c88f5-124">Query parameter</span></span>       | <span data-ttu-id="c88f5-125">类型</span><span class="sxs-lookup"><span data-stu-id="c88f5-125">Type</span></span> | <span data-ttu-id="c88f5-126">说明</span><span class="sxs-lookup"><span data-stu-id="c88f5-126">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="c88f5-127">RoomList</span><span class="sxs-lookup"><span data-stu-id="c88f5-127">RoomList</span></span> | <span data-ttu-id="c88f5-128">string</span><span class="sxs-lookup"><span data-stu-id="c88f5-128">string</span></span> | <span data-ttu-id="c88f5-129">与会议室列表关联的 SMTP 地址。</span><span class="sxs-lookup"><span data-stu-id="c88f5-129">The SMTP address associated with the room list.</span></span> <span data-ttu-id="c88f5-130">每个会议室列表用包含 SMTP 地址的 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="c88f5-130">Each room list is represented by an [emailAddress](../resources/emailaddress.md) instance that includes an SMTP address.</span></span> |

## <a name="request-headers"></a><span data-ttu-id="c88f5-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="c88f5-131">Request headers</span></span>
| <span data-ttu-id="c88f5-132">名称</span><span class="sxs-lookup"><span data-stu-id="c88f5-132">Name</span></span>       | <span data-ttu-id="c88f5-133">类型</span><span class="sxs-lookup"><span data-stu-id="c88f5-133">Type</span></span> | <span data-ttu-id="c88f5-134">说明</span><span class="sxs-lookup"><span data-stu-id="c88f5-134">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="c88f5-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="c88f5-135">Authorization</span></span>  | <span data-ttu-id="c88f5-136">string</span><span class="sxs-lookup"><span data-stu-id="c88f5-136">string</span></span>  | <span data-ttu-id="c88f5-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c88f5-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c88f5-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c88f5-139">Content-Type</span></span>  | <span data-ttu-id="c88f5-140">string</span><span class="sxs-lookup"><span data-stu-id="c88f5-140">string</span></span>  | <span data-ttu-id="c88f5-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c88f5-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="c88f5-143">请求正文</span><span class="sxs-lookup"><span data-stu-id="c88f5-143">Request body</span></span>
<span data-ttu-id="c88f5-144">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c88f5-144">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c88f5-145">响应</span><span class="sxs-lookup"><span data-stu-id="c88f5-145">Response</span></span>

<span data-ttu-id="c88f5-146">如果成功，此方法将在响应主体中返回 `200 OK` 响应代码和 [emailAddress](../resources/emailaddress.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c88f5-146">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/emailaddress.md) objects in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="c88f5-147">示例</span><span class="sxs-lookup"><span data-stu-id="c88f5-147">Example</span></span>

##### <a name="request-1"></a><span data-ttu-id="c88f5-148">请求 1</span><span class="sxs-lookup"><span data-stu-id="c88f5-148">Request 1</span></span>

<span data-ttu-id="c88f5-149">第一个示例将获取代表登录用户租户中定义的所有会议室的 [emailAddress](../resources/emailaddress.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c88f5-149">The first example gets all the rooms defined in the signed-in user's tenant.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_in_tenant"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms
```

##### <a name="response-1"></a><span data-ttu-id="c88f5-150">响应 1</span><span class="sxs-lookup"><span data-stu-id="c88f5-150">Response 1</span></span>
<span data-ttu-id="c88f5-151">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c88f5-151">Here is an example of the response.</span></span> 

<span data-ttu-id="c88f5-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c88f5-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c88f5-154">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c88f5-154">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c88f5-155">C#</span><span class="sxs-lookup"><span data-stu-id="c88f5-155">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c88f5-156">Javascript</span><span class="sxs-lookup"><span data-stu-id="c88f5-156">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c88f5-157">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c88f5-157">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_get_rooms_in_tenant-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

##### <a name="request-2"></a><span data-ttu-id="c88f5-158">请求 2</span><span class="sxs-lookup"><span data-stu-id="c88f5-158">Request 2</span></span>

<span data-ttu-id="c88f5-159">第二个示例将获取 [emailAddress](../resources/emailaddress.md) 对象，该对象代表由电子邮件地址 Building2Rooms@contoso.onmicrosoft.com 标识的特定会议室列表中的会议室。</span><span class="sxs-lookup"><span data-stu-id="c88f5-159">The second example gets the rooms in the specified room list identified by the email address Building2Rooms@contoso.onmicrosoft.com.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_rooms_from_specific_list"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRooms(RoomList='Building2Rooms@contoso.onmicrosoft.com') 
```

##### <a name="response-2"></a><span data-ttu-id="c88f5-160">响应 2</span><span class="sxs-lookup"><span data-stu-id="c88f5-160">Response 2</span></span>
<span data-ttu-id="c88f5-161">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c88f5-161">Here is an example of the response.</span></span> 

<span data-ttu-id="c88f5-p107">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c88f5-p107">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c88f5-164">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c88f5-164">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c88f5-165">C#</span><span class="sxs-lookup"><span data-stu-id="c88f5-165">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c88f5-166">Javascript</span><span class="sxs-lookup"><span data-stu-id="c88f5-166">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="c88f5-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c88f5-167">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/user_get_rooms_from_specific_list-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]


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
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-findrooms.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
