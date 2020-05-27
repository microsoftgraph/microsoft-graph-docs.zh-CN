---
title: 列出 accessPackageAssignmentRequests
description: 检索 accessPackageAssignmentRequest 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4e73ccbd556ad63cc6adf92e343cdaa9c4c3c4b
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383488"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="e0cd6-103">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="e0cd6-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="e0cd6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0cd6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0cd6-105">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="e0cd6-106">生成的列表包括在所有目录和访问包中，呼叫者有权读取的所有工作分配请求、当前和已过期。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="e0cd6-107">权限</span><span class="sxs-lookup"><span data-stu-id="e0cd6-107">Permissions</span></span>

<span data-ttu-id="e0cd6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e0cd6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0cd6-110">Permission type</span></span>                        | <span data-ttu-id="e0cd6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e0cd6-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="e0cd6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0cd6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="e0cd6-113">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="e0cd6-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="e0cd6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0cd6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e0cd6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-115">Not supported.</span></span> |
| <span data-ttu-id="e0cd6-116">Application</span><span class="sxs-lookup"><span data-stu-id="e0cd6-116">Application</span></span>                            | <span data-ttu-id="e0cd6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e0cd6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0cd6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e0cd6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e0cd6-119">Optional query parameters</span></span>

<span data-ttu-id="e0cd6-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e0cd6-121">例如，若要检索每个请求的访问包，请 `$expand=accessPackage` 在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="e0cd6-122">若要仅检索对特定访问包的请求，请在查询中包括中的筛选器 `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` 。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>  <span data-ttu-id="e0cd6-123">若要检索生成的工作分配，请 `$expand=accessPackageAssignment` 在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-123">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>
<span data-ttu-id="e0cd6-124">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-124">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e0cd6-125">请求头</span><span class="sxs-lookup"><span data-stu-id="e0cd6-125">Request headers</span></span>

| <span data-ttu-id="e0cd6-126">名称</span><span class="sxs-lookup"><span data-stu-id="e0cd6-126">Name</span></span>      |<span data-ttu-id="e0cd6-127">说明</span><span class="sxs-lookup"><span data-stu-id="e0cd6-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e0cd6-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0cd6-128">Authorization</span></span> | <span data-ttu-id="e0cd6-129">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-129">Bearer \{token\}.</span></span> <span data-ttu-id="e0cd6-130">必填。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-130">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e0cd6-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0cd6-131">Request body</span></span>

<span data-ttu-id="e0cd6-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e0cd6-133">响应</span><span class="sxs-lookup"><span data-stu-id="e0cd6-133">Response</span></span>

<span data-ttu-id="e0cd6-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-134">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e0cd6-135">示例</span><span class="sxs-lookup"><span data-stu-id="e0cd6-135">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e0cd6-136">请求</span><span class="sxs-lookup"><span data-stu-id="e0cd6-136">Request</span></span>

<span data-ttu-id="e0cd6-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-137">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e0cd6-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="e0cd6-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="e0cd6-139">C#</span><span class="sxs-lookup"><span data-stu-id="e0cd6-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e0cd6-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e0cd6-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e0cd6-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e0cd6-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e0cd6-142">响应</span><span class="sxs-lookup"><span data-stu-id="e0cd6-142">Response</span></span>

<span data-ttu-id="e0cd6-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-143">The following is an example of the response.</span></span>

> <span data-ttu-id="e0cd6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e0cd6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "433dafca-5047-4614-95f7-a03510b1ded3",
      "requestType": "AdminAdd",
      "requestState": "Delivered",
      "requestStatus": "Fulfilled",
      "isValidationOnly": false,
      "createdDateTime": "2019-10-25T22:55:11.623Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
