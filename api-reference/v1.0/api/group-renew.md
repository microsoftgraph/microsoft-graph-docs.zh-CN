---
title: 'group: renew'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
author: yyuank
ms.prod: groups
doc_type: apiPageType
ms.openlocfilehash: 8e1e9403acf31df4544c5e894895aa17a1e86e2a
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43124124"
---
# <a name="group-renew"></a><span data-ttu-id="43a29-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="43a29-104">group: renew</span></span>

<span data-ttu-id="43a29-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43a29-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="43a29-106">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="43a29-106">Renews a group's expiration.</span></span> <span data-ttu-id="43a29-107">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="43a29-107">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="43a29-108">权限</span><span class="sxs-lookup"><span data-stu-id="43a29-108">Permissions</span></span>

<span data-ttu-id="43a29-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43a29-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="43a29-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="43a29-111">Permission type</span></span>      | <span data-ttu-id="43a29-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43a29-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="43a29-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43a29-113">Delegated (work or school account)</span></span> | <span data-ttu-id="43a29-114">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a29-114">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="43a29-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43a29-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="43a29-116">不支持</span><span class="sxs-lookup"><span data-stu-id="43a29-116">Not supported</span></span> |
|<span data-ttu-id="43a29-117">Application</span><span class="sxs-lookup"><span data-stu-id="43a29-117">Application</span></span> | <span data-ttu-id="43a29-118">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43a29-118">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="43a29-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43a29-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="43a29-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="43a29-120">Request headers</span></span>
| <span data-ttu-id="43a29-121">名称</span><span class="sxs-lookup"><span data-stu-id="43a29-121">Name</span></span>       | <span data-ttu-id="43a29-122">说明</span><span class="sxs-lookup"><span data-stu-id="43a29-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="43a29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="43a29-123">Authorization</span></span>  | <span data-ttu-id="43a29-124">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="43a29-124">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="43a29-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="43a29-125">Request body</span></span>

<span data-ttu-id="43a29-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43a29-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43a29-127">响应</span><span class="sxs-lookup"><span data-stu-id="43a29-127">Response</span></span>

<span data-ttu-id="43a29-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="43a29-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43a29-130">示例</span><span class="sxs-lookup"><span data-stu-id="43a29-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="43a29-131">请求</span><span class="sxs-lookup"><span data-stu-id="43a29-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="43a29-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="43a29-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```
# <a name="c"></a>[<span data-ttu-id="43a29-133">C#</span><span class="sxs-lookup"><span data-stu-id="43a29-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-renew-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="43a29-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="43a29-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-renew-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="43a29-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="43a29-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-renew-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="43a29-136">Java</span><span class="sxs-lookup"><span data-stu-id="43a29-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-renew-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="43a29-137">响应</span><span class="sxs-lookup"><span data-stu-id="43a29-137">Response</span></span>
<span data-ttu-id="43a29-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43a29-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
