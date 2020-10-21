---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 3ae917f9b92ee743173842b3ed9ccf2a2bea3edd
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634858"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="a5bef-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="a5bef-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="a5bef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a5bef-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a5bef-105">更新 [governanceRoleSetting](../resources/governancerolesetting.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="a5bef-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5bef-106">权限</span><span class="sxs-lookup"><span data-stu-id="a5bef-106">Permissions</span></span>
<span data-ttu-id="a5bef-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference#privileged-access-permissions)。</span><span class="sxs-lookup"><span data-stu-id="a5bef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference#privileged-access-permissions).</span></span>

><span data-ttu-id="a5bef-109">**注意：** 此 API 还要求请求者在资源上至少有一个 `Active` 管理员角色分配 (`owner` 或 `user access administrator`) 。</span><span class="sxs-lookup"><span data-stu-id="a5bef-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="a5bef-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5bef-110">Permission type</span></span>      | <span data-ttu-id="a5bef-111">权限</span><span class="sxs-lookup"><span data-stu-id="a5bef-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5bef-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5bef-112">Delegated (work or school account)</span></span> | <span data-ttu-id="a5bef-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a5bef-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="a5bef-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5bef-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5bef-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5bef-115">Not supported.</span></span>    |
|<span data-ttu-id="a5bef-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5bef-116">Application</span></span> | <span data-ttu-id="a5bef-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5bef-117">Not supported.</span></span> |
### <a name="azure-resources"></a><span data-ttu-id="a5bef-118">Azure 资源</span><span class="sxs-lookup"><span data-stu-id="a5bef-118">Azure resources</span></span>

| <span data-ttu-id="a5bef-119">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5bef-119">Permission type</span></span> | <span data-ttu-id="a5bef-120">权限</span><span class="sxs-lookup"><span data-stu-id="a5bef-120">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="a5bef-121">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5bef-121">Delegated (work or school account)</span></span> | <span data-ttu-id="a5bef-122">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="a5bef-122">PrivilegedAccess.ReadWrite.AzureResources</span></span> |
| <span data-ttu-id="a5bef-123">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5bef-123">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5bef-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5bef-124">Not supported.</span></span> |
| <span data-ttu-id="a5bef-125">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5bef-125">Application</span></span> | <span data-ttu-id="a5bef-126">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5bef-126">Not supported.</span></span> |

### <a name="azure-ad"></a><span data-ttu-id="a5bef-127">Azure AD</span><span class="sxs-lookup"><span data-stu-id="a5bef-127">Azure AD</span></span>

| <span data-ttu-id="a5bef-128">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5bef-128">Permission type</span></span> | <span data-ttu-id="a5bef-129">权限</span><span class="sxs-lookup"><span data-stu-id="a5bef-129">Permissions</span></span> |
|:--------------- |:----------- |
| <span data-ttu-id="a5bef-130">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5bef-130">Delegated (work or school account)</span></span> | <span data-ttu-id="a5bef-131">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="a5bef-131">PrivilegedAccess.ReadWrite.AzureAD</span></span> |
| <span data-ttu-id="a5bef-132">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5bef-132">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5bef-133">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5bef-133">Not supported.</span></span> |
| <span data-ttu-id="a5bef-134">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5bef-134">Application</span></span> | <span data-ttu-id="a5bef-135">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5bef-135">Not supported.</span></span> |

### <a name="groups"></a><span data-ttu-id="a5bef-136">组</span><span class="sxs-lookup"><span data-stu-id="a5bef-136">Groups</span></span>

