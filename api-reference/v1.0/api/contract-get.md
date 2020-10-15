---
title: 获取合同
description: 检索 contract 对象的属性和关系。
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 71622ab33eff6183694b90d65c3a6f84e3da238c
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48459220"
---
# <a name="get-contract"></a><span data-ttu-id="ed2a3-103">获取合同</span><span class="sxs-lookup"><span data-stu-id="ed2a3-103">Get Contract</span></span>

<span data-ttu-id="ed2a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed2a3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ed2a3-105">检索 [contract](../resources/contract.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ed2a3-105">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed2a3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="ed2a3-106">Permissions</span></span>

<span data-ttu-id="ed2a3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed2a3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ed2a3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed2a3-109">Permission type</span></span>      | <span data-ttu-id="ed2a3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed2a3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ed2a3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed2a3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ed2a3-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ed2a3-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ed2a3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed2a3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ed2a3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed2a3-114">Not supported.</span></span>    |
|<span data-ttu-id="ed2a3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed2a3-115">Application</span></span> | <span data-ttu-id="ed2a3-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed2a3-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ed2a3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed2a3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed2a3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed2a3-118">Optional query parameters</span></span>

<span data-ttu-id="ed2a3-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ed2a3-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed2a3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed2a3-120">Request headers</span></span>

| <span data-ttu-id="ed2a3-121">名称</span><span class="sxs-lookup"><span data-stu-id="ed2a3-121">Name</span></span>      |<span data-ttu-id="ed2a3-122">说明</span><span class="sxs-lookup"><span data-stu-id="ed2a3-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ed2a3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed2a3-123">Authorization</span></span>  | <span data-ttu-id="ed2a3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed2a3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ed2a3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed2a3-126">Request body</span></span>

<span data-ttu-id="ed2a3-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed2a3-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed2a3-128">响应</span><span class="sxs-lookup"><span data-stu-id="ed2a3-128">Response</span></span>

<span data-ttu-id="ed2a3-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [Contract](../resources/contract.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ed2a3-129">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ed2a3-130">示例</span><span class="sxs-lookup"><span data-stu-id="ed2a3-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed2a3-131">请求</span><span class="sxs-lookup"><span data-stu-id="ed2a3-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="ed2a3-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="ed2a3-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts/{id}
```
# <a name="c"></a>[<span data-ttu-id="ed2a3-133">C#</span><span class="sxs-lookup"><span data-stu-id="ed2a3-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ed2a3-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ed2a3-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ed2a3-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ed2a3-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ed2a3-136">Java</span><span class="sxs-lookup"><span data-stu-id="ed2a3-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ed2a3-137">响应</span><span class="sxs-lookup"><span data-stu-id="ed2a3-137">Response</span></span>
<span data-ttu-id="ed2a3-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ed2a3-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.contract"
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
<!-- {
  "type": "#page.annotation",
  "description": "Get Contract",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
