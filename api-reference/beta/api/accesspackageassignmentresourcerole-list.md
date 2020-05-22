---
title: 列出 accessPackageAssignmentResourceRoles
description: 检索 accessPackageAssignmentResourceRole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 77b5482bca2db2ca105095add0e7ab5e5709d311
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345616"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="11d47-103">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="11d47-103">List accessPackageAssignmentResourceRoles</span></span>

<span data-ttu-id="11d47-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11d47-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="11d47-105">检索[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="11d47-105">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="11d47-106">生成的列表包含呼叫者有权读取的所有目录和访问包中的所有工作分配的所有资源角色。</span><span class="sxs-lookup"><span data-stu-id="11d47-106">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="11d47-107">权限</span><span class="sxs-lookup"><span data-stu-id="11d47-107">Permissions</span></span>

<span data-ttu-id="11d47-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11d47-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="11d47-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11d47-110">Permission type</span></span>                        | <span data-ttu-id="11d47-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11d47-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="11d47-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11d47-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="11d47-113">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="11d47-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="11d47-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11d47-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11d47-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11d47-115">Not supported.</span></span> |
| <span data-ttu-id="11d47-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="11d47-116">Application</span></span>                            | <span data-ttu-id="11d47-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="11d47-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="11d47-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11d47-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="11d47-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="11d47-119">Optional query parameters</span></span>

<span data-ttu-id="11d47-120">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="11d47-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="11d47-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="11d47-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="11d47-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="11d47-122">Request headers</span></span>

| <span data-ttu-id="11d47-123">名称</span><span class="sxs-lookup"><span data-stu-id="11d47-123">Name</span></span>      |<span data-ttu-id="11d47-124">说明</span><span class="sxs-lookup"><span data-stu-id="11d47-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="11d47-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="11d47-125">Authorization</span></span> | <span data-ttu-id="11d47-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="11d47-126">Bearer \{token\}.</span></span> <span data-ttu-id="11d47-127">必填。</span><span class="sxs-lookup"><span data-stu-id="11d47-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="11d47-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="11d47-128">Request body</span></span>

<span data-ttu-id="11d47-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11d47-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11d47-130">响应</span><span class="sxs-lookup"><span data-stu-id="11d47-130">Response</span></span>

<span data-ttu-id="11d47-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="11d47-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="11d47-132">示例</span><span class="sxs-lookup"><span data-stu-id="11d47-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="11d47-133">请求</span><span class="sxs-lookup"><span data-stu-id="11d47-133">Request</span></span>

<span data-ttu-id="11d47-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11d47-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="11d47-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="11d47-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```
# <a name="c"></a>[<span data-ttu-id="11d47-136">C#</span><span class="sxs-lookup"><span data-stu-id="11d47-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11d47-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11d47-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11d47-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11d47-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11d47-139">响应</span><span class="sxs-lookup"><span data-stu-id="11d47-139">Response</span></span>

<span data-ttu-id="11d47-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="11d47-140">The following is an example of the response.</span></span>

> <span data-ttu-id="11d47-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="11d47-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