|<span data-ttu-id="a5bef-137">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5bef-137">Permission type</span></span> | <span data-ttu-id="a5bef-138">权限</span><span class="sxs-lookup"><span data-stu-id="a5bef-138">Permissions</span></span> |
|:-------------- |:----------- |
| <span data-ttu-id="a5bef-139">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5bef-139">Delegated (work or school account)</span></span> | <span data-ttu-id="a5bef-140">PrivilegedAccess AzureADGroups</span><span class="sxs-lookup"><span data-stu-id="a5bef-140">PrivilegedAccess.ReadWrite.AzureADGroups</span></span> |
| <span data-ttu-id="a5bef-141">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5bef-141">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5bef-142">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5bef-142">Not supported.</span></span> |
| <span data-ttu-id="a5bef-143">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5bef-143">Application</span></span> | <span data-ttu-id="a5bef-144">不支持。</span><span class="sxs-lookup"><span data-stu-id="a5bef-144">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a5bef-145">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5bef-145">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a5bef-146">请求标头</span><span class="sxs-lookup"><span data-stu-id="a5bef-146">Request headers</span></span>
| <span data-ttu-id="a5bef-147">名称</span><span class="sxs-lookup"><span data-stu-id="a5bef-147">Name</span></span>       | <span data-ttu-id="a5bef-148">说明</span><span class="sxs-lookup"><span data-stu-id="a5bef-148">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a5bef-149">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5bef-149">Authorization</span></span>  | <span data-ttu-id="a5bef-150">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="a5bef-150">Bearer {token}</span></span>|
| <span data-ttu-id="a5bef-151">Content-type</span><span class="sxs-lookup"><span data-stu-id="a5bef-151">Content-type</span></span>  | <span data-ttu-id="a5bef-152">application/json</span><span class="sxs-lookup"><span data-stu-id="a5bef-152">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="a5bef-153">请求正文</span><span class="sxs-lookup"><span data-stu-id="a5bef-153">Request body</span></span>
<span data-ttu-id="a5bef-154">在请求正文中，提供需要更新的 [governanceRuleSettings](../resources/governancerulesetting.md) 的值。</span><span class="sxs-lookup"><span data-stu-id="a5bef-154">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="a5bef-155">属性</span><span class="sxs-lookup"><span data-stu-id="a5bef-155">Property</span></span>     | <span data-ttu-id="a5bef-156">类型</span><span class="sxs-lookup"><span data-stu-id="a5bef-156">Type</span></span>   |<span data-ttu-id="a5bef-157">说明</span><span class="sxs-lookup"><span data-stu-id="a5bef-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5bef-158">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="a5bef-158">adminEligibleSettings</span></span>|<span data-ttu-id="a5bef-159">[governanceRuleSetting](../resources/governancerulesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5bef-159">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="a5bef-160">在管理员尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="a5bef-160">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="a5bef-161">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="a5bef-161">adminMemberSettings</span></span>|<span data-ttu-id="a5bef-162">[governanceRuleSetting](../resources/governancerulesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5bef-162">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="a5bef-163">在管理员尝试添加直接成员角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="a5bef-163">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="a5bef-164">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="a5bef-164">userEligibleSettings</span></span>|<span data-ttu-id="a5bef-165">[governanceRuleSetting](../resources/governancerulesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5bef-165">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="a5bef-166">用户尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="a5bef-166">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="a5bef-167">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="a5bef-167">userMemberSettings</span></span>|<span data-ttu-id="a5bef-168">[governanceRuleSetting](../resources/governancerulesetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a5bef-168">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="a5bef-169">用户尝试激活他的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="a5bef-169">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="a5bef-170">响应</span><span class="sxs-lookup"><span data-stu-id="a5bef-170">Response</span></span>
<span data-ttu-id="a5bef-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a5bef-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="a5bef-173">错误代码</span><span class="sxs-lookup"><span data-stu-id="a5bef-173">Error codes</span></span>
<span data-ttu-id="a5bef-174">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="a5bef-174">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="a5bef-175">此外，它还返回以下自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="a5bef-175">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="a5bef-176">错误代码</span><span class="sxs-lookup"><span data-stu-id="a5bef-176">Error code</span></span>     | <span data-ttu-id="a5bef-177">错误消息</span><span class="sxs-lookup"><span data-stu-id="a5bef-177">Error message</span></span>         | <span data-ttu-id="a5bef-178">详细信息</span><span class="sxs-lookup"><span data-stu-id="a5bef-178">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="a5bef-179">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a5bef-179">400 BadRequest</span></span>| <span data-ttu-id="a5bef-180">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="a5bef-180">RoleSettingNotFound</span></span>   | <span data-ttu-id="a5bef-181">[GovernanceRoleSetting](../resources/governancerolesetting.md)在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="a5bef-181">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="a5bef-182">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="a5bef-182">400 BadRequest</span></span>| <span data-ttu-id="a5bef-183">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="a5bef-183">InvalidRoleSetting</span></span>    | <span data-ttu-id="a5bef-184">请求正文中提供的 [governanceRuleSettings](../resources/governancerulesetting.md) 值无效。</span><span class="sxs-lookup"><span data-stu-id="a5bef-184">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="a5bef-185">示例</span><span class="sxs-lookup"><span data-stu-id="a5bef-185">Example</span></span> 
<span data-ttu-id="a5bef-186">本示例更新订阅 Wingtip 玩具-生产版中的自定义角色3的角色设置。</span><span class="sxs-lookup"><span data-stu-id="a5bef-186">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="a5bef-187">请求</span><span class="sxs-lookup"><span data-stu-id="a5bef-187">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a5bef-188">HTTP</span><span class="sxs-lookup"><span data-stu-id="a5bef-188">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="a5bef-189">C#</span><span class="sxs-lookup"><span data-stu-id="a5bef-189">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a5bef-190">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a5bef-190">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a5bef-191">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a5bef-191">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a5bef-192">响应</span><span class="sxs-lookup"><span data-stu-id="a5bef-192">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
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


