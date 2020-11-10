---
title: 获取 accessPackageAssignmentRequest
description: 检索 accessPackageAssignmentRequest 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 17734190492163d0cfdb89bf0296b48835f8aeb9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48952117"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="18307-103">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="18307-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="18307-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18307-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18307-105">在 [AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="18307-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="18307-106">权限</span><span class="sxs-lookup"><span data-stu-id="18307-106">Permissions</span></span>

<span data-ttu-id="18307-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18307-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18307-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18307-109">Permission type</span></span>                        | <span data-ttu-id="18307-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18307-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18307-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18307-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18307-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="18307-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="18307-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18307-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18307-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18307-114">Not supported.</span></span> |
| <span data-ttu-id="18307-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18307-115">Application</span></span>                            | <span data-ttu-id="18307-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18307-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="18307-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18307-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18307-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="18307-118">Optional query parameters</span></span>

<span data-ttu-id="18307-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="18307-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="18307-120">例如，若要检索请求的访问包，请 `$expand=accessPackage` 在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="18307-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="18307-121">若要检索生成的工作分配，请 `$expand=accessPackageAssignment` 在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="18307-121">To retrieve the resulting assignment, include `$expand=accessPackageAssignment` in the query.</span></span>  <span data-ttu-id="18307-122">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="18307-122">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="18307-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="18307-123">Request headers</span></span>

| <span data-ttu-id="18307-124">名称</span><span class="sxs-lookup"><span data-stu-id="18307-124">Name</span></span>      |<span data-ttu-id="18307-125">说明</span><span class="sxs-lookup"><span data-stu-id="18307-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="18307-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="18307-126">Authorization</span></span> | <span data-ttu-id="18307-127">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="18307-127">Bearer \{token\}.</span></span> <span data-ttu-id="18307-128">必填。</span><span class="sxs-lookup"><span data-stu-id="18307-128">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="18307-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="18307-129">Request body</span></span>

<span data-ttu-id="18307-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18307-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18307-131">响应</span><span class="sxs-lookup"><span data-stu-id="18307-131">Response</span></span>

<span data-ttu-id="18307-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="18307-132">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18307-133">示例</span><span class="sxs-lookup"><span data-stu-id="18307-133">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18307-134">请求</span><span class="sxs-lookup"><span data-stu-id="18307-134">Request</span></span>

<span data-ttu-id="18307-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="18307-135">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="18307-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="18307-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="18307-137">C#</span><span class="sxs-lookup"><span data-stu-id="18307-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="18307-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="18307-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="18307-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="18307-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="18307-140">Java</span><span class="sxs-lookup"><span data-stu-id="18307-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentrequest-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="18307-141">响应</span><span class="sxs-lookup"><span data-stu-id="18307-141">Response</span></span>

<span data-ttu-id="18307-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="18307-142">The following is an example of the response.</span></span>

> <span data-ttu-id="18307-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="18307-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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


