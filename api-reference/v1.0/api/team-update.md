---
title: 更新团队
description: 更新指定团队的属性。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 20f71b2de2fda180bd6e1c4f03a22159c56714d8
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290333"
---
# <a name="update-team"></a><span data-ttu-id="eef75-103">更新团队</span><span class="sxs-lookup"><span data-stu-id="eef75-103">Update team</span></span>

<span data-ttu-id="eef75-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eef75-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="eef75-105">更新指定[团队](../resources/team.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="eef75-105">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eef75-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="eef75-106">Permissions</span></span>
<span data-ttu-id="eef75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eef75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="eef75-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eef75-109">Permission type</span></span>      | <span data-ttu-id="eef75-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="eef75-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eef75-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eef75-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eef75-112">TeamSettings、Group 写全部、所有的 ReadWrite。 All</span><span class="sxs-lookup"><span data-stu-id="eef75-112">TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |
|<span data-ttu-id="eef75-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eef75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eef75-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eef75-114">Not supported.</span></span>    |
|<span data-ttu-id="eef75-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eef75-115">Application</span></span> | <span data-ttu-id="eef75-116">TeamSettings （[RSC](https://aka.ms/teams-rsc)）、TeamSettings、All、group、All、All 和 All。 all</span><span class="sxs-lookup"><span data-stu-id="eef75-116">TeamSettings.Edit.Group ([RSC](https://aka.ms/teams-rsc)), TeamSettings.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

> <span data-ttu-id="eef75-117">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="eef75-117">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="eef75-118">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="eef75-118">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="eef75-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eef75-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```

## <a name="request-headers"></a><span data-ttu-id="eef75-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eef75-120">Request headers</span></span>
| <span data-ttu-id="eef75-121">标头</span><span class="sxs-lookup"><span data-stu-id="eef75-121">Header</span></span>       | <span data-ttu-id="eef75-122">值</span><span class="sxs-lookup"><span data-stu-id="eef75-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="eef75-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eef75-123">Authorization</span></span>  | <span data-ttu-id="eef75-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="eef75-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="eef75-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="eef75-126">Content-Type</span></span>  | <span data-ttu-id="eef75-127">application/json</span><span class="sxs-lookup"><span data-stu-id="eef75-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="eef75-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="eef75-128">Request body</span></span>
<span data-ttu-id="eef75-129">在请求正文中，提供[team](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eef75-129">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="eef75-130">响应</span><span class="sxs-lookup"><span data-stu-id="eef75-130">Response</span></span>

<span data-ttu-id="eef75-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="eef75-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="eef75-132">示例</span><span class="sxs-lookup"><span data-stu-id="eef75-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="eef75-133">请求</span><span class="sxs-lookup"><span data-stu-id="eef75-133">Request</span></span>
<span data-ttu-id="eef75-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="eef75-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="eef75-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="eef75-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/teams/{id}
Content-type: application/json
Content-length: 211

{  
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
  }
}
```
# <a name="c"></a>[<span data-ttu-id="eef75-136">C#</span><span class="sxs-lookup"><span data-stu-id="eef75-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-team-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="eef75-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eef75-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-team-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="eef75-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="eef75-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-team-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="eef75-139">Java</span><span class="sxs-lookup"><span data-stu-id="eef75-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-team-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="eef75-140">响应</span><span class="sxs-lookup"><span data-stu-id="eef75-140">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update Team",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
