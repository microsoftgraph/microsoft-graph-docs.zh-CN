---
title: 列出 accessPackageAssignmentPolicies
description: 检索 accessPackageAssignmentPolicy 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1a56b7b9c86c7717421719569815009a27fcde37
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331197"
---
# <a name="list-accesspackageassignmentpolicies"></a><span data-ttu-id="f572c-103">列出 accessPackageAssignmentPolicies</span><span class="sxs-lookup"><span data-stu-id="f572c-103">List accessPackageAssignmentPolicies</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f572c-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="f572c-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects.</span></span>   <span data-ttu-id="f572c-105">生成的列表包括呼叫者有权读取的所有目录和访问包中的所有分配策略。</span><span class="sxs-lookup"><span data-stu-id="f572c-105">The resulting list includes all the assignment policies which the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="f572c-106">权限</span><span class="sxs-lookup"><span data-stu-id="f572c-106">Permissions</span></span>

<span data-ttu-id="f572c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f572c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="f572c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f572c-109">Permission type</span></span>                        | <span data-ttu-id="f572c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f572c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="f572c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f572c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="f572c-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f572c-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="f572c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f572c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f572c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f572c-114">Not supported.</span></span> |
| <span data-ttu-id="f572c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f572c-115">Application</span></span>                            | <span data-ttu-id="f572c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f572c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f572c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f572c-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f572c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f572c-118">Optional query parameters</span></span>

<span data-ttu-id="f572c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f572c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="f572c-120">例如，若要检索具有指定显示名称的 access 程序包分配策略，请在`$filter=displayName eq 'Employee sales support'`查询中加入。</span><span class="sxs-lookup"><span data-stu-id="f572c-120">For example, to retrieve a access package assignment policy with a specifed display name, include `$filter=displayName eq 'Employee sales support'` in the query.</span></span> <span data-ttu-id="f572c-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="f572c-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="f572c-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f572c-122">Request headers</span></span>

| <span data-ttu-id="f572c-123">名称</span><span class="sxs-lookup"><span data-stu-id="f572c-123">Name</span></span>      |<span data-ttu-id="f572c-124">说明</span><span class="sxs-lookup"><span data-stu-id="f572c-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f572c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f572c-125">Authorization</span></span> | <span data-ttu-id="f572c-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="f572c-126">Bearer \{token\}.</span></span> <span data-ttu-id="f572c-127">必填。</span><span class="sxs-lookup"><span data-stu-id="f572c-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f572c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f572c-128">Request body</span></span>

<span data-ttu-id="f572c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f572c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f572c-130">响应</span><span class="sxs-lookup"><span data-stu-id="f572c-130">Response</span></span>

<span data-ttu-id="f572c-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f572c-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f572c-132">示例</span><span class="sxs-lookup"><span data-stu-id="f572c-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f572c-133">请求</span><span class="sxs-lookup"><span data-stu-id="f572c-133">Request</span></span>

<span data-ttu-id="f572c-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="f572c-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f572c-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="f572c-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicies"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies
```
# <a name="c"></a>[<span data-ttu-id="f572c-136">C#</span><span class="sxs-lookup"><span data-stu-id="f572c-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f572c-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f572c-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f572c-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f572c-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f572c-139">响应</span><span class="sxs-lookup"><span data-stu-id="f572c-139">Response</span></span>

<span data-ttu-id="f572c-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="f572c-140">The following is an example of the response.</span></span>

> <span data-ttu-id="f572c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="f572c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
      "isDenyPolicy": false,
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
