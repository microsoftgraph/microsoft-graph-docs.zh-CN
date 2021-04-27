---
title: 获取 accessPackage
description: 检索 accessPackage 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 192ddb37ef7b6ab1372d7504d1785299cbcf0e86
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52038661"
---
# <a name="get-accesspackage"></a><span data-ttu-id="5c8b4-103">获取 accessPackage</span><span class="sxs-lookup"><span data-stu-id="5c8b4-103">Get accessPackage</span></span>

<span data-ttu-id="5c8b4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5c8b4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5c8b4-105">检索 [accessPackage](../resources/accesspackage.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-105">Retrieve the properties and relationships of an [accessPackage](../resources/accesspackage.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5c8b4-106">权限</span><span class="sxs-lookup"><span data-stu-id="5c8b4-106">Permissions</span></span>

<span data-ttu-id="5c8b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5c8b4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c8b4-109">Permission type</span></span>                        | <span data-ttu-id="5c8b4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5c8b4-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5c8b4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c8b4-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5c8b4-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c8b4-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5c8b4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c8b4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5c8b4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-114">Not supported.</span></span> |
| <span data-ttu-id="5c8b4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c8b4-115">Application</span></span>                            | <span data-ttu-id="5c8b4-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c8b4-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="5c8b4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c8b4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackages/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5c8b4-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5c8b4-118">Optional query parameters</span></span>

<span data-ttu-id="5c8b4-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5c8b4-120">例如，若要检索访问包策略，请添加 `$expand=accessPackageAssignmentPolicies` 。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-120">For example, to retrieve the access package policies, add `$expand=accessPackageAssignmentPolicies`.</span></span> <span data-ttu-id="5c8b4-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5c8b4-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c8b4-122">Request headers</span></span>

| <span data-ttu-id="5c8b4-123">名称</span><span class="sxs-lookup"><span data-stu-id="5c8b4-123">Name</span></span>      |<span data-ttu-id="5c8b4-124">说明</span><span class="sxs-lookup"><span data-stu-id="5c8b4-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5c8b4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c8b4-125">Authorization</span></span> | <span data-ttu-id="5c8b4-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5c8b4-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c8b4-128">Request body</span></span>

<span data-ttu-id="5c8b4-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5c8b4-130">响应</span><span class="sxs-lookup"><span data-stu-id="5c8b4-130">Response</span></span>

<span data-ttu-id="5c8b4-131">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [accessPackage](../resources/accesspackage.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-131">If successful, this method returns a `200 OK` response code and the requested [accessPackage](../resources/accesspackage.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5c8b4-132">示例</span><span class="sxs-lookup"><span data-stu-id="5c8b4-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5c8b4-133">请求</span><span class="sxs-lookup"><span data-stu-id="5c8b4-133">Request</span></span>

<span data-ttu-id="5c8b4-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5c8b4-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="5c8b4-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackage"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackages/{id}
```
# <a name="c"></a>[<span data-ttu-id="5c8b4-136">C#</span><span class="sxs-lookup"><span data-stu-id="5c8b4-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackage-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5c8b4-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5c8b4-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackage-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5c8b4-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5c8b4-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackage-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5c8b4-139">Java</span><span class="sxs-lookup"><span data-stu-id="5c8b4-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackage-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5c8b4-140">响应</span><span class="sxs-lookup"><span data-stu-id="5c8b4-140">Response</span></span>

<span data-ttu-id="5c8b4-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-141">The following is an example of the response.</span></span>

> <span data-ttu-id="5c8b4-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5c8b4-142">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackage"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package",
    "displayName":"Access package for testing",
    "isHidden":false,
    "catalogId":"662d99e7-6ceb-4c21-9cb4-9b0bbfdefccc",
    "isRoleScopesVisible":false,
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackage",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


