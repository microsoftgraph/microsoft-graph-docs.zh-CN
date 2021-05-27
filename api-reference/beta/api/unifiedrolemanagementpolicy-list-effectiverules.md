---
title: 列出 effectiveRules
description: 从 effectiveRules 导航属性获取 unifiedRoleManagementPolicyRule 资源。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 7dcc8a410d7ae47552c6c5d294334e64e1721124
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682340"
---
# <a name="list-effectiverules"></a><span data-ttu-id="37a77-103">列出 effectiveRules</span><span class="sxs-lookup"><span data-stu-id="37a77-103">List effectiveRules</span></span>
<span data-ttu-id="37a77-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37a77-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="37a77-105">从 effectiveRules 导航属性获取 unifiedRoleManagementPolicyRule 资源。</span><span class="sxs-lookup"><span data-stu-id="37a77-105">Get the unifiedRoleManagementPolicyRule resources from the effectiveRules navigation property.</span></span>

## <a name="permissions"></a><span data-ttu-id="37a77-106">权限</span><span class="sxs-lookup"><span data-stu-id="37a77-106">Permissions</span></span>
<span data-ttu-id="37a77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37a77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37a77-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="37a77-109">Permission type</span></span>|<span data-ttu-id="37a77-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37a77-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37a77-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37a77-111">Delegated (work or school account)</span></span>|<span data-ttu-id="37a77-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="37a77-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="37a77-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37a77-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37a77-114">不支持</span><span class="sxs-lookup"><span data-stu-id="37a77-114">Not supported</span></span>|
|<span data-ttu-id="37a77-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="37a77-115">Application</span></span>|<span data-ttu-id="37a77-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="37a77-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="37a77-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37a77-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules
```

## <a name="optional-query-parameters"></a><span data-ttu-id="37a77-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="37a77-118">Optional query parameters</span></span>
<span data-ttu-id="37a77-119">此方法支持所有 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="37a77-119">This method supports all of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="37a77-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="37a77-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="37a77-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="37a77-121">Request headers</span></span>
|<span data-ttu-id="37a77-122">名称</span><span class="sxs-lookup"><span data-stu-id="37a77-122">Name</span></span>|<span data-ttu-id="37a77-123">说明</span><span class="sxs-lookup"><span data-stu-id="37a77-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="37a77-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="37a77-124">Authorization</span></span>|<span data-ttu-id="37a77-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="37a77-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="37a77-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37a77-127">Request body</span></span>
<span data-ttu-id="37a77-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="37a77-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="37a77-129">响应</span><span class="sxs-lookup"><span data-stu-id="37a77-129">Response</span></span>

<span data-ttu-id="37a77-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="37a77-130">If successful, this method returns a `200 OK` response code and a collection of [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="37a77-131">示例</span><span class="sxs-lookup"><span data-stu-id="37a77-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="37a77-132">请求</span><span class="sxs-lookup"><span data-stu-id="37a77-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="37a77-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="37a77-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba/effectiveRules
```
# <a name="c"></a>[<span data-ttu-id="37a77-134">C#</span><span class="sxs-lookup"><span data-stu-id="37a77-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="37a77-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="37a77-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="37a77-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="37a77-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="37a77-137">Java</span><span class="sxs-lookup"><span data-stu-id="37a77-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="37a77-138">响应</span><span class="sxs-lookup"><span data-stu-id="37a77-138">Response</span></span>
<span data-ttu-id="37a77-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="37a77-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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

