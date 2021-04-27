---
title: 列出 accessPackageAssignments
description: 检索 accesspackageassignment 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: a37d14901cdb3105fb6a648268a7b72fb85dd1b3
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048636"
---
# <a name="list-accesspackageassignments"></a><span data-ttu-id="7ac8b-103">列出 accessPackageAssignments</span><span class="sxs-lookup"><span data-stu-id="7ac8b-103">List accessPackageAssignments</span></span>

<span data-ttu-id="7ac8b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ac8b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7ac8b-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索 [accessPackageAssignment 对象](../resources/accesspackageassignment.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve a list of [accessPackageAssignment](../resources/accesspackageassignment.md) objects.</span></span> <span data-ttu-id="7ac8b-106">对于目录范围的管理员，结果列表包括调用方有权访问的所有目录和访问包的所有分配（当前分配和过期分配）。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-106">For directory-wide administrators, the resulting list includes all the assignments, current and well as expired, that the caller has access to read, across all catalogs and access packages.</span></span>  <span data-ttu-id="7ac8b-107">如果调用方代表仅分配给特定于目录的委派管理角色的委派用户，则请求必须提供筛选器来指示特定访问包，例如 `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` ：。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-107">If the caller is on behalf of a delegated user who is assigned only to catalog-specific delegated administrative roles, the request must supply a filter to indicate a specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span>


## <a name="permissions"></a><span data-ttu-id="7ac8b-108">权限</span><span class="sxs-lookup"><span data-stu-id="7ac8b-108">Permissions</span></span>

<span data-ttu-id="7ac8b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7ac8b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ac8b-111">Permission type</span></span>                        | <span data-ttu-id="7ac8b-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7ac8b-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7ac8b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac8b-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="7ac8b-114">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac8b-114">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="7ac8b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac8b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7ac8b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-116">Not supported.</span></span> |
| <span data-ttu-id="7ac8b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ac8b-117">Application</span></span>                            | <span data-ttu-id="7ac8b-118">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac8b-118">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7ac8b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ac8b-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7ac8b-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7ac8b-120">Optional query parameters</span></span>

<span data-ttu-id="7ac8b-121">如果调用方代表仅分配给特定于目录的委派管理角色的委派用户，则请求必须提供筛选器来指示特定访问包，例如 `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'` ：。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-121">If the caller is on behalf of a delegated user who is assigned only to catalog-specific delegated administrative roles, the request must supply a filter to indicate a specific access package, such as: `$filter=accessPackage/id eq 'a914b616-e04e-476b-aa37-91038f0b165b'`.</span></span>  <span data-ttu-id="7ac8b-122">此方法还支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-122">This method also supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="7ac8b-123">例如，若要同时返回目标主题和访问包，请包含 `$expand=target,accessPackage` 。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-123">For example, to also return the target subject and access package, include `$expand=target,accessPackage`.</span></span> <span data-ttu-id="7ac8b-124">若要仅检索已传递的工作分配，可以包括查询 `$filter=assignmentState eq 'Delivered'` 。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-124">To retrieve only delivered assignments, you can include a query `$filter=assignmentState eq 'Delivered'`.</span></span> <span data-ttu-id="7ac8b-125">若要仅检索特定用户的工作分配，可以包含一个包含针对该用户的对象 ID 的工作分配的查询 `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` ：。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-125">To retrieve only assignments for a particular user, you can include a query with assignments targeting the object ID of that user: `$expand=target&$filter=target/objectid+eq+'7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="7ac8b-126">若要仅检索特定用户和特定访问包的工作分配，可以包含包含针对该访问包的工作分配和该用户的对象 ID 的查询 `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'` ：。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-126">To retrieve only assignments for a particular user and a particular access package, you can include a query with assignments targeting that access package and the object ID of that user: `$expand=accessPackage,target&$filter=accessPackage/id eq '9bbe5f7d-f1e7-4eb1-a586-38cdf6f8b1ea' and target/objectid eq '7deff43e-1f17-44ef-9e5f-d516b0ba11d4'`.</span></span>  <span data-ttu-id="7ac8b-127">若要仅检索特定访问包分配策略生成的分配，可以包括该策略的查询 `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'` ：。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-127">To retrieve only assignments resulting from a particular access package assignment policy, you can include a query for that policy: `$filter=accessPackageAssignmentPolicy/id eq 'd92ebb54-9b46-492d-ab7f-01f76767da7f'`.</span></span>

<span data-ttu-id="7ac8b-128">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-128">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="7ac8b-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ac8b-129">Request headers</span></span>

| <span data-ttu-id="7ac8b-130">名称</span><span class="sxs-lookup"><span data-stu-id="7ac8b-130">Name</span></span>      |<span data-ttu-id="7ac8b-131">说明</span><span class="sxs-lookup"><span data-stu-id="7ac8b-131">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7ac8b-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ac8b-132">Authorization</span></span> | <span data-ttu-id="7ac8b-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7ac8b-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ac8b-135">Request body</span></span>

<span data-ttu-id="7ac8b-136">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7ac8b-137">响应</span><span class="sxs-lookup"><span data-stu-id="7ac8b-137">Response</span></span>

<span data-ttu-id="7ac8b-138">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignment](../resources/accesspackageassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-138">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignment](../resources/accesspackageassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7ac8b-139">示例</span><span class="sxs-lookup"><span data-stu-id="7ac8b-139">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7ac8b-140">请求</span><span class="sxs-lookup"><span data-stu-id="7ac8b-140">Request</span></span>

<span data-ttu-id="7ac8b-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-141">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7ac8b-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="7ac8b-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignments"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignments
```
# <a name="c"></a>[<span data-ttu-id="7ac8b-143">C#</span><span class="sxs-lookup"><span data-stu-id="7ac8b-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="7ac8b-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7ac8b-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7ac8b-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7ac8b-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7ac8b-146">Java</span><span class="sxs-lookup"><span data-stu-id="7ac8b-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7ac8b-147">响应</span><span class="sxs-lookup"><span data-stu-id="7ac8b-147">Response</span></span>

<span data-ttu-id="7ac8b-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-148">The following is an example of the response.</span></span>

> <span data-ttu-id="7ac8b-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7ac8b-149">**Note:** The response object shown here might be shortened for readability.</span></span>

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


