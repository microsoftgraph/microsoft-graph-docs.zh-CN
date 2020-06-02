---
title: 更新 authorizationpolicy
description: 更新 authorizationPolicy 对象的属性。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ac605e93603cb39491fd980e78a9b0f0026541eb
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44492200"
---
# <a name="update-authorizationpolicy"></a><span data-ttu-id="4088f-103">更新 authorizationPolicy</span><span class="sxs-lookup"><span data-stu-id="4088f-103">Update authorizationPolicy</span></span>

<span data-ttu-id="4088f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4088f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4088f-105">更新[authorizationPolicy](../resources/authorizationpolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4088f-105">Update the properties of a [authorizationPolicy](../resources/authorizationpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4088f-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="4088f-106">Permissions</span></span>

<span data-ttu-id="4088f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4088f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4088f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4088f-109">Permission type</span></span>                        | <span data-ttu-id="4088f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4088f-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="4088f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4088f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4088f-112">Policy。读身份验证</span><span class="sxs-lookup"><span data-stu-id="4088f-112">Policy.ReadWrite.Authorization</span></span>|
| <span data-ttu-id="4088f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4088f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4088f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4088f-114">Not supported.</span></span> |
| <span data-ttu-id="4088f-115">Application</span><span class="sxs-lookup"><span data-stu-id="4088f-115">Application</span></span>                            | <span data-ttu-id="4088f-116">Policy。读身份验证</span><span class="sxs-lookup"><span data-stu-id="4088f-116">Policy.ReadWrite.Authorization</span></span>|

## <a name="http-request"></a><span data-ttu-id="4088f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4088f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /policies/authorizationPolicy/authorizationPolicy
```

## <a name="request-headers"></a><span data-ttu-id="4088f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4088f-118">Request headers</span></span>

| <span data-ttu-id="4088f-119">名称</span><span class="sxs-lookup"><span data-stu-id="4088f-119">Name</span></span>       | <span data-ttu-id="4088f-120">说明</span><span class="sxs-lookup"><span data-stu-id="4088f-120">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="4088f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4088f-121">Authorization</span></span> | <span data-ttu-id="4088f-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="4088f-122">Bearer {token}</span></span> |
| <span data-ttu-id="4088f-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="4088f-123">Content-type</span></span> | <span data-ttu-id="4088f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4088f-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="4088f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4088f-125">Request body</span></span>

<span data-ttu-id="4088f-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="4088f-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4088f-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="4088f-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4088f-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4088f-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4088f-129">属性</span><span class="sxs-lookup"><span data-stu-id="4088f-129">Property</span></span>     | <span data-ttu-id="4088f-130">类型</span><span class="sxs-lookup"><span data-stu-id="4088f-130">Type</span></span>        | <span data-ttu-id="4088f-131">Description</span><span class="sxs-lookup"><span data-stu-id="4088f-131">Description</span></span> |
|:-------------|:------------|:------------|  
|<span data-ttu-id="4088f-132">displayName</span><span class="sxs-lookup"><span data-stu-id="4088f-132">displayName</span></span>|<span data-ttu-id="4088f-133">String</span><span class="sxs-lookup"><span data-stu-id="4088f-133">String</span></span>| <span data-ttu-id="4088f-134">此策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4088f-134">Display name for this policy.</span></span> |  
|<span data-ttu-id="4088f-135">说明</span><span class="sxs-lookup"><span data-stu-id="4088f-135">description</span></span>|<span data-ttu-id="4088f-136">String</span><span class="sxs-lookup"><span data-stu-id="4088f-136">String</span></span>| <span data-ttu-id="4088f-137">此策略的说明。</span><span class="sxs-lookup"><span data-stu-id="4088f-137">Description of this policy.</span></span> |  
|<span data-ttu-id="4088f-138">guestUserRoleId</span><span class="sxs-lookup"><span data-stu-id="4088f-138">guestUserRoleId</span></span>|<span data-ttu-id="4088f-139">Guid</span><span class="sxs-lookup"><span data-stu-id="4088f-139">Guid</span></span>| <span data-ttu-id="4088f-140">表示应向来宾用户授予的角色的角色 templateId。</span><span class="sxs-lookup"><span data-stu-id="4088f-140">Represents role templateId for the role that should be granted to guest user.</span></span> <span data-ttu-id="4088f-141">若要查找可用角色模板的列表，请参阅[List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) 。</span><span class="sxs-lookup"><span data-stu-id="4088f-141">Refer to [List unifiedRoleDefinitions](https://docs.microsoft.com/graph/api/rbacapplication-list-roledefinitions?view=graph-rest-beta&tabs=http) to find the list of available role templates.</span></span> <span data-ttu-id="4088f-142">目前只有受支持的角色是用户（a0b1b346-4d3e-4e8b-98f8-753987be4970）、来宾用户（10dae51f-b6af-4016-8d66-8c2a99b929b3）和受限制的来宾用户（2af84b1e-32c8-42b7-82bc-daa82404023b）。</span><span class="sxs-lookup"><span data-stu-id="4088f-142">Only supported roles today are User (a0b1b346-4d3e-4e8b-98f8-753987be4970), Guest User (10dae51f-b6af-4016-8d66-8c2a99b929b3), and Restricted Guest User (2af84b1e-32c8-42b7-82bc-daa82404023b).</span></span> | 
|<span data-ttu-id="4088f-143">enabledPreviewFeatures</span><span class="sxs-lookup"><span data-stu-id="4088f-143">enabledPreviewFeatures</span></span>|<span data-ttu-id="4088f-144">集合（string）</span><span class="sxs-lookup"><span data-stu-id="4088f-144">Collection(string)</span></span>| <span data-ttu-id="4088f-145">租户上启用了专用预览的功能列表。</span><span class="sxs-lookup"><span data-stu-id="4088f-145">List of features enabled for private preview on the tenant.</span></span> | 
|<span data-ttu-id="4088f-146">blockMsolPowerShell</span><span class="sxs-lookup"><span data-stu-id="4088f-146">blockMsolPowerShell</span></span>|<span data-ttu-id="4088f-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="4088f-147">Boolean</span></span>| <span data-ttu-id="4088f-148">若要禁用 MSOL PowerShell 的使用，请将此属性设置为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="4088f-148">To disable the use of MSOL PowerShell, set this property to `true`.</span></span> <span data-ttu-id="4088f-149">设置为 `true` 将禁用对 MSOL PowerShell 使用的旧版服务终结点的基于用户的访问。</span><span class="sxs-lookup"><span data-stu-id="4088f-149">Setting to `true` will also disable user-based access to the legacy service endpoint used by MSOL PowerShell.</span></span> <span data-ttu-id="4088f-150">这不会影响 Azure AD Connect 或 Microsoft Graph。</span><span class="sxs-lookup"><span data-stu-id="4088f-150">This does not affect Azure AD Connect or Microsoft Graph.</span></span> | 

## <a name="response"></a><span data-ttu-id="4088f-151">响应</span><span class="sxs-lookup"><span data-stu-id="4088f-151">Response</span></span>

<span data-ttu-id="4088f-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="4088f-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4088f-154">示例</span><span class="sxs-lookup"><span data-stu-id="4088f-154">Examples</span></span>

### <a name="example-1-update-or-set-guest-user-access-level-for-the-tenant"></a><span data-ttu-id="4088f-155">示例1：更新或设置租户的来宾用户访问级别</span><span class="sxs-lookup"><span data-stu-id="4088f-155">Example 1: Update or set Guest user access level for the tenant</span></span>

#### <a name="request"></a><span data-ttu-id="4088f-156">请求</span><span class="sxs-lookup"><span data-stu-id="4088f-156">Request</span></span>

<span data-ttu-id="4088f-157">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4088f-157">The following is an example of the request.</span></span> <span data-ttu-id="4088f-158">在此示例中，将来宾访问级别修改为受限制的来宾用户。</span><span class="sxs-lookup"><span data-stu-id="4088f-158">In this example, guest access level is modified to Restricted Guest User.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "guestUserRole": "2af84b1e-32c8-42b7-82bc-daa82404023b"
}

```
#### <a name="response"></a><span data-ttu-id="4088f-159">响应</span><span class="sxs-lookup"><span data-stu-id="4088f-159">Response</span></span>

<span data-ttu-id="4088f-160">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4088f-160">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content

```

### <a name="example-2-enable-new-feature-for-preview-on-tenant"></a><span data-ttu-id="4088f-161">示例2：在租户上为预览启用新功能</span><span class="sxs-lookup"><span data-stu-id="4088f-161">Example 2: Enable new feature for preview on tenant</span></span>

#### <a name="request"></a><span data-ttu-id="4088f-162">请求</span><span class="sxs-lookup"><span data-stu-id="4088f-162">Request</span></span>

<span data-ttu-id="4088f-163">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4088f-163">The following is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "enabledPreviewFeatures": ["assignGroupsToRoles"]
}

```
#### <a name="response"></a><span data-ttu-id="4088f-164">响应</span><span class="sxs-lookup"><span data-stu-id="4088f-164">Response</span></span>

<span data-ttu-id="4088f-165">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4088f-165">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```


### <a name="example-3-block-msol-powershell-in-tenant"></a><span data-ttu-id="4088f-166">示例3：阻止租户中的 MSOL PowerShell</span><span class="sxs-lookup"><span data-stu-id="4088f-166">Example 3: Block MSOL PowerShell in tenant</span></span>

#### <a name="request"></a><span data-ttu-id="4088f-167">请求</span><span class="sxs-lookup"><span data-stu-id="4088f-167">Request</span></span>

<span data-ttu-id="4088f-168">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4088f-168">The following is an example of the request.</span></span>

```http
PATCH https://graph.microsoft.com/beta/policies/authorizationPolicy/authorizationPolicy
{
  "blockMsolPowerShell": true
}

```
#### <a name="response"></a><span data-ttu-id="4088f-169">响应</span><span class="sxs-lookup"><span data-stu-id="4088f-169">Response</span></span>

<span data-ttu-id="4088f-170">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4088f-170">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.authorizationPolicyPolicy"
} -->

```http
HTTP/1.1 204 No Content
```
