---
title: 更新域
description: 更新域对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 05819b5e0a33fdf92072f64442c5ceb30a30b085
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260394"
---
# <a name="update-domain"></a><span data-ttu-id="bf1fe-103">更新域</span><span class="sxs-lookup"><span data-stu-id="bf1fe-103">Update domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf1fe-104">更新域对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="bf1fe-105">**重要说明:** 仅已验证的域可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf1fe-106">权限</span><span class="sxs-lookup"><span data-stu-id="bf1fe-106">Permissions</span></span>

<span data-ttu-id="bf1fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="bf1fe-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf1fe-109">Permission type</span></span>      | <span data-ttu-id="bf1fe-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf1fe-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf1fe-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf1fe-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bf1fe-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf1fe-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf1fe-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf1fe-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf1fe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-114">Not supported.</span></span>    |
|<span data-ttu-id="bf1fe-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf1fe-115">Application</span></span> | <span data-ttu-id="bf1fe-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf1fe-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf1fe-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf1fe-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="bf1fe-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf1fe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf1fe-119">Request headers</span></span>

| <span data-ttu-id="bf1fe-120">名称</span><span class="sxs-lookup"><span data-stu-id="bf1fe-120">Name</span></span>       | <span data-ttu-id="bf1fe-121">说明</span><span class="sxs-lookup"><span data-stu-id="bf1fe-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bf1fe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf1fe-122">Authorization</span></span>  | <span data-ttu-id="bf1fe-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bf1fe-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bf1fe-125">Content-Type</span></span>  | <span data-ttu-id="bf1fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bf1fe-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bf1fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf1fe-127">Request body</span></span>

<span data-ttu-id="bf1fe-128">在请求正文中, 提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="bf1fe-129">未包含在请求正文中的现有属性将保留其以前的值, 或根据对其他属性值的更改重新计算这些属性。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bf1fe-130">为了获得最佳性能, 仅包含更改的值。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="bf1fe-131">响应</span><span class="sxs-lookup"><span data-stu-id="bf1fe-131">Response</span></span>

<span data-ttu-id="bf1fe-132">如果成功, 此方法将`204 No Content`返回响应代码, 不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="bf1fe-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf1fe-133">示例</span><span class="sxs-lookup"><span data-stu-id="bf1fe-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bf1fe-134">请求</span><span class="sxs-lookup"><span data-stu-id="bf1fe-134">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/beta/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="bf1fe-135">响应</span><span class="sxs-lookup"><span data-stu-id="bf1fe-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="bf1fe-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="bf1fe-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="bf1fe-137">C#</span><span class="sxs-lookup"><span data-stu-id="bf1fe-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bf1fe-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="bf1fe-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_domain-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="bf1fe-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="bf1fe-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/update_domain-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
