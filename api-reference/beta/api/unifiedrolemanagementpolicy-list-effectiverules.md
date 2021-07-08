---
title: 列出 effectiveRules
description: 从 effectiveRules 导航属性获取 unifiedRoleManagementPolicyRule 资源。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 2db7b8098b0663cbf102677352728d2e153280ba
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334526"
---
# <a name="list-effectiverules"></a><span data-ttu-id="3cb0a-103">列出 effectiveRules</span><span class="sxs-lookup"><span data-stu-id="3cb0a-103">List effectiveRules</span></span>
<span data-ttu-id="3cb0a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cb0a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3cb0a-105">从 effectiveRules 导航属性获取 unifiedRoleManagementPolicyRule 资源。</span><span class="sxs-lookup"><span data-stu-id="3cb0a-105">Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="3cb0a-106">权限</span><span class="sxs-lookup"><span data-stu-id="3cb0a-106">Permissions</span></span>
<span data-ttu-id="3cb0a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cb0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cb0a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cb0a-109">Permission type</span></span>|<span data-ttu-id="3cb0a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cb0a-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cb0a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cb0a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3cb0a-112">RoleManagementPolicy.Read.Directory、RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagementPolicy.ReadWrite.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="3cb0a-112">RoleManagementPolicy.Read.Directory, RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="3cb0a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cb0a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cb0a-114">不支持</span><span class="sxs-lookup"><span data-stu-id="3cb0a-114">Not supported</span></span>|
|<span data-ttu-id="3cb0a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cb0a-115">Application</span></span>|<span data-ttu-id="3cb0a-116">RoleManagement.Read.Directory、RoleManagement.Read.All、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="3cb0a-116">RoleManagement.Read.Directory, RoleManagement.Read.All, RoleManagement.ReadWrite.Directory</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cb0a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cb0a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3cb0a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3cb0a-118">Optional query parameters</span></span>
<span data-ttu-id="3cb0a-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3cb0a-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3cb0a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3cb0a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3cb0a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cb0a-121">Request headers</span></span>
|<span data-ttu-id="3cb0a-122">名称</span><span class="sxs-lookup"><span data-stu-id="3cb0a-122">Name</span></span>|<span data-ttu-id="3cb0a-123">说明</span><span class="sxs-lookup"><span data-stu-id="3cb0a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3cb0a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cb0a-124">Authorization</span></span>|<span data-ttu-id="3cb0a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3cb0a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cb0a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cb0a-127">Request body</span></span>
<span data-ttu-id="3cb0a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3cb0a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3cb0a-129">响应</span><span class="sxs-lookup"><span data-stu-id="3cb0a-129">Response</span></span>

<span data-ttu-id="3cb0a-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3cb0a-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3cb0a-131">示例</span><span class="sxs-lookup"><span data-stu-id="3cb0a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3cb0a-132">请求</span><span class="sxs-lookup"><span data-stu-id="3cb0a-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="3cb0a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="3cb0a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/effectiveRules
```
# <a name="c"></a>[<span data-ttu-id="3cb0a-134">C#</span><span class="sxs-lookup"><span data-stu-id="3cb0a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3cb0a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3cb0a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3cb0a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3cb0a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3cb0a-137">Java</span><span class="sxs-lookup"><span data-stu-id="3cb0a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="3cb0a-138">响应</span><span class="sxs-lookup"><span data-stu-id="3cb0a-138">Response</span></span>
<span data-ttu-id="3cb0a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3cb0a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.unifiedRoleManagementPolicyRule)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
      "target": {
        "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
      }
    }
  ]
}
```

