---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2cd81e24f6719ea47e7c6cf86486fbb63cd26d3b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42420813"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="5ebf0-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="5ebf0-103">Update governanceRoleSetting</span></span>

<span data-ttu-id="5ebf0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5ebf0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ebf0-105">更新[governanceRoleSetting](../resources/governancerolesetting.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-105">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="5ebf0-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ebf0-106">Permissions</span></span>
<span data-ttu-id="5ebf0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="5ebf0-109">**注意：** 此 API 还要求请求者在资源上至少有`Active`一个管理员角色分配`owner` （ `user access administrator`或）。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-109">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="5ebf0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ebf0-110">Permission type</span></span>      | <span data-ttu-id="5ebf0-111">权限</span><span class="sxs-lookup"><span data-stu-id="5ebf0-111">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5ebf0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ebf0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="5ebf0-113">PrivilegedAccess.ReadWrite.AzureResources</span><span class="sxs-lookup"><span data-stu-id="5ebf0-113">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="5ebf0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ebf0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ebf0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-115">Not supported.</span></span>    |
|<span data-ttu-id="5ebf0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ebf0-116">Application</span></span> | <span data-ttu-id="5ebf0-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5ebf0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ebf0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="5ebf0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ebf0-119">Request headers</span></span>
| <span data-ttu-id="5ebf0-120">名称</span><span class="sxs-lookup"><span data-stu-id="5ebf0-120">Name</span></span>       | <span data-ttu-id="5ebf0-121">说明</span><span class="sxs-lookup"><span data-stu-id="5ebf0-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5ebf0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ebf0-122">Authorization</span></span>  | <span data-ttu-id="5ebf0-123">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="5ebf0-123">Bearer {token}</span></span>|
| <span data-ttu-id="5ebf0-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="5ebf0-124">Content-type</span></span>  | <span data-ttu-id="5ebf0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ebf0-125">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="5ebf0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ebf0-126">Request body</span></span>
<span data-ttu-id="5ebf0-127">在请求正文中，提供需要更新的[governanceRuleSettings](../resources/governancerulesetting.md)的值。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-127">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="5ebf0-128">属性</span><span class="sxs-lookup"><span data-stu-id="5ebf0-128">Property</span></span>     | <span data-ttu-id="5ebf0-129">类型</span><span class="sxs-lookup"><span data-stu-id="5ebf0-129">Type</span></span>   |<span data-ttu-id="5ebf0-130">说明</span><span class="sxs-lookup"><span data-stu-id="5ebf0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ebf0-131">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="5ebf0-131">adminEligibleSettings</span></span>|<span data-ttu-id="5ebf0-132">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ebf0-132">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="5ebf0-133">在管理员尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-133">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="5ebf0-134">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="5ebf0-134">adminMemberSettings</span></span>|<span data-ttu-id="5ebf0-135">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ebf0-135">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="5ebf0-136">在管理员尝试添加直接成员角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-136">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="5ebf0-137">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="5ebf0-137">userEligibleSettings</span></span>|<span data-ttu-id="5ebf0-138">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ebf0-138">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="5ebf0-139">用户尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-139">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="5ebf0-140">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="5ebf0-140">userMemberSettings</span></span>|<span data-ttu-id="5ebf0-141">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="5ebf0-141">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="5ebf0-142">用户尝试激活他的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-142">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="5ebf0-143">响应</span><span class="sxs-lookup"><span data-stu-id="5ebf0-143">Response</span></span>
<span data-ttu-id="5ebf0-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="5ebf0-146">错误代码</span><span class="sxs-lookup"><span data-stu-id="5ebf0-146">Error codes</span></span>
<span data-ttu-id="5ebf0-147">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-147">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="5ebf0-148">此外，它还返回以下自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-148">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="5ebf0-149">错误代码</span><span class="sxs-lookup"><span data-stu-id="5ebf0-149">Error code</span></span>     | <span data-ttu-id="5ebf0-150">错误消息</span><span class="sxs-lookup"><span data-stu-id="5ebf0-150">Error message</span></span>         | <span data-ttu-id="5ebf0-151">详细信息</span><span class="sxs-lookup"><span data-stu-id="5ebf0-151">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="5ebf0-152">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5ebf0-152">400 BadRequest</span></span>| <span data-ttu-id="5ebf0-153">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="5ebf0-153">RoleSettingNotFound</span></span>   | <span data-ttu-id="5ebf0-154">[GovernanceRoleSetting](../resources/governancerolesetting.md)在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-154">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="5ebf0-155">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="5ebf0-155">400 BadRequest</span></span>| <span data-ttu-id="5ebf0-156">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="5ebf0-156">InvalidRoleSetting</span></span>    | <span data-ttu-id="5ebf0-157">请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值无效。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-157">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="5ebf0-158">示例</span><span class="sxs-lookup"><span data-stu-id="5ebf0-158">Example</span></span> 
<span data-ttu-id="5ebf0-159">本示例更新订阅 Wingtip 玩具-生产版中的自定义角色3的角色设置。</span><span class="sxs-lookup"><span data-stu-id="5ebf0-159">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="5ebf0-160">请求</span><span class="sxs-lookup"><span data-stu-id="5ebf0-160">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5ebf0-161">HTTP</span><span class="sxs-lookup"><span data-stu-id="5ebf0-161">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="5ebf0-162">C#</span><span class="sxs-lookup"><span data-stu-id="5ebf0-162">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5ebf0-163">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5ebf0-163">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5ebf0-164">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5ebf0-164">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5ebf0-165">响应</span><span class="sxs-lookup"><span data-stu-id="5ebf0-165">Response</span></span>
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
