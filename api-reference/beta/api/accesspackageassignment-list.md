---
title: 列出 accessPackageAssignments
description: 检索 accesspackageassignment 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: fc71acca245159cf04fb493364156e4e501a1c2a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991815"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="5ab61-103">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="5ab61-103">List accessPackageAssignments</span></span>

<span data-ttu-id="5ab61-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ab61-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ab61-105">在 [AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索 [accessPackageAssignment](../resources/accesspackageassignment.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5ab61-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span> <span data-ttu-id="5ab61-106">生成的列表包括呼叫者在所有目录和访问包中具有读取权限的所有工作分配、当前和已过期。</span><span class="sxs-lookup"><span data-stu-id="5ab61-106">The resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ab61-107">权限</span><span class="sxs-lookup"><span data-stu-id="5ab61-107">Permissions</span></span>

<span data-ttu-id="5ab61-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ab61-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ab61-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ab61-110">Permission type</span></span>                        | <span data-ttu-id="5ab61-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ab61-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5ab61-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ab61-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ab61-113">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="5ab61-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="5ab61-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ab61-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ab61-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ab61-115">Not supported.</span></span> |
| <span data-ttu-id="5ab61-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ab61-116">Application</span></span>                            | <span data-ttu-id="5ab61-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ab61-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ab61-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ab61-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5ab61-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5ab61-119">Optional query parameters</span></span>

<span data-ttu-id="5ab61-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5ab61-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="5ab61-121">例如，若要同时返回目标主题和访问包，请包括 `$expand=target,accessPackage` 。</span><span class="sxs-lookup"><span data-stu-id="5ab61-121">For example, to also return the target subject and access package, include `$expand=target,accessPackage`.</span></span> <span data-ttu-id="5ab61-122">若要仅检索已传递的工作分配，可以包含查询 `$filter=assignmentState eq 'Delivered'` 。</span><span class="sxs-lookup"><span data-stu-id="5ab61-122">To retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="5ab61-123">若要仅检索特定用户的工作分配，可以包含一个查询，该查询具有针对该用户的对象 ID 的工作分配： `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` 。</span><span class="sxs-lookup"><span data-stu-id="5ab61-123">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID of that user: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="5ab61-124">若要仅检索特定用户和特定访问包的工作分配，您可以包含具有针对该用户的访问包和对象 ID 的工作分配的查询： `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` 。</span><span class="sxs-lookup"><span data-stu-id="5ab61-124">To retrieve only assignments for a particular user and a particular access package, you can include a query with assignments targeting that access package and the object ID of that user: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="5ab61-125">若要仅检索由特定访问包分配策略产生的工作分配，可以包括该策略的查询： `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'` 。</span><span class="sxs-lookup"><span data-stu-id="5ab61-125">To retrieve only assignments resulting from a particular access package assignment policy, you can include a query for that policy: `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'`.</span></span>

<span data-ttu-id="5ab61-126">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="5ab61-126">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="5ab61-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ab61-127">Request headers</span></span>

| <span data-ttu-id="5ab61-128">名称</span><span class="sxs-lookup"><span data-stu-id="5ab61-128">Name</span></span>      |<span data-ttu-id="5ab61-129">说明</span><span class="sxs-lookup"><span data-stu-id="5ab61-129">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5ab61-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ab61-130">Authorization</span></span> | <span data-ttu-id="5ab61-131">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="5ab61-131">Bearer \{token\}.</span></span> <span data-ttu-id="5ab61-132">必需。</span><span class="sxs-lookup"><span data-stu-id="5ab61-132">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5ab61-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ab61-133">Request body</span></span>

<span data-ttu-id="5ab61-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ab61-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ab61-135">响应</span><span class="sxs-lookup"><span data-stu-id="5ab61-135">Response</span></span>

<span data-ttu-id="5ab61-136">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [accessPackageAssignment](../resources/accesspackageassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5ab61-136">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5ab61-137">示例</span><span class="sxs-lookup"><span data-stu-id="5ab61-137">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ab61-138">请求</span><span class="sxs-lookup"><span data-stu-id="5ab61-138">Request</span></span>

<span data-ttu-id="5ab61-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5ab61-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5ab61-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ab61-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="c"></a>[<span data-ttu-id="5ab61-141">C#</span><span class="sxs-lookup"><span data-stu-id="5ab61-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ab61-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ab61-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ab61-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ab61-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5ab61-144">响应</span><span class="sxs-lookup"><span data-stu-id="5ab61-144">Response</span></span>

<span data-ttu-id="5ab61-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5ab61-145">The following is an example of the response.</span></span>

> <span data-ttu-id="5ab61-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5ab61-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignment",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "9bdae7b4-6ece-487b-9eb8-9679dbd67aa2",
      "catalogId": "cc30dc98-6d3c-4fa0-bed8-fd76d0efd993",
      "accessPackageId": "e3f47362-993f-4fcb-8a38-532ffca16150",
      "assignmentPolicyId": "63ebd106-8116-40e7-a0ab-01ae475d11bb",
      "targetId": "ab4291f6-66b7-42bf-b597-a05b29414f5c",
      "assignmentStatus": "ExpiredNotificationTriggered",
      "assignmentState": "Expired",
      "isExtended": false,
      "expiredDateTime": "2019-04-25T23:45:40.42Z"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


