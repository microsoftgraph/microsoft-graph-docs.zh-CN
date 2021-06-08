---
title: 更新域
description: 更新 domain 对象的属性。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: fc400d4790326e79d8ad8dea387d6027baf8f1de
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787301"
---
# <a name="update-domain"></a><span data-ttu-id="94865-103">更新域</span><span class="sxs-lookup"><span data-stu-id="94865-103">Update domain</span></span>

<span data-ttu-id="94865-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94865-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="94865-105">更新 domain 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="94865-105">Update the properties of domain object.</span></span>

> <span data-ttu-id="94865-106">**重要提示：** 只能更新已验证的域。</span><span class="sxs-lookup"><span data-stu-id="94865-106">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="94865-107">权限</span><span class="sxs-lookup"><span data-stu-id="94865-107">Permissions</span></span>

<span data-ttu-id="94865-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="94865-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="94865-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="94865-110">Permission type</span></span>      | <span data-ttu-id="94865-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="94865-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94865-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="94865-112">Delegated (work or school account)</span></span> | <span data-ttu-id="94865-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="94865-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="94865-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="94865-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94865-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="94865-115">Not supported.</span></span>    |
|<span data-ttu-id="94865-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="94865-116">Application</span></span> | <span data-ttu-id="94865-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94865-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94865-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="94865-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="94865-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="94865-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="94865-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="94865-120">Request headers</span></span>

| <span data-ttu-id="94865-121">名称</span><span class="sxs-lookup"><span data-stu-id="94865-121">Name</span></span>       | <span data-ttu-id="94865-122">说明</span><span class="sxs-lookup"><span data-stu-id="94865-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="94865-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="94865-123">Authorization</span></span>  | <span data-ttu-id="94865-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="94865-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="94865-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94865-126">Content-Type</span></span>  | <span data-ttu-id="94865-127">application/json</span><span class="sxs-lookup"><span data-stu-id="94865-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="94865-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="94865-128">Request body</span></span>

<span data-ttu-id="94865-129">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="94865-129">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="94865-130">请求正文中未包含的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="94865-130">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="94865-131">为获得最佳性能，仅包括更改的值。</span><span class="sxs-lookup"><span data-stu-id="94865-131">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="94865-132">响应</span><span class="sxs-lookup"><span data-stu-id="94865-132">Response</span></span>

<span data-ttu-id="94865-133">如果成功，此方法返回 响应 `204 No Content` 代码，无响应正文。</span><span class="sxs-lookup"><span data-stu-id="94865-133">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="94865-134">示例</span><span class="sxs-lookup"><span data-stu-id="94865-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94865-135">请求</span><span class="sxs-lookup"><span data-stu-id="94865-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="94865-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="94865-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="94865-137">C#</span><span class="sxs-lookup"><span data-stu-id="94865-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94865-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94865-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94865-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94865-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94865-140">Java</span><span class="sxs-lookup"><span data-stu-id="94865-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94865-141">响应</span><span class="sxs-lookup"><span data-stu-id="94865-141">Response</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

