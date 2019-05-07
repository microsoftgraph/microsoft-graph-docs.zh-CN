---
title: 删除威胁情报指标
description: 删除 tiIndicator 对象。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: aa7ceefca5201930f97d5e7befb6a7cc43c5715a
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637596"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="d8baf-103">删除威胁情报指标</span><span class="sxs-lookup"><span data-stu-id="d8baf-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d8baf-104">删除[tiIndicator](../resources/tiindicator.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8baf-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8baf-105">权限</span><span class="sxs-lookup"><span data-stu-id="d8baf-105">Permissions</span></span>

<span data-ttu-id="d8baf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8baf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="d8baf-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8baf-108">Permission type</span></span>                        | <span data-ttu-id="d8baf-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8baf-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="d8baf-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8baf-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="d8baf-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d8baf-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="d8baf-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8baf-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8baf-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8baf-113">Not supported.</span></span> |
| <span data-ttu-id="d8baf-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8baf-114">Application</span></span>                            | <span data-ttu-id="d8baf-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="d8baf-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8baf-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8baf-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="d8baf-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8baf-117">Request headers</span></span>

| <span data-ttu-id="d8baf-118">名称</span><span class="sxs-lookup"><span data-stu-id="d8baf-118">Name</span></span>          | <span data-ttu-id="d8baf-119">说明</span><span class="sxs-lookup"><span data-stu-id="d8baf-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="d8baf-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8baf-120">Authorization</span></span> | <span data-ttu-id="d8baf-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="d8baf-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="d8baf-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8baf-122">Request body</span></span>

<span data-ttu-id="d8baf-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d8baf-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d8baf-124">响应</span><span class="sxs-lookup"><span data-stu-id="d8baf-124">Response</span></span>

<span data-ttu-id="d8baf-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="d8baf-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d8baf-127">示例</span><span class="sxs-lookup"><span data-stu-id="d8baf-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d8baf-128">请求</span><span class="sxs-lookup"><span data-stu-id="d8baf-128">Request</span></span>

<span data-ttu-id="d8baf-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d8baf-129">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```

### <a name="response"></a><span data-ttu-id="d8baf-130">响应</span><span class="sxs-lookup"><span data-stu-id="d8baf-130">Response</span></span>

<span data-ttu-id="d8baf-131">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="d8baf-131">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="d8baf-132">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d8baf-132">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d8baf-133">语言</span><span class="sxs-lookup"><span data-stu-id="d8baf-133">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d8baf-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d8baf-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/delete_tiindicator-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/tiindicator-delete.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
