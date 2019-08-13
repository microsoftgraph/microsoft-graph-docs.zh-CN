---
title: 删除威胁情报指标
description: 删除 tiIndicator 对象。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 790509aa9cc74dcd13ebcbed68e0e5816d6d0566
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36362785"
---
# <a name="delete-threat-intelligence-indicator"></a><span data-ttu-id="2030f-103">删除威胁情报指标</span><span class="sxs-lookup"><span data-stu-id="2030f-103">Delete threat intelligence indicator</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2030f-104">删除[tiIndicator](../resources/tiindicator.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2030f-104">Delete a [tiIndicator](../resources/tiindicator.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2030f-105">权限</span><span class="sxs-lookup"><span data-stu-id="2030f-105">Permissions</span></span>

<span data-ttu-id="2030f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2030f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2030f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2030f-108">Permission type</span></span>                        | <span data-ttu-id="2030f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2030f-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2030f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2030f-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="2030f-111">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2030f-111">ThreatIndicators.ReadWrite.OwnedBy</span></span> |
| <span data-ttu-id="2030f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2030f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2030f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2030f-113">Not supported.</span></span> |
| <span data-ttu-id="2030f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2030f-114">Application</span></span>                            | <span data-ttu-id="2030f-115">ThreatIndicators.ReadWrite.OwnedBy</span><span class="sxs-lookup"><span data-stu-id="2030f-115">ThreatIndicators.ReadWrite.OwnedBy</span></span> |

## <a name="http-request"></a><span data-ttu-id="2030f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2030f-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
DELETE /security/tiIndicators/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2030f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2030f-117">Request headers</span></span>

| <span data-ttu-id="2030f-118">名称</span><span class="sxs-lookup"><span data-stu-id="2030f-118">Name</span></span>          | <span data-ttu-id="2030f-119">说明</span><span class="sxs-lookup"><span data-stu-id="2030f-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2030f-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2030f-120">Authorization</span></span> | <span data-ttu-id="2030f-121">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="2030f-121">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="2030f-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="2030f-122">Request body</span></span>

<span data-ttu-id="2030f-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2030f-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2030f-124">响应</span><span class="sxs-lookup"><span data-stu-id="2030f-124">Response</span></span>

<span data-ttu-id="2030f-p102">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="2030f-p102">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2030f-127">示例</span><span class="sxs-lookup"><span data-stu-id="2030f-127">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2030f-128">请求</span><span class="sxs-lookup"><span data-stu-id="2030f-128">Request</span></span>

<span data-ttu-id="2030f-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2030f-129">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="2030f-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="2030f-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_tiindicator"
}-->

```http
DELETE https://graph.microsoft.com/beta/security/tiIndicators/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2030f-131">C#</span><span class="sxs-lookup"><span data-stu-id="2030f-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-tiindicator-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2030f-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2030f-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-tiindicator-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2030f-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="2030f-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-tiindicator-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2030f-134">Java</span><span class="sxs-lookup"><span data-stu-id="2030f-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-tiindicator-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2030f-135">响应</span><span class="sxs-lookup"><span data-stu-id="2030f-135">Response</span></span>

<span data-ttu-id="2030f-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2030f-136">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete tiIndicator",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
