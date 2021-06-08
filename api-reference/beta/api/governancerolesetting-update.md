---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 7a301bb12271f6b31e7fef4dac565881139de994
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787259"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="06a71-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="06a71-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="06a71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06a71-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06a71-105">更新 [governanceRoleSetting 的属性](../resources/governancerolesetting.md)。</span><span class="sxs-lookup"><span data-stu-id="06a71-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06a71-106">权限</span><span class="sxs-lookup"><span data-stu-id="06a71-106">Permissions</span></span>
<span data-ttu-id="06a71-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="06a71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="06a71-109">**注意：** 此 API 还要求请求者至少具有一个角色分配 (`Active` `owner` 或) `user access administrator` 管理员。</span><span class="sxs-lookup"><span data-stu-id="06a71-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="06a71-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="06a71-110">Permission type</span></span>      | <span data-ttu-id="06a71-111">权限</span><span class="sxs-lookup"><span data-stu-id="06a71-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="06a71-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06a71-112">Delegated (work or school account)</span></span> | <span data-ttu-id="06a71-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="06a71-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="06a71-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06a71-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06a71-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a71-115">Not supported.</span></span>    |
|<span data-ttu-id="06a71-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="06a71-116">Application</span></span> | <span data-ttu-id="06a71-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a71-117">Not supported.</span></span> |
### <a name="azure-resources"></a><span data-ttu-id="06a71-118">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="06a71-118">Azure resources</span></span>

| <span data-ttu-id="06a71-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="06a71-119">Permission type</span></span> | <span data-ttu-id="06a71-120">权限</span><span class="sxs-lookup"><span data-stu-id="06a71-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="06a71-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06a71-121">Delegated (work or school account)</span></span> | <span data-ttu-id="06a71-122">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="06a71-122">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="06a71-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06a71-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06a71-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a71-124">Not supported.</span></span> |
| <span data-ttu-id="06a71-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="06a71-125">Application</span></span> | <span data-ttu-id="06a71-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a71-126">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="06a71-127">Azure AD</span><span class="sxs-lookup"><span data-stu-id="06a71-127">Azure AD</span></span>

| <span data-ttu-id="06a71-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="06a71-128">Permission type</span></span> | <span data-ttu-id="06a71-129">权限</span><span class="sxs-lookup"><span data-stu-id="06a71-129">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="06a71-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06a71-130">Delegated (work or school account)</span></span> | <span data-ttu-id="06a71-131">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="06a71-131">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="06a71-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06a71-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06a71-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a71-133">Not supported.</span></span> |
| <span data-ttu-id="06a71-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="06a71-134">Application</span></span> | <span data-ttu-id="06a71-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a71-135">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="06a71-136">组</span><span class="sxs-lookup"><span data-stu-id="06a71-136">Groups</span></span>

