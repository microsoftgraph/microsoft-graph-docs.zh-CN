---
title: 更新 governanceRoleSetting
description: 更新 governanceRoleSetting 的属性。
localization_priority: Normal
doc_type: apiPageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 20e41f118f0da2248f0744c64ab25d69da8061f2
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041777"
---
# <a name="update-governancerolesetting"></a><span data-ttu-id="eb661-103">更新 governanceRoleSetting</span><span class="sxs-lookup"><span data-stu-id="eb661-103">Update governanceRoleSetting</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb661-104">更新[governanceRoleSetting](../resources/governancerolesetting.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="eb661-104">Update the properties of [governanceRoleSetting](../resources/governancerolesetting.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="eb661-105">权限</span><span class="sxs-lookup"><span data-stu-id="eb661-105">Permissions</span></span>
<span data-ttu-id="eb661-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eb661-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="eb661-108">**注意：** 此 API 还要求请求者在资源上至少有`Active`一个管理员角色分配`owner` （ `user access administrator`或）。</span><span class="sxs-lookup"><span data-stu-id="eb661-108">**Note:** This API also requires that the requester have at least one `Active` administrator role assignment (`owner` or `user access administrator`) on the resource.</span></span>

|<span data-ttu-id="eb661-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eb661-109">Permission type</span></span>      | <span data-ttu-id="eb661-110">权限</span><span class="sxs-lookup"><span data-stu-id="eb661-110">Permissions</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="eb661-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eb661-111">Delegated (work or school account)</span></span> | <span data-ttu-id="eb661-112">PrivilegedAccess AzureResources</span><span class="sxs-lookup"><span data-stu-id="eb661-112">PrivilegedAccess.ReadWrite.AzureResources</span></span>  |
|<span data-ttu-id="eb661-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eb661-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="eb661-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb661-114">Not supported.</span></span>    |
|<span data-ttu-id="eb661-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eb661-115">Application</span></span> | <span data-ttu-id="eb661-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eb661-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="eb661-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eb661-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /privilegedAccess/azureResources/roleSettings/{id}
```
## <a name="request-headers"></a><span data-ttu-id="eb661-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="eb661-118">Request headers</span></span>
| <span data-ttu-id="eb661-119">名称</span><span class="sxs-lookup"><span data-stu-id="eb661-119">Name</span></span>       | <span data-ttu-id="eb661-120">说明</span><span class="sxs-lookup"><span data-stu-id="eb661-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="eb661-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eb661-121">Authorization</span></span>  | <span data-ttu-id="eb661-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="eb661-122">Bearer {token}</span></span>|
| <span data-ttu-id="eb661-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="eb661-123">Content-type</span></span>  | <span data-ttu-id="eb661-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eb661-124">application/json</span></span>|


## <a name="request-body"></a><span data-ttu-id="eb661-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eb661-125">Request body</span></span>
<span data-ttu-id="eb661-126">在请求正文中，提供需要更新的[governanceRuleSettings](../resources/governancerulesetting.md)的值。</span><span class="sxs-lookup"><span data-stu-id="eb661-126">In the request body, supply the values for [governanceRuleSettings](../resources/governancerulesetting.md) that need to be updated.</span></span> 

| <span data-ttu-id="eb661-127">属性</span><span class="sxs-lookup"><span data-stu-id="eb661-127">Property</span></span>     | <span data-ttu-id="eb661-128">类型</span><span class="sxs-lookup"><span data-stu-id="eb661-128">Type</span></span>   |<span data-ttu-id="eb661-129">说明</span><span class="sxs-lookup"><span data-stu-id="eb661-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eb661-130">adminEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="eb661-130">adminEligibleSettings</span></span>|<span data-ttu-id="eb661-131">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="eb661-131">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="eb661-132">在管理员尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="eb661-132">The rule settings that are evaluated when an administrator tries to add an eligible role assignment.</span></span>|
|<span data-ttu-id="eb661-133">adminMemberSettings</span><span class="sxs-lookup"><span data-stu-id="eb661-133">adminMemberSettings</span></span>|<span data-ttu-id="eb661-134">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="eb661-134">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="eb661-135">在管理员尝试添加直接成员角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="eb661-135">The rule settings that are evaluated when an administrator tries to add a direct member role assignment.</span></span>|
|<span data-ttu-id="eb661-136">userEligibleSettings</span><span class="sxs-lookup"><span data-stu-id="eb661-136">userEligibleSettings</span></span>|<span data-ttu-id="eb661-137">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="eb661-137">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="eb661-138">用户尝试添加符合条件的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="eb661-138">The rule settings that are evaluated when a user tries to add an eligible role assignment.</span></span> |
|<span data-ttu-id="eb661-139">userMemberSettings</span><span class="sxs-lookup"><span data-stu-id="eb661-139">userMemberSettings</span></span>|<span data-ttu-id="eb661-140">[governanceRuleSetting](../resources/governancerulesetting.md)集合</span><span class="sxs-lookup"><span data-stu-id="eb661-140">[governanceRuleSetting](../resources/governancerulesetting.md) collection</span></span>|<span data-ttu-id="eb661-141">用户尝试激活他的角色分配时评估的规则设置。</span><span class="sxs-lookup"><span data-stu-id="eb661-141">The rule settings that are evaluated when a user tries to activate his role assignment.</span></span>|

## <a name="response"></a><span data-ttu-id="eb661-142">响应</span><span class="sxs-lookup"><span data-stu-id="eb661-142">Response</span></span>
<span data-ttu-id="eb661-p102">如果成功，此方法返回 `204 NoContent` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="eb661-p102">If successful, this method returns a `204 NoContent` response code. It does not return anything in the response body.</span></span> 

### <a name="error-codes"></a><span data-ttu-id="eb661-145">错误代码</span><span class="sxs-lookup"><span data-stu-id="eb661-145">Error codes</span></span>
<span data-ttu-id="eb661-146">此 API 返回标准的 HTTP 错误代码。</span><span class="sxs-lookup"><span data-stu-id="eb661-146">This API returns the standard HTTP error codes.</span></span> <span data-ttu-id="eb661-147">此外，它还返回以下自定义错误代码。</span><span class="sxs-lookup"><span data-stu-id="eb661-147">In addition, it returns the following custom error codes.</span></span>

|<span data-ttu-id="eb661-148">错误代码</span><span class="sxs-lookup"><span data-stu-id="eb661-148">Error code</span></span>     | <span data-ttu-id="eb661-149">错误消息</span><span class="sxs-lookup"><span data-stu-id="eb661-149">Error message</span></span>         | <span data-ttu-id="eb661-150">详细信息</span><span class="sxs-lookup"><span data-stu-id="eb661-150">Details</span></span>             |
|:--------------| :---------------------|:--------------------|
| <span data-ttu-id="eb661-151">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eb661-151">400 BadRequest</span></span>| <span data-ttu-id="eb661-152">RoleSettingNotFound</span><span class="sxs-lookup"><span data-stu-id="eb661-152">RoleSettingNotFound</span></span>   | <span data-ttu-id="eb661-153">[GovernanceRoleSetting](../resources/governancerolesetting.md)在系统中不存在。</span><span class="sxs-lookup"><span data-stu-id="eb661-153">The [governanceRoleSetting](../resources/governancerolesetting.md) does not exist in system.</span></span>
| <span data-ttu-id="eb661-154">400 BadRequest</span><span class="sxs-lookup"><span data-stu-id="eb661-154">400 BadRequest</span></span>| <span data-ttu-id="eb661-155">InvalidRoleSetting</span><span class="sxs-lookup"><span data-stu-id="eb661-155">InvalidRoleSetting</span></span>    | <span data-ttu-id="eb661-156">请求正文中提供的[governanceRuleSettings](../resources/governancerulesetting.md)值无效。</span><span class="sxs-lookup"><span data-stu-id="eb661-156">The [governanceRuleSettings](../resources/governancerulesetting.md) values provided in the request body are not valid.</span></span>

## <a name="example"></a><span data-ttu-id="eb661-157">示例</span><span class="sxs-lookup"><span data-stu-id="eb661-157">Example</span></span> 
<span data-ttu-id="eb661-158">本示例更新订阅 Wingtip 玩具-生产版中的自定义角色3的角色设置。</span><span class="sxs-lookup"><span data-stu-id="eb661-158">This example updates the role setting for Custom Role 3 in the subscription Wingtip Toys - Prod.</span></span>
##### <a name="request"></a><span data-ttu-id="eb661-159">请求</span><span class="sxs-lookup"><span data-stu-id="eb661-159">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="eb661-160">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="eb661-160">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="eb661-161">C#</span><span class="sxs-lookup"><span data-stu-id="eb661-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-governancerolesetting-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="eb661-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="eb661-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-governancerolesetting-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="eb661-163">目标-C</span><span class="sxs-lookup"><span data-stu-id="eb661-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-governancerolesetting-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="eb661-164">响应</span><span class="sxs-lookup"><span data-stu-id="eb661-164">Response</span></span>
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
