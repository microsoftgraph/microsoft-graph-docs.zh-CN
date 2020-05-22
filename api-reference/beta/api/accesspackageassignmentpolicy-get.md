---
title: 获取 accessPackageAssignmentPolicy
description: 检索 accessPackageAassignmentPolicy 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e24604cd36f866a60c64e12cc3c399c583bfae73
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345220"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="9e8c9-103">获取 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="9e8c9-103">Get accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="9e8c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e8c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e8c9-105">在[AZURE AD 权限管理](../resources/entitlementmanagement-root.md)中，检索[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="9e8c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="9e8c9-106">Permissions</span></span>

<span data-ttu-id="9e8c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9e8c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e8c9-109">Permission type</span></span>                        | <span data-ttu-id="9e8c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9e8c9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="9e8c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e8c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9e8c9-112">EntitlementManagement、EntitlementManagement 和所有</span><span class="sxs-lookup"><span data-stu-id="9e8c9-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="9e8c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e8c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9e8c9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-114">Not supported.</span></span> |
| <span data-ttu-id="9e8c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e8c9-115">Application</span></span>                            | <span data-ttu-id="9e8c9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9e8c9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e8c9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9e8c9-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9e8c9-118">Optional query parameters</span></span>

<span data-ttu-id="9e8c9-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="9e8c9-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9e8c9-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e8c9-121">Request headers</span></span>

| <span data-ttu-id="9e8c9-122">名称</span><span class="sxs-lookup"><span data-stu-id="9e8c9-122">Name</span></span>      |<span data-ttu-id="9e8c9-123">说明</span><span class="sxs-lookup"><span data-stu-id="9e8c9-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="9e8c9-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e8c9-124">Authorization</span></span> | <span data-ttu-id="9e8c9-125">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-125">Bearer \{token\}.</span></span> <span data-ttu-id="9e8c9-126">必填。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9e8c9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e8c9-127">Request body</span></span>

<span data-ttu-id="9e8c9-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9e8c9-129">响应</span><span class="sxs-lookup"><span data-stu-id="9e8c9-129">Response</span></span>

<span data-ttu-id="9e8c9-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的[accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9e8c9-131">示例</span><span class="sxs-lookup"><span data-stu-id="9e8c9-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="9e8c9-132">请求</span><span class="sxs-lookup"><span data-stu-id="9e8c9-132">Request</span></span>

<span data-ttu-id="9e8c9-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9e8c9-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9e8c9-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="9e8c9-135">C#</span><span class="sxs-lookup"><span data-stu-id="9e8c9-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9e8c9-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9e8c9-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9e8c9-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9e8c9-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="9e8c9-138">响应</span><span class="sxs-lookup"><span data-stu-id="9e8c9-138">Response</span></span>

<span data-ttu-id="9e8c9-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-139">The following is an example of the response.</span></span>

> <span data-ttu-id="9e8c9-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9e8c9-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "All users in the directory can request access.",
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
