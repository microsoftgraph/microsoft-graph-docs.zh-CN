---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予应用程序的 (OAuth 2.0 作用域) 的委派权限，这通常是由用户或管理员同意流程导致的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 32a3acf998b9be8c5a7001ea83a50f177c332933
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026563"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="96e8c-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="96e8c-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="96e8c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96e8c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96e8c-105">表示已授予应用程序的服务主体的委派权限。</span><span class="sxs-lookup"><span data-stu-id="96e8c-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="96e8c-106">委派权限授予可因用户同意应用程序的访问 API 的请求而创建，或直接创建。</span><span class="sxs-lookup"><span data-stu-id="96e8c-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="96e8c-107">委派权限有时称为 "OAuth 2.0 作用域" 或 "作用域"。</span><span class="sxs-lookup"><span data-stu-id="96e8c-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="96e8c-108">方法</span><span class="sxs-lookup"><span data-stu-id="96e8c-108">Methods</span></span>

| <span data-ttu-id="96e8c-109">方法</span><span class="sxs-lookup"><span data-stu-id="96e8c-109">Method</span></span> | <span data-ttu-id="96e8c-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="96e8c-110">Return Type</span></span> | <span data-ttu-id="96e8c-111">说明</span><span class="sxs-lookup"><span data-stu-id="96e8c-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="96e8c-112">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="96e8c-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="96e8c-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96e8c-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="96e8c-114">检索委派权限授予的列表。</span><span class="sxs-lookup"><span data-stu-id="96e8c-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="96e8c-115">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="96e8c-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="96e8c-117">阅读单个委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="96e8c-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="96e8c-118">创建 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="96e8c-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="96e8c-120">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="96e8c-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="96e8c-121">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="96e8c-122">无</span><span class="sxs-lookup"><span data-stu-id="96e8c-122">None</span></span> | <span data-ttu-id="96e8c-123">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="96e8c-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="96e8c-124">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="96e8c-125">无</span><span class="sxs-lookup"><span data-stu-id="96e8c-125">None</span></span>  | <span data-ttu-id="96e8c-126">删除委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="96e8c-126">Delete a delegated permission grant.</span></span> |

## <a name="properties"></a><span data-ttu-id="96e8c-127">属性</span><span class="sxs-lookup"><span data-stu-id="96e8c-127">Properties</span></span>

