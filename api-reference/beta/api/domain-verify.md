---
title: 域：验证
description: 验证域的所有权。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 32e559328e834f1f1bcce025222556d4b22fab7b
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436440"
---
# <a name="domain-verify"></a><span data-ttu-id="3f542-103">域：验证</span><span class="sxs-lookup"><span data-stu-id="3f542-103">domain: verify</span></span>

<span data-ttu-id="3f542-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f542-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3f542-105">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="3f542-105">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="3f542-p101">**重要说明：** 仅适用于未验证的域。对于未验证的域，[域](../resources/domain.md)的 isVerified 属性为 false。</span><span class="sxs-lookup"><span data-stu-id="3f542-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="3f542-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="3f542-108">Permissions</span></span>

<span data-ttu-id="3f542-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3f542-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="3f542-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f542-111">Permission type</span></span>      | <span data-ttu-id="3f542-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3f542-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3f542-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f542-113">Delegated (work or school account)</span></span> | <span data-ttu-id="3f542-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="3f542-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="3f542-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f542-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3f542-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f542-116">Not supported.</span></span>    |
|<span data-ttu-id="3f542-117">Application</span><span class="sxs-lookup"><span data-stu-id="3f542-117">Application</span></span> | <span data-ttu-id="3f542-118">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f542-118">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3f542-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f542-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="3f542-120">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="3f542-120">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="3f542-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f542-121">Request headers</span></span>

| <span data-ttu-id="3f542-122">名称</span><span class="sxs-lookup"><span data-stu-id="3f542-122">Name</span></span>       | <span data-ttu-id="3f542-123">说明</span><span class="sxs-lookup"><span data-stu-id="3f542-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3f542-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3f542-124">Authorization</span></span>  | <span data-ttu-id="3f542-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3f542-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="3f542-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3f542-127">Content-Type</span></span>  | <span data-ttu-id="3f542-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3f542-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="3f542-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f542-129">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3f542-130">响应</span><span class="sxs-lookup"><span data-stu-id="3f542-130">Response</span></span>

<span data-ttu-id="3f542-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f542-131">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f542-132">示例</span><span class="sxs-lookup"><span data-stu-id="3f542-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3f542-133">请求</span><span class="sxs-lookup"><span data-stu-id="3f542-133">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3f542-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="3f542-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```
# <a name="c"></a>[<span data-ttu-id="3f542-135">C#</span><span class="sxs-lookup"><span data-stu-id="3f542-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-verify-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3f542-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3f542-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-verify-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3f542-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3f542-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-verify-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3f542-138">Java</span><span class="sxs-lookup"><span data-stu-id="3f542-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-verify-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="3f542-139">响应</span><span class="sxs-lookup"><span data-stu-id="3f542-139">Response</span></span>
<span data-ttu-id="3f542-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f542-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true,
  "name": "contoso.com"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domain: verify",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


