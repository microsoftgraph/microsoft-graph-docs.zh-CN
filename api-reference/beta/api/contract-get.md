---
title: 获取合同
description: 检索 contract 对象的属性和关系。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 99de2eafa59008b6d3ea75c544aa5a1c3ca6c25c
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417884"
---
# <a name="get-contract"></a><span data-ttu-id="c4dde-103">获取合同</span><span class="sxs-lookup"><span data-stu-id="c4dde-103">Get Contract</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4dde-104">检索[contract](../resources/contract.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c4dde-104">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c4dde-105">权限</span><span class="sxs-lookup"><span data-stu-id="c4dde-105">Permissions</span></span>

<span data-ttu-id="c4dde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c4dde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="c4dde-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c4dde-108">Permission type</span></span>      | <span data-ttu-id="c4dde-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c4dde-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c4dde-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c4dde-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c4dde-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c4dde-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c4dde-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c4dde-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c4dde-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c4dde-113">Not supported.</span></span>    |
|<span data-ttu-id="c4dde-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c4dde-114">Application</span></span> | <span data-ttu-id="c4dde-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c4dde-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c4dde-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c4dde-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c4dde-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c4dde-117">Optional query parameters</span></span>

<span data-ttu-id="c4dde-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c4dde-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c4dde-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c4dde-119">Request headers</span></span>

| <span data-ttu-id="c4dde-120">名称</span><span class="sxs-lookup"><span data-stu-id="c4dde-120">Name</span></span>      |<span data-ttu-id="c4dde-121">说明</span><span class="sxs-lookup"><span data-stu-id="c4dde-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c4dde-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c4dde-122">Authorization</span></span>  | <span data-ttu-id="c4dde-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c4dde-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c4dde-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c4dde-125">Request body</span></span>

<span data-ttu-id="c4dde-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c4dde-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c4dde-127">响应</span><span class="sxs-lookup"><span data-stu-id="c4dde-127">Response</span></span>

<span data-ttu-id="c4dde-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[Contract](../resources/contract.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c4dde-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c4dde-129">示例</span><span class="sxs-lookup"><span data-stu-id="c4dde-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c4dde-130">请求</span><span class="sxs-lookup"><span data-stu-id="c4dde-130">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c4dde-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c4dde-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```http
GET https://graph.microsoft.com/beta/contracts/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c4dde-132">C#</span><span class="sxs-lookup"><span data-stu-id="c4dde-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c4dde-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c4dde-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c4dde-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="c4dde-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="c4dde-135">响应</span><span class="sxs-lookup"><span data-stu-id="c4dde-135">Response</span></span>
<span data-ttu-id="c4dde-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c4dde-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.Contract"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 186

{
  "contractType": "contractType-value",
  "customerId": "customerId-value",
  "defaultDomainName": "defaultDomainName-value",
  "displayName": "displayName-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
