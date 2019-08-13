---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
doc_type: apiPageType
author: ''
ms.prod: ''
ms.openlocfilehash: 71351c6ae478fd26f87024550de1d953911f5de6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326483"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="bc335-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bc335-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bc335-104">更新[governanceRoleSetting](../resources/governancerolesetting.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="bc335-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="bc335-105">权限</span><span class="sxs-lookup"><span data-stu-id="bc335-105">Permissions</span></span>
<span data-ttu-id="bc335-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bc335-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="bc335-108">**注意:** 此 API 还要求请求者在资源上至少有`Active`一个管理员角色分配`owner` ( `user access administrator`或)。</span><span class="sxs-lookup"><span data-stu-id="bc335-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="bc335-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="bc335-109">Permission type</span></span>      | <span data-ttu-id="bc335-110">权限</span><span class="sxs-lookup"><span data-stu-id="bc335-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bc335-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bc335-111">Delegated (work or school account)</span></span> | <span data-ttu-id="bc335-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="bc335-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="bc335-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bc335-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bc335-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc335-114">Not supported.</span></span>    |
|<span data-ttu-id="bc335-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="bc335-115">Application</span></span> | <span data-ttu-id="bc335-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bc335-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="bc335-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bc335-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="bc335-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bc335-118">Request headers</span></span>
| <span data-ttu-id="bc335-119">名称</span><span class="sxs-lookup"><span data-stu-id="bc335-119">Name</span></span>       | <span data-ttu-id="bc335-120">说明</span><span class="sxs-lookup"><span data-stu-id="bc335-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bc335-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bc335-121">Authorization</span></span>  | <span data-ttu-id="bc335-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="bc335-122">Bearer {code}</span></span>|
| <span data-ttu-id="bc335-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="bc335-123">Content-type</span></span>  | <span data-ttu-id="bc335-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bc335-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="bc335-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bc335-125">Request body</span></span>
<span data-ttu-id="bc335-126">在请求正文中, 提供需要更新的[governanceRuleSettings](../resources/governancerulesetting.md)的值。</span><span class="sxs-lookup"><span data-stu-id="bc335-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="bc335-127">属性</span><span class="sxs-lookup"><span data-stu-id="bc335-127">Property</span></span>     | <span data-ttu-id="bc335-128">类型</span><span class="sxs-lookup"><span data-stu-id="bc335-128">Type</span></span>   |<span data-ttu-id="bc335-129">说明</span><span class="sxs-lookup"><span data-stu-id="bc335-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc335-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="bc335-130">adminEligibleSettings</span></span>|<span data-ttu-id="bc335-131">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="bc335-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bc335-132">在管理员尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="bc335-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="bc335-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bc335-133">adminMemberSettings</span></span>|<span data-ttu-id="bc335-134">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="bc335-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bc335-135">在管理员尝试添加直接成员角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="bc335-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="bc335-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="bc335-136">userEligibleSettings</span></span>|<span data-ttu-id="bc335-137">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="bc335-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bc335-138">用户尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="bc335-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="bc335-139">目前不支持这`pimforazurerbac`种情况, 在将来的方案中可能会用到。</span><span class="sxs-lookup"><span data-stu-id="bc335-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="bc335-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="bc335-140">userMemberSettings</span></span>|<span data-ttu-id="bc335-141">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="bc335-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="bc335-142">用户尝试激活他的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="bc335-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="bc335-143">响应</span><span class="sxs-lookup"><span data-stu-id="bc335-143">Response</span></span>
<span data-ttu-id="bc335-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="bc335-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="bc335-146">错误代码</span><span class="sxs-lookup"><span data-stu-id="bc335-146">Error codes</span></span>
<span data-ttu-id="bc335-147">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="bc335-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="bc335-148">此外, 它还返回以下自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="bc335-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="bc335-149">错误代码</span><span class="sxs-lookup"><span data-stu-id="bc335-149">Error code</span></span>     | <span data-ttu-id="bc335-150">错误消息</span><span class="sxs-lookup"><span data-stu-id="bc335-150">Error message</span></span>         | <span data-ttu-id="bc335-151">详细信息</span><span class="sxs-lookup"><span data-stu-id="bc335-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="bc335-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bc335-152">400 BadRequest</span></span>| <span data-ttu-id="bc335-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="bc335-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="bc335-154">[GovernanceRoleSetting](../resources/governancerolesetting.md)在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="bc335-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="bc335-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="bc335-155">400 BadRequest</span></span>| <span data-ttu-id="bc335-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="bc335-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="bc335-157">请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值无效。</span><span class="sxs-lookup"><span data-stu-id="bc335-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="bc335-158">示例</span><span class="sxs-lookup"><span data-stu-id="bc335-158">Example</span></span> 
<span data-ttu-id="bc335-159">本示例更新订阅 Wingtip 玩具-生产版中的自定义角色3的角色设置。</span><span class="sxs-lookup"><span data-stu-id="bc335-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="bc335-160">请求</span><span class="sxs-lookup"><span data-stu-id="bc335-160">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bc335-161">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="bc335-161">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="bc335-162">C#</span><span class="sxs-lookup"><span data-stu-id="bc335-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bc335-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bc335-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bc335-164">目标-C</span><span class="sxs-lookup"><span data-stu-id="bc335-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bc335-165">Java</span><span class="sxs-lookup"><span data-stu-id="bc335-165">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-governancerolesetting-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bc335-166">响应</span><span class="sxs-lookup"><span data-stu-id="bc335-166">Response</span></span>
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
