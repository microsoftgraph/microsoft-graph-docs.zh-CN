---
title: 用户：findRoomLists
description: 获取租户中定义的会议室列表。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1946b7080bf37d0852964f3fac677e04052f55d3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35867749"
---
# <a name="user-findroomlists"></a><span data-ttu-id="05967-103">用户：findRoomLists</span><span class="sxs-lookup"><span data-stu-id="05967-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="05967-104">获取租户中定义的会议室列表，如其 [emailAddress](../resources/emailaddress.md) 对象所表示。</span><span class="sxs-lookup"><span data-stu-id="05967-104">Get the room lists defined in a tenant, as represented by their [emailAddress](../resources/emailaddress.md) objects.</span></span>

<span data-ttu-id="05967-105">租户可以将会议室整理到会议室列表。</span><span class="sxs-lookup"><span data-stu-id="05967-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="05967-106">在此 API 中，每个会议室和会议室列表由 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="05967-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="05967-107">可以获取租户中的所欲会议室列表、获取租户中的[所有会议室](user-findrooms.md)或获取特定会议室列表的[所有会议室](user-findrooms.md)。</span><span class="sxs-lookup"><span data-stu-id="05967-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="05967-108">权限</span><span class="sxs-lookup"><span data-stu-id="05967-108">Permissions</span></span>
<span data-ttu-id="05967-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="05967-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="05967-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="05967-111">Permission type</span></span>      | <span data-ttu-id="05967-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="05967-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="05967-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05967-113">Delegated (work or school account)</span></span> | <span data-ttu-id="05967-114">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="05967-114">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="05967-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05967-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="05967-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05967-116">Not supported.</span></span>    |
|<span data-ttu-id="05967-117">Application</span><span class="sxs-lookup"><span data-stu-id="05967-117">Application</span></span> | <span data-ttu-id="05967-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="05967-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="05967-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05967-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="05967-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05967-120">Request headers</span></span>
| <span data-ttu-id="05967-121">名称</span><span class="sxs-lookup"><span data-stu-id="05967-121">Name</span></span>       | <span data-ttu-id="05967-122">类型</span><span class="sxs-lookup"><span data-stu-id="05967-122">Type</span></span> | <span data-ttu-id="05967-123">说明</span><span class="sxs-lookup"><span data-stu-id="05967-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="05967-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="05967-124">Authorization</span></span>  | <span data-ttu-id="05967-125">string</span><span class="sxs-lookup"><span data-stu-id="05967-125">string</span></span>  | <span data-ttu-id="05967-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="05967-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="05967-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="05967-128">Content-Type</span></span>  | <span data-ttu-id="05967-129">string</span><span class="sxs-lookup"><span data-stu-id="05967-129">string</span></span>  | <span data-ttu-id="05967-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="05967-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="05967-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="05967-132">Request body</span></span>
<span data-ttu-id="05967-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05967-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05967-134">响应</span><span class="sxs-lookup"><span data-stu-id="05967-134">Response</span></span>

<span data-ttu-id="05967-135">如果成功，此方法将在响应主体中返回 `200 OK` 响应代码和 [emailAddress](../resources/emailaddress.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="05967-135">If successful, this method returns a `200 OK` response code and collection of [Attachment](../resources/emailaddress.md) objects in the response body.</span></span>

<span data-ttu-id="05967-136">如果租户中未定义任何列表，则会返回空数组。</span><span class="sxs-lookup"><span data-stu-id="05967-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="05967-137">示例</span><span class="sxs-lookup"><span data-stu-id="05967-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="05967-138">请求</span><span class="sxs-lookup"><span data-stu-id="05967-138">Request</span></span>

<span data-ttu-id="05967-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05967-139">Here is an example of the request.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="05967-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="05967-140">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="05967-141">C#</span><span class="sxs-lookup"><span data-stu-id="05967-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-get-room-lists-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="05967-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="05967-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-get-room-lists-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="05967-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="05967-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-get-room-lists-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="05967-144">Java</span><span class="sxs-lookup"><span data-stu-id="05967-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-get-room-lists-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="05967-145">响应</span><span class="sxs-lookup"><span data-stu-id="05967-145">Response</span></span>
<span data-ttu-id="05967-146">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="05967-146">Here is an example of the response.</span></span> 

<span data-ttu-id="05967-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05967-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "name": "user_get_room_lists",
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
            "name": "Building 1 Rooms",
            "address": "Building1Rooms@contoso.onmicrosoft.com"
        },
        {
            "name": "Building 2 Rooms",
            "address": "Building2Rooms@contoso.onmicrosoft.com"
        }
    ]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
