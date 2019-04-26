---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
ms.openlocfilehash: d002317a4bf626f9a60cf98f6bd73b2075bf5727
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33329670"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="f1337-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="f1337-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f1337-104">更新[governanceRoleSetting](../resources/governancerolesetting.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="f1337-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="f1337-105">权限</span><span class="sxs-lookup"><span data-stu-id="f1337-105">Permissions</span></span>
<span data-ttu-id="f1337-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f1337-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f1337-108">**注意:** 此 API 还要求请求者在资源上至少有`Active`一个管理员角色分配`owner` ( `user access administrator`或)。</span><span class="sxs-lookup"><span data-stu-id="f1337-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="f1337-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f1337-109">Permission type</span></span>      | <span data-ttu-id="f1337-110">权限</span><span class="sxs-lookup"><span data-stu-id="f1337-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f1337-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f1337-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f1337-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="f1337-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="f1337-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f1337-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f1337-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f1337-114">Not supported.</span></span>    |
|<span data-ttu-id="f1337-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f1337-115">Application</span></span> | <span data-ttu-id="f1337-116">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="f1337-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="f1337-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f1337-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="f1337-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f1337-118">Request headers</span></span>
| <span data-ttu-id="f1337-119">名称</span><span class="sxs-lookup"><span data-stu-id="f1337-119">Name</span></span>       | <span data-ttu-id="f1337-120">说明</span><span class="sxs-lookup"><span data-stu-id="f1337-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="f1337-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f1337-121">Authorization</span></span>  | <span data-ttu-id="f1337-122">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="f1337-122">Bearer {code}</span></span>|
| <span data-ttu-id="f1337-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="f1337-123">Content-type</span></span>  | <span data-ttu-id="f1337-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f1337-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="f1337-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f1337-125">Request body</span></span>
<span data-ttu-id="f1337-126">在请求正文中, 提供需要更新的[governanceRuleSettings](../resources/governancerulesetting.md)的值。</span><span class="sxs-lookup"><span data-stu-id="f1337-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="f1337-127">属性</span><span class="sxs-lookup"><span data-stu-id="f1337-127">Property</span></span>     | <span data-ttu-id="f1337-128">类型</span><span class="sxs-lookup"><span data-stu-id="f1337-128">Type</span></span>   |<span data-ttu-id="f1337-129">说明</span><span class="sxs-lookup"><span data-stu-id="f1337-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f1337-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="f1337-130">adminEligibleSettings</span></span>|<span data-ttu-id="f1337-131">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1337-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f1337-132">在管理员尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="f1337-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="f1337-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="f1337-133">adminMemberSettings</span></span>|<span data-ttu-id="f1337-134">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1337-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f1337-135">在管理员尝试添加直接成员角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="f1337-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="f1337-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="f1337-136">userEligibleSettings</span></span>|<span data-ttu-id="f1337-137">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1337-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f1337-138">用户尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="f1337-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="f1337-139">目前不支持这`pimforazurerbac`种情况, 在将来的方案中可能会用到。</span><span class="sxs-lookup"><span data-stu-id="f1337-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="f1337-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="f1337-140">userMemberSettings</span></span>|<span data-ttu-id="f1337-141">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="f1337-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="f1337-142">用户尝试激活他的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="f1337-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="f1337-143">响应</span><span class="sxs-lookup"><span data-stu-id="f1337-143">Response</span></span>
<span data-ttu-id="f1337-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="f1337-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="f1337-146">错误代码</span><span class="sxs-lookup"><span data-stu-id="f1337-146">Error codes</span></span>
<span data-ttu-id="f1337-147">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="f1337-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="f1337-148">此外, 它还返回以下自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="f1337-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="f1337-149">错误代码</span><span class="sxs-lookup"><span data-stu-id="f1337-149">Error code</span></span>     | <span data-ttu-id="f1337-150">错误消息</span><span class="sxs-lookup"><span data-stu-id="f1337-150">Error message</span></span>         | <span data-ttu-id="f1337-151">详细信息</span><span class="sxs-lookup"><span data-stu-id="f1337-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="f1337-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f1337-152">400 BadRequest</span></span>| <span data-ttu-id="f1337-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="f1337-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="f1337-154">[governanceRoleSetting](../resources/governancerolesetting.md)在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="f1337-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="f1337-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="f1337-155">400 BadRequest</span></span>| <span data-ttu-id="f1337-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="f1337-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="f1337-157">请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值无效。</span><span class="sxs-lookup"><span data-stu-id="f1337-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="f1337-158">示例</span><span class="sxs-lookup"><span data-stu-id="f1337-158">Example</span></span> 
<span data-ttu-id="f1337-159">本示例更新订阅 Wingtip 玩具-生产版中的自定义角色3的角色设置。</span><span class="sxs-lookup"><span data-stu-id="f1337-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="f1337-160">请求</span><span class="sxs-lookup"><span data-stu-id="f1337-160">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="f1337-161">响应</span><span class="sxs-lookup"><span data-stu-id="f1337-161">Response</span></span>
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
  "suppressions": []
}
-->
