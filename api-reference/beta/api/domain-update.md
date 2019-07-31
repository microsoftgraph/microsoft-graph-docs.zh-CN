---
title: 更新域
description: 更新域对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 8eaabaddb5e167f87b3bf4b5e75eb3c1fd80581c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957386"
---
# <a name="update-domain"></a><span data-ttu-id="d0527-103">更新域</span><span class="sxs-lookup"><span data-stu-id="d0527-103">Update domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0527-104">更新域对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d0527-104">Update the properties of domain object.</span></span>

> <span data-ttu-id="d0527-105">**重要说明:** 仅已验证的域可以进行更新。</span><span class="sxs-lookup"><span data-stu-id="d0527-105">**Important:** Only verified domains can be updated.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0527-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0527-106">Permissions</span></span>

<span data-ttu-id="d0527-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0527-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d0527-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0527-109">Permission type</span></span>      | <span data-ttu-id="d0527-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0527-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0527-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0527-111">Delegated (work or school account)</span></span> | <span data-ttu-id="d0527-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0527-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0527-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0527-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0527-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0527-114">Not supported.</span></span>    |
|<span data-ttu-id="d0527-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0527-115">Application</span></span> | <span data-ttu-id="d0527-116">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0527-116">Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0527-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0527-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /domains/{id}
```

> <span data-ttu-id="d0527-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="d0527-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0527-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0527-119">Request headers</span></span>

| <span data-ttu-id="d0527-120">名称</span><span class="sxs-lookup"><span data-stu-id="d0527-120">Name</span></span>       | <span data-ttu-id="d0527-121">说明</span><span class="sxs-lookup"><span data-stu-id="d0527-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d0527-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0527-122">Authorization</span></span>  | <span data-ttu-id="d0527-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0527-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0527-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0527-125">Content-Type</span></span>  | <span data-ttu-id="d0527-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d0527-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0527-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0527-127">Request body</span></span>

<span data-ttu-id="d0527-128">在请求正文中, 提供要更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="d0527-128">In the request body, supply the values for relevant fields to be updated.</span></span> <span data-ttu-id="d0527-129">未包含在请求正文中的现有属性将保留其以前的值, 或根据对其他属性值的更改重新计算这些属性。</span><span class="sxs-lookup"><span data-stu-id="d0527-129">Existing properties not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="d0527-130">为了获得最佳性能, 仅包含更改的值。</span><span class="sxs-lookup"><span data-stu-id="d0527-130">For best performance, only include changed values.</span></span>

## <a name="response"></a><span data-ttu-id="d0527-131">响应</span><span class="sxs-lookup"><span data-stu-id="d0527-131">Response</span></span>

<span data-ttu-id="d0527-132">如果成功, 此方法将`204 No Content`返回响应代码, 不返回任何响应正文。</span><span class="sxs-lookup"><span data-stu-id="d0527-132">If successful, this method returns a `204 No Content` response code and no response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0527-133">示例</span><span class="sxs-lookup"><span data-stu-id="d0527-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0527-134">请求</span><span class="sxs-lookup"><span data-stu-id="d0527-134">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d0527-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d0527-135">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="d0527-136">C#</span><span class="sxs-lookup"><span data-stu-id="d0527-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0527-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0527-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d0527-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="d0527-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d0527-139">Java</span><span class="sxs-lookup"><span data-stu-id="d0527-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d0527-140">响应</span><span class="sxs-lookup"><span data-stu-id="d0527-140">Response</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "Update domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