|<span data-ttu-id="06a71-137">权限类型</span><span class="sxs-lookup"><span data-stu-id="06a71-137">Permission type</span></span> | <span data-ttu-id="06a71-138">权限</span><span class="sxs-lookup"><span data-stu-id="06a71-138">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="06a71-139">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06a71-139">Delegated (work or school account)</span></span> | <span data-ttu-id="06a71-140">PrivilegedAccess.ReadWrite.AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="06a71-140">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="06a71-141">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06a71-141">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="06a71-142">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a71-142">Not supported.</span></span> |
| <span data-ttu-id="06a71-143">应用程序</span><span class="sxs-lookup"><span data-stu-id="06a71-143">Application</span></span> | <span data-ttu-id="06a71-144">不支持。</span><span class="sxs-lookup"><span data-stu-id="06a71-144">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="06a71-145">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06a71-145">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="06a71-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="06a71-146">Request headers</span></span>
| <span data-ttu-id="06a71-147">名称</span><span class="sxs-lookup"><span data-stu-id="06a71-147">Name</span></span>       | <span data-ttu-id="06a71-148">说明</span><span class="sxs-lookup"><span data-stu-id="06a71-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="06a71-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="06a71-149">Authorization</span></span>  | <span data-ttu-id="06a71-150">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="06a71-150">Bearer {token}</span></span>|
| <span data-ttu-id="06a71-151">Content-type</span><span class="sxs-lookup"><span data-stu-id="06a71-151">Content-type</span></span>  | <span data-ttu-id="06a71-152">application/json</span><span class="sxs-lookup"><span data-stu-id="06a71-152">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="06a71-153">请求正文</span><span class="sxs-lookup"><span data-stu-id="06a71-153">Request body</span></span>
<span data-ttu-id="06a71-154">在请求正文中，提供 [需要更新的 governanceRuleSettings](../resources/governancerulesetting.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="06a71-154">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="06a71-155">属性</span><span class="sxs-lookup"><span data-stu-id="06a71-155">Property</span></span>     | <span data-ttu-id="06a71-156">类型</span><span class="sxs-lookup"><span data-stu-id="06a71-156">Type</span></span>   |<span data-ttu-id="06a71-157">说明</span><span class="sxs-lookup"><span data-stu-id="06a71-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="06a71-158">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="06a71-158">adminEligibleSettings</span></span>|<span data-ttu-id="06a71-159">[governanceRuleSetting](../resources/governancerulesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06a71-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="06a71-160">管理员尝试添加符合条件的规则时评估的规则角色分配。</span><span class="sxs-lookup"><span data-stu-id="06a71-160">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="06a71-161">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="06a71-161">adminMemberSettings</span></span>|<span data-ttu-id="06a71-162">[governanceRuleSetting](../resources/governancerulesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06a71-162">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="06a71-163">管理员尝试向用户添加直接成员时评估的规则角色分配。</span><span class="sxs-lookup"><span data-stu-id="06a71-163">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="06a71-164">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="06a71-164">userEligibleSettings</span></span>|<span data-ttu-id="06a71-165">[governanceRuleSetting](../resources/governancerulesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06a71-165">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="06a71-166">用户尝试添加符合条件的规则时评估的规则角色分配。</span><span class="sxs-lookup"><span data-stu-id="06a71-166">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="06a71-167">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="06a71-167">userMemberSettings</span></span>|<span data-ttu-id="06a71-168">[governanceRuleSetting](../resources/governancerulesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="06a71-168">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="06a71-169">用户尝试激活其密码时评估的规则角色分配。</span><span class="sxs-lookup"><span data-stu-id="06a71-169">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="06a71-170">响应</span><span class="sxs-lookup"><span data-stu-id="06a71-170">Response</span></span>
<span data-ttu-id="06a71-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="06a71-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="06a71-173">错误代码</span><span class="sxs-lookup"><span data-stu-id="06a71-173">Error codes</span></span>
<span data-ttu-id="06a71-174">此 API 返回标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="06a71-174">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="06a71-175">此外，它返回以下自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="06a71-175">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="06a71-176">错误代码</span><span class="sxs-lookup"><span data-stu-id="06a71-176">Error code</span></span>     | <span data-ttu-id="06a71-177">错误消息</span><span class="sxs-lookup"><span data-stu-id="06a71-177">Error message</span></span>         | <span data-ttu-id="06a71-178">详细信息</span><span class="sxs-lookup"><span data-stu-id="06a71-178">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="06a71-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="06a71-179">400 BadRequest</span></span>| <span data-ttu-id="06a71-180">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="06a71-180">RoleSettingNotFound</span></span>   | <span data-ttu-id="06a71-181">[governanceRoleSetting](../resources/governancerolesetting.md)在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="06a71-181">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="06a71-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="06a71-182">400 BadRequest</span></span>| <span data-ttu-id="06a71-183">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="06a71-183">InvalidRoleSetting</span></span>    | <span data-ttu-id="06a71-184">请求 [正文中提供的 governanceRuleSettings](../resources/governancerulesetting.md) 值无效。</span><span class="sxs-lookup"><span data-stu-id="06a71-184">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="06a71-185">示例</span><span class="sxs-lookup"><span data-stu-id="06a71-185">Example</span></span> 
<span data-ttu-id="06a71-186">本示例更新订阅 Wingtip Toys - Prod 中自定义角色 3 的角色设置。</span><span class="sxs-lookup"><span data-stu-id="06a71-186">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="06a71-187">请求</span><span class="sxs-lookup"><span data-stu-id="06a71-187">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="06a71-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="06a71-188">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/azureResources/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
   "adminEligibleSettings":[
      {
         "ruleIdentifier":"ExpirationRule",
         "setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"
      }
   ]
}
```
# <a name="c"></a>[<span data-ttu-id="06a71-189">C#</span><span class="sxs-lookup"><span data-stu-id="06a71-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="06a71-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="06a71-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="06a71-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="06a71-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="06a71-192">Java</span><span class="sxs-lookup"><span data-stu-id="06a71-192">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="06a71-193">响应</span><span class="sxs-lookup"><span data-stu-id="06a71-193">Response</span></span>
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


