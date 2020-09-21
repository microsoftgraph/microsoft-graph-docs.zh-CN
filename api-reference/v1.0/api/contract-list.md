---
title: 列出合同
description: 检索与合作伙伴租户关联的合同对象的列表。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1876ce76ffde8750a268ae1fed769a7b8ab7658e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010052"
---
# <a name="list-contracts"></a><span data-ttu-id="33697-103">列出合同</span><span class="sxs-lookup"><span data-stu-id="33697-103">List contracts</span></span>

<span data-ttu-id="33697-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="33697-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="33697-105">检索与合作伙伴租户关联的 [合同](../resources/contract.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="33697-105">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="33697-106">权限</span><span class="sxs-lookup"><span data-stu-id="33697-106">Permissions</span></span>

<span data-ttu-id="33697-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="33697-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="33697-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="33697-109">Permission type</span></span>      | <span data-ttu-id="33697-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="33697-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="33697-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33697-111">Delegated (work or school account)</span></span> | <span data-ttu-id="33697-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="33697-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="33697-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33697-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="33697-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="33697-114">Not supported.</span></span>    |
|<span data-ttu-id="33697-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="33697-115">Application</span></span> | <span data-ttu-id="33697-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33697-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="33697-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33697-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="33697-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="33697-118">Optional query parameters</span></span>

<span data-ttu-id="33697-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="33697-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="33697-120">对 customerId、defaultDomainName 和 displayName 支持筛选。</span><span class="sxs-lookup"><span data-stu-id="33697-120">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="33697-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="33697-121">Request headers</span></span>

| <span data-ttu-id="33697-122">名称</span><span class="sxs-lookup"><span data-stu-id="33697-122">Name</span></span>      |<span data-ttu-id="33697-123">说明</span><span class="sxs-lookup"><span data-stu-id="33697-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="33697-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="33697-124">Authorization</span></span>  | <span data-ttu-id="33697-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="33697-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="33697-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="33697-127">Request body</span></span>

<span data-ttu-id="33697-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="33697-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="33697-129">响应</span><span class="sxs-lookup"><span data-stu-id="33697-129">Response</span></span>

<span data-ttu-id="33697-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [Contract](../resources/contract.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="33697-130">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33697-131">示例</span><span class="sxs-lookup"><span data-stu-id="33697-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="33697-132">请求</span><span class="sxs-lookup"><span data-stu-id="33697-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="33697-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="33697-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts
```
# <a name="c"></a>[<span data-ttu-id="33697-134">C#</span><span class="sxs-lookup"><span data-stu-id="33697-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="33697-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="33697-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="33697-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="33697-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="33697-137">Java</span><span class="sxs-lookup"><span data-stu-id="33697-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="33697-138">响应</span><span class="sxs-lookup"><span data-stu-id="33697-138">Response</span></span>

<span data-ttu-id="33697-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33697-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

