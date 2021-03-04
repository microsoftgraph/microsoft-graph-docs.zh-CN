---
title: 列出 accessPackageAssignmentPolicies
description: 检索 accessPackageAssignmentPolicy 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be973adb399d60846282acd55f9d44d5968af7ce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50439707"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="758a6-103">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="758a6-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="758a6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="758a6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="758a6-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索 [accessPackageAssignmentPolicy 对象](../resources/accesspackageassignmentpolicy.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="758a6-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span> <span data-ttu-id="758a6-106">如果委派的用户是目录角色，则生成的列表包括调用方有权访问的所有目录和访问包读取的所有分配策略。</span><span class="sxs-lookup"><span data-stu-id="758a6-106">If the delegated user is in a directory role, the resulting list includes all the assignment policies that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="758a6-107">如果委派的用户是访问包管理器或目录所有者，则他们应改为检索他们可以通过列表 [accessPackages](accesspackage-list.md) 读取的访问包的策略，包括为 `$expand=accessPackageAssignmentPolicies` 查询参数。</span><span class="sxs-lookup"><span data-stu-id="758a6-107">If the delegated user is an access package manager or catalog owner, they should instead retrieve the policies for the access packages they can read with [list accessPackages](accesspackage-list.md) by including `$expand=accessPackageAssignmentPolicies` as a query parameter.</span></span>

## <a name="permissions"></a><span data-ttu-id="758a6-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="758a6-108">Permissions</span></span>

<span data-ttu-id="758a6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="758a6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="758a6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="758a6-111">Permission type</span></span>                        | <span data-ttu-id="758a6-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="758a6-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="758a6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="758a6-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="758a6-114">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="758a6-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="758a6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="758a6-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="758a6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="758a6-116">Not supported.</span></span> |
| <span data-ttu-id="758a6-117">Application</span><span class="sxs-lookup"><span data-stu-id="758a6-117">Application</span></span>                            | <span data-ttu-id="758a6-118">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="758a6-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="758a6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="758a6-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="758a6-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="758a6-120">Optional query parameters</span></span>

<span data-ttu-id="758a6-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="758a6-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="758a6-122">例如，若要检索具有指定权限的访问包分配显示名称，请包括在 `$filter=displayName eq 'Employee sales support'` 查询中。</span><span class="sxs-lookup"><span data-stu-id="758a6-122">For example, to retrieve an access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="758a6-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="758a6-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="758a6-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="758a6-124">Request headers</span></span>

| <span data-ttu-id="758a6-125">名称</span><span class="sxs-lookup"><span data-stu-id="758a6-125">Name</span></span>      |<span data-ttu-id="758a6-126">说明</span><span class="sxs-lookup"><span data-stu-id="758a6-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="758a6-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="758a6-127">Authorization</span></span> | <span data-ttu-id="758a6-128">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="758a6-128">Bearer \{token\}.</span></span> <span data-ttu-id="758a6-129">必需。</span><span class="sxs-lookup"><span data-stu-id="758a6-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="758a6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="758a6-130">Request body</span></span>

<span data-ttu-id="758a6-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="758a6-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="758a6-132">响应</span><span class="sxs-lookup"><span data-stu-id="758a6-132">Response</span></span>

<span data-ttu-id="758a6-133">如果成功，此方法在响应正文中返回响应代码 `200 OK` 和 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="758a6-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="758a6-134">示例</span><span class="sxs-lookup"><span data-stu-id="758a6-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="758a6-135">请求</span><span class="sxs-lookup"><span data-stu-id="758a6-135">Request</span></span>

<span data-ttu-id="758a6-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="758a6-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="758a6-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="758a6-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="758a6-138">C#</span><span class="sxs-lookup"><span data-stu-id="758a6-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="758a6-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="758a6-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="758a6-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="758a6-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="758a6-141">Java</span><span class="sxs-lookup"><span data-stu-id="758a6-141">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="758a6-142">响应</span><span class="sxs-lookup"><span data-stu-id="758a6-142">Response</span></span>

<span data-ttu-id="758a6-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="758a6-143">The following is an example of the response.</span></span>

> <span data-ttu-id="758a6-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="758a6-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "b2eba9a1-b357-42ee-83a8-336522ed6cbf",
      "accessPackageId": "1b153a13-76da-4d07-9afa-c6c2b1f2e824",
      "displayName": "All Users",
      "description": "All users can request for access to the directory.",
      "canExtend": false,
      "durationInDays": 365,
      "accessReviewSettings": null
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentPolicies",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


