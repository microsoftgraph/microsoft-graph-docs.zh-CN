---
title: 获取合同
description: 检索 contract 对象的属性和关系。
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 65583a3db22eb5ae85c4a4432fdfb10644143f89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50963915"
---
# <a name="get-contract"></a><span data-ttu-id="f6c8a-103">获取合同</span><span class="sxs-lookup"><span data-stu-id="f6c8a-103">Get Contract</span></span>

<span data-ttu-id="f6c8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6c8a-105">检索 contract 对象 [的属性和](../resources/contract.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="f6c8a-105">Retrieve the properties and relationships of [contract](../resources/contract.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6c8a-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6c8a-106">Permissions</span></span>

<span data-ttu-id="f6c8a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6c8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f6c8a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6c8a-109">Permission type</span></span>      | <span data-ttu-id="f6c8a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f6c8a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f6c8a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c8a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f6c8a-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f6c8a-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f6c8a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6c8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f6c8a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6c8a-114">Not supported.</span></span>    |
|<span data-ttu-id="f6c8a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6c8a-115">Application</span></span> | <span data-ttu-id="f6c8a-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6c8a-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f6c8a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6c8a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /contracts/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f6c8a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f6c8a-118">Optional query parameters</span></span>

<span data-ttu-id="f6c8a-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f6c8a-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6c8a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6c8a-120">Request headers</span></span>

| <span data-ttu-id="f6c8a-121">名称</span><span class="sxs-lookup"><span data-stu-id="f6c8a-121">Name</span></span>      |<span data-ttu-id="f6c8a-122">说明</span><span class="sxs-lookup"><span data-stu-id="f6c8a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6c8a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6c8a-123">Authorization</span></span>  | <span data-ttu-id="f6c8a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f6c8a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6c8a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6c8a-126">Request body</span></span>

<span data-ttu-id="f6c8a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6c8a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6c8a-128">响应</span><span class="sxs-lookup"><span data-stu-id="f6c8a-128">Response</span></span>

<span data-ttu-id="f6c8a-129">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/contract.md) 代码和 Contract 对象。</span><span class="sxs-lookup"><span data-stu-id="f6c8a-129">If successful, this method returns a `200 OK` response code and [Contract](../resources/contract.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6c8a-130">示例</span><span class="sxs-lookup"><span data-stu-id="f6c8a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6c8a-131">请求</span><span class="sxs-lookup"><span data-stu-id="f6c8a-131">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f6c8a-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f6c8a-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_contract_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/contracts/{id}
```
# <a name="c"></a>[<span data-ttu-id="f6c8a-133">C#</span><span class="sxs-lookup"><span data-stu-id="f6c8a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-contract-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f6c8a-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f6c8a-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-contract-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f6c8a-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f6c8a-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-contract-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f6c8a-136">Java</span><span class="sxs-lookup"><span data-stu-id="f6c8a-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-contract-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f6c8a-137">响应</span><span class="sxs-lookup"><span data-stu-id="f6c8a-137">Response</span></span>
<span data-ttu-id="f6c8a-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6c8a-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