| <span data-ttu-id="96e8c-128">属性</span><span class="sxs-lookup"><span data-stu-id="96e8c-128">Property</span></span> | <span data-ttu-id="96e8c-129">类型</span><span class="sxs-lookup"><span data-stu-id="96e8c-129">Type</span></span> | <span data-ttu-id="96e8c-130">说明</span><span class="sxs-lookup"><span data-stu-id="96e8c-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="96e8c-131">id</span><span class="sxs-lookup"><span data-stu-id="96e8c-131">id</span></span> | <span data-ttu-id="96e8c-132">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-132">String</span></span> | <span data-ttu-id="96e8c-133">**OAuth2PermissionGrant**的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="96e8c-133">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="96e8c-134">只读。</span><span class="sxs-lookup"><span data-stu-id="96e8c-134">Read-only.</span></span>|
| <span data-ttu-id="96e8c-135">clientId</span><span class="sxs-lookup"><span data-stu-id="96e8c-135">clientId</span></span> | <span data-ttu-id="96e8c-136">字符串</span><span class="sxs-lookup"><span data-stu-id="96e8c-136">String</span></span> | <span data-ttu-id="96e8c-137">授权在访问 API 时代表登录用户执行操作的应用程序的客户端[服务主体](serviceprincipal.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="96e8c-137">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="96e8c-138">必需。</span><span class="sxs-lookup"><span data-stu-id="96e8c-138">Required.</span></span> <span data-ttu-id="96e8c-139">`$filter`仅支持 `eq`)  (。</span><span class="sxs-lookup"><span data-stu-id="96e8c-139">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="96e8c-140">consentType</span><span class="sxs-lookup"><span data-stu-id="96e8c-140">consentType</span></span> | <span data-ttu-id="96e8c-141">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-141">String</span></span> | <span data-ttu-id="96e8c-142">指示是否向客户端应用程序授予了授权以模拟所有用户或仅模拟特定用户。</span><span class="sxs-lookup"><span data-stu-id="96e8c-142">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="96e8c-143">*AllPrincipals* 表示模拟所有用户的授权。</span><span class="sxs-lookup"><span data-stu-id="96e8c-143">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="96e8c-144">*主体* 指示模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="96e8c-144">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="96e8c-145">管理员可以授予代表所有用户的同意。</span><span class="sxs-lookup"><span data-stu-id="96e8c-145">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="96e8c-146">在某些情况下，对于某些委派权限，非管理员用户可能有权代表自己同意代表自己。</span><span class="sxs-lookup"><span data-stu-id="96e8c-146">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="96e8c-147">必需。</span><span class="sxs-lookup"><span data-stu-id="96e8c-147">Required.</span></span> <span data-ttu-id="96e8c-148">`$filter`仅支持 `eq`)  (。</span><span class="sxs-lookup"><span data-stu-id="96e8c-148">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="96e8c-149">principalId</span><span class="sxs-lookup"><span data-stu-id="96e8c-149">principalId</span></span> | <span data-ttu-id="96e8c-150">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-150">String</span></span> | <span data-ttu-id="96e8c-151">当**consentType**为*Principal*时，代表其授权客户端访问该资源的[用户](user.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="96e8c-151">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="96e8c-152">如果 **consentType** 为 *AllPrincipals* ，则此值为 null。</span><span class="sxs-lookup"><span data-stu-id="96e8c-152">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="96e8c-153">当 **consentType** 为 *Principal*时是必需的。</span><span class="sxs-lookup"><span data-stu-id="96e8c-153">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="96e8c-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="96e8c-154">resourceId</span></span> | <span data-ttu-id="96e8c-155">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-155">String</span></span> | <span data-ttu-id="96e8c-156">向其授予访问权限的资源[服务主体](serviceprincipal.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="96e8c-156">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="96e8c-157">这将标识客户端授权尝试代表已登录用户呼叫的 API。</span><span class="sxs-lookup"><span data-stu-id="96e8c-157">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="96e8c-158">scope</span><span class="sxs-lookup"><span data-stu-id="96e8c-158">scope</span></span> | <span data-ttu-id="96e8c-159">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-159">String</span></span> | <span data-ttu-id="96e8c-160">委派权限的声明值列表，应包含在 API)  (的资源应用程序的访问令牌中。</span><span class="sxs-lookup"><span data-stu-id="96e8c-160">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="96e8c-161">例如，`openid User.Read GroupMember.Read.All`。</span><span class="sxs-lookup"><span data-stu-id="96e8c-161">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="96e8c-162">每个声明值都应与 API 定义的某个委派权限的**值**字段相匹配，这些权限在资源[服务主体](serviceprincipal.md)的**publishedPermissionScopes**属性中列出。</span><span class="sxs-lookup"><span data-stu-id="96e8c-162">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |
| <span data-ttu-id="96e8c-163">startTime</span><span class="sxs-lookup"><span data-stu-id="96e8c-163">startTime</span></span> | <span data-ttu-id="96e8c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96e8c-164">DateTimeOffset</span></span> | <span data-ttu-id="96e8c-165">目前，启动时间值被忽略，但在创建 **oAuth2PermissionGrant**时需要一个值。</span><span class="sxs-lookup"><span data-stu-id="96e8c-165">Currently, the start time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="96e8c-166">必需。</span><span class="sxs-lookup"><span data-stu-id="96e8c-166">Required.</span></span> |
| <span data-ttu-id="96e8c-167">expiryTime</span><span class="sxs-lookup"><span data-stu-id="96e8c-167">expiryTime</span></span> | <span data-ttu-id="96e8c-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96e8c-168">DateTimeOffset</span></span> | <span data-ttu-id="96e8c-169">目前，结束时间值将被忽略，但在创建 **oAuth2PermissionGrant**时需要一个值。</span><span class="sxs-lookup"><span data-stu-id="96e8c-169">Currently, the end time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="96e8c-170">必需。</span><span class="sxs-lookup"><span data-stu-id="96e8c-170">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96e8c-171">关系</span><span class="sxs-lookup"><span data-stu-id="96e8c-171">Relationships</span></span>

<span data-ttu-id="96e8c-172">无。</span><span class="sxs-lookup"><span data-stu-id="96e8c-172">None.</span></span>

<span data-ttu-id="96e8c-173">该资源支持通过提供 [delta](../api/oauth2permissiongrant-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="96e8c-173">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="96e8c-174">方法</span><span class="sxs-lookup"><span data-stu-id="96e8c-174">Methods</span></span>

| <span data-ttu-id="96e8c-175">方法</span><span class="sxs-lookup"><span data-stu-id="96e8c-175">Method</span></span>           | <span data-ttu-id="96e8c-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="96e8c-176">Return Type</span></span>    |<span data-ttu-id="96e8c-177">说明</span><span class="sxs-lookup"><span data-stu-id="96e8c-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="96e8c-178">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="96e8c-178">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="96e8c-179">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96e8c-179">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="96e8c-180">检索 **oauth2PermissionGrant** 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="96e8c-180">Retrieve a list of **oauth2PermissionGrant** objects.</span></span> |
|[<span data-ttu-id="96e8c-181">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-181">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="96e8c-182">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-182">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="96e8c-183">读取 **oAuth2PermissionGrant** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96e8c-183">Read the properties and relationships of an **oAuth2PermissionGrant** object.</span></span>|
|[<span data-ttu-id="96e8c-184">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-184">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="96e8c-185">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-185">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="96e8c-186">更新  **oAuth2PermissionGrant** 对象。</span><span class="sxs-lookup"><span data-stu-id="96e8c-186">Update an  **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="96e8c-187">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-187">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="96e8c-188">无</span><span class="sxs-lookup"><span data-stu-id="96e8c-188">None</span></span> |<span data-ttu-id="96e8c-189">删除 **oAuth2PermissionGrant** 对象。</span><span class="sxs-lookup"><span data-stu-id="96e8c-189">Delete an **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="96e8c-190">Get delta</span><span class="sxs-lookup"><span data-stu-id="96e8c-190">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="96e8c-191">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="96e8c-191">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="96e8c-192">获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而不执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="96e8c-192">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="96e8c-193">属性</span><span class="sxs-lookup"><span data-stu-id="96e8c-193">Properties</span></span>
| <span data-ttu-id="96e8c-194">属性</span><span class="sxs-lookup"><span data-stu-id="96e8c-194">Property</span></span>     | <span data-ttu-id="96e8c-195">类型</span><span class="sxs-lookup"><span data-stu-id="96e8c-195">Type</span></span>   |<span data-ttu-id="96e8c-196">说明</span><span class="sxs-lookup"><span data-stu-id="96e8c-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96e8c-197">clientId</span><span class="sxs-lookup"><span data-stu-id="96e8c-197">clientId</span></span>|<span data-ttu-id="96e8c-198">字符串</span><span class="sxs-lookup"><span data-stu-id="96e8c-198">String</span></span>| <span data-ttu-id="96e8c-199">在访问资源 (由 resourceId 属性) 所代表的资源时，已授予同意模拟用户的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="96e8c-199">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="96e8c-200">consentType</span><span class="sxs-lookup"><span data-stu-id="96e8c-200">consentType</span></span>|<span data-ttu-id="96e8c-201">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-201">String</span></span>| <span data-ttu-id="96e8c-202">指示管理员是由管理员 (代表组织) 还是由个人提供。</span><span class="sxs-lookup"><span data-stu-id="96e8c-202">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="96e8c-203">可能的值为 *AllPrincipals* 或 *Principal*。</span><span class="sxs-lookup"><span data-stu-id="96e8c-203">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="96e8c-204">expiryTime</span><span class="sxs-lookup"><span data-stu-id="96e8c-204">expiryTime</span></span>|<span data-ttu-id="96e8c-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96e8c-205">DateTimeOffset</span></span>| <span data-ttu-id="96e8c-206">目前，到期时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="96e8c-206">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="96e8c-207">id</span><span class="sxs-lookup"><span data-stu-id="96e8c-207">id</span></span>|<span data-ttu-id="96e8c-208">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-208">String</span></span>| <span data-ttu-id="96e8c-209">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="96e8c-209">Unique identifier.</span></span> <span data-ttu-id="96e8c-210">只读。</span><span class="sxs-lookup"><span data-stu-id="96e8c-210">Read-only.</span></span>|
|<span data-ttu-id="96e8c-211">principalId</span><span class="sxs-lookup"><span data-stu-id="96e8c-211">principalId</span></span>|<span data-ttu-id="96e8c-212">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-212">String</span></span>| <span data-ttu-id="96e8c-213">如果 consentType 为 *AllPrincipals* ，则此值为 null，并且同意适用于组织中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="96e8c-213">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="96e8c-214">如果 consentType 为 *Principal*，则此属性指定授予同意的用户的 id，并且仅适用于该用户。</span><span class="sxs-lookup"><span data-stu-id="96e8c-214">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="96e8c-215">resourceId</span><span class="sxs-lookup"><span data-stu-id="96e8c-215">resourceId</span></span>|<span data-ttu-id="96e8c-216">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-216">String</span></span>| <span data-ttu-id="96e8c-217">指定已向其授予访问权限的资源服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="96e8c-217">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="96e8c-218">scope</span><span class="sxs-lookup"><span data-stu-id="96e8c-218">scope</span></span>|<span data-ttu-id="96e8c-219">String</span><span class="sxs-lookup"><span data-stu-id="96e8c-219">String</span></span>| <span data-ttu-id="96e8c-220">指定在 OAuth 2.0 访问令牌中，资源应用程序应预期的 [范围](/graph/permissions-reference) 声明的值。</span><span class="sxs-lookup"><span data-stu-id="96e8c-220">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="96e8c-221">例如， *User. Read*</span><span class="sxs-lookup"><span data-stu-id="96e8c-221">For example, *User.Read*</span></span> |
|<span data-ttu-id="96e8c-222">startTime</span><span class="sxs-lookup"><span data-stu-id="96e8c-222">startTime</span></span>|<span data-ttu-id="96e8c-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96e8c-223">DateTimeOffset</span></span>| <span data-ttu-id="96e8c-224">目前，开始时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="96e8c-224">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96e8c-225">关系</span><span class="sxs-lookup"><span data-stu-id="96e8c-225">Relationships</span></span>
<span data-ttu-id="96e8c-226">无。</span><span class="sxs-lookup"><span data-stu-id="96e8c-226">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="96e8c-227">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="96e8c-227">JSON representation</span></span>

<span data-ttu-id="96e8c-228">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96e8c-228">The following is a JSON representation of the resource.</span></span>

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


