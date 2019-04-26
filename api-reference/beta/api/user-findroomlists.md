---
title: 用户：findRoomLists
description: 获取租户中定义的会议室列表。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1cc26367c9cecd16604f7cfefb3be5ce265e3c2c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32547912"
---
# <a name="user-findroomlists"></a><span data-ttu-id="a258b-103">用户：findRoomLists</span><span class="sxs-lookup"><span data-stu-id="a258b-103">user: findRoomLists</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a258b-104">获取租户中定义的会议室列表。</span><span class="sxs-lookup"><span data-stu-id="a258b-104">Get the room lists defined in a tenant.</span></span>

<span data-ttu-id="a258b-105">租户可以将会议室整理到会议室列表。</span><span class="sxs-lookup"><span data-stu-id="a258b-105">Tenants can organize meeting rooms into room lists.</span></span> <span data-ttu-id="a258b-106">每个会议室和会议室列表用 [emailAddress](../resources/emailaddress.md) 实例表示。</span><span class="sxs-lookup"><span data-stu-id="a258b-106">Each meeting room and room list is represented by an [emailAddress](../resources/emailaddress.md) instance.</span></span>
<span data-ttu-id="a258b-107">可以获取租户中的所欲会议室列表、获取租户中的[所有会议室](user-findrooms.md)或获取特定会议室列表的[所有会议室](user-findrooms.md)。</span><span class="sxs-lookup"><span data-stu-id="a258b-107">You can get all the room lists in the tenant, [get all the rooms](user-findrooms.md) in the tenant, or [get all the rooms](user-findrooms.md) in a specific room list.</span></span>


## <a name="permissions"></a><span data-ttu-id="a258b-108">权限</span><span class="sxs-lookup"><span data-stu-id="a258b-108">Permissions</span></span>
<span data-ttu-id="a258b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a258b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a258b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a258b-111">Permission type</span></span>      | <span data-ttu-id="a258b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a258b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a258b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a258b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a258b-114">User.ReadBasic.All、User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a258b-114">User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="a258b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a258b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a258b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a258b-116">Not supported.</span></span>    |
|<span data-ttu-id="a258b-117">Application</span><span class="sxs-lookup"><span data-stu-id="a258b-117">Application</span></span> | <span data-ttu-id="a258b-118">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="a258b-118">User.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a258b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a258b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/findRoomLists
GET /users/<id>/findRoomLists

```

## <a name="request-headers"></a><span data-ttu-id="a258b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a258b-120">Request headers</span></span>
| <span data-ttu-id="a258b-121">名称</span><span class="sxs-lookup"><span data-stu-id="a258b-121">Name</span></span>       | <span data-ttu-id="a258b-122">类型</span><span class="sxs-lookup"><span data-stu-id="a258b-122">Type</span></span> | <span data-ttu-id="a258b-123">说明</span><span class="sxs-lookup"><span data-stu-id="a258b-123">Description</span></span> |
|:---------------|:----------|:----------|
| <span data-ttu-id="a258b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a258b-124">Authorization</span></span>  | <span data-ttu-id="a258b-125">string</span><span class="sxs-lookup"><span data-stu-id="a258b-125">string</span></span>  | <span data-ttu-id="a258b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a258b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a258b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a258b-128">Content-Type</span></span>  | <span data-ttu-id="a258b-129">string</span><span class="sxs-lookup"><span data-stu-id="a258b-129">string</span></span>  | <span data-ttu-id="a258b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a258b-p104">application/json. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="a258b-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="a258b-132">Request body</span></span>
<span data-ttu-id="a258b-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a258b-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a258b-134">响应</span><span class="sxs-lookup"><span data-stu-id="a258b-134">Response</span></span>

<span data-ttu-id="a258b-135">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [emailAddress](../resources/emailaddress.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="a258b-135">If successful, this method returns a `200 OK` response code and [emailAddress](../resources/emailaddress.md) collection object in the response body.</span></span>

<span data-ttu-id="a258b-136">如果租户中未定义任何列表，则会返回空数组。</span><span class="sxs-lookup"><span data-stu-id="a258b-136">If no lists are defined in the tenant, then an empty array is returned.</span></span>

## <a name="example"></a><span data-ttu-id="a258b-137">示例</span><span class="sxs-lookup"><span data-stu-id="a258b-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a258b-138">请求</span><span class="sxs-lookup"><span data-stu-id="a258b-138">Request</span></span>

<span data-ttu-id="a258b-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a258b-139">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_get_room_lists"
}-->
```http
GET https://graph.microsoft.com/beta/me/findRoomLists
```

##### <a name="response"></a><span data-ttu-id="a258b-140">响应</span><span class="sxs-lookup"><span data-stu-id="a258b-140">Response</span></span>
<span data-ttu-id="a258b-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a258b-141">Here is an example of the response.</span></span> 

<span data-ttu-id="a258b-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a258b-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/user-findroomlists.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
