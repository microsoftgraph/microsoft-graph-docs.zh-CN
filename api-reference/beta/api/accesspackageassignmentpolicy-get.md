---
title: 获取 accessPackageAssignmentPolicy
description: 检索 accessPackageAassignmentPolicy 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: cebad5285d9c45c1c5bade244f83e23e6b16bd77
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331169"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="3ed35-103">获取 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="3ed35-103">Get accessPackageAssignmentPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ed35-104">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3ed35-104">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ed35-105">权限</span><span class="sxs-lookup"><span data-stu-id="3ed35-105">Permissions</span></span>

<span data-ttu-id="3ed35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3ed35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ed35-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3ed35-108">Permission type</span></span>                        | <span data-ttu-id="3ed35-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3ed35-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ed35-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed35-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="3ed35-111">EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3ed35-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3ed35-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3ed35-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ed35-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed35-113">Not supported.</span></span> |
| <span data-ttu-id="3ed35-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3ed35-114">Application</span></span>                            | <span data-ttu-id="3ed35-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3ed35-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ed35-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3ed35-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ed35-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3ed35-117">Optional query parameters</span></span>

<span data-ttu-id="3ed35-118">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3ed35-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3ed35-119">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3ed35-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ed35-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3ed35-120">Request headers</span></span>

| <span data-ttu-id="3ed35-121">名称</span><span class="sxs-lookup"><span data-stu-id="3ed35-121">Name</span></span>      |<span data-ttu-id="3ed35-122">说明</span><span class="sxs-lookup"><span data-stu-id="3ed35-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ed35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3ed35-123">Authorization</span></span> | <span data-ttu-id="3ed35-124">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="3ed35-124">Bearer \{token\}.</span></span> <span data-ttu-id="3ed35-125">必填。</span><span class="sxs-lookup"><span data-stu-id="3ed35-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ed35-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3ed35-126">Request body</span></span>

<span data-ttu-id="3ed35-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3ed35-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ed35-128">响应</span><span class="sxs-lookup"><span data-stu-id="3ed35-128">Response</span></span>

<span data-ttu-id="3ed35-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和请求的[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3ed35-129">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ed35-130">示例</span><span class="sxs-lookup"><span data-stu-id="3ed35-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ed35-131">请求</span><span class="sxs-lookup"><span data-stu-id="3ed35-131">Request</span></span>

<span data-ttu-id="3ed35-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3ed35-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="3ed35-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3ed35-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="3ed35-134">C#</span><span class="sxs-lookup"><span data-stu-id="3ed35-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3ed35-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3ed35-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3ed35-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3ed35-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3ed35-137">响应</span><span class="sxs-lookup"><span data-stu-id="3ed35-137">Response</span></span>

<span data-ttu-id="3ed35-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3ed35-138">The following is an example of the response.</span></span>

> <span data-ttu-id="3ed35-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="3ed35-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageAssignmentPolicy"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

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
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageAssignmentPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
