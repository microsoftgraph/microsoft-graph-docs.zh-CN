---
title: 列出 accessPackageAssignmentRequests
description: 检索 accessPackageAssignmentRequest 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 193e257656abbcc13ea54099cd8d09897ffdb340
ms.sourcegitcommit: 8b23038be1141d7f22eb61de6aafdb16d4f9c826
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401011"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="752a9-103">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="752a9-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="752a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="752a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="752a9-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索 [accessPackageAssignmentRequest 对象](../resources/accesspackageassignmentrequest.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="752a9-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="752a9-106">生成的列表包括所有目录和访问包中调用方有权访问的分配请求（当前和过期）。</span><span class="sxs-lookup"><span data-stu-id="752a9-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="752a9-107">权限</span><span class="sxs-lookup"><span data-stu-id="752a9-107">Permissions</span></span>

<span data-ttu-id="752a9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="752a9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="752a9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="752a9-110">Permission type</span></span>                        | <span data-ttu-id="752a9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="752a9-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="752a9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="752a9-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="752a9-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="752a9-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="752a9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="752a9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="752a9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="752a9-115">Not supported.</span></span> |
| <span data-ttu-id="752a9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="752a9-116">Application</span></span>                            | <span data-ttu-id="752a9-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="752a9-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="752a9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="752a9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="752a9-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="752a9-119">Optional query parameters</span></span>

<span data-ttu-id="752a9-120">此方法支持 `$expand` 和 `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="752a9-120">This method supports the `$expand` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="752a9-121">例如，若要检索每个请求的访问包，请包括在 `$expand=accessPackage` 查询中。</span><span class="sxs-lookup"><span data-stu-id="752a9-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="752a9-122">若要仅检索特定访问包的请求，在查询中包括筛选器（如 `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` ）。</span><span class="sxs-lookup"><span data-stu-id="752a9-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>  <span data-ttu-id="752a9-123">若要检索结果分配，请包括在 `$expand=accessPackageAssignment` 查询中。</span><span class="sxs-lookup"><span data-stu-id="752a9-123">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="752a9-124">若要获取有关请求程序的详细信息，请包含 `$expand=requestor` 到查询中。</span><span class="sxs-lookup"><span data-stu-id="752a9-124">To obtain more details on the requestor, include `$expand=requestor` in the query.</span></span>
<span data-ttu-id="752a9-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="752a9-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="752a9-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="752a9-126">Request headers</span></span>

| <span data-ttu-id="752a9-127">名称</span><span class="sxs-lookup"><span data-stu-id="752a9-127">Name</span></span>      |<span data-ttu-id="752a9-128">说明</span><span class="sxs-lookup"><span data-stu-id="752a9-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="752a9-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="752a9-129">Authorization</span></span> | <span data-ttu-id="752a9-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="752a9-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="752a9-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="752a9-132">Request body</span></span>

<span data-ttu-id="752a9-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="752a9-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="752a9-134">响应</span><span class="sxs-lookup"><span data-stu-id="752a9-134">Response</span></span>

<span data-ttu-id="752a9-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="752a9-135">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="752a9-136">示例</span><span class="sxs-lookup"><span data-stu-id="752a9-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="752a9-137">请求</span><span class="sxs-lookup"><span data-stu-id="752a9-137">Request</span></span>

<span data-ttu-id="752a9-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="752a9-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="752a9-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="752a9-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="752a9-140">C#</span><span class="sxs-lookup"><span data-stu-id="752a9-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="752a9-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="752a9-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="752a9-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="752a9-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="752a9-143">Java</span><span class="sxs-lookup"><span data-stu-id="752a9-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="752a9-144">响应</span><span class="sxs-lookup"><span data-stu-id="752a9-144">Response</span></span>

<span data-ttu-id="752a9-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="752a9-145">The following is an example of the response.</span></span>

> <span data-ttu-id="752a9-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="752a9-146">**Note:** The response object shown here might be shortened for readability.</span></span>

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

