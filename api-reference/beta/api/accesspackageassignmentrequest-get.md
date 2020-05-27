---
title: 获取 accessPackageAssignmentRequest
description: 检索 accessPackageAssignmentRequest 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4f218e01cf389668ea1f7b680c2c58af4afa9094
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383491"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="a900b-103">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="a900b-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="a900b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a900b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a900b-105">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a900b-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a900b-106">权限</span><span class="sxs-lookup"><span data-stu-id="a900b-106">Permissions</span></span>

<span data-ttu-id="a900b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a900b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a900b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a900b-109">Permission type</span></span>                        | <span data-ttu-id="a900b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a900b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a900b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a900b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a900b-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="a900b-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="a900b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a900b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a900b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a900b-114">Not supported.</span></span> |
| <span data-ttu-id="a900b-115">Application</span><span class="sxs-lookup"><span data-stu-id="a900b-115">Application</span></span>                            | <span data-ttu-id="a900b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a900b-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a900b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a900b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a900b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a900b-118">Optional query parameters</span></span>

<span data-ttu-id="a900b-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a900b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="a900b-120">例如，若要检索请求的访问包，请 `$expand=accessPackage` 在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="a900b-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="a900b-121">若要检索生成的工作分配，请 `$expand=accessPackageAssignment` 在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="a900b-121">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="a900b-122">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a900b-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="a900b-123">请求头</span><span class="sxs-lookup"><span data-stu-id="a900b-123">Request headers</span></span>

| <span data-ttu-id="a900b-124">名称</span><span class="sxs-lookup"><span data-stu-id="a900b-124">Name</span></span>      |<span data-ttu-id="a900b-125">说明</span><span class="sxs-lookup"><span data-stu-id="a900b-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="a900b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a900b-126">Authorization</span></span> | <span data-ttu-id="a900b-127">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="a900b-127">Bearer \{token\}.</span></span> <span data-ttu-id="a900b-128">必填。</span><span class="sxs-lookup"><span data-stu-id="a900b-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a900b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a900b-129">Request body</span></span>

<span data-ttu-id="a900b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a900b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a900b-131">响应</span><span class="sxs-lookup"><span data-stu-id="a900b-131">Response</span></span>

<span data-ttu-id="a900b-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a900b-132">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a900b-133">示例</span><span class="sxs-lookup"><span data-stu-id="a900b-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a900b-134">请求</span><span class="sxs-lookup"><span data-stu-id="a900b-134">Request</span></span>

<span data-ttu-id="a900b-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a900b-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a900b-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="a900b-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="a900b-137">C#</span><span class="sxs-lookup"><span data-stu-id="a900b-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a900b-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a900b-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a900b-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a900b-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="a900b-140">响应</span><span class="sxs-lookup"><span data-stu-id="a900b-140">Response</span></span>

<span data-ttu-id="a900b-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a900b-141">The following is an example of the response.</span></span>

> <span data-ttu-id="a900b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a900b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentRequest"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "433dafca-5047-4614-95f7-a03510b1ded3",
  "requestType": "AdminAdd",
  "requestState": "Delivered",
  "requestStatus": "Fulfilled",
  "isValidationOnly": false,
  "createdDateTime": "2019-10-25T22:55:11.623Z"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentRequest",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
