---
title: 获取域
description: 检索 domain 对象的属性和关系。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: d2b777a59118160cddef98f9b2f1fbf3c7a0855c
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135221"
---
# <a name="get-domain"></a><span data-ttu-id="fe87a-103">获取域</span><span class="sxs-lookup"><span data-stu-id="fe87a-103">Get domain</span></span>

<span data-ttu-id="fe87a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe87a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe87a-105">检索 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe87a-105">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe87a-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fe87a-106">Permissions</span></span>

<span data-ttu-id="fe87a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe87a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fe87a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe87a-109">Permission type</span></span>      | <span data-ttu-id="fe87a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe87a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe87a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe87a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fe87a-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe87a-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="fe87a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe87a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe87a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe87a-114">Not supported.</span></span>    |
|<span data-ttu-id="fe87a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe87a-115">Application</span></span> | <span data-ttu-id="fe87a-116">Domain.Read.All、Domain.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe87a-116">Domain.Read.All, Domain.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe87a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe87a-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="fe87a-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="fe87a-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="fe87a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fe87a-119">Optional query parameters</span></span>

<span data-ttu-id="fe87a-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fe87a-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe87a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe87a-121">Request headers</span></span>

| <span data-ttu-id="fe87a-122">名称</span><span class="sxs-lookup"><span data-stu-id="fe87a-122">Name</span></span>      |<span data-ttu-id="fe87a-123">说明</span><span class="sxs-lookup"><span data-stu-id="fe87a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fe87a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe87a-124">Authorization</span></span>  | <span data-ttu-id="fe87a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe87a-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="fe87a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fe87a-127">Content-Type</span></span>  | <span data-ttu-id="fe87a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fe87a-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="fe87a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe87a-129">Request body</span></span>
<span data-ttu-id="fe87a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe87a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe87a-131">响应</span><span class="sxs-lookup"><span data-stu-id="fe87a-131">Response</span></span>

<span data-ttu-id="fe87a-132">如果成功，此方法在响应 `200 OK` 正文中返回响应[](../resources/domain.md)代码和域对象。</span><span class="sxs-lookup"><span data-stu-id="fe87a-132">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fe87a-133">示例</span><span class="sxs-lookup"><span data-stu-id="fe87a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe87a-134">请求</span><span class="sxs-lookup"><span data-stu-id="fe87a-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fe87a-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe87a-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="fe87a-136">C#</span><span class="sxs-lookup"><span data-stu-id="fe87a-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe87a-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe87a-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe87a-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe87a-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe87a-139">Java</span><span class="sxs-lookup"><span data-stu-id="fe87a-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="fe87a-140">响应</span><span class="sxs-lookup"><span data-stu-id="fe87a-140">Response</span></span>
<span data-ttu-id="fe87a-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fe87a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Get domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
