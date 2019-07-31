---
title: 域：验证
description: 验证域的所有权。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 35117ca704e369466dc05d66d7501994f340c0eb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35957358"
---
# <a name="domain-verify"></a><span data-ttu-id="23c7b-103">域：验证</span><span class="sxs-lookup"><span data-stu-id="23c7b-103">domain: verify</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="23c7b-104">验证域的所有权。</span><span class="sxs-lookup"><span data-stu-id="23c7b-104">Validates the ownership of the domain.</span></span>

> <span data-ttu-id="23c7b-p101">**重要说明：** 仅适用于未验证的域。对于未验证的域，[域](../resources/domain.md)的 isVerified 属性为 false。</span><span class="sxs-lookup"><span data-stu-id="23c7b-p101">**Important:** Only applies to an unverified domain. For an unverified domain, the isVerified property of the [domain](../resources/domain.md) is false.</span></span>

## <a name="permissions"></a><span data-ttu-id="23c7b-107">权限</span><span class="sxs-lookup"><span data-stu-id="23c7b-107">Permissions</span></span>

<span data-ttu-id="23c7b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="23c7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="23c7b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="23c7b-110">Permission type</span></span>      | <span data-ttu-id="23c7b-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="23c7b-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="23c7b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23c7b-112">Delegated (work or school account)</span></span> | <span data-ttu-id="23c7b-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="23c7b-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="23c7b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23c7b-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="23c7b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="23c7b-115">Not supported.</span></span>    |
|<span data-ttu-id="23c7b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="23c7b-116">Application</span></span> | <span data-ttu-id="23c7b-117">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="23c7b-117">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="23c7b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23c7b-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains/{id}/verify
```

> <span data-ttu-id="23c7b-119">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="23c7b-119">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="request-headers"></a><span data-ttu-id="23c7b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="23c7b-120">Request headers</span></span>

| <span data-ttu-id="23c7b-121">名称</span><span class="sxs-lookup"><span data-stu-id="23c7b-121">Name</span></span>       | <span data-ttu-id="23c7b-122">说明</span><span class="sxs-lookup"><span data-stu-id="23c7b-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="23c7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="23c7b-123">Authorization</span></span>  | <span data-ttu-id="23c7b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="23c7b-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="23c7b-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="23c7b-126">Content-Type</span></span>  | <span data-ttu-id="23c7b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="23c7b-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="23c7b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="23c7b-128">Request body</span></span>

## <a name="response"></a><span data-ttu-id="23c7b-129">响应</span><span class="sxs-lookup"><span data-stu-id="23c7b-129">Response</span></span>

<span data-ttu-id="23c7b-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23c7b-130">If successful, this method returns `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23c7b-131">示例</span><span class="sxs-lookup"><span data-stu-id="23c7b-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="23c7b-132">请求</span><span class="sxs-lookup"><span data-stu-id="23c7b-132">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="23c7b-133">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="23c7b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "domain_verify"
}-->
```http
POST https://graph.microsoft.com/beta/domains/contoso.com/verify
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="23c7b-134">C#</span><span class="sxs-lookup"><span data-stu-id="23c7b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/domain-verify-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="23c7b-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="23c7b-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/domain-verify-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="23c7b-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="23c7b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/domain-verify-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="23c7b-137">Java</span><span class="sxs-lookup"><span data-stu-id="23c7b-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/domain-verify-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="23c7b-138">响应</span><span class="sxs-lookup"><span data-stu-id="23c7b-138">Response</span></span>
<span data-ttu-id="23c7b-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23c7b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
