---
title: 列出 accessPackageAssignmentResourceRoles
description: 检索 accessPackageAssignmentResourceRole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 23d4b5a2169c6e43bc496147d127719d111ff4f5
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048580"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="dd8c6-103">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="dd8c6-103">List accessPackageAssignmentResourceRoles</span></span>

<span data-ttu-id="dd8c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd8c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dd8c6-105">检索 [accessPackageAssignmentResourceRole 对象](../resources/accesspackageassignmentresourcerole.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-105">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="dd8c6-106">生成的列表包括所有目录和访问包中调用方有权访问的所有分配的所有资源角色。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-106">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="dd8c6-107">权限</span><span class="sxs-lookup"><span data-stu-id="dd8c6-107">Permissions</span></span>

<span data-ttu-id="dd8c6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="dd8c6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd8c6-110">Permission type</span></span>                        | <span data-ttu-id="dd8c6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dd8c6-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="dd8c6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd8c6-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="dd8c6-113">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd8c6-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="dd8c6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd8c6-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dd8c6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-115">Not supported.</span></span> |
| <span data-ttu-id="dd8c6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd8c6-116">Application</span></span>                            | <span data-ttu-id="dd8c6-117">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd8c6-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dd8c6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd8c6-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="dd8c6-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dd8c6-119">Optional query parameters</span></span>

<span data-ttu-id="dd8c6-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="dd8c6-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

<span data-ttu-id="dd8c6-122">例如，若要仅为特定用户检索访问包分配资源角色，可以包括具有面向该用户的对象 ID 的筛选器的查询 `?$expand=accessPackageSubject&$filter=accessPackageSubject/objectId+eq+'9b835e5c-bf18-4ad9-8556-9b1ea0019c6b'` 。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-122">For example, to retrieve only access package assignment resource roles for a particular user, you can include a query with a filter targeting the object ID of that user `?$expand=accessPackageSubject&$filter=accessPackageSubject/objectId+eq+'9b835e5c-bf18-4ad9-8556-9b1ea0019c6b'`.</span></span>


## <a name="request-headers"></a><span data-ttu-id="dd8c6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd8c6-123">Request headers</span></span>

| <span data-ttu-id="dd8c6-124">名称</span><span class="sxs-lookup"><span data-stu-id="dd8c6-124">Name</span></span>      |<span data-ttu-id="dd8c6-125">说明</span><span class="sxs-lookup"><span data-stu-id="dd8c6-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dd8c6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd8c6-126">Authorization</span></span> | <span data-ttu-id="dd8c6-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dd8c6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd8c6-129">Request body</span></span>

<span data-ttu-id="dd8c6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dd8c6-131">响应</span><span class="sxs-lookup"><span data-stu-id="dd8c6-131">Response</span></span>

<span data-ttu-id="dd8c6-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-132">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="dd8c6-133">示例</span><span class="sxs-lookup"><span data-stu-id="dd8c6-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="dd8c6-134">请求</span><span class="sxs-lookup"><span data-stu-id="dd8c6-134">Request</span></span>

<span data-ttu-id="dd8c6-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dd8c6-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="dd8c6-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```
# <a name="c"></a>[<span data-ttu-id="dd8c6-137">C#</span><span class="sxs-lookup"><span data-stu-id="dd8c6-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dd8c6-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dd8c6-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dd8c6-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dd8c6-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dd8c6-140">Java</span><span class="sxs-lookup"><span data-stu-id="dd8c6-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentresourceroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="dd8c6-141">响应</span><span class="sxs-lookup"><span data-stu-id="dd8c6-141">Response</span></span>

<span data-ttu-id="dd8c6-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-142">The following is an example of the response.</span></span>

> <span data-ttu-id="dd8c6-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="dd8c6-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentResourceRole",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "1bf101d2-4d9c-437f-bbf5-3d13d98f5479",
      "originId": "originId-value",
      "originSystem": "SharePointOnline",
      "status": "Fulfilled"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageAssignmentResourceRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


