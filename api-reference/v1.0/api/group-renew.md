---
title: 'group: renew'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 533f82fa737c85fd816da04d75b712072d95a46c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042007"
---
# <a name="group-renew"></a><span data-ttu-id="f7e04-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="f7e04-104">group: renew</span></span>

<span data-ttu-id="f7e04-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7e04-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f7e04-106">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="f7e04-106">Renews a group's expiration.</span></span> <span data-ttu-id="f7e04-107">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="f7e04-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="f7e04-108">权限</span><span class="sxs-lookup"><span data-stu-id="f7e04-108">Permissions</span></span>

<span data-ttu-id="f7e04-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7e04-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="f7e04-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7e04-111">Permission type</span></span>      | <span data-ttu-id="f7e04-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f7e04-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f7e04-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e04-113">Delegated (work or school account)</span></span> | <span data-ttu-id="f7e04-114">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e04-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="f7e04-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7e04-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f7e04-116">不支持</span><span class="sxs-lookup"><span data-stu-id="f7e04-116">Not supported</span></span> |
|<span data-ttu-id="f7e04-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7e04-117">Application</span></span> | <span data-ttu-id="f7e04-118">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7e04-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f7e04-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7e04-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="f7e04-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7e04-120">Request headers</span></span>
| <span data-ttu-id="f7e04-121">名称</span><span class="sxs-lookup"><span data-stu-id="f7e04-121">Name</span></span>       | <span data-ttu-id="f7e04-122">说明</span><span class="sxs-lookup"><span data-stu-id="f7e04-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f7e04-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7e04-123">Authorization</span></span>  | <span data-ttu-id="f7e04-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f7e04-p104">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="f7e04-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7e04-126">Request body</span></span>

<span data-ttu-id="f7e04-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7e04-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7e04-128">响应</span><span class="sxs-lookup"><span data-stu-id="f7e04-128">Response</span></span>

<span data-ttu-id="f7e04-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f7e04-p105">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7e04-131">示例</span><span class="sxs-lookup"><span data-stu-id="f7e04-131">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f7e04-132">请求</span><span class="sxs-lookup"><span data-stu-id="f7e04-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f7e04-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f7e04-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="c"></a>[<span data-ttu-id="f7e04-134">C#</span><span class="sxs-lookup"><span data-stu-id="f7e04-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f7e04-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f7e04-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f7e04-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f7e04-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f7e04-137">Java</span><span class="sxs-lookup"><span data-stu-id="f7e04-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f7e04-138">响应</span><span class="sxs-lookup"><span data-stu-id="f7e04-138">Response</span></span>
<span data-ttu-id="f7e04-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7e04-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

