---
title: 列出 accessPackageAssignmentPolicies
description: 检索 accessPackageAssignmentPolicy 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 84c9110fa45df5083a2c5b47ad6b40f3ac57a3f9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47983891"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="12193-103">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="12193-103">List accessPackageAssignmentPolicies</span></span>

<span data-ttu-id="12193-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12193-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12193-105">在 [AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="12193-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span> <span data-ttu-id="12193-106">如果委派用户位于目录角色中，则生成的列表将包含呼叫者有权读取的所有编录和访问包中的所有分配策略。</span><span class="sxs-lookup"><span data-stu-id="12193-106">If the delegated user is in a directory role, the resulting list includes all the assignment policies that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="12193-107">如果委派的用户是访问包管理器或目录所有者，则应改用通过将其作为查询参数包括的访问包的策略，从而检索可通过 [列表 accessPackages](accesspackage-list.md) 读取的访问包的策略 `$expand=accessPackageAssignmentPolicies` 。</span><span class="sxs-lookup"><span data-stu-id="12193-107">If the delegated user is an access package manager or catalog owner, they should instead retrieve the policies for the access packages they can read with [list accessPackages](accesspackage-list.md) by including `$expand=accessPackageAssignmentPolicies` as a query parameter.</span></span>

## <a name="permissions"></a><span data-ttu-id="12193-108">权限</span><span class="sxs-lookup"><span data-stu-id="12193-108">Permissions</span></span>

<span data-ttu-id="12193-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="12193-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="12193-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="12193-111">Permission type</span></span>                        | <span data-ttu-id="12193-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="12193-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="12193-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="12193-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="12193-114">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="12193-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="12193-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="12193-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="12193-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="12193-116">Not supported.</span></span> |
| <span data-ttu-id="12193-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="12193-117">Application</span></span>                            | <span data-ttu-id="12193-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="12193-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="12193-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="12193-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="12193-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="12193-120">Optional query parameters</span></span>

<span data-ttu-id="12193-121">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="12193-121">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="12193-122">例如，若要检索具有指定显示名称的 access 程序包分配策略，请 `$filter=displayName eq 'Employee sales support'` 在查询中加入。</span><span class="sxs-lookup"><span data-stu-id="12193-122">For example, to retrieve an access package assignment policy with a specified display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="12193-123">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="12193-123">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="12193-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="12193-124">Request headers</span></span>

| <span data-ttu-id="12193-125">名称</span><span class="sxs-lookup"><span data-stu-id="12193-125">Name</span></span>      |<span data-ttu-id="12193-126">说明</span><span class="sxs-lookup"><span data-stu-id="12193-126">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="12193-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="12193-127">Authorization</span></span> | <span data-ttu-id="12193-128">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="12193-128">Bearer \{token\}.</span></span> <span data-ttu-id="12193-129">必需。</span><span class="sxs-lookup"><span data-stu-id="12193-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="12193-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="12193-130">Request body</span></span>

<span data-ttu-id="12193-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="12193-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="12193-132">响应</span><span class="sxs-lookup"><span data-stu-id="12193-132">Response</span></span>

<span data-ttu-id="12193-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="12193-133">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="12193-134">示例</span><span class="sxs-lookup"><span data-stu-id="12193-134">Examples</span></span>

### <a name="request"></a><span data-ttu-id="12193-135">请求</span><span class="sxs-lookup"><span data-stu-id="12193-135">Request</span></span>

<span data-ttu-id="12193-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="12193-136">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="12193-137">HTTP</span><span class="sxs-lookup"><span data-stu-id="12193-137">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="12193-138">C#</span><span class="sxs-lookup"><span data-stu-id="12193-138">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="12193-139">JavaScript</span><span class="sxs-lookup"><span data-stu-id="12193-139">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="12193-140">Objective-C</span><span class="sxs-lookup"><span data-stu-id="12193-140">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="12193-141">响应</span><span class="sxs-lookup"><span data-stu-id="12193-141">Response</span></span>

<span data-ttu-id="12193-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="12193-142">The following is an example of the response.</span></span>

> <span data-ttu-id="12193-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="12193-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


