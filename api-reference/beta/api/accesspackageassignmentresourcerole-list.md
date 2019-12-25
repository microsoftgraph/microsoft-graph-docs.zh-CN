---
title: 列出 accessPackageAssignmentResourceRoles
description: 检索 accessPackageAssignmentResourceRole 对象的列表。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 63ece8b5abcf6014e6ccbc293a773ea3dab8f462
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868007"
---
# <a name="list-accesspackageassignmentresourceroles"></a><span data-ttu-id="fc9c7-103">列出 accessPackageAssignmentResourceRoles</span><span class="sxs-lookup"><span data-stu-id="fc9c7-103">List accessPackageAssignmentResourceRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc9c7-104">检索[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-104">Retrieve a list of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects.</span></span>  <span data-ttu-id="fc9c7-105">生成的列表包含呼叫者有权读取的所有目录和访问包中的所有工作分配的所有资源角色。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-105">The resulting list includes all the resource roles of all assignments that the caller has access to read, across all catalogs and access packages.</span></span>

## <a name="permissions"></a><span data-ttu-id="fc9c7-106">权限</span><span class="sxs-lookup"><span data-stu-id="fc9c7-106">Permissions</span></span>

<span data-ttu-id="fc9c7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fc9c7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc9c7-109">Permission type</span></span>                        | <span data-ttu-id="fc9c7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc9c7-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="fc9c7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc9c7-111">Delegated (work or school account)</span></span>     |  <span data-ttu-id="fc9c7-112">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc9c7-112">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="fc9c7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc9c7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc9c7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-114">Not supported.</span></span> |
| <span data-ttu-id="fc9c7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc9c7-115">Application</span></span>                            | <span data-ttu-id="fc9c7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc9c7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc9c7-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fc9c7-118">可选查询参数</span><span class="sxs-lookup"><span data-stu-id="fc9c7-118">Optional query parameters</span></span>

<span data-ttu-id="fc9c7-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="fc9c7-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="fc9c7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc9c7-121">Request headers</span></span>

| <span data-ttu-id="fc9c7-122">名称</span><span class="sxs-lookup"><span data-stu-id="fc9c7-122">Name</span></span>      |<span data-ttu-id="fc9c7-123">说明</span><span class="sxs-lookup"><span data-stu-id="fc9c7-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="fc9c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc9c7-124">Authorization</span></span> | <span data-ttu-id="fc9c7-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-125">Bearer \{token\}.</span></span> <span data-ttu-id="fc9c7-126">必需。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc9c7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc9c7-127">Request body</span></span>

<span data-ttu-id="fc9c7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc9c7-129">响应</span><span class="sxs-lookup"><span data-stu-id="fc9c7-129">Response</span></span>

<span data-ttu-id="fc9c7-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-130">If successful, this method returns a `200 OK` response code and a collection of [accessPackageAssignmentResourceRole](../resources/accesspackageassignmentresourcerole.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fc9c7-131">示例</span><span class="sxs-lookup"><span data-stu-id="fc9c7-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fc9c7-132">请求</span><span class="sxs-lookup"><span data-stu-id="fc9c7-132">Request</span></span>

<span data-ttu-id="fc9c7-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-133">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="fc9c7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc9c7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentresourceroles"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentResourceRoles
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="fc9c7-135">C#</span><span class="sxs-lookup"><span data-stu-id="fc9c7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentresourceroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="fc9c7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc9c7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentresourceroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="fc9c7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc9c7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentresourceroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fc9c7-138">响应</span><span class="sxs-lookup"><span data-stu-id="fc9c7-138">Response</span></span>

<span data-ttu-id="fc9c7-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-139">The following is an example of the response.</span></span>

> <span data-ttu-id="fc9c7-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="fc9c7-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
