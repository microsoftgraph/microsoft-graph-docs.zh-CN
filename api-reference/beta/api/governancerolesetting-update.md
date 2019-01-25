---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
ms.openlocfilehash: e5fc297690816227e1031af363ea7d4d38199e25
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509327"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="9316b-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="9316b-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9316b-104">更新的[governanceRoleSetting](../resources/governancerolesetting.md)属性。</span><span class="sxs-lookup"><span data-stu-id="9316b-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9316b-105">权限</span><span class="sxs-lookup"><span data-stu-id="9316b-105">Permissions</span></span>
<span data-ttu-id="9316b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9316b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="9316b-108">**注意：** 此 API 还需要请求者必须至少一个`Active`管理员角色分配 (`owner`或`user access administrator`) 对资源。</span><span class="sxs-lookup"><span data-stu-id="9316b-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="9316b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9316b-109">Permission type</span></span>      | <span data-ttu-id="9316b-110">权限</span><span class="sxs-lookup"><span data-stu-id="9316b-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9316b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9316b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9316b-112">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9316b-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="9316b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9316b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9316b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9316b-114">Not supported.</span></span>    |
|<span data-ttu-id="9316b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9316b-115">Application</span></span> | <span data-ttu-id="9316b-116">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="9316b-116">PrivilegedAccess.ReadWrite.AzureResources</span></span> |

## <a name="http-request"></a><span data-ttu-id="9316b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9316b-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9316b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9316b-118">Request headers</span></span>
| <span data-ttu-id="9316b-119">名称</span><span class="sxs-lookup"><span data-stu-id="9316b-119">Name</span></span>       | <span data-ttu-id="9316b-120">说明</span><span class="sxs-lookup"><span data-stu-id="9316b-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="9316b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9316b-121">Authorization</span></span>  | <span data-ttu-id="9316b-122">持有者 {code}</span><span class="sxs-lookup"><span data-stu-id="9316b-122">Bearer {code}</span></span>|
| <span data-ttu-id="9316b-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="9316b-123">Content-type</span></span>  | <span data-ttu-id="9316b-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9316b-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="9316b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9316b-125">Request body</span></span>
<span data-ttu-id="9316b-126">在请求正文中，提供[governanceRuleSettings](../resources/governancerulesetting.md)更新所需的值。</span><span class="sxs-lookup"><span data-stu-id="9316b-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="9316b-127">属性</span><span class="sxs-lookup"><span data-stu-id="9316b-127">Property</span></span>     | <span data-ttu-id="9316b-128">类型</span><span class="sxs-lookup"><span data-stu-id="9316b-128">Type</span></span>   |<span data-ttu-id="9316b-129">说明</span><span class="sxs-lookup"><span data-stu-id="9316b-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9316b-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="9316b-130">adminEligibleSettings</span></span>|[<span data-ttu-id="9316b-131">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="9316b-131">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="9316b-132">管理员尝试添加合格的角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="9316b-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="9316b-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="9316b-133">adminMemberSettings</span></span>|[<span data-ttu-id="9316b-134">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="9316b-134">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="9316b-135">管理员尝试添加直接成员角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="9316b-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="9316b-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="9316b-136">userEligibleSettings</span></span>|[<span data-ttu-id="9316b-137">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="9316b-137">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="9316b-138">当用户尝试添加合格的角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="9316b-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> <span data-ttu-id="9316b-139">此操作不受支持的`pimforazurerbac`方案现在，以及可在以后的方案。</span><span class="sxs-lookup"><span data-stu-id="9316b-139">This is not supported for `pimforazurerbac` scenario for now, and may be available in the future scenarios.</span></span>|
|<span data-ttu-id="9316b-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="9316b-140">userMemberSettings</span></span>|[<span data-ttu-id="9316b-141">governanceRuleSetting</span><span class="sxs-lookup"><span data-stu-id="9316b-141">governanceRuleSetting</span></span>](../resources/governancerulesetting.md)|<span data-ttu-id="9316b-142">当用户尝试激活其角色分配时计算规则设置。</span><span class="sxs-lookup"><span data-stu-id="9316b-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="9316b-143">响应</span><span class="sxs-lookup"><span data-stu-id="9316b-143">Response</span></span>
<span data-ttu-id="9316b-p103">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="9316b-p103">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="9316b-146">错误代码</span><span class="sxs-lookup"><span data-stu-id="9316b-146">Error codes</span></span>
<span data-ttu-id="9316b-147">此 API 返回的标准 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="9316b-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="9316b-148">此外，它将返回以下自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="9316b-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="9316b-149">错误代码</span><span class="sxs-lookup"><span data-stu-id="9316b-149">Error code</span></span>     | <span data-ttu-id="9316b-150">错误消息</span><span class="sxs-lookup"><span data-stu-id="9316b-150">Error message</span></span>         | <span data-ttu-id="9316b-151">详细信息</span><span class="sxs-lookup"><span data-stu-id="9316b-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="9316b-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9316b-152">400 BadRequest</span></span>| <span data-ttu-id="9316b-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="9316b-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="9316b-154">[GovernanceRoleSetting](../resources/governancerolesetting.md)系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="9316b-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="9316b-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="9316b-155">400 BadRequest</span></span>| <span data-ttu-id="9316b-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="9316b-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="9316b-157">在请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值不是有效的。</span><span class="sxs-lookup"><span data-stu-id="9316b-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="9316b-158">示例</span><span class="sxs-lookup"><span data-stu-id="9316b-158">Example</span></span> 
<span data-ttu-id="9316b-159">本示例更新自定义角色 3 中的订阅 Wingtip Toys-prod 移角色设置。</span><span class="sxs-lookup"><span data-stu-id="9316b-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="9316b-160">请求</span><span class="sxs-lookup"><span data-stu-id="9316b-160">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="9316b-161">响应</span><span class="sxs-lookup"><span data-stu-id="9316b-161">Response</span></span>
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
