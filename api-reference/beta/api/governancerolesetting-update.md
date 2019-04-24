---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
ms.openlocfilehash: f9c851f95df340693626ff82c960243eb2f85b54
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32503035"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="baa61-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="baa61-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="baa61-104">更新[governanceRoleSetting](../resources/governancerolesetting.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="baa61-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="baa61-105">权限</span><span class="sxs-lookup"><span data-stu-id="baa61-105">Permissions</span></span>
<span data-ttu-id="baa61-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="baa61-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="baa61-108">**注意:** 此 API 还要求请求者在资源上至少有`Active`一个管理员角色分配`owner` ( `user access administrator`或)。</span><span class="sxs-lookup"><span data-stu-id="baa61-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="baa61-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="baa61-109">Permission type</span></span>      | <span data-ttu-id="baa61-110">权限</span><span class="sxs-lookup"><span data-stu-id="baa61-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="baa61-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="baa61-111">Delegated (work or school account)</span></span> | <span data-ttu-id="baa61-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="baa61-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="baa61-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="baa61-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="baa61-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="baa61-114">Not supported.</span></span>    |
|<span data-ttu-id="baa61-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="baa61-115">Application</span></span> | <span data-ttu-id="baa61-116">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="baa61-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="baa61-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="baa61-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="baa61-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="baa61-118">Request headers</span></span>
| <span data-ttu-id="baa61-119">名称</span><span class="sxs-lookup"><span data-stu-id="baa61-119">Name</span></span>       | <span data-ttu-id="baa61-120">说明</span><span class="sxs-lookup"><span data-stu-id="baa61-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="baa61-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="baa61-121">Authorization</span></span>  | <span data-ttu-id="baa61-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="baa61-122">Bearer {code}</span></span>|
| <span data-ttu-id="baa61-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="baa61-123">Content-type</span></span>  | <span data-ttu-id="baa61-124">application/json</span><span class="sxs-lookup"><span data-stu-id="baa61-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="baa61-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="baa61-125">Request body</span></span>
<span data-ttu-id="baa61-126">在请求正文中, 提供需要更新的[governanceRuleSettings](../resources/governancerulesetting.md)的值。</span><span class="sxs-lookup"><span data-stu-id="baa61-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="baa61-127">属性</span><span class="sxs-lookup"><span data-stu-id="baa61-127">Property</span></span>     | <span data-ttu-id="baa61-128">类型</span><span class="sxs-lookup"><span data-stu-id="baa61-128">Type</span></span>   |<span data-ttu-id="baa61-129">说明</span><span class="sxs-lookup"><span data-stu-id="baa61-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baa61-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="baa61-130">adminEligibleSettings</span></span>|<span data-ttu-id="baa61-131">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="baa61-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="baa61-132">在管理员尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="baa61-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="baa61-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="baa61-133">adminMemberSettings</span></span>|<span data-ttu-id="baa61-134">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="baa61-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="baa61-135">在管理员尝试添加直接成员角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="baa61-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="baa61-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="baa61-136">userEligibleSettings</span></span>|<span data-ttu-id="baa61-137">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="baa61-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="baa61-138">用户尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="baa61-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="baa61-139">目前不支持这`pimforazurerbac`种情况, 在将来的方案中可能会用到。</span><span class="sxs-lookup"><span data-stu-id="baa61-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="baa61-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="baa61-140">userMemberSettings</span></span>|<span data-ttu-id="baa61-141">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="baa61-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="baa61-142">用户尝试激活他的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="baa61-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="baa61-143">响应</span><span class="sxs-lookup"><span data-stu-id="baa61-143">Response</span></span>
<span data-ttu-id="baa61-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="baa61-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="baa61-146">错误代码</span><span class="sxs-lookup"><span data-stu-id="baa61-146">Error codes</span></span>
<span data-ttu-id="baa61-147">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="baa61-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="baa61-148">此外, 它还返回以下自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="baa61-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="baa61-149">错误代码</span><span class="sxs-lookup"><span data-stu-id="baa61-149">Error code</span></span>     | <span data-ttu-id="baa61-150">错误消息</span><span class="sxs-lookup"><span data-stu-id="baa61-150">Error message</span></span>         | <span data-ttu-id="baa61-151">详细信息</span><span class="sxs-lookup"><span data-stu-id="baa61-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="baa61-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="baa61-152">400 BadRequest</span></span>| <span data-ttu-id="baa61-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="baa61-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="baa61-154">[governanceRoleSetting](../resources/governancerolesetting.md)在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="baa61-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="baa61-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="baa61-155">400 BadRequest</span></span>| <span data-ttu-id="baa61-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="baa61-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="baa61-157">请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值无效。</span><span class="sxs-lookup"><span data-stu-id="baa61-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="baa61-158">示例</span><span class="sxs-lookup"><span data-stu-id="baa61-158">Example</span></span> 
<span data-ttu-id="baa61-159">本示例更新订阅 Wingtip 玩具-生产版中的自定义角色3的角色设置。</span><span class="sxs-lookup"><span data-stu-id="baa61-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="baa61-160">请求</span><span class="sxs-lookup"><span data-stu-id="baa61-160">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_governancerolesetting"
}-->
```http
PATCH https://graph.microsoft.com/beta/privilegedAccess/pimforazurerbac/roleSettings/5fb5aef8-1081-4b8e-bb16-9d5d0385bab5
Content-type: application/json
Content-length: 350

{
  "adminEligibleSettings":[{"ruleIdentifier":"ExpirationRule","setting":"{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}"}]
}
```
##### <a name="response"></a><span data-ttu-id="baa61-161">响应</span><span class="sxs-lookup"><span data-stu-id="baa61-161">Response</span></span>
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
    "Error: /api-reference/beta/api/governancerolesetting-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
