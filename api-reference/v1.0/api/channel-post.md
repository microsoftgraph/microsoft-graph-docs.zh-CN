---
title: 创建频道
description: 在 Microsoft 团队中创建请求正文中指定的新频道。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9a63834cc83c9f96e5e0776d8c676b1741c075ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48063869"
---
# <a name="create-channel"></a><span data-ttu-id="5e3ac-103">创建频道</span><span class="sxs-lookup"><span data-stu-id="5e3ac-103">Create Channel</span></span>

<span data-ttu-id="5e3ac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e3ac-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="5e3ac-105">在 Microsoft 团队中创建请求正文中指定的新[频道](../resources/channel.md)。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-105">Create a new [channel](../resources/channel.md) in a Microsoft Team, as specified in the request body.</span></span>

> <span data-ttu-id="5e3ac-106">**请注意**：应用程序权限和此 API 存在已知问题。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-106">**Note**: There is a known issue with application permissions and this API.</span></span> <span data-ttu-id="5e3ac-107">有关详细信息，请参阅[已知问题列表](/graph/known-issues#application-permissions)。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-107">For details, see the [known issues list](/graph/known-issues#application-permissions).</span></span>

## <a name="permissions"></a><span data-ttu-id="5e3ac-108">权限</span><span class="sxs-lookup"><span data-stu-id="5e3ac-108">Permissions</span></span>
<span data-ttu-id="5e3ac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="5e3ac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e3ac-111">Permission type</span></span>      | <span data-ttu-id="5e3ac-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e3ac-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5e3ac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e3ac-113">Delegated (work or school account)</span></span> | <span data-ttu-id="5e3ac-114">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e3ac-114">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="5e3ac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e3ac-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e3ac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-116">Not supported.</span></span>    |
|<span data-ttu-id="5e3ac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e3ac-117">Application</span></span> | <span data-ttu-id="5e3ac-118">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e3ac-118">Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="5e3ac-119">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-119">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="5e3ac-120">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-120">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="5e3ac-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e3ac-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /teams/{id}/channels
```
## <a name="request-headers"></a><span data-ttu-id="5e3ac-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e3ac-122">Request headers</span></span>
| <span data-ttu-id="5e3ac-123">标头</span><span class="sxs-lookup"><span data-stu-id="5e3ac-123">Header</span></span>       | <span data-ttu-id="5e3ac-124">值</span><span class="sxs-lookup"><span data-stu-id="5e3ac-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="5e3ac-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e3ac-125">Authorization</span></span>  | <span data-ttu-id="5e3ac-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5e3ac-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e3ac-128">Content-Type</span></span>  | <span data-ttu-id="5e3ac-129">application/json</span><span class="sxs-lookup"><span data-stu-id="5e3ac-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="5e3ac-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e3ac-130">Request body</span></span>
<span data-ttu-id="5e3ac-131">在请求正文中，提供 [channel](../resources/channel.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-131">In the request body, supply a JSON representation of [channel](../resources/channel.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5e3ac-132">响应</span><span class="sxs-lookup"><span data-stu-id="5e3ac-132">Response</span></span>

<span data-ttu-id="5e3ac-133">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [channel](../resources/channel.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-133">If successful, this method returns `201 Created` response code and [channel](../resources/channel.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e3ac-134">示例</span><span class="sxs-lookup"><span data-stu-id="5e3ac-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5e3ac-135">请求</span><span class="sxs-lookup"><span data-stu-id="5e3ac-135">Request</span></span>
<span data-ttu-id="5e3ac-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-136">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e3ac-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e3ac-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_channel_from_group"
}-->
```http
POST https://graph.microsoft.com/v1.0/teams/{id}/channels
Content-type: application/json

{
  "displayName": "Architecture Discussion",
  "description": "This channel is where we debate all future architecture plans"
}
```
# <a name="c"></a>[<span data-ttu-id="5e3ac-138">C#</span><span class="sxs-lookup"><span data-stu-id="5e3ac-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-channel-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e3ac-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e3ac-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-channel-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e3ac-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e3ac-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-channel-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e3ac-141">Java</span><span class="sxs-lookup"><span data-stu-id="5e3ac-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-channel-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5e3ac-142">响应</span><span class="sxs-lookup"><span data-stu-id="5e3ac-142">Response</span></span>
<span data-ttu-id="5e3ac-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5e3ac-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.channel"
} -->
```http
HTTP/1.1 201 Created
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
<!-- {
  "type": "#page.annotation",
  "description": "Create Channel",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

