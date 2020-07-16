---
title: 删除成员
description: 使用此 API 可以通过**members**导航属性从 Microsoft 365 组、安全组或启用邮件的安全组中删除成员。 可以删除用户或其他组。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: e4d91d97f48f1a0adec10c0d42d51be399fb0f28
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44895865"
---
# <a name="remove-member"></a><span data-ttu-id="88739-104">删除成员</span><span class="sxs-lookup"><span data-stu-id="88739-104">Remove member</span></span>

<span data-ttu-id="88739-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88739-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88739-106">使用此 API 通过**成员**导航属性从组中删除成员。</span><span class="sxs-lookup"><span data-stu-id="88739-106">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="88739-107">权限</span><span class="sxs-lookup"><span data-stu-id="88739-107">Permissions</span></span>
<span data-ttu-id="88739-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88739-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88739-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="88739-110">Permission type</span></span>      | <span data-ttu-id="88739-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88739-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="88739-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88739-112">Delegated (work or school account)</span></span> | <span data-ttu-id="88739-113">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="88739-113">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="88739-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88739-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88739-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="88739-115">Not supported.</span></span> |
|<span data-ttu-id="88739-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="88739-116">Application</span></span> | <span data-ttu-id="88739-117">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88739-117">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="88739-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88739-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="88739-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="88739-119">Request headers</span></span>
| <span data-ttu-id="88739-120">名称</span><span class="sxs-lookup"><span data-stu-id="88739-120">Name</span></span>       | <span data-ttu-id="88739-121">类型</span><span class="sxs-lookup"><span data-stu-id="88739-121">Type</span></span> | <span data-ttu-id="88739-122">说明</span><span class="sxs-lookup"><span data-stu-id="88739-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="88739-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88739-123">Authorization</span></span>  | <span data-ttu-id="88739-124">string</span><span class="sxs-lookup"><span data-stu-id="88739-124">string</span></span>  | <span data-ttu-id="88739-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88739-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="88739-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88739-127">Request body</span></span>
<span data-ttu-id="88739-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="88739-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="88739-129">响应</span><span class="sxs-lookup"><span data-stu-id="88739-129">Response</span></span>
<span data-ttu-id="88739-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="88739-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88739-132">示例</span><span class="sxs-lookup"><span data-stu-id="88739-132">Example</span></span>
#### <a name="request"></a><span data-ttu-id="88739-133">请求</span><span class="sxs-lookup"><span data-stu-id="88739-133">Request</span></span>
<span data-ttu-id="88739-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="88739-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="88739-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="88739-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/beta/groups/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="88739-136">C#</span><span class="sxs-lookup"><span data-stu-id="88739-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="88739-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="88739-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="88739-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="88739-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="88739-139">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="88739-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="88739-140">响应</span><span class="sxs-lookup"><span data-stu-id="88739-140">Response</span></span>
<span data-ttu-id="88739-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="88739-141">The following is an example of the response.</span></span>
><span data-ttu-id="88739-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="88739-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="88739-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="88739-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

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
  ]
}
-->
