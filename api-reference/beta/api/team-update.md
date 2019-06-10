---
title: 更新团队
description: 更新指定团队的属性。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: d55c9b1465da588d19f96cc6e67bab1ddd44fb55
ms.sourcegitcommit: b742da101a3a232356bf748c42da3ba08a7539d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2019
ms.locfileid: "34812934"
---
# <a name="update-team"></a><span data-ttu-id="04636-103">更新团队</span><span class="sxs-lookup"><span data-stu-id="04636-103">Update team</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04636-104">更新指定[团队](../resources/team.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="04636-104">Update the properties of the specified [team](../resources/team.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="04636-105">权限</span><span class="sxs-lookup"><span data-stu-id="04636-105">Permissions</span></span>
<span data-ttu-id="04636-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04636-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="04636-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="04636-108">Permission type</span></span>      | <span data-ttu-id="04636-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="04636-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="04636-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04636-110">Delegated (work or school account)</span></span> | <span data-ttu-id="04636-111">Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04636-111">Group.ReadWrite.All</span></span>    |
|<span data-ttu-id="04636-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04636-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="04636-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="04636-113">Not supported.</span></span>    |
|<span data-ttu-id="04636-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="04636-114">Application</span></span> | <span data-ttu-id="04636-115">Group.Read.All、Group.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04636-115">Group.Read.All, Group.ReadWrite.All</span></span>    |

> <span data-ttu-id="04636-116">**注意**：此 API 支持管理员权限。</span><span class="sxs-lookup"><span data-stu-id="04636-116">**Note**: This API supports admin permissions.</span></span> <span data-ttu-id="04636-117">全局管理员和 Microsoft Teams 服务管理员可以访问自己不是其中成员的团队。</span><span class="sxs-lookup"><span data-stu-id="04636-117">Global admins and Microsoft Teams service admins can access teams that they are not a member of.</span></span>

## <a name="http-request"></a><span data-ttu-id="04636-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04636-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /teams/{id}
```
## <a name="request-headers"></a><span data-ttu-id="04636-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="04636-119">Request headers</span></span>
| <span data-ttu-id="04636-120">标头</span><span class="sxs-lookup"><span data-stu-id="04636-120">Header</span></span>       | <span data-ttu-id="04636-121">值</span><span class="sxs-lookup"><span data-stu-id="04636-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="04636-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04636-122">Authorization</span></span>  | <span data-ttu-id="04636-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="04636-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="04636-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="04636-125">Content-Type</span></span>  | <span data-ttu-id="04636-126">application/json</span><span class="sxs-lookup"><span data-stu-id="04636-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="04636-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="04636-127">Request body</span></span>
<span data-ttu-id="04636-128">在请求正文中, 提供[team](../resources/team.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04636-128">In the request body, supply a JSON representation of [team](../resources/team.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="04636-129">响应</span><span class="sxs-lookup"><span data-stu-id="04636-129">Response</span></span>

<span data-ttu-id="04636-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="04636-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04636-131">示例</span><span class="sxs-lookup"><span data-stu-id="04636-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="04636-132">请求</span><span class="sxs-lookup"><span data-stu-id="04636-132">Request</span></span>
<span data-ttu-id="04636-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="04636-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_team"
}-->
```http
PATCH https://graph.microsoft.com/beta/teams/{id}
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
  },
  "discoverySettings": {
    "showInTeamsSearchAndSuggestions": true
  }
}
```
#### <a name="response"></a><span data-ttu-id="04636-134">响应</span><span class="sxs-lookup"><span data-stu-id="04636-134">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.team"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="04636-135">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="04636-135">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="04636-136">C#</span><span class="sxs-lookup"><span data-stu-id="04636-136">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_team-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="04636-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="04636-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_team-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/team-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/team-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
