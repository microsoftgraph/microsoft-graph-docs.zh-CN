---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予 (OAuth 2.0) 的委派权限，通常是由于用户或管理员同意过程而授予的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 944a96858bea7a1e46ea1f59ef6b67092e4b06a6
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442929"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="5085b-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="5085b-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="5085b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5085b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5085b-105">表示已授予应用程序的服务主体的委派权限。</span><span class="sxs-lookup"><span data-stu-id="5085b-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="5085b-106">委派的权限授予可以在用户同意应用程序访问 API 的请求后创建，也可以直接创建。</span><span class="sxs-lookup"><span data-stu-id="5085b-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="5085b-107">委派的权限有时称为"OAuth 2.0 范围"或"作用域"。</span><span class="sxs-lookup"><span data-stu-id="5085b-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="5085b-108">Methods</span><span class="sxs-lookup"><span data-stu-id="5085b-108">Methods</span></span>

| <span data-ttu-id="5085b-109">方法</span><span class="sxs-lookup"><span data-stu-id="5085b-109">Method</span></span> | <span data-ttu-id="5085b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="5085b-110">Return Type</span></span> | <span data-ttu-id="5085b-111">说明</span><span class="sxs-lookup"><span data-stu-id="5085b-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="5085b-112">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="5085b-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="5085b-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5085b-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="5085b-114">检索委派权限授予的列表。</span><span class="sxs-lookup"><span data-stu-id="5085b-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="5085b-115">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="5085b-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="5085b-117">读取单个委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="5085b-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="5085b-118">创建 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="5085b-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="5085b-120">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="5085b-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="5085b-121">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="5085b-122">无</span><span class="sxs-lookup"><span data-stu-id="5085b-122">None</span></span> | <span data-ttu-id="5085b-123">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="5085b-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="5085b-124">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="5085b-125">无</span><span class="sxs-lookup"><span data-stu-id="5085b-125">None</span></span>  | <span data-ttu-id="5085b-126">删除委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="5085b-126">Delete a delegated permission grant.</span></span> |

## <a name="properties"></a><span data-ttu-id="5085b-127">属性</span><span class="sxs-lookup"><span data-stu-id="5085b-127">Properties</span></span>

