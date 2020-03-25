---
title: 删除成员
description: 使用此 API 通过**成员**导航属性从组中删除成员。
localization_priority: Priority
author: dkershaw10
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 7a5071120969394c0f60ff8cbb9632581375c369
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42892812"
---
# <a name="remove-member"></a><span data-ttu-id="dc9b8-103">删除成员</span><span class="sxs-lookup"><span data-stu-id="dc9b8-103">Remove member</span></span>

<span data-ttu-id="dc9b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dc9b8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dc9b8-105">使用此 API 通过**成员**导航属性从组中删除成员。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-105">Use this API to remove a member from a group via the **members** navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc9b8-106">权限</span><span class="sxs-lookup"><span data-stu-id="dc9b8-106">Permissions</span></span>
<span data-ttu-id="dc9b8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc9b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc9b8-109">Permission type</span></span>      | <span data-ttu-id="dc9b8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc9b8-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc9b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc9b8-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc9b8-112">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dc9b8-112">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
|<span data-ttu-id="dc9b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc9b8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc9b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-114">Not supported.</span></span> |
|<span data-ttu-id="dc9b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc9b8-115">Application</span></span> | <span data-ttu-id="dc9b8-116">GroupMember.ReadWrite.All、Group.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc9b8-116">GroupMember.ReadWrite.All, Group.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dc9b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc9b8-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /groups/{id}/members/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="dc9b8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dc9b8-118">Request headers</span></span>
| <span data-ttu-id="dc9b8-119">名称</span><span class="sxs-lookup"><span data-stu-id="dc9b8-119">Name</span></span>       | <span data-ttu-id="dc9b8-120">类型</span><span class="sxs-lookup"><span data-stu-id="dc9b8-120">Type</span></span> | <span data-ttu-id="dc9b8-121">说明</span><span class="sxs-lookup"><span data-stu-id="dc9b8-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dc9b8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dc9b8-122">Authorization</span></span>  | <span data-ttu-id="dc9b8-123">string</span><span class="sxs-lookup"><span data-stu-id="dc9b8-123">string</span></span>  | <span data-ttu-id="dc9b8-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dc9b8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dc9b8-126">Request body</span></span>
<span data-ttu-id="dc9b8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dc9b8-128">响应</span><span class="sxs-lookup"><span data-stu-id="dc9b8-128">Response</span></span>
<span data-ttu-id="dc9b8-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc9b8-131">示例</span><span class="sxs-lookup"><span data-stu-id="dc9b8-131">Example</span></span>
#### <a name="request"></a><span data-ttu-id="dc9b8-132">请求</span><span class="sxs-lookup"><span data-stu-id="dc9b8-132">Request</span></span>
<span data-ttu-id="dc9b8-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dc9b8-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc9b8-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_member_from_group"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/groups/{id}/members/{id}/$ref
```
# <a name="c"></a>[<span data-ttu-id="dc9b8-135">C#</span><span class="sxs-lookup"><span data-stu-id="dc9b8-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-member-from-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dc9b8-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc9b8-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-member-from-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dc9b8-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc9b8-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-member-from-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dc9b8-138">Java</span><span class="sxs-lookup"><span data-stu-id="dc9b8-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-member-from-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="dc9b8-139">在请求中，指定要在 $ref 段后删除的 directory 对象 `id`。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-139">In the request, specify the `id` of the directory object you want to remove after the $ref segment.</span></span>

#### <a name="response"></a><span data-ttu-id="dc9b8-140">响应</span><span class="sxs-lookup"><span data-stu-id="dc9b8-140">Response</span></span>
<span data-ttu-id="dc9b8-141">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-141">The following is an example of the response.</span></span>
><span data-ttu-id="dc9b8-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="dc9b8-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="dc9b8-143">All the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create member",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
