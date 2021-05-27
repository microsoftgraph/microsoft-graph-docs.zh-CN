---
title: 获取 unifiedRoleManagementPolicyRule
description: 读取 unifiedRoleManagementPolicyRule 对象的属性和关系。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 76fb785c11f9ccbd321a6a44e314b05a4e0169f5
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680232"
---
# <a name="get-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="049de-103">获取 unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="049de-103">Get unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="049de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="049de-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="049de-105">读取 [unifiedRoleManagementPolicyRule 对象的属性和](../resources/unifiedrolemanagementpolicyrule.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="049de-105">Read the properties and relationships of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="049de-106">权限</span><span class="sxs-lookup"><span data-stu-id="049de-106">Permissions</span></span>
<span data-ttu-id="049de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="049de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="049de-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="049de-109">Permission type</span></span>|<span data-ttu-id="049de-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="049de-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="049de-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="049de-111">Delegated (work or school account)</span></span>|<span data-ttu-id="049de-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="049de-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="049de-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="049de-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="049de-114">不支持</span><span class="sxs-lookup"><span data-stu-id="049de-114">Not supported</span></span>|
|<span data-ttu-id="049de-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="049de-115">Application</span></span>|<span data-ttu-id="049de-116">PrivilegedAccess.Read.AzureAD</span><span class="sxs-lookup"><span data-stu-id="049de-116">PrivilegedAccess.Read.AzureAD</span></span>|

## <a name="http-request"></a><span data-ttu-id="049de-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="049de-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
GET /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="049de-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="049de-118">Optional query parameters</span></span>
<span data-ttu-id="049de-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="049de-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="049de-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="049de-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="049de-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="049de-121">Request headers</span></span>
|<span data-ttu-id="049de-122">名称</span><span class="sxs-lookup"><span data-stu-id="049de-122">Name</span></span>|<span data-ttu-id="049de-123">说明</span><span class="sxs-lookup"><span data-stu-id="049de-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="049de-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="049de-124">Authorization</span></span>|<span data-ttu-id="049de-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="049de-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="049de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="049de-127">Request body</span></span>
<span data-ttu-id="049de-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="049de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="049de-129">响应</span><span class="sxs-lookup"><span data-stu-id="049de-129">Response</span></span>

<span data-ttu-id="049de-130">如果成功，此方法在响应 `200 OK` 正文中返回 响应 [代码和 unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="049de-130">If successful, this method returns a `200 OK` response code and an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="049de-131">示例</span><span class="sxs-lookup"><span data-stu-id="049de-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="049de-132">请求</span><span class="sxs-lookup"><span data-stu-id="049de-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="049de-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="049de-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_unifiedrolemanagementpolicyrule"
}
-->
``` http
GET https://graph.microsoft.com/beta/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
```
# <a name="c"></a>[<span data-ttu-id="049de-134">C#</span><span class="sxs-lookup"><span data-stu-id="049de-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="049de-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="049de-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="049de-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="049de-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="049de-137">Java</span><span class="sxs-lookup"><span data-stu-id="049de-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="049de-138">响应</span><span class="sxs-lookup"><span data-stu-id="049de-138">Response</span></span>
<span data-ttu-id="049de-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="049de-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
    "target": {
      "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
    }
  }
}
```

