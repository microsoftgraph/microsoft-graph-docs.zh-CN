---
title: 更新域
description: 更新域对象的属性。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b22677f64057cfa0baf16afb76d58a0d6d456203
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2020
ms.locfileid: "43179407"
---
# <a name="update-domain"></a><span data-ttu-id="837c7-103">更新域</span><span class="sxs-lookup"><span data-stu-id="837c7-103">Update domain</span></span>

<span data-ttu-id="837c7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="837c7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="837c7-105">更新域对象的属性。</span><span class="sxs-lookup"><span data-stu-id="837c7-105">Update the properties of domain object.</span></span>

> <span data-ttu-id="837c7-106">**重要说明：** 仅已验证的域可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="837c7-106">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="837c7-107">权限</span><span class="sxs-lookup"><span data-stu-id="837c7-107">Permissions</span></span>

<span data-ttu-id="837c7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="837c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="837c7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="837c7-110">Permission type</span></span>      | <span data-ttu-id="837c7-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="837c7-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="837c7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="837c7-112">Delegated (work or school account)</span></span> | <span data-ttu-id="837c7-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="837c7-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="837c7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="837c7-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="837c7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="837c7-115">Not supported.</span></span>    |
|<span data-ttu-id="837c7-116">Application</span><span class="sxs-lookup"><span data-stu-id="837c7-116">Application</span></span> | <span data-ttu-id="837c7-117">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="837c7-117">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="837c7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="837c7-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="837c7-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="837c7-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="837c7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="837c7-120">Request headers</span></span>

| <span data-ttu-id="837c7-121">名称</span><span class="sxs-lookup"><span data-stu-id="837c7-121">Name</span></span>       | <span data-ttu-id="837c7-122">说明</span><span class="sxs-lookup"><span data-stu-id="837c7-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="837c7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="837c7-123">Authorization</span></span>  | <span data-ttu-id="837c7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="837c7-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="837c7-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="837c7-126">Content-Type</span></span>  | <span data-ttu-id="837c7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="837c7-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="837c7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="837c7-128">Request body</span></span>

<span data-ttu-id="837c7-129">在请求正文中，提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="837c7-129">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="837c7-130">未包含在请求正文中的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算这些属性。</span><span class="sxs-lookup"><span data-stu-id="837c7-130">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="837c7-131">为了获得最佳性能，仅包含更改的值。</span><span class="sxs-lookup"><span data-stu-id="837c7-131">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="837c7-132">响应</span><span class="sxs-lookup"><span data-stu-id="837c7-132">Response</span></span>

<span data-ttu-id="837c7-133">如果成功，此方法将`204 No Content`返回响应代码，不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="837c7-133">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="837c7-134">示例</span><span class="sxs-lookup"><span data-stu-id="837c7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="837c7-135">请求</span><span class="sxs-lookup"><span data-stu-id="837c7-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="837c7-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="837c7-136">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="837c7-137">C#</span><span class="sxs-lookup"><span data-stu-id="837c7-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="837c7-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="837c7-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="837c7-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="837c7-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="837c7-140">Java</span><span class="sxs-lookup"><span data-stu-id="837c7-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="837c7-141">响应</span><span class="sxs-lookup"><span data-stu-id="837c7-141">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
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
