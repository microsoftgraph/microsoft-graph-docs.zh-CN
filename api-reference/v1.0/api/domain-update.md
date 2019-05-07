---
title: 更新域
description: 更新域对象的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f1821abf0fa89d4f0b11d63d39f74fb231b7c22f
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33617045"
---
# <a name="update-domain"></a><span data-ttu-id="93269-103">更新域</span><span class="sxs-lookup"><span data-stu-id="93269-103">Update domain</span></span>

<span data-ttu-id="93269-104">更新域对象的属性。</span><span class="sxs-lookup"><span data-stu-id="93269-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="93269-105">**重要说明:** 仅已验证的域可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="93269-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="93269-106">权限</span><span class="sxs-lookup"><span data-stu-id="93269-106">Permissions</span></span>

<span data-ttu-id="93269-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="93269-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="93269-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="93269-109">Permission type</span></span>      | <span data-ttu-id="93269-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="93269-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="93269-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93269-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93269-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93269-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="93269-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93269-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93269-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="93269-114">Not supported.</span></span>    |
|<span data-ttu-id="93269-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="93269-115">Application</span></span> | <span data-ttu-id="93269-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93269-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93269-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93269-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="93269-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="93269-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93269-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="93269-119">Request headers</span></span>

| <span data-ttu-id="93269-120">名称</span><span class="sxs-lookup"><span data-stu-id="93269-120">Name</span></span>       | <span data-ttu-id="93269-121">说明</span><span class="sxs-lookup"><span data-stu-id="93269-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="93269-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93269-122">Authorization</span></span>  | <span data-ttu-id="93269-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="93269-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93269-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="93269-125">Content-Type</span></span>  | <span data-ttu-id="93269-126">application/json</span><span class="sxs-lookup"><span data-stu-id="93269-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="93269-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="93269-127">Request body</span></span>

<span data-ttu-id="93269-128">在请求正文中, 提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="93269-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="93269-129">未包含在请求正文中的现有属性将保留其以前的值, 或根据对其他属性值的更改重新计算这些属性。</span><span class="sxs-lookup"><span data-stu-id="93269-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="93269-130">为了获得最佳性能, 仅包含更改的值。</span><span class="sxs-lookup"><span data-stu-id="93269-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="93269-131">响应</span><span class="sxs-lookup"><span data-stu-id="93269-131">Response</span></span>

<span data-ttu-id="93269-132">如果成功, 此方法将`204 No Content`返回响应代码, 不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="93269-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="93269-133">示例</span><span class="sxs-lookup"><span data-stu-id="93269-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="93269-134">请求</span><span class="sxs-lookup"><span data-stu-id="93269-134">Request</span></span>

<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "update_domain"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/domains/contoso.com
Content-type: application/json

{
  "isDefault": true,
  "supportedServices": [
    "Email",
    "OfficeCommunicationsOnline"
  ]
}
```

##### <a name="response"></a><span data-ttu-id="93269-135">响应</span><span class="sxs-lookup"><span data-stu-id="93269-135">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 204 No Content
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="93269-136">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="93269-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="93269-137">语言</span><span class="sxs-lookup"><span data-stu-id="93269-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/update_domain-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="93269-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="93269-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/update_domain-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/domain-update.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
