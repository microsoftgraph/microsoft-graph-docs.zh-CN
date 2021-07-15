---
title: 列出 accessPackagesIncompatibleWith
description: 检索指示其访问权限与特定访问包不兼容的 accesspackages 列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: def48d58dbbc757c6a248fe8dac40adff9372320
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53439199"
---
# <a name="list-accesspackagesincompatiblewith"></a><span data-ttu-id="639b6-103">列出 accessPackagesIncompatibleWith</span><span class="sxs-lookup"><span data-stu-id="639b6-103">List accessPackagesIncompatibleWith</span></span>

<span data-ttu-id="639b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="639b6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="639b6-105">检索将 [指定 accessPackage](../resources/accesspackage.md) 标记为不兼容的 [accessPackage 对象](../resources/accesspackage.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="639b6-105">Retrieve a list of the [accessPackage](../resources/accesspackage.md) objects that have marked a specified [accessPackage](../resources/accesspackage.md) as incompatible.</span></span>

## <a name="permissions"></a><span data-ttu-id="639b6-106">权限</span><span class="sxs-lookup"><span data-stu-id="639b6-106">Permissions</span></span>

<span data-ttu-id="639b6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="639b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="639b6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="639b6-109">Permission type</span></span>                        | <span data-ttu-id="639b6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="639b6-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="639b6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="639b6-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="639b6-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="639b6-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="639b6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="639b6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="639b6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="639b6-114">Not supported.</span></span> |
| <span data-ttu-id="639b6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="639b6-115">Application</span></span>                            | <span data-ttu-id="639b6-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="639b6-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="639b6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="639b6-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/accessPackagesIncompatibleWith
```

## <a name="optional-query-parameters"></a><span data-ttu-id="639b6-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="639b6-118">Optional query parameters</span></span>

<span data-ttu-id="639b6-119">此方法支持通过大型响应对服务器端分页使用 OData 查询参数。</span><span class="sxs-lookup"><span data-stu-id="639b6-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="639b6-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="639b6-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="639b6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="639b6-121">Request headers</span></span>

| <span data-ttu-id="639b6-122">名称</span><span class="sxs-lookup"><span data-stu-id="639b6-122">Name</span></span>      |<span data-ttu-id="639b6-123">说明</span><span class="sxs-lookup"><span data-stu-id="639b6-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="639b6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="639b6-124">Authorization</span></span> | <span data-ttu-id="639b6-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="639b6-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="639b6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="639b6-127">Request body</span></span>

<span data-ttu-id="639b6-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="639b6-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="639b6-129">响应</span><span class="sxs-lookup"><span data-stu-id="639b6-129">Response</span></span>

<span data-ttu-id="639b6-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackage](../resources/accesspackage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="639b6-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="639b6-131">示例</span><span class="sxs-lookup"><span data-stu-id="639b6-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="639b6-132">请求</span><span class="sxs-lookup"><span data-stu-id="639b6-132">Request</span></span>

<span data-ttu-id="639b6-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="639b6-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="639b6-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="639b6-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackagesincompatiblewith"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/accessPackagesIncompatibleWith
```
# <a name="c"></a>[<span data-ttu-id="639b6-135">C#</span><span class="sxs-lookup"><span data-stu-id="639b6-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackagesincompatiblewith-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="639b6-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="639b6-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackagesincompatiblewith-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="639b6-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="639b6-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackagesincompatiblewith-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="639b6-138">Java</span><span class="sxs-lookup"><span data-stu-id="639b6-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackagesincompatiblewith-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="639b6-139">响应</span><span class="sxs-lookup"><span data-stu-id="639b6-139">Response</span></span>

<span data-ttu-id="639b6-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="639b6-140">The following is an example of the response.</span></span>

> <span data-ttu-id="639b6-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="639b6-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "c0a74b4d-2694-4d5d-a964-1bee4ff0aaf2",
      "catalogId": "c955f54f-e248-4155-b314-0bdd63f5aae9",
      "displayName": "accesspackage"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackagesIncompatibleWith",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