| <span data-ttu-id="5085b-128">属性</span><span class="sxs-lookup"><span data-stu-id="5085b-128">Property</span></span> | <span data-ttu-id="5085b-129">类型</span><span class="sxs-lookup"><span data-stu-id="5085b-129">Type</span></span> | <span data-ttu-id="5085b-130">说明</span><span class="sxs-lookup"><span data-stu-id="5085b-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="5085b-131">id</span><span class="sxs-lookup"><span data-stu-id="5085b-131">id</span></span> | <span data-ttu-id="5085b-132">String</span><span class="sxs-lookup"><span data-stu-id="5085b-132">String</span></span> | <span data-ttu-id="5085b-133">**oAuth2PermissionGrant 的唯一标识符**。</span><span class="sxs-lookup"><span data-stu-id="5085b-133">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="5085b-134">只读。</span><span class="sxs-lookup"><span data-stu-id="5085b-134">Read-only.</span></span>|
| <span data-ttu-id="5085b-135">clientId</span><span class="sxs-lookup"><span data-stu-id="5085b-135">clientId</span></span> | <span data-ttu-id="5085b-136">字符串</span><span class="sxs-lookup"><span data-stu-id="5085b-136">String</span></span> | <span data-ttu-id="5085b-137">**应用程序** 客户端 [服务](serviceprincipal.md)主体的 ID，授权在访问 API 时代表登录用户操作。</span><span class="sxs-lookup"><span data-stu-id="5085b-137">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="5085b-138">必需。</span><span class="sxs-lookup"><span data-stu-id="5085b-138">Required.</span></span> <span data-ttu-id="5085b-139">支持 `$filter`（仅 `eq`）。</span><span class="sxs-lookup"><span data-stu-id="5085b-139">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="5085b-140">consentType</span><span class="sxs-lookup"><span data-stu-id="5085b-140">consentType</span></span> | <span data-ttu-id="5085b-141">String</span><span class="sxs-lookup"><span data-stu-id="5085b-141">String</span></span> | <span data-ttu-id="5085b-142">指示是否向客户端应用程序授予了模拟所有用户或仅模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="5085b-142">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="5085b-143">*AllPrincipals* 指示对模拟所有用户的授权。</span><span class="sxs-lookup"><span data-stu-id="5085b-143">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="5085b-144">*主体* 指示对模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="5085b-144">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="5085b-145">管理员可以代表所有用户授予同意。</span><span class="sxs-lookup"><span data-stu-id="5085b-145">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="5085b-146">在某些情况下，对于某些委派权限，非管理员用户可能有权代表自己同意。</span><span class="sxs-lookup"><span data-stu-id="5085b-146">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="5085b-147">必需。</span><span class="sxs-lookup"><span data-stu-id="5085b-147">Required.</span></span> <span data-ttu-id="5085b-148">支持 `$filter`（仅 `eq`）。</span><span class="sxs-lookup"><span data-stu-id="5085b-148">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="5085b-149">principalId</span><span class="sxs-lookup"><span data-stu-id="5085b-149">principalId</span></span> | <span data-ttu-id="5085b-150">String</span><span class="sxs-lookup"><span data-stu-id="5085b-150">String</span></span> | <span data-ttu-id="5085b-151">**consentType** 为 [Principal](user.md)时，客户端有权访问资源的用户的 *ID。*</span><span class="sxs-lookup"><span data-stu-id="5085b-151">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="5085b-152">如果 **consentType** *为 AllPrincipals，* 则此值为 null。</span><span class="sxs-lookup"><span data-stu-id="5085b-152">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="5085b-153">consentType 为 **主体** 时 *必需*。</span><span class="sxs-lookup"><span data-stu-id="5085b-153">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="5085b-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="5085b-154">resourceId</span></span> | <span data-ttu-id="5085b-155">String</span><span class="sxs-lookup"><span data-stu-id="5085b-155">String</span></span> | <span data-ttu-id="5085b-156">**有权访问** 的资源 [服务](serviceprincipal.md)主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="5085b-156">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="5085b-157">这标识了客户端有权尝试代表登录用户调用的 API。</span><span class="sxs-lookup"><span data-stu-id="5085b-157">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="5085b-158">scope</span><span class="sxs-lookup"><span data-stu-id="5085b-158">scope</span></span> | <span data-ttu-id="5085b-159">String</span><span class="sxs-lookup"><span data-stu-id="5085b-159">String</span></span> | <span data-ttu-id="5085b-160">由空格分隔的委派权限声明值列表，应包含在 API 应用程序的资源应用程序访问令牌 (API) 。</span><span class="sxs-lookup"><span data-stu-id="5085b-160">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="5085b-161">例如，`openid User.Read GroupMember.Read.All`。</span><span class="sxs-lookup"><span data-stu-id="5085b-161">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="5085b-162">每个声明值应匹配由API 定义的委派权限之一的值字段，在资源服务主体的 **publishedPermissionScopes** 属性 [中列出](serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="5085b-162">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |
| <span data-ttu-id="5085b-163">startTime</span><span class="sxs-lookup"><span data-stu-id="5085b-163">startTime</span></span> | <span data-ttu-id="5085b-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5085b-164">DateTimeOffset</span></span> | <span data-ttu-id="5085b-165">目前，开始时间值将被忽略，但创建 **oAuth2PermissionGrant** 时需要一个值。</span><span class="sxs-lookup"><span data-stu-id="5085b-165">Currently, the start time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="5085b-166">必需。</span><span class="sxs-lookup"><span data-stu-id="5085b-166">Required.</span></span> |
| <span data-ttu-id="5085b-167">expiryTime</span><span class="sxs-lookup"><span data-stu-id="5085b-167">expiryTime</span></span> | <span data-ttu-id="5085b-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5085b-168">DateTimeOffset</span></span> | <span data-ttu-id="5085b-169">目前，将忽略结束时间值，但创建 **oAuth2PermissionGrant** 时需要一个值。</span><span class="sxs-lookup"><span data-stu-id="5085b-169">Currently, the end time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="5085b-170">必填。</span><span class="sxs-lookup"><span data-stu-id="5085b-170">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5085b-171">关系</span><span class="sxs-lookup"><span data-stu-id="5085b-171">Relationships</span></span>

<span data-ttu-id="5085b-172">无。</span><span class="sxs-lookup"><span data-stu-id="5085b-172">None.</span></span>

