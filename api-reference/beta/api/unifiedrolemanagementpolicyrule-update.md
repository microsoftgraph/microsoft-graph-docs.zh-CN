---
title: 更新 unifiedRoleManagementPolicyRule
description: 更新 unifiedRoleManagementPolicyRule 对象的属性。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 263198c0ad771493bd34a7343a0c3f59e4c95735
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474246"
---
# <a name="update-unifiedrolemanagementpolicyrule"></a><span data-ttu-id="2dc21-103">更新 unifiedRoleManagementPolicyRule</span><span class="sxs-lookup"><span data-stu-id="2dc21-103">Update unifiedRoleManagementPolicyRule</span></span>
<span data-ttu-id="2dc21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2dc21-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2dc21-105">更新 [unifiedRoleManagementPolicyRule 对象](../resources/unifiedrolemanagementpolicyrule.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2dc21-105">Update the properties of an [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="2dc21-106">权限</span><span class="sxs-lookup"><span data-stu-id="2dc21-106">Permissions</span></span>
<span data-ttu-id="2dc21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2dc21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2dc21-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2dc21-109">Permission type</span></span>|<span data-ttu-id="2dc21-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2dc21-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2dc21-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2dc21-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2dc21-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="2dc21-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="2dc21-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2dc21-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2dc21-114">不支持</span><span class="sxs-lookup"><span data-stu-id="2dc21-114">Not supported</span></span>|
|<span data-ttu-id="2dc21-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2dc21-115">Application</span></span>|<span data-ttu-id="2dc21-116">不支持</span><span class="sxs-lookup"><span data-stu-id="2dc21-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="2dc21-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2dc21-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}
PATCH /policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/effectiveRules/{unifiedRoleManagementPolicyRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="2dc21-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2dc21-118">Request headers</span></span>
|<span data-ttu-id="2dc21-119">名称</span><span class="sxs-lookup"><span data-stu-id="2dc21-119">Name</span></span>|<span data-ttu-id="2dc21-120">说明</span><span class="sxs-lookup"><span data-stu-id="2dc21-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2dc21-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2dc21-121">Authorization</span></span>|<span data-ttu-id="2dc21-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2dc21-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2dc21-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2dc21-124">Content-Type</span></span>|<span data-ttu-id="2dc21-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2dc21-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2dc21-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2dc21-127">Request body</span></span>
<span data-ttu-id="2dc21-128">在请求正文中，提供 [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2dc21-128">In the request body, supply a JSON representation of the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object.</span></span>

<span data-ttu-id="2dc21-129">下表显示更新 [unifiedRoleManagementPolicyRule 时所需的属性](../resources/unifiedrolemanagementpolicyrule.md)。</span><span class="sxs-lookup"><span data-stu-id="2dc21-129">The following table shows the properties that are required when you update the [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md).</span></span>

|<span data-ttu-id="2dc21-130">属性</span><span class="sxs-lookup"><span data-stu-id="2dc21-130">Property</span></span>|<span data-ttu-id="2dc21-131">类型</span><span class="sxs-lookup"><span data-stu-id="2dc21-131">Type</span></span>|<span data-ttu-id="2dc21-132">说明</span><span class="sxs-lookup"><span data-stu-id="2dc21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2dc21-133">id</span><span class="sxs-lookup"><span data-stu-id="2dc21-133">id</span></span>|<span data-ttu-id="2dc21-134">String</span><span class="sxs-lookup"><span data-stu-id="2dc21-134">String</span></span>|<span data-ttu-id="2dc21-135">规则的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2dc21-135">Unique identifier for the rule.</span></span>|
|<span data-ttu-id="2dc21-136">target</span><span class="sxs-lookup"><span data-stu-id="2dc21-136">target</span></span>|[<span data-ttu-id="2dc21-137">unifiedRoleManagementPolicyRuleTarget</span><span class="sxs-lookup"><span data-stu-id="2dc21-137">unifiedRoleManagementPolicyRuleTarget</span></span>](../resources/unifiedrolemanagementpolicyruletarget.md)|<span data-ttu-id="2dc21-138">策略规则的目标。</span><span class="sxs-lookup"><span data-stu-id="2dc21-138">The target for the policy rule.</span></span>|



## <a name="response"></a><span data-ttu-id="2dc21-139">响应</span><span class="sxs-lookup"><span data-stu-id="2dc21-139">Response</span></span>

<span data-ttu-id="2dc21-140">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2dc21-140">If successful, this method returns a `200 OK` response code and an updated [unifiedRoleManagementPolicyRule](../resources/unifiedrolemanagementpolicyrule.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2dc21-141">示例</span><span class="sxs-lookup"><span data-stu-id="2dc21-141">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2dc21-142">请求</span><span class="sxs-lookup"><span data-stu-id="2dc21-142">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2dc21-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="2dc21-143">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="2dc21-144">C#</span><span class="sxs-lookup"><span data-stu-id="2dc21-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-unifiedrolemanagementpolicyrule-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2dc21-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2dc21-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-unifiedrolemanagementpolicyrule-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2dc21-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2dc21-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-unifiedrolemanagementpolicyrule-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2dc21-147">Java</span><span class="sxs-lookup"><span data-stu-id="2dc21-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-unifiedrolemanagementpolicyrule-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2dc21-148">响应</span><span class="sxs-lookup"><span data-stu-id="2dc21-148">Response</span></span>
<span data-ttu-id="2dc21-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2dc21-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.unifiedRoleManagementPolicyRule"
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
