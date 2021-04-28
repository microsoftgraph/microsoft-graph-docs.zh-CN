---
title: 'group: renew'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: fccf59c57a160a6517479463b432d73cfd5278be
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053067"
---
# <a name="group-renew"></a><span data-ttu-id="9fb0b-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="9fb0b-104">group: renew</span></span>

<span data-ttu-id="9fb0b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9fb0b-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9fb0b-106">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="9fb0b-106">Renews a group's expiration.</span></span> <span data-ttu-id="9fb0b-107">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="9fb0b-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="9fb0b-108">权限</span><span class="sxs-lookup"><span data-stu-id="9fb0b-108">Permissions</span></span>

<span data-ttu-id="9fb0b-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9fb0b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="9fb0b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9fb0b-111">Permission type</span></span>      | <span data-ttu-id="9fb0b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9fb0b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9fb0b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9fb0b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="9fb0b-114">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fb0b-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="9fb0b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9fb0b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9fb0b-116">不支持</span><span class="sxs-lookup"><span data-stu-id="9fb0b-116">Not supported</span></span> |
|<span data-ttu-id="9fb0b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9fb0b-117">Application</span></span> | <span data-ttu-id="9fb0b-118">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9fb0b-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="9fb0b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9fb0b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="9fb0b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9fb0b-120">Request headers</span></span>
| <span data-ttu-id="9fb0b-121">名称</span><span class="sxs-lookup"><span data-stu-id="9fb0b-121">Name</span></span>       | <span data-ttu-id="9fb0b-122">说明</span><span class="sxs-lookup"><span data-stu-id="9fb0b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9fb0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9fb0b-123">Authorization</span></span>  | <span data-ttu-id="9fb0b-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9fb0b-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="9fb0b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9fb0b-126">Request body</span></span>

<span data-ttu-id="9fb0b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9fb0b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9fb0b-128">响应</span><span class="sxs-lookup"><span data-stu-id="9fb0b-128">Response</span></span>

<span data-ttu-id="9fb0b-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9fb0b-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9fb0b-131">示例</span><span class="sxs-lookup"><span data-stu-id="9fb0b-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9fb0b-132">请求</span><span class="sxs-lookup"><span data-stu-id="9fb0b-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9fb0b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9fb0b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="c"></a>[<span data-ttu-id="9fb0b-134">C#</span><span class="sxs-lookup"><span data-stu-id="9fb0b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9fb0b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9fb0b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9fb0b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9fb0b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9fb0b-137">Java</span><span class="sxs-lookup"><span data-stu-id="9fb0b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9fb0b-138">响应</span><span class="sxs-lookup"><span data-stu-id="9fb0b-138">Response</span></span>
<span data-ttu-id="9fb0b-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9fb0b-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

