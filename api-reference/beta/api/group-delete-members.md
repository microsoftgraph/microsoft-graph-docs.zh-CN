---
title: 删除成员
description: 使用此 API 可以通过 **members** 导航属性从 Office 365 组、安全组或启用邮件的安全组中删除成员。可以删除用户或其他组。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 12e26fb08f12f0cf177836baf0b5906237953f56
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35263327"
---
# <a name="remove-member"></a><span data-ttu-id="259db-104">删除成员</span><span class="sxs-lookup"><span data-stu-id="259db-104">Remove member</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="259db-105">使用此 API 可以通过**members**导航属性从组中删除成员。</span><span class="sxs-lookup"><span data-stu-id="259db-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="259db-106">权限</span><span class="sxs-lookup"><span data-stu-id="259db-106">Permissions</span></span>
<span data-ttu-id="259db-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="259db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="259db-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="259db-109">Permission type</span></span>      | <span data-ttu-id="259db-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="259db-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="259db-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="259db-111">Delegated (work or school account)</span></span> | <span data-ttu-id="259db-112">Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="259db-112">Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="259db-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="259db-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="259db-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="259db-114">Not supported.</span></span> |
|<span data-ttu-id="259db-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="259db-115">Application</span></span> | <span data-ttu-id="259db-116">Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="259db-116">Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="259db-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="259db-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="259db-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="259db-118">Request headers</span></span>
| <span data-ttu-id="259db-119">名称</span><span class="sxs-lookup"><span data-stu-id="259db-119">Name</span></span>       | <span data-ttu-id="259db-120">类型</span><span class="sxs-lookup"><span data-stu-id="259db-120">Type</span></span> | <span data-ttu-id="259db-121">说明</span><span class="sxs-lookup"><span data-stu-id="259db-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="259db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="259db-122">Authorization</span></span>  | <span data-ttu-id="259db-123">string</span><span class="sxs-lookup"><span data-stu-id="259db-123">string</span></span>  | <span data-ttu-id="259db-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="259db-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="259db-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="259db-126">Request body</span></span>
<span data-ttu-id="259db-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="259db-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="259db-128">响应</span><span class="sxs-lookup"><span data-stu-id="259db-128">Response</span></span>
<span data-ttu-id="259db-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="259db-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="259db-131">示例</span><span class="sxs-lookup"><span data-stu-id="259db-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="259db-132">请求</span><span class="sxs-lookup"><span data-stu-id="259db-132">Request</span></span>
<span data-ttu-id="259db-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="259db-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
<span data-ttu-id="259db-134">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="259db-134">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="259db-135">响应</span><span class="sxs-lookup"><span data-stu-id="259db-135">Response</span></span>
<span data-ttu-id="259db-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="259db-136">The following is an example of the response.</span></span>
><span data-ttu-id="259db-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="259db-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="259db-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="259db-138">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="259db-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="259db-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="259db-140">C#</span><span class="sxs-lookup"><span data-stu-id="259db-140">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="259db-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="259db-141">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="259db-142">目标-C</span><span class="sxs-lookup"><span data-stu-id="259db-142">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryobject_from_group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/group-delete-members.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
