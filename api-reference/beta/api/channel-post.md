---
title: 创建频道
description: 在 Microsoft 团队中创建请求正文中指定的新频道。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: 499dd2f868fef5e2a5e355a32e768bd4f87609d3
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35864397"
---
# <a name="create-channel"></a><span data-ttu-id="e02aa-103">创建频道</span><span class="sxs-lookup"><span data-stu-id="e02aa-103">Create Channel</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e02aa-104">在 Microsoft 团队中创建请求正文中指定的新[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="e02aa-104">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="e02aa-105">**请注意**：应用程序权限和此 API 存在已知问题。</span><span class="sxs-lookup"><span data-stu-id="e02aa-105">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="e02aa-106">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="e02aa-106">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="e02aa-107">权限</span><span class="sxs-lookup"><span data-stu-id="e02aa-107">Permissions</span></span>
<span data-ttu-id="e02aa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e02aa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e02aa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e02aa-110">Permission type</span></span>      | <span data-ttu-id="e02aa-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e02aa-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e02aa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e02aa-112">Delegated (work or school account)</span></span> | <span data-ttu-id="e02aa-113">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e02aa-113">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="e02aa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e02aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e02aa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e02aa-115">Not supported.</span></span>    |
|<span data-ttu-id="e02aa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e02aa-116">Application</span></span> | <span data-ttu-id="e02aa-117">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e02aa-117">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="e02aa-118">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="e02aa-118">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="e02aa-119">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="e02aa-119">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="e02aa-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e02aa-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="e02aa-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e02aa-121">Request headers</span></span>
| <span data-ttu-id="e02aa-122">标头</span><span class="sxs-lookup"><span data-stu-id="e02aa-122">Header</span></span>       | <span data-ttu-id="e02aa-123">值</span><span class="sxs-lookup"><span data-stu-id="e02aa-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e02aa-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e02aa-124">Authorization</span></span>  | <span data-ttu-id="e02aa-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e02aa-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e02aa-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e02aa-127">Content-Type</span></span>  | <span data-ttu-id="e02aa-128">application/json</span><span class="sxs-lookup"><span data-stu-id="e02aa-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e02aa-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="e02aa-129">Request body</span></span>
<span data-ttu-id="e02aa-130">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e02aa-130">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e02aa-131">响应</span><span class="sxs-lookup"><span data-stu-id="e02aa-131">Response</span></span>

<span data-ttu-id="e02aa-132">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e02aa-132">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e02aa-133">示例</span><span class="sxs-lookup"><span data-stu-id="e02aa-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e02aa-134">请求</span><span class="sxs-lookup"><span data-stu-id="e02aa-134">Request</span></span>
<span data-ttu-id="e02aa-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e02aa-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="e02aa-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="e02aa-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/beta/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="e02aa-137">C#</span><span class="sxs-lookup"><span data-stu-id="e02aa-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e02aa-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="e02aa-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="e02aa-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="e02aa-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="e02aa-140">Java</span><span class="sxs-lookup"><span data-stu-id="e02aa-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="e02aa-141">响应</span><span class="sxs-lookup"><span data-stu-id="e02aa-141">Response</span></span>
<span data-ttu-id="e02aa-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e02aa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 201

{
  "id": "id-value",
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
