---
title: 获取域
description: 检索 domain 对象的属性和关系。
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 2575eefb2ce3585466de3e10fefb71e76859650c
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52046508"
---
# <a name="get-domain"></a><span data-ttu-id="4e7b5-103">获取域</span><span class="sxs-lookup"><span data-stu-id="4e7b5-103">Get domain</span></span>

<span data-ttu-id="4e7b5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4e7b5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4e7b5-105">检索 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-105">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4e7b5-106">权限</span><span class="sxs-lookup"><span data-stu-id="4e7b5-106">Permissions</span></span>

<span data-ttu-id="4e7b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4e7b5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4e7b5-109">Permission type</span></span>      | <span data-ttu-id="4e7b5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4e7b5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4e7b5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4e7b5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4e7b5-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e7b5-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="4e7b5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4e7b5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4e7b5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-114">Not supported.</span></span>    |
|<span data-ttu-id="4e7b5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4e7b5-115">Application</span></span> | <span data-ttu-id="4e7b5-116">Domain.Read.All、Domain.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4e7b5-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4e7b5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4e7b5-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="4e7b5-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="4e7b5-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4e7b5-119">Optional query parameters</span></span>

<span data-ttu-id="4e7b5-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4e7b5-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4e7b5-121">Request headers</span></span>

| <span data-ttu-id="4e7b5-122">名称</span><span class="sxs-lookup"><span data-stu-id="4e7b5-122">Name</span></span>      |<span data-ttu-id="4e7b5-123">说明</span><span class="sxs-lookup"><span data-stu-id="4e7b5-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4e7b5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e7b5-124">Authorization</span></span>  | <span data-ttu-id="4e7b5-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4e7b5-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4e7b5-127">Content-Type</span></span>  | <span data-ttu-id="4e7b5-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4e7b5-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4e7b5-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4e7b5-129">Request body</span></span>
<span data-ttu-id="4e7b5-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4e7b5-131">响应</span><span class="sxs-lookup"><span data-stu-id="4e7b5-131">Response</span></span>

<span data-ttu-id="4e7b5-132">如果成功，此方法在响应 `200 OK` 正文中返回[](../resources/domain.md)响应代码和 domain 对象。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-132">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4e7b5-133">示例</span><span class="sxs-lookup"><span data-stu-id="4e7b5-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4e7b5-134">请求</span><span class="sxs-lookup"><span data-stu-id="4e7b5-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4e7b5-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4e7b5-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="4e7b5-136">C#</span><span class="sxs-lookup"><span data-stu-id="4e7b5-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4e7b5-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4e7b5-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4e7b5-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4e7b5-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4e7b5-139">Java</span><span class="sxs-lookup"><span data-stu-id="4e7b5-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4e7b5-140">响应</span><span class="sxs-lookup"><span data-stu-id="4e7b5-140">Response</span></span>
<span data-ttu-id="4e7b5-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="4e7b5-141">Note: The response object shown here might be shortened for readability.</span></span>
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
