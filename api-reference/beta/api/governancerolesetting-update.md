---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
ms.openlocfilehash: ca5752d51e5d59578594a12c80ae1cac316b48bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041717"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="02b82-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="02b82-103">Update governanceRoleSetting</span></span>

> <span data-ttu-id="02b82-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="02b82-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02b82-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="02b82-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02b82-106">更新的[governanceRoleSetting](../resources/governancerolesetting.md)属性。</span><span class="sxs-lookup"><span data-stu-id="02b82-106">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="02b82-107">权限</span><span class="sxs-lookup"><span data-stu-id="02b82-107">Permissions</span></span>
<span data-ttu-id="02b82-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02b82-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02b82-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="02b82-110">Permission type</span></span>      | <span data-ttu-id="02b82-111">Permissions</span><span class="sxs-lookup"><span data-stu-id="02b82-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02b82-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02b82-112">Delegated (work or school account)</span></span> | <span data-ttu-id="02b82-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="02b82-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="02b82-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02b82-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02b82-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="02b82-115">Not supported.</span></span>    |
|<span data-ttu-id="02b82-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="02b82-116">Application</span></span> | <span data-ttu-id="02b82-117">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="02b82-117">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

<span data-ttu-id="02b82-118">除了权限范围，此 API 要求至少有一个请求程序`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="02b82-118">Besides the permission scope, this API requires the requestor to have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>
## <a name="http-request"></a><span data-ttu-id="02b82-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02b82-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="02b82-120">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="02b82-120">Optional request headers</span></span>
| <span data-ttu-id="02b82-121">名称</span><span class="sxs-lookup"><span data-stu-id="02b82-121">Name</span></span>       | <span data-ttu-id="02b82-122">说明</span><span class="sxs-lookup"><span data-stu-id="02b82-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="02b82-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02b82-123">Authorization</span></span>  | <span data-ttu-id="02b82-124">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="02b82-124">Bearer {code}</span></span>|
| <span data-ttu-id="02b82-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="02b82-125">Content-type</span></span>  | <span data-ttu-id="02b82-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02b82-126">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="02b82-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="02b82-127">Request body</span></span>
<span data-ttu-id="02b82-128">在请求正文中，提供[governanceRuleSettings](../resources/governancerulesetting.md)更新所需的值。</span><span class="sxs-lookup"><span data-stu-id="02b82-128">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that needs to be updated.</span></span> 

| <span data-ttu-id="02b82-129">属性</span><span class="sxs-lookup"><span data-stu-id="02b82-129">Property</span></span>     | <span data-ttu-id="02b82-130">类型</span><span class="sxs-lookup"><span data-stu-id="02b82-130">Type</span></span>   |<span data-ttu-id="02b82-131">说明</span><span class="sxs-lookup"><span data-stu-id="02b82-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="02b82-132">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="02b82-132">adminEligibleSettings</span></span>|[<span data-ttu-id="02b82-133">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="02b82-133">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="02b82-134">管理员尝试添加合格的角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="02b82-134">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="02b82-135">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="02b82-135">adminMemberSettings</span></span>|[<span data-ttu-id="02b82-136">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="02b82-136">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="02b82-137">管理员尝试添加直接成员角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="02b82-137">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="02b82-138">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="02b82-138">userEligibleSettings</span></span>|[<span data-ttu-id="02b82-139">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="02b82-139">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="02b82-140">当用户尝试添加合格的角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="02b82-140">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="02b82-141">此操作不受支持的`pimforazurerbac`方案现在，以及可在以后的方案。</span><span class="sxs-lookup"><span data-stu-id="02b82-141">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="02b82-142">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="02b82-142">userMemberSettings</span></span>|[<span data-ttu-id="02b82-143">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="02b82-143">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="02b82-144">当用户尝试激活其角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="02b82-144">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="02b82-145">响应</span><span class="sxs-lookup"><span data-stu-id="02b82-145">Response</span></span>
<span data-ttu-id="02b82-p104">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="02b82-p104">If successful, this method returns `204 NoContent` response code. It does not return anything in the response body.</span></span> 

## <a name="error-codes"></a><span data-ttu-id="02b82-148">错误代码</span><span class="sxs-lookup"><span data-stu-id="02b82-148">Error codes</span></span>
<span data-ttu-id="02b82-149">此 API 遵循标准的 HTTP 代码。</span><span class="sxs-lookup"><span data-stu-id="02b82-149">This API follows the standard of HTTP codes.</span></span> <span data-ttu-id="02b82-150">此外，如下所示的自定义的错误代码。</span><span class="sxs-lookup"><span data-stu-id="02b82-150">Besides, the custom error codes are shown below.</span></span>
|<span data-ttu-id="02b82-151">错误代码</span><span class="sxs-lookup"><span data-stu-id="02b82-151">Error code</span></span>     | <span data-ttu-id="02b82-152">错误消息</span><span class="sxs-lookup"><span data-stu-id="02b82-152">Error message</span></span>         | <span data-ttu-id="02b82-153">详细信息</span><span class="sxs-lookup"><span data-stu-id="02b82-153">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="02b82-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="02b82-154">400 BadRequest</span></span>| <span data-ttu-id="02b82-155">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="02b82-155">RoleSettingNotFound</span></span>   | <span data-ttu-id="02b82-156">[GovernanceRoleSetting](../resources/governancerolesetting.md)系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="02b82-156">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="02b82-157">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="02b82-157">400 BadRequest</span></span>| <span data-ttu-id="02b82-158">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="02b82-158">InvalidRoleSetting</span></span>    | <span data-ttu-id="02b82-159">在请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值不是有效的。</span><span class="sxs-lookup"><span data-stu-id="02b82-159">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="02b82-160">示例</span><span class="sxs-lookup"><span data-stu-id="02b82-160">Example</span></span> 
<span data-ttu-id="02b82-161">本示例更新自定义角色 3 中的订阅 Wingtip Toys-prod 移角色设置。</span><span class="sxs-lookup"><span data-stu-id="02b82-161">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="02b82-162">请求</span><span class="sxs-lookup"><span data-stu-id="02b82-162">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="02b82-163">响应</span><span class="sxs-lookup"><span data-stu-id="02b82-163">Response</span></span>
<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update governanceRoleSetting",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
