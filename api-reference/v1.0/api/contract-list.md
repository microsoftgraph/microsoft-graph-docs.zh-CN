---
title: 列出合同
description: 检索与合作伙伴租户关联的合同对象列表。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: da5c6e1d6e4b3bffc6be502eb901ed4ada1c1a9f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50434718"
---
# <a name="list-contracts"></a><span data-ttu-id="f0ed4-103">列出合同</span><span class="sxs-lookup"><span data-stu-id="f0ed4-103">List contracts</span></span>

<span data-ttu-id="f0ed4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0ed4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f0ed4-105">检索与 [合作伙伴](../resources/contract.md) 租户关联的合同对象列表。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-105">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="f0ed4-106">权限</span><span class="sxs-lookup"><span data-stu-id="f0ed4-106">Permissions</span></span>

<span data-ttu-id="f0ed4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f0ed4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0ed4-109">Permission type</span></span>      | <span data-ttu-id="f0ed4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f0ed4-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f0ed4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0ed4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f0ed4-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f0ed4-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f0ed4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0ed4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f0ed4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-114">Not supported.</span></span>    |
|<span data-ttu-id="f0ed4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0ed4-115">Application</span></span> | <span data-ttu-id="f0ed4-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0ed4-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f0ed4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0ed4-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f0ed4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f0ed4-118">Optional query parameters</span></span>

<span data-ttu-id="f0ed4-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span> 

> <span data-ttu-id="f0ed4-120">customerId、defaultDomainName 和 displayName 支持筛选。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-120">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f0ed4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0ed4-121">Request headers</span></span>

| <span data-ttu-id="f0ed4-122">名称</span><span class="sxs-lookup"><span data-stu-id="f0ed4-122">Name</span></span>      |<span data-ttu-id="f0ed4-123">说明</span><span class="sxs-lookup"><span data-stu-id="f0ed4-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f0ed4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0ed4-124">Authorization</span></span>  | <span data-ttu-id="f0ed4-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f0ed4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0ed4-127">Request body</span></span>

<span data-ttu-id="f0ed4-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f0ed4-129">响应</span><span class="sxs-lookup"><span data-stu-id="f0ed4-129">Response</span></span>

<span data-ttu-id="f0ed4-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [Contract](../resources/contract.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-130">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0ed4-131">示例</span><span class="sxs-lookup"><span data-stu-id="f0ed4-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f0ed4-132">请求</span><span class="sxs-lookup"><span data-stu-id="f0ed4-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f0ed4-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f0ed4-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts
```
# <a name="c"></a>[<span data-ttu-id="f0ed4-134">C#</span><span class="sxs-lookup"><span data-stu-id="f0ed4-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f0ed4-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f0ed4-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f0ed4-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f0ed4-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f0ed4-137">Java</span><span class="sxs-lookup"><span data-stu-id="f0ed4-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f0ed4-138">响应</span><span class="sxs-lookup"><span data-stu-id="f0ed4-138">Response</span></span>

<span data-ttu-id="f0ed4-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0ed4-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
    {
      "contractType": "contractType-value",
      "customerId": "customerId-value",
      "defaultDomainName": "defaultDomainName-value",
      "displayName": "displayName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
