---
title: 列出合同
description: 检索与合作伙伴租户关联的合同对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c86fef2272d2294511f7aaa57af1e26dd3e10996
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36372544"
---
# <a name="list-contracts"></a><span data-ttu-id="b5fe9-103">列出合同</span><span class="sxs-lookup"><span data-stu-id="b5fe9-103">List contracts</span></span>

<span data-ttu-id="b5fe9-104">检索与合作伙伴租户关联的[合同](../resources/contract.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-104">Retrieve a list of [contract](../resources/contract.md) objects associated to a partner tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5fe9-105">权限</span><span class="sxs-lookup"><span data-stu-id="b5fe9-105">Permissions</span></span>

<span data-ttu-id="b5fe9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b5fe9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5fe9-108">Permission type</span></span>      | <span data-ttu-id="b5fe9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5fe9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5fe9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5fe9-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b5fe9-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b5fe9-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b5fe9-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5fe9-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5fe9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-113">Not supported.</span></span>    |
|<span data-ttu-id="b5fe9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5fe9-114">Application</span></span> | <span data-ttu-id="b5fe9-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5fe9-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5fe9-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5fe9-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /contracts
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b5fe9-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b5fe9-117">Optional query parameters</span></span>

<span data-ttu-id="b5fe9-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> 

> <span data-ttu-id="b5fe9-119">对 customerId、defaultDomainName 和 displayName 支持筛选。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-119">Filtering is supported for customerId, defaultDomainName, and displayName.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b5fe9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5fe9-120">Request headers</span></span>

| <span data-ttu-id="b5fe9-121">名称</span><span class="sxs-lookup"><span data-stu-id="b5fe9-121">Name</span></span>      |<span data-ttu-id="b5fe9-122">说明</span><span class="sxs-lookup"><span data-stu-id="b5fe9-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b5fe9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5fe9-123">Authorization</span></span>  | <span data-ttu-id="b5fe9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b5fe9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5fe9-126">Request body</span></span>

<span data-ttu-id="b5fe9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5fe9-128">响应</span><span class="sxs-lookup"><span data-stu-id="b5fe9-128">Response</span></span>

<span data-ttu-id="b5fe9-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[Contract](../resources/contract.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-129">If successful, this method returns a `200 OK` response code and a collection of [Contract](../resources/contract.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5fe9-130">示例</span><span class="sxs-lookup"><span data-stu-id="b5fe9-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b5fe9-131">请求</span><span class="sxs-lookup"><span data-stu-id="b5fe9-131">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="b5fe9-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b5fe9-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/v1.0/contracts
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b5fe9-133">C#</span><span class="sxs-lookup"><span data-stu-id="b5fe9-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b5fe9-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b5fe9-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b5fe9-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="b5fe9-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b5fe9-136">Java</span><span class="sxs-lookup"><span data-stu-id="b5fe9-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="b5fe9-137">响应</span><span class="sxs-lookup"><span data-stu-id="b5fe9-137">Response</span></span>

<span data-ttu-id="b5fe9-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5fe9-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
