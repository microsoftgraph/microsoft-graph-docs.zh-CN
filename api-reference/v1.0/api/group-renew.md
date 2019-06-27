---
title: 'group: renew'
description: 续订组以更新到期时间。 续订后，组的有效期就会延长策略中定义的天数。
localization_priority: Normal
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 70f0ef9c40d5e23b80b5ba5c4f959369412137a1
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277642"
---
# <a name="group-renew"></a><span data-ttu-id="8b139-104">group: renew</span><span class="sxs-lookup"><span data-stu-id="8b139-104">group: renew</span></span>

<span data-ttu-id="8b139-105">续订组以更新到期时间。</span><span class="sxs-lookup"><span data-stu-id="8b139-105">Renews a group's expiration.</span></span> <span data-ttu-id="8b139-106">续订后，组的有效期就会延长策略中定义的天数。</span><span class="sxs-lookup"><span data-stu-id="8b139-106">When a group is renewed, the group expiration is extended by the number of days defined in the policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="8b139-107">权限</span><span class="sxs-lookup"><span data-stu-id="8b139-107">Permissions</span></span>

<span data-ttu-id="8b139-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b139-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>
 

|<span data-ttu-id="8b139-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b139-110">Permission type</span></span>      | <span data-ttu-id="8b139-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b139-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8b139-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b139-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8b139-113">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b139-113">Group.ReadWrite.All or Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="8b139-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b139-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8b139-115">不支持</span><span class="sxs-lookup"><span data-stu-id="8b139-115">Not supported</span></span> |
|<span data-ttu-id="8b139-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b139-116">Application</span></span> | <span data-ttu-id="8b139-117">Group.ReadWrite.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b139-117">Group.ReadWrite.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8b139-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b139-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /groups/{id}/renew
```

## <a name="request-headers"></a><span data-ttu-id="8b139-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b139-119">Request headers</span></span>
| <span data-ttu-id="8b139-120">名称</span><span class="sxs-lookup"><span data-stu-id="8b139-120">Name</span></span>       | <span data-ttu-id="8b139-121">说明</span><span class="sxs-lookup"><span data-stu-id="8b139-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8b139-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b139-122">Authorization</span></span>  | <span data-ttu-id="8b139-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="8b139-123">Bearer {token}</span></span> |


## <a name="request-body"></a><span data-ttu-id="8b139-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b139-124">Request body</span></span>

<span data-ttu-id="8b139-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8b139-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8b139-126">响应</span><span class="sxs-lookup"><span data-stu-id="8b139-126">Response</span></span>

<span data-ttu-id="8b139-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="8b139-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b139-129">示例</span><span class="sxs-lookup"><span data-stu-id="8b139-129">Example</span></span>

##### <a name="request"></a><span data-ttu-id="8b139-130">请求</span><span class="sxs-lookup"><span data-stu-id="8b139-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "group_renew"
}-->
```http
POST https://graph.microsoft.com/v1.0/groups/{id}/renew
```

##### <a name="response"></a><span data-ttu-id="8b139-131">响应</span><span class="sxs-lookup"><span data-stu-id="8b139-131">Response</span></span>
<span data-ttu-id="8b139-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8b139-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Boolean"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="8b139-134">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="8b139-134">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="8b139-135">C#</span><span class="sxs-lookup"><span data-stu-id="8b139-135">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/group_renew-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="8b139-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="8b139-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/group_renew-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="8b139-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="8b139-137">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/group_renew-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "group: renew",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/group-renew.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/group-renew.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/group-renew.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
