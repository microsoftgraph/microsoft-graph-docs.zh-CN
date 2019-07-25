---
title: 获取域
description: 检索 domain 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 285c938816f2b0d0f76bcc9207ae6ab07333cf44
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861937"
---
# <a name="get-domain"></a><span data-ttu-id="d2622-103">获取域</span><span class="sxs-lookup"><span data-stu-id="d2622-103">Get domain</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d2622-104">检索 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d2622-104">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="d2622-105">权限</span><span class="sxs-lookup"><span data-stu-id="d2622-105">Permissions</span></span>

<span data-ttu-id="d2622-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d2622-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d2622-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d2622-108">Permission type</span></span>      | <span data-ttu-id="d2622-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d2622-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d2622-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d2622-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d2622-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2622-111">Directory.Read.All</span></span>    |
|<span data-ttu-id="d2622-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d2622-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d2622-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d2622-113">Not supported.</span></span>    |
|<span data-ttu-id="d2622-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d2622-114">Application</span></span> | <span data-ttu-id="d2622-115">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d2622-115">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d2622-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d2622-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="d2622-117">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="d2622-117">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="d2622-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d2622-118">Optional query parameters</span></span>

<span data-ttu-id="d2622-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d2622-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2622-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d2622-120">Request headers</span></span>

| <span data-ttu-id="d2622-121">名称</span><span class="sxs-lookup"><span data-stu-id="d2622-121">Name</span></span>      |<span data-ttu-id="d2622-122">说明</span><span class="sxs-lookup"><span data-stu-id="d2622-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d2622-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2622-123">Authorization</span></span>  | <span data-ttu-id="d2622-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d2622-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d2622-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d2622-126">Content-Type</span></span>  | <span data-ttu-id="d2622-127">application/json</span><span class="sxs-lookup"><span data-stu-id="d2622-127">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d2622-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d2622-128">Request body</span></span>
<span data-ttu-id="d2622-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d2622-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2622-130">响应</span><span class="sxs-lookup"><span data-stu-id="d2622-130">Response</span></span>

<span data-ttu-id="d2622-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[domain](../resources/domain.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d2622-131">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d2622-132">示例</span><span class="sxs-lookup"><span data-stu-id="d2622-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d2622-133">请求</span><span class="sxs-lookup"><span data-stu-id="d2622-133">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="d2622-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d2622-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```http
GET https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d2622-135">C#</span><span class="sxs-lookup"><span data-stu-id="d2622-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d2622-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d2622-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d2622-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="d2622-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="d2622-138">Java</span><span class="sxs-lookup"><span data-stu-id="d2622-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d2622-139">响应</span><span class="sxs-lookup"><span data-stu-id="d2622-139">Response</span></span>
<span data-ttu-id="d2622-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d2622-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
