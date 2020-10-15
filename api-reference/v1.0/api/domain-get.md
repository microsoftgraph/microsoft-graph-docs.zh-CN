---
title: 获取域
description: 检索 domain 对象的属性和关系。
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cf7557ecf9ff34cf0746f4267aa8461e277a9004
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48457763"
---
# <a name="get-domain"></a><span data-ttu-id="4d195-103">获取域</span><span class="sxs-lookup"><span data-stu-id="4d195-103">Get domain</span></span>

<span data-ttu-id="4d195-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4d195-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4d195-105">检索 domain 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4d195-105">Retrieve the properties and relationships of domain object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4d195-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4d195-106">Permissions</span></span>

<span data-ttu-id="4d195-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4d195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="4d195-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4d195-109">Permission type</span></span>      | <span data-ttu-id="4d195-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4d195-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4d195-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4d195-111">Delegated (work or school account)</span></span> | <span data-ttu-id="4d195-112">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="4d195-112">Directory.Read.All</span></span>    |
|<span data-ttu-id="4d195-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4d195-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4d195-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4d195-114">Not supported.</span></span>    |
|<span data-ttu-id="4d195-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4d195-115">Application</span></span> | <span data-ttu-id="4d195-116">Directory.Read.All、Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4d195-116">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4d195-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4d195-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}
```

> <span data-ttu-id="4d195-118">对于 {id}，请使用其完全限定的域名指定该域。</span><span class="sxs-lookup"><span data-stu-id="4d195-118">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="4d195-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4d195-119">Optional query parameters</span></span>

<span data-ttu-id="4d195-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4d195-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4d195-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4d195-121">Request headers</span></span>

| <span data-ttu-id="4d195-122">名称</span><span class="sxs-lookup"><span data-stu-id="4d195-122">Name</span></span>      |<span data-ttu-id="4d195-123">说明</span><span class="sxs-lookup"><span data-stu-id="4d195-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="4d195-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4d195-124">Authorization</span></span>  | <span data-ttu-id="4d195-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4d195-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="4d195-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4d195-127">Content-Type</span></span>  | <span data-ttu-id="4d195-128">application/json</span><span class="sxs-lookup"><span data-stu-id="4d195-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4d195-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="4d195-129">Request body</span></span>
<span data-ttu-id="4d195-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4d195-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4d195-131">响应</span><span class="sxs-lookup"><span data-stu-id="4d195-131">Response</span></span>

<span data-ttu-id="4d195-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [domain](../resources/domain.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4d195-132">If successful, this method returns a `200 OK` response code and [domain](../resources/domain.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4d195-133">示例</span><span class="sxs-lookup"><span data-stu-id="4d195-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4d195-134">请求</span><span class="sxs-lookup"><span data-stu-id="4d195-134">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4d195-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="4d195-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "sampleKeys": ["contoso.com"],
  "name": "get_domain"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/domains/contoso.com
```
# <a name="c"></a>[<span data-ttu-id="4d195-136">C#</span><span class="sxs-lookup"><span data-stu-id="4d195-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-domain-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4d195-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4d195-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-domain-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4d195-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4d195-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-domain-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4d195-139">Java</span><span class="sxs-lookup"><span data-stu-id="4d195-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-domain-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4d195-140">响应</span><span class="sxs-lookup"><span data-stu-id="4d195-140">Response</span></span>
<span data-ttu-id="4d195-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4d195-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
