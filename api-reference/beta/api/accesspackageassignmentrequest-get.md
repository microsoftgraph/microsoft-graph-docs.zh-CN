---
title: 获取 accessPackageAssignmentRequest
description: 检索 accessPackageAssignmentRequest 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da26d23027cd77e986a40c66cb6e7acbdff08ef8
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345658"
---
# <a name="get-accesspackageassignmentrequest"></a><span data-ttu-id="9568d-103">获取 accessPackageAssignmentRequest</span><span class="sxs-lookup"><span data-stu-id="9568d-103">Get accessPackageAssignmentRequest</span></span>

<span data-ttu-id="9568d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9568d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9568d-105">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9568d-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an  [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9568d-106">权限</span><span class="sxs-lookup"><span data-stu-id="9568d-106">Permissions</span></span>

<span data-ttu-id="9568d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9568d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9568d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9568d-109">Permission type</span></span>                        | <span data-ttu-id="9568d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9568d-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9568d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9568d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9568d-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="9568d-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span>  |
| <span data-ttu-id="9568d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9568d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9568d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9568d-114">Not supported.</span></span> |
| <span data-ttu-id="9568d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9568d-115">Application</span></span>                            | <span data-ttu-id="9568d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9568d-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9568d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9568d-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9568d-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9568d-118">Optional query parameters</span></span>

<span data-ttu-id="9568d-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9568d-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9568d-120">例如，若要检索请求的访问包，请 `$expand=accessPackage` 在查询中包含。</span><span class="sxs-lookup"><span data-stu-id="9568d-120">For example, to retrieve the access package that was requested, include `$expand=accessPackage` in the query.</span></span> <span data-ttu-id="9568d-121">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9568d-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9568d-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="9568d-122">Request headers</span></span>

| <span data-ttu-id="9568d-123">名称</span><span class="sxs-lookup"><span data-stu-id="9568d-123">Name</span></span>      |<span data-ttu-id="9568d-124">说明</span><span class="sxs-lookup"><span data-stu-id="9568d-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9568d-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="9568d-125">Authorization</span></span> | <span data-ttu-id="9568d-126">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="9568d-126">Bearer \{token\}.</span></span> <span data-ttu-id="9568d-127">必填。</span><span class="sxs-lookup"><span data-stu-id="9568d-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9568d-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="9568d-128">Request body</span></span>

<span data-ttu-id="9568d-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9568d-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9568d-130">响应</span><span class="sxs-lookup"><span data-stu-id="9568d-130">Response</span></span>

<span data-ttu-id="9568d-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9568d-131">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentRequest](../resources/accesspackageassignmentrequest.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9568d-132">示例</span><span class="sxs-lookup"><span data-stu-id="9568d-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9568d-133">请求</span><span class="sxs-lookup"><span data-stu-id="9568d-133">Request</span></span>

<span data-ttu-id="9568d-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9568d-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9568d-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="9568d-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentrequest"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}
```
# <a name="c"></a>[<span data-ttu-id="9568d-136">C#</span><span class="sxs-lookup"><span data-stu-id="9568d-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentrequest-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9568d-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9568d-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentrequest-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9568d-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9568d-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentrequest-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9568d-139">响应</span><span class="sxs-lookup"><span data-stu-id="9568d-139">Response</span></span>

<span data-ttu-id="9568d-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9568d-140">The following is an example of the response.</span></span>

> <span data-ttu-id="9568d-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9568d-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
