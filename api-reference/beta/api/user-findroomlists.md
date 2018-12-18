---
title: 用户： findRoomLists
description: 获取在租户中定义的会议室列表。
author: dkershaw10
ms.openlocfilehash: f96f8e5c6349e87d2d71820b7b7cd3b0367908f9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310771"
---
# <a name="user-findroomlists"></a><span data-ttu-id="bf80a-103">用户： findRoomLists</span><span class="sxs-lookup"><span data-stu-id="bf80a-103">user: findRoomLists</span></span>

> <span data-ttu-id="bf80a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf80a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf80a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf80a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf80a-106">获取在租户中定义的会议室列表。</span><span class="sxs-lookup"><span data-stu-id="bf80a-106">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="bf80a-107">租户可以将会议房间组织为会议室列表。</span><span class="sxs-lookup"><span data-stu-id="bf80a-107">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="bf80a-108">[EmailAddress](../resources/emailaddress.md)实例表示每个会议室和会议室列表。</span><span class="sxs-lookup"><span data-stu-id="bf80a-108">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="bf80a-109">您可以获取租户、 租户，[获取所有聊天室](user-findrooms.md)或都特定聊天室列表中的[都获取的所有聊天室](user-findrooms.md)中的所有会议室列表。</span><span class="sxs-lookup"><span data-stu-id="bf80a-109">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="bf80a-110">权限</span><span class="sxs-lookup"><span data-stu-id="bf80a-110">Permissions</span></span>
<span data-ttu-id="bf80a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf80a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bf80a-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf80a-113">Permission type</span></span>      | <span data-ttu-id="bf80a-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf80a-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf80a-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf80a-115">Delegated (work or school account)</span></span> | <span data-ttu-id="bf80a-116">User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf80a-116">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="bf80a-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf80a-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf80a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf80a-118">Not supported.</span></span>    |
|<span data-ttu-id="bf80a-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf80a-119">Application</span></span> | <span data-ttu-id="bf80a-120">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="bf80a-120">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf80a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf80a-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="bf80a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf80a-122">Request headers</span></span>
| <span data-ttu-id="bf80a-123">Name</span><span class="sxs-lookup"><span data-stu-id="bf80a-123">Name</span></span>       | <span data-ttu-id="bf80a-124">类型</span><span class="sxs-lookup"><span data-stu-id="bf80a-124">Type</span></span> | <span data-ttu-id="bf80a-125">说明</span><span class="sxs-lookup"><span data-stu-id="bf80a-125">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="bf80a-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf80a-126">Authorization</span></span>  | <span data-ttu-id="bf80a-127">string</span><span class="sxs-lookup"><span data-stu-id="bf80a-127">string</span></span>  | <span data-ttu-id="bf80a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf80a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf80a-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf80a-130">Content-Type</span></span>  | <span data-ttu-id="bf80a-131">string</span><span class="sxs-lookup"><span data-stu-id="bf80a-131">string</span></span>  | <span data-ttu-id="bf80a-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="bf80a-p105">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bf80a-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf80a-134">Request body</span></span>
<span data-ttu-id="bf80a-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bf80a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf80a-136">响应</span><span class="sxs-lookup"><span data-stu-id="bf80a-136">Response</span></span>

<span data-ttu-id="bf80a-137">如果成功，此方法返回`200 OK`响应正文中的响应代码和[emailAddress](../resources/emailaddress.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="bf80a-137">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="bf80a-138">如果租户中不定义任何列表，则返回空数组。</span><span class="sxs-lookup"><span data-stu-id="bf80a-138">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="bf80a-139">示例</span><span class="sxs-lookup"><span data-stu-id="bf80a-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf80a-140">请求</span><span class="sxs-lookup"><span data-stu-id="bf80a-140">Request</span></span>

<span data-ttu-id="bf80a-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf80a-141">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="bf80a-142">响应</span><span class="sxs-lookup"><span data-stu-id="bf80a-142">Response</span></span>
<span data-ttu-id="bf80a-143">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="bf80a-143">Here is an example of the response.</span></span> 

<span data-ttu-id="bf80a-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf80a-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "user: findRoomLists",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->