---
title: 更新团队
description: 更新指定团队的属性。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9ec5fd97ee1c747553752abced48efd0743bc65e
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786690"
---
# <a name="update-team"></a><span data-ttu-id="4a775-103">更新团队</span><span class="sxs-lookup"><span data-stu-id="4a775-103">Update team</span></span>

<span data-ttu-id="4a775-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a775-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a775-105">更新指定团队 [的属性](../resources/team.md)。</span><span class="sxs-lookup"><span data-stu-id="4a775-105">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="4a775-106">权限</span><span class="sxs-lookup"><span data-stu-id="4a775-106">Permissions</span></span>
<span data-ttu-id="4a775-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4a775-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4a775-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4a775-109">Permission type</span></span>      | <span data-ttu-id="4a775-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4a775-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4a775-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4a775-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4a775-112">TeamSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a775-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="4a775-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4a775-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4a775-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4a775-114">Not supported.</span></span>    |
|<span data-ttu-id="4a775-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4a775-115">Application</span></span> | <span data-ttu-id="4a775-116">TeamSettings.ReadWrite.Group\*、TeamSettings.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a775-116">TeamSettings.ReadWrite.Group\*, TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="4a775-117">**注意**：标有 \* 的权限用于 [特定于资源的同意](https://aka.ms/teams-rsc)。</span><span class="sxs-lookup"><span data-stu-id="4a775-117">**Note**: Permissions marked with \* use [resource-specific consent](https://aka.ms/teams-rsc).</span></span>

> <span data-ttu-id="4a775-p102">**注意**：此 API 支持管理员权限。全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="4a775-p102">**Note**: This API supports admin permissions. Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="4a775-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4a775-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{team-id}
```
## <a name="request-headers"></a><span data-ttu-id="4a775-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4a775-121">Request headers</span></span>
| <span data-ttu-id="4a775-122">标头</span><span class="sxs-lookup"><span data-stu-id="4a775-122">Header</span></span>       | <span data-ttu-id="4a775-123">值</span><span class="sxs-lookup"><span data-stu-id="4a775-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4a775-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4a775-124">Authorization</span></span>  | <span data-ttu-id="4a775-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4a775-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4a775-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4a775-127">Content-Type</span></span>  | <span data-ttu-id="4a775-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4a775-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4a775-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4a775-129">Request body</span></span>
<span data-ttu-id="4a775-130">在请求正文中，提供 team 对象的 JSON [表示](../resources/team.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="4a775-130">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="4a775-131">响应</span><span class="sxs-lookup"><span data-stu-id="4a775-131">Response</span></span>

<span data-ttu-id="4a775-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4a775-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4a775-133">示例</span><span class="sxs-lookup"><span data-stu-id="4a775-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="4a775-134">请求</span><span class="sxs-lookup"><span data-stu-id="4a775-134">Request</span></span>
<span data-ttu-id="4a775-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4a775-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4a775-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="4a775-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
Content-type: application/json
Content-length: 211

{  
 "isMembershipLimitedToOwners": true,
  "memberSettings": {
    "allowCreateUpdateChannels": true
  },
  "messagingSettings": {
    "allowUserEditMessages": true,
    "allowUserDeleteMessages": true
  },
  "funSettings": {
    "allowGiphy": true,
    "giphyContentRating": "strict"
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="4a775-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4a775-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="4a775-138">C#</span><span class="sxs-lookup"><span data-stu-id="4a775-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4a775-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4a775-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4a775-140">Java</span><span class="sxs-lookup"><span data-stu-id="4a775-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="4a775-141">响应</span><span class="sxs-lookup"><span data-stu-id="4a775-141">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


