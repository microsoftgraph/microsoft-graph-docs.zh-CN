---
title: 列出 incompatibleAccessPackages
description: 检索其访问权限与特定访问包不兼容的 accesspackages 列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: fc30ee9ae6a80b04820b363dea87f376e5db638b
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401064"
---
# <a name="list-incompatibleaccesspackages"></a><span data-ttu-id="3ece3-103">列出 incompatibleAccessPackages</span><span class="sxs-lookup"><span data-stu-id="3ece3-103">List incompatibleAccessPackages</span></span>

<span data-ttu-id="3ece3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ece3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ece3-105">检索 [accessPackage](../resources/accesspackage.md) 对象的列表，这些对象已在 [accessPackage](../resources/accesspackage.md)上标记为不兼容。</span><span class="sxs-lookup"><span data-stu-id="3ece3-105">Retrieve a list of the [accessPackage](../resources/accesspackage.md) objects that have been marked as incompatible on an [accessPackage](../resources/accesspackage.md).</span></span>  

## <a name="permissions"></a><span data-ttu-id="3ece3-106">权限</span><span class="sxs-lookup"><span data-stu-id="3ece3-106">Permissions</span></span>

<span data-ttu-id="3ece3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ece3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ece3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ece3-109">Permission type</span></span>                        | <span data-ttu-id="3ece3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ece3-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ece3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ece3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ece3-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ece3-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3ece3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ece3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ece3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ece3-114">Not supported.</span></span> |
| <span data-ttu-id="3ece3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ece3-115">Application</span></span>                            | <span data-ttu-id="3ece3-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ece3-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ece3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ece3-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackage/{id}/incompatibleAccessPackages
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ece3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3ece3-118">Optional query parameters</span></span>

<span data-ttu-id="3ece3-119">此方法支持通过大型响应对服务器端分页使用 OData 查询参数。</span><span class="sxs-lookup"><span data-stu-id="3ece3-119">This method supports the OData query parameters for server-side paging through a large response.</span></span> <span data-ttu-id="3ece3-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3ece3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ece3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ece3-121">Request headers</span></span>

| <span data-ttu-id="3ece3-122">名称</span><span class="sxs-lookup"><span data-stu-id="3ece3-122">Name</span></span>      |<span data-ttu-id="3ece3-123">说明</span><span class="sxs-lookup"><span data-stu-id="3ece3-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ece3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ece3-124">Authorization</span></span> | <span data-ttu-id="3ece3-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="3ece3-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ece3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ece3-127">Request body</span></span>

<span data-ttu-id="3ece3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ece3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ece3-129">响应</span><span class="sxs-lookup"><span data-stu-id="3ece3-129">Response</span></span>

<span data-ttu-id="3ece3-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackage](../resources/accesspackage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3ece3-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackage](../resources/accesspackage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ece3-131">示例</span><span class="sxs-lookup"><span data-stu-id="3ece3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ece3-132">请求</span><span class="sxs-lookup"><span data-stu-id="3ece3-132">Request</span></span>

<span data-ttu-id="3ece3-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3ece3-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_incompatibleaccesspackages"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}/incompatibleAccessPackages
### Response

The following is an example of the response.

> **Note:** The response object shown here might be shortened for readability.

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
  "description": "List incompatibleAccessPackages",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