<span data-ttu-id="5085b-173">该资源支持通过提供 [delta](../api/oauth2permissiongrant-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="5085b-173">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="5085b-174">方法</span><span class="sxs-lookup"><span data-stu-id="5085b-174">Methods</span></span>

| <span data-ttu-id="5085b-175">方法</span><span class="sxs-lookup"><span data-stu-id="5085b-175">Method</span></span>           | <span data-ttu-id="5085b-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="5085b-176">Return Type</span></span>    |<span data-ttu-id="5085b-177">说明</span><span class="sxs-lookup"><span data-stu-id="5085b-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5085b-178">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="5085b-178">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="5085b-179">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="5085b-179">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="5085b-180">检索 **oauth2PermissionGrant 对象** 的列表。</span><span class="sxs-lookup"><span data-stu-id="5085b-180">Retrieve a list of **oauth2PermissionGrant** objects.</span></span> |
|[<span data-ttu-id="5085b-181">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-181">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="5085b-182">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-182">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="5085b-183">读取 **oAuth2PermissionGrant 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="5085b-183">Read the properties and relationships of an **oAuth2PermissionGrant** object.</span></span>|
|[<span data-ttu-id="5085b-184">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-184">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="5085b-185">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-185">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="5085b-186">更新  **oAuth2PermissionGrant** 对象。</span><span class="sxs-lookup"><span data-stu-id="5085b-186">Update an  **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="5085b-187">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-187">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="5085b-188">无</span><span class="sxs-lookup"><span data-stu-id="5085b-188">None</span></span> |<span data-ttu-id="5085b-189">删除 **oAuth2PermissionGrant** 对象。</span><span class="sxs-lookup"><span data-stu-id="5085b-189">Delete an **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="5085b-190">获取 delta</span><span class="sxs-lookup"><span data-stu-id="5085b-190">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="5085b-191">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="5085b-191">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="5085b-192">获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而无需执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="5085b-192">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="5085b-193">属性</span><span class="sxs-lookup"><span data-stu-id="5085b-193">Properties</span></span>
| <span data-ttu-id="5085b-194">属性</span><span class="sxs-lookup"><span data-stu-id="5085b-194">Property</span></span>     | <span data-ttu-id="5085b-195">类型</span><span class="sxs-lookup"><span data-stu-id="5085b-195">Type</span></span>   |<span data-ttu-id="5085b-196">说明</span><span class="sxs-lookup"><span data-stu-id="5085b-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5085b-197">clientId</span><span class="sxs-lookup"><span data-stu-id="5085b-197">clientId</span></span>|<span data-ttu-id="5085b-198">字符串</span><span class="sxs-lookup"><span data-stu-id="5085b-198">String</span></span>| <span data-ttu-id="5085b-199">在访问由 resourceId 属性表示的资源 (时，授予其同意模拟用户的服务主体) 。</span><span class="sxs-lookup"><span data-stu-id="5085b-199">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="5085b-200">consentType</span><span class="sxs-lookup"><span data-stu-id="5085b-200">consentType</span></span>|<span data-ttu-id="5085b-201">String</span><span class="sxs-lookup"><span data-stu-id="5085b-201">String</span></span>| <span data-ttu-id="5085b-202">指示管理员是代表组织 (还是由) 提供同意。</span><span class="sxs-lookup"><span data-stu-id="5085b-202">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="5085b-203">可能的值为 *AllPrincipals* 或 *Principal。*</span><span class="sxs-lookup"><span data-stu-id="5085b-203">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="5085b-204">expiryTime</span><span class="sxs-lookup"><span data-stu-id="5085b-204">expiryTime</span></span>|<span data-ttu-id="5085b-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5085b-205">DateTimeOffset</span></span>| <span data-ttu-id="5085b-206">目前，过期时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="5085b-206">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="5085b-207">id</span><span class="sxs-lookup"><span data-stu-id="5085b-207">id</span></span>|<span data-ttu-id="5085b-208">String</span><span class="sxs-lookup"><span data-stu-id="5085b-208">String</span></span>| <span data-ttu-id="5085b-209">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="5085b-209">Unique identifier.</span></span> <span data-ttu-id="5085b-210">只读。</span><span class="sxs-lookup"><span data-stu-id="5085b-210">Read-only.</span></span>|
|<span data-ttu-id="5085b-211">principalId</span><span class="sxs-lookup"><span data-stu-id="5085b-211">principalId</span></span>|<span data-ttu-id="5085b-212">String</span><span class="sxs-lookup"><span data-stu-id="5085b-212">String</span></span>| <span data-ttu-id="5085b-213">如果 consentType *为 AllPrincipals，* 则此值为 null，并且同意适用于组织中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="5085b-213">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="5085b-214">如果 consentType 为 *Principal，* 则此属性指定已授予同意并仅适用于该用户的用户 ID。</span><span class="sxs-lookup"><span data-stu-id="5085b-214">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="5085b-215">resourceId</span><span class="sxs-lookup"><span data-stu-id="5085b-215">resourceId</span></span>|<span data-ttu-id="5085b-216">String</span><span class="sxs-lookup"><span data-stu-id="5085b-216">String</span></span>| <span data-ttu-id="5085b-217">指定已授予其访问权限的资源服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="5085b-217">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="5085b-218">scope</span><span class="sxs-lookup"><span data-stu-id="5085b-218">scope</span></span>|<span data-ttu-id="5085b-219">String</span><span class="sxs-lookup"><span data-stu-id="5085b-219">String</span></span>| <span data-ttu-id="5085b-220">指定资源应用程序应在 OAuth 2.0 访问令牌中预期的范围声明的值。 [](/graph/permissions-reference)</span><span class="sxs-lookup"><span data-stu-id="5085b-220">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="5085b-221">例如 *，User.Read*</span><span class="sxs-lookup"><span data-stu-id="5085b-221">For example, *User.Read*</span></span> |
|<span data-ttu-id="5085b-222">startTime</span><span class="sxs-lookup"><span data-stu-id="5085b-222">startTime</span></span>|<span data-ttu-id="5085b-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5085b-223">DateTimeOffset</span></span>| <span data-ttu-id="5085b-224">目前，开始时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="5085b-224">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5085b-225">关系</span><span class="sxs-lookup"><span data-stu-id="5085b-225">Relationships</span></span>
<span data-ttu-id="5085b-226">无。</span><span class="sxs-lookup"><span data-stu-id="5085b-226">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5085b-227">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5085b-227">JSON representation</span></span>

<span data-ttu-id="5085b-228">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5085b-228">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.oAuth2PermissionGrant"
}-->

```json
{
  "clientId": "string",
  "consentType": "string",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)",
  "expiryTime": "String (timestamp)"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2PermissionGrant resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


