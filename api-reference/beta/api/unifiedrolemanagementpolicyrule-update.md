---
title: 更新 unifiedRoleManagementPolicyRule
description: 更新 unifiedRoleManagementPolicyRule 对象的属性。
author: shauliu
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 4d70b105f3516547c851e8be21be18b15009439a
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334694"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="6fb13-103">更新 unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="6fb13-103">Update unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="6fb13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6fb13-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6fb13-105">更新 [unifiedRoleManagementPolicyRule 对象](../resources/unifiedrolemanagementpolicyrule.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6fb13-105">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="6fb13-106">权限</span><span class="sxs-lookup"><span data-stu-id="6fb13-106">Permissions</span></span>
<span data-ttu-id="6fb13-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6fb13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6fb13-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6fb13-109">Permission type</span></span>|<span data-ttu-id="6fb13-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6fb13-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6fb13-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6fb13-112">RoleManagementPolicy.ReadWrite.Directory、RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="6fb13-112">RoleManagementPolicy.ReadWrite.Directory, RoleManagement.ReadWrite.Directory</span></span>|
|<span data-ttu-id="6fb13-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6fb13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6fb13-114">不支持</span><span class="sxs-lookup"><span data-stu-id="6fb13-114">Not supported</span></span>|
|<span data-ttu-id="6fb13-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6fb13-115">Application</span></span>|<span data-ttu-id="6fb13-116">不支持</span><span class="sxs-lookup"><span data-stu-id="6fb13-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="6fb13-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6fb13-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="6fb13-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6fb13-118">Request headers</span></span>
|<span data-ttu-id="6fb13-119">名称</span><span class="sxs-lookup"><span data-stu-id="6fb13-119">Name</span></span>|<span data-ttu-id="6fb13-120">说明</span><span class="sxs-lookup"><span data-stu-id="6fb13-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6fb13-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6fb13-121">Authorization</span></span>|<span data-ttu-id="6fb13-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6fb13-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6fb13-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6fb13-124">Content-Type</span></span>|<span data-ttu-id="6fb13-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6fb13-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6fb13-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6fb13-127">Request body</span></span>
<span data-ttu-id="6fb13-128">在请求正文中，提供 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6fb13-128">In the request body, supply a JSON representation of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

<span data-ttu-id="6fb13-129">下表显示更新 [unifiedRoleManagementPolicyRule 时所需的属性](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="6fb13-129">The following table shows the properties that are required when you update the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

|<span data-ttu-id="6fb13-130">属性</span><span class="sxs-lookup"><span data-stu-id="6fb13-130">Property</span></span>|<span data-ttu-id="6fb13-131">类型</span><span class="sxs-lookup"><span data-stu-id="6fb13-131">Type</span></span>|<span data-ttu-id="6fb13-132">说明</span><span class="sxs-lookup"><span data-stu-id="6fb13-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6fb13-133">id</span><span class="sxs-lookup"><span data-stu-id="6fb13-133">id</span></span>|<span data-ttu-id="6fb13-134">String</span><span class="sxs-lookup"><span data-stu-id="6fb13-134">String</span></span>|<span data-ttu-id="6fb13-135">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6fb13-135">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="6fb13-136">target</span><span class="sxs-lookup"><span data-stu-id="6fb13-136">target</span></span>|[<span data-ttu-id="6fb13-137">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="6fb13-137">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="6fb13-138">策略规则的目标。</span><span class="sxs-lookup"><span data-stu-id="6fb13-138">The target for the policy rule.</span></span>|



## <a name="response"></a><span data-ttu-id="6fb13-139">响应</span><span class="sxs-lookup"><span data-stu-id="6fb13-139">Response</span></span>

<span data-ttu-id="6fb13-140">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6fb13-140">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6fb13-141">示例</span><span class="sxs-lookup"><span data-stu-id="6fb13-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6fb13-142">请求</span><span class="sxs-lookup"><span data-stu-id="6fb13-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="6fb13-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6fb13-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_unifiedrolemanagementpolicyrule"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
Content-Type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```
# <a name="c"></a>[<span data-ttu-id="6fb13-144">C#</span><span class="sxs-lookup"><span data-stu-id="6fb13-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6fb13-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6fb13-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6fb13-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6fb13-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6fb13-147">Java</span><span class="sxs-lookup"><span data-stu-id="6fb13-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="6fb13-148">响应</span><span class="sxs-lookup"><span data-stu-id="6fb13-148">Response</span></span>
<span data-ttu-id="6fb13-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6fb13-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
```http
HTTP/1.1 204 OK

```
<!--
{
  "@odata.type": "#microsoft.graph.unifiedRoleManagementPolicyRule",
  "id": "ba9cc2d6-c2d6-ba9c-d6c2-9cbad6c29cba",
  "target": {
    "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRuleTarget"
  }
}
```
-->
