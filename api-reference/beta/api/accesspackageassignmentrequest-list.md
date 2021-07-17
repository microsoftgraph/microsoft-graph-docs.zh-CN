---
title: 列出 accessPackageAssignmentRequests
description: 检索 accessPackageAssignmentRequest 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: d5ce1ca824f104de9058be4ed748d5b87a731e71
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53466934"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="3e27d-103">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="3e27d-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="3e27d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e27d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e27d-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索 [accessPackageAssignmentRequest 对象](../resources/accesspackageassignmentrequest.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="3e27d-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="3e27d-106">生成的列表包括所有目录和访问包中调用方有权访问的分配请求（当前和过期）。</span><span class="sxs-lookup"><span data-stu-id="3e27d-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e27d-107">权限</span><span class="sxs-lookup"><span data-stu-id="3e27d-107">Permissions</span></span>

<span data-ttu-id="3e27d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e27d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3e27d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e27d-110">Permission type</span></span>                        | <span data-ttu-id="3e27d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e27d-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3e27d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e27d-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="3e27d-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e27d-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3e27d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e27d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e27d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e27d-115">Not supported.</span></span> |
| <span data-ttu-id="3e27d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e27d-116">Application</span></span>                            | <span data-ttu-id="3e27d-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e27d-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e27d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e27d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3e27d-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3e27d-119">Optional query parameters</span></span>

<span data-ttu-id="3e27d-120">此方法支持 `$expand` 和 `$filter` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3e27d-120">This method supports the `$expand` and `$filter` OData query parameters to help customize the response.</span></span> <span data-ttu-id="3e27d-121">例如，若要检索每个请求的访问包，请包括在 `$expand=accessPackage` 查询中。</span><span class="sxs-lookup"><span data-stu-id="3e27d-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="3e27d-122">若要仅检索特定访问包的请求，在查询中包括筛选器（如 `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'` ）。</span><span class="sxs-lookup"><span data-stu-id="3e27d-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>  <span data-ttu-id="3e27d-123">若要检索结果分配，请包括在 `$expand=accessPackageAssignment` 查询中。</span><span class="sxs-lookup"><span data-stu-id="3e27d-123">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="3e27d-124">若要获取有关请求程序的详细信息，请包含 `$expand=requestor` 到查询中。</span><span class="sxs-lookup"><span data-stu-id="3e27d-124">To obtain more details on the requestor, include `$expand=requestor` in the query.</span></span>
<span data-ttu-id="3e27d-125">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3e27d-125">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3e27d-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e27d-126">Request headers</span></span>

| <span data-ttu-id="3e27d-127">名称</span><span class="sxs-lookup"><span data-stu-id="3e27d-127">Name</span></span>      |<span data-ttu-id="3e27d-128">说明</span><span class="sxs-lookup"><span data-stu-id="3e27d-128">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3e27d-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e27d-129">Authorization</span></span> | <span data-ttu-id="3e27d-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e27d-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3e27d-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e27d-132">Request body</span></span>

<span data-ttu-id="3e27d-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e27d-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3e27d-134">响应</span><span class="sxs-lookup"><span data-stu-id="3e27d-134">Response</span></span>

<span data-ttu-id="3e27d-135">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3e27d-135">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3e27d-136">示例</span><span class="sxs-lookup"><span data-stu-id="3e27d-136">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3e27d-137">请求</span><span class="sxs-lookup"><span data-stu-id="3e27d-137">Request</span></span>

<span data-ttu-id="3e27d-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3e27d-138">The following is an example of the request.</span></span> <span data-ttu-id="3e27d-139">请求 URI 包括仅返回特定状态的请求，以及返回请求者 `$filter` `$expand` 及其已连接组织的详细信息。</span><span class="sxs-lookup"><span data-stu-id="3e27d-139">The request URI includes `$filter` to only return requests in a particular state, and `$expand` to return details of the requestor and their connected organization as well.</span></span>

# <a name="http"></a>[<span data-ttu-id="3e27d-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e27d-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests?$expand=requestor($expand=connectedOrganization)&$filter=(requestState eq 'PendingApproval')
```
# <a name="c"></a>[<span data-ttu-id="3e27d-141">C#</span><span class="sxs-lookup"><span data-stu-id="3e27d-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e27d-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e27d-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e27d-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e27d-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e27d-144">Java</span><span class="sxs-lookup"><span data-stu-id="3e27d-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3e27d-145">响应</span><span class="sxs-lookup"><span data-stu-id="3e27d-145">Response</span></span>

<span data-ttu-id="3e27d-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3e27d-146">The following is an example of the response.</span></span>

> <span data-ttu-id="3e27d-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3e27d-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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
      "requestType": "UserAdd",
      "requestState": "PendingApproval",
      "createdDateTime": "2019-10-25T22:55:11.623Z",
      "justification": "Need access",
      "answers": [],
      "requestor": {
        "connectedOrganizationId": "c3c2adbc-a863-437f-9383-ee578665317d",
        "id": "ba7ef0fb-e16f-474b-87aa-02815d061e67",
        "displayName": "displayname",
        "email": "displayname@example.com",
        "type": "User",
        "connectedOrganization": {
          "id": "c3c2adbc-a863-437f-9383-ee578665317d",
          "displayName": "example"
        }
      }
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

