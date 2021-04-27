---
title: 获取 accessPackageAssignmentPolicy
description: 检索 accessPackageAassignmentPolicy 对象的属性和关系。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 8b3f98108aa18221a513b6dc187fa1ed68b7017b
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048622"
---
# <a name="get-accesspackageassignmentpolicy"></a><span data-ttu-id="2ed88-103">获取 accessPackageAssignmentPolicy</span><span class="sxs-lookup"><span data-stu-id="2ed88-103">Get accessPackageAssignmentPolicy</span></span>

<span data-ttu-id="2ed88-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ed88-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ed88-105">在 [Azure AD 权利管理](../resources/entitlementmanagement-root.md)中，检索 [accessPackageAssignmentPolicy 对象的属性和](../resources/accesspackageassignmentpolicy.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="2ed88-105">In [Azure AD entitlement management](../resources/entitlementmanagement-root.md), retrieve the properties and relationships of an [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2ed88-106">权限</span><span class="sxs-lookup"><span data-stu-id="2ed88-106">Permissions</span></span>

<span data-ttu-id="2ed88-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ed88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2ed88-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ed88-109">Permission type</span></span>                        | <span data-ttu-id="2ed88-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2ed88-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2ed88-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed88-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2ed88-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ed88-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="2ed88-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed88-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2ed88-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed88-114">Not supported.</span></span> |
| <span data-ttu-id="2ed88-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ed88-115">Application</span></span>                            | <span data-ttu-id="2ed88-116">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ed88-116">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2ed88-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ed88-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2ed88-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2ed88-118">Optional query parameters</span></span>

<span data-ttu-id="2ed88-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2ed88-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2ed88-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2ed88-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2ed88-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ed88-121">Request headers</span></span>

| <span data-ttu-id="2ed88-122">名称</span><span class="sxs-lookup"><span data-stu-id="2ed88-122">Name</span></span>      |<span data-ttu-id="2ed88-123">说明</span><span class="sxs-lookup"><span data-stu-id="2ed88-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2ed88-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ed88-124">Authorization</span></span> | <span data-ttu-id="2ed88-p103">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ed88-p103">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2ed88-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ed88-127">Request body</span></span>

<span data-ttu-id="2ed88-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ed88-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ed88-129">响应</span><span class="sxs-lookup"><span data-stu-id="2ed88-129">Response</span></span>

<span data-ttu-id="2ed88-130">如果成功，此方法在响应正文中返回 响应代码和请求的 `200 OK` [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ed88-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageAssignmentPolicy](../resources/accesspackageassignmentpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ed88-131">示例</span><span class="sxs-lookup"><span data-stu-id="2ed88-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ed88-132">请求</span><span class="sxs-lookup"><span data-stu-id="2ed88-132">Request</span></span>

<span data-ttu-id="2ed88-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2ed88-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="2ed88-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ed88-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageassignmentpolicy"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentPolicies/{id}
```
# <a name="c"></a>[<span data-ttu-id="2ed88-135">C#</span><span class="sxs-lookup"><span data-stu-id="2ed88-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageassignmentpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ed88-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ed88-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageassignmentpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ed88-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ed88-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageassignmentpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ed88-138">Java</span><span class="sxs-lookup"><span data-stu-id="2ed88-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageassignmentpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ed88-139">响应</span><span class="sxs-lookup"><span data-stu-id="2ed88-139">Response</span></span>

<span data-ttu-id="2ed88-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2ed88-140">The following is an example of the response.</span></span>

> <span data-ttu-id="2ed88-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ed88-141">**Note:** The response object shown here might be shortened for readability.</span></span>

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


