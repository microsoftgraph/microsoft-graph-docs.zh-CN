---
title: 列出 accessPackageAssignmentRequests
description: 检索 accessPackageAssignmentRequest 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e6b436c59feda5fbb890a5f83cb5d11a3c3dc0de
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42442038"
---
# <a name="list-accesspackageassignmentrequests"></a><span data-ttu-id="6c98e-103">列出 accessPackageAssignmentRequests</span><span class="sxs-lookup"><span data-stu-id="6c98e-103">List accessPackageAssignmentRequests</span></span>

<span data-ttu-id="6c98e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6c98e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6c98e-105">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="6c98e-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects.</span></span>  <span data-ttu-id="6c98e-106">生成的列表包括在所有目录和访问包中，呼叫者有权读取的所有工作分配请求、当前和已过期。</span><span class="sxs-lookup"><span data-stu-id="6c98e-106">The resulting list includes all the assignment requests, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c98e-107">权限</span><span class="sxs-lookup"><span data-stu-id="6c98e-107">Permissions</span></span>

<span data-ttu-id="6c98e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c98e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c98e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c98e-110">Permission type</span></span>                        | <span data-ttu-id="6c98e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c98e-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6c98e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c98e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c98e-113">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c98e-113">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="6c98e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c98e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c98e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c98e-115">Not supported.</span></span> |
| <span data-ttu-id="6c98e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c98e-116">Application</span></span>                            | <span data-ttu-id="6c98e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c98e-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c98e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c98e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c98e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6c98e-119">Optional query parameters</span></span>

<span data-ttu-id="6c98e-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6c98e-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="6c98e-121">例如，若要检索每个请求的访问包，请`$expand=accessPackage`在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="6c98e-121">For example, to retrieve the access package of each request, include `$expand=accessPackage` in the query.</span></span>  <span data-ttu-id="6c98e-122">若要仅检索对特定访问包的请求，请在查询中包括中的`$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`筛选器。</span><span class="sxs-lookup"><span data-stu-id="6c98e-122">To retrieve only requests for a specific access package, include in the query a filter such as `$expand=accessPackage&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea'`.</span></span>
<span data-ttu-id="6c98e-123">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6c98e-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c98e-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c98e-124">Request headers</span></span>

| <span data-ttu-id="6c98e-125">名称</span><span class="sxs-lookup"><span data-stu-id="6c98e-125">Name</span></span>      |<span data-ttu-id="6c98e-126">说明</span><span class="sxs-lookup"><span data-stu-id="6c98e-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6c98e-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c98e-127">Authorization</span></span> | <span data-ttu-id="6c98e-128">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="6c98e-128">Bearer \{token\}.</span></span> <span data-ttu-id="6c98e-129">必填。</span><span class="sxs-lookup"><span data-stu-id="6c98e-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c98e-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c98e-130">Request body</span></span>

<span data-ttu-id="6c98e-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c98e-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c98e-132">响应</span><span class="sxs-lookup"><span data-stu-id="6c98e-132">Response</span></span>

<span data-ttu-id="6c98e-133">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6c98e-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6c98e-134">示例</span><span class="sxs-lookup"><span data-stu-id="6c98e-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6c98e-135">请求</span><span class="sxs-lookup"><span data-stu-id="6c98e-135">Request</span></span>

<span data-ttu-id="6c98e-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6c98e-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6c98e-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c98e-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequests"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests
```
# <a name="c"></a>[<span data-ttu-id="6c98e-138">C#</span><span class="sxs-lookup"><span data-stu-id="6c98e-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6c98e-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c98e-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c98e-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c98e-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6c98e-141">响应</span><span class="sxs-lookup"><span data-stu-id="6c98e-141">Response</span></span>

<span data-ttu-id="6c98e-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6c98e-142">The following is an example of the response.</span></span>

> <span data-ttu-id="6c98e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="6c98e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
