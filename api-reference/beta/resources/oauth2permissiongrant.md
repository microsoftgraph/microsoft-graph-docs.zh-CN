---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予应用程序的委派权限（OAuth 2.0 作用域），这通常是由用户或管理员的同意过程造成的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 39401f1708e8e27443348a766f171680fbd9efd7
ms.sourcegitcommit: 7a6231aeb570ff45d01b3db3df07a411f9f60fd1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2020
ms.locfileid: "44383747"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="cf137-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf137-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="cf137-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf137-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf137-105">表示已授予应用程序的服务主体的委派权限。</span><span class="sxs-lookup"><span data-stu-id="cf137-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="cf137-106">委派权限授予可因用户同意应用程序的访问 API 的请求而创建，或直接创建。</span><span class="sxs-lookup"><span data-stu-id="cf137-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="cf137-107">委派权限有时称为 "OAuth 2.0 作用域" 或 "作用域"。</span><span class="sxs-lookup"><span data-stu-id="cf137-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="cf137-108">Methods</span><span class="sxs-lookup"><span data-stu-id="cf137-108">Methods</span></span>

| <span data-ttu-id="cf137-109">方法</span><span class="sxs-lookup"><span data-stu-id="cf137-109">Method</span></span> | <span data-ttu-id="cf137-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf137-110">Return Type</span></span> | <span data-ttu-id="cf137-111">说明</span><span class="sxs-lookup"><span data-stu-id="cf137-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="cf137-112">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="cf137-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="cf137-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cf137-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="cf137-114">检索委派权限授予的列表。</span><span class="sxs-lookup"><span data-stu-id="cf137-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="cf137-115">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="cf137-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="cf137-117">阅读单个委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="cf137-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="cf137-118">创建 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="cf137-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="cf137-120">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="cf137-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="cf137-121">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="cf137-122">无</span><span class="sxs-lookup"><span data-stu-id="cf137-122">None</span></span> | <span data-ttu-id="cf137-123">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="cf137-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="cf137-124">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="cf137-125">无</span><span class="sxs-lookup"><span data-stu-id="cf137-125">None</span></span>  | <span data-ttu-id="cf137-126">删除委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="cf137-126">Delete a delegated permission grant.</span></span> |

## <a name="properties"></a><span data-ttu-id="cf137-127">属性</span><span class="sxs-lookup"><span data-stu-id="cf137-127">Properties</span></span>

| <span data-ttu-id="cf137-128">属性</span><span class="sxs-lookup"><span data-stu-id="cf137-128">Property</span></span> | <span data-ttu-id="cf137-129">类型</span><span class="sxs-lookup"><span data-stu-id="cf137-129">Type</span></span> | <span data-ttu-id="cf137-130">说明</span><span class="sxs-lookup"><span data-stu-id="cf137-130">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="cf137-131">id</span><span class="sxs-lookup"><span data-stu-id="cf137-131">id</span></span> | <span data-ttu-id="cf137-132">String</span><span class="sxs-lookup"><span data-stu-id="cf137-132">String</span></span> | <span data-ttu-id="cf137-133">**OAuth2PermissionGrant**的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cf137-133">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="cf137-134">只读。</span><span class="sxs-lookup"><span data-stu-id="cf137-134">Read-only.</span></span>|
| <span data-ttu-id="cf137-135">clientId</span><span class="sxs-lookup"><span data-stu-id="cf137-135">clientId</span></span> | <span data-ttu-id="cf137-136">字符串</span><span class="sxs-lookup"><span data-stu-id="cf137-136">String</span></span> | <span data-ttu-id="cf137-137">授权在访问 API 时代表登录用户执行操作的应用程序的客户端[服务主体](serviceprincipal.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="cf137-137">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="cf137-138">必填。</span><span class="sxs-lookup"><span data-stu-id="cf137-138">Required.</span></span> <span data-ttu-id="cf137-139">支持 `$filter` （ `eq` 仅限）。</span><span class="sxs-lookup"><span data-stu-id="cf137-139">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="cf137-140">consentType</span><span class="sxs-lookup"><span data-stu-id="cf137-140">consentType</span></span> | <span data-ttu-id="cf137-141">String</span><span class="sxs-lookup"><span data-stu-id="cf137-141">String</span></span> | <span data-ttu-id="cf137-142">指示是否向客户端应用程序授予了授权以模拟所有用户或仅模拟特定用户。</span><span class="sxs-lookup"><span data-stu-id="cf137-142">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="cf137-143">*AllPrincipals*表示模拟所有用户的授权。</span><span class="sxs-lookup"><span data-stu-id="cf137-143">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="cf137-144">*主体*指示模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="cf137-144">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="cf137-145">管理员可以授予代表所有用户的同意。</span><span class="sxs-lookup"><span data-stu-id="cf137-145">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="cf137-146">在某些情况下，对于某些委派权限，非管理员用户可能有权代表自己同意代表自己。</span><span class="sxs-lookup"><span data-stu-id="cf137-146">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="cf137-147">必填。</span><span class="sxs-lookup"><span data-stu-id="cf137-147">Required.</span></span> <span data-ttu-id="cf137-148">支持 `$filter` （ `eq` 仅限）。</span><span class="sxs-lookup"><span data-stu-id="cf137-148">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="cf137-149">principalId</span><span class="sxs-lookup"><span data-stu-id="cf137-149">principalId</span></span> | <span data-ttu-id="cf137-150">String</span><span class="sxs-lookup"><span data-stu-id="cf137-150">String</span></span> | <span data-ttu-id="cf137-151">当**consentType**为*Principal*时，代表其授权客户端访问该资源的[用户](user.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="cf137-151">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="cf137-152">如果**consentType**为*AllPrincipals* ，则此值为 null。</span><span class="sxs-lookup"><span data-stu-id="cf137-152">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="cf137-153">当**consentType**为*Principal*时是必需的。</span><span class="sxs-lookup"><span data-stu-id="cf137-153">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="cf137-154">resourceId</span><span class="sxs-lookup"><span data-stu-id="cf137-154">resourceId</span></span> | <span data-ttu-id="cf137-155">String</span><span class="sxs-lookup"><span data-stu-id="cf137-155">String</span></span> | <span data-ttu-id="cf137-156">向其授予访问权限的资源[服务主体](serviceprincipal.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="cf137-156">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="cf137-157">这将标识客户端授权尝试代表已登录用户呼叫的 API。</span><span class="sxs-lookup"><span data-stu-id="cf137-157">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="cf137-158">scope</span><span class="sxs-lookup"><span data-stu-id="cf137-158">scope</span></span> | <span data-ttu-id="cf137-159">String</span><span class="sxs-lookup"><span data-stu-id="cf137-159">String</span></span> | <span data-ttu-id="cf137-160">应包含在资源应用程序（API）的访问令牌中的委派权限的声明值列表（以空格分隔）。</span><span class="sxs-lookup"><span data-stu-id="cf137-160">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="cf137-161">例如，`openid User.Read GroupMember.Read.All`。</span><span class="sxs-lookup"><span data-stu-id="cf137-161">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="cf137-162">每个声明值都应与 API 定义的某个委派权限的**值**字段相匹配，这些权限在资源[服务主体](serviceprincipal.md)的**publishedPermissionScopes**属性中列出。</span><span class="sxs-lookup"><span data-stu-id="cf137-162">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |
| <span data-ttu-id="cf137-163">startTime</span><span class="sxs-lookup"><span data-stu-id="cf137-163">startTime</span></span> | <span data-ttu-id="cf137-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf137-164">DateTimeOffset</span></span> | <span data-ttu-id="cf137-165">目前，启动时间值被忽略，但在创建**oAuth2PermissionGrant**时需要一个值。</span><span class="sxs-lookup"><span data-stu-id="cf137-165">Currently, the start time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="cf137-166">必填。</span><span class="sxs-lookup"><span data-stu-id="cf137-166">Required.</span></span> |
| <span data-ttu-id="cf137-167">expiryTime</span><span class="sxs-lookup"><span data-stu-id="cf137-167">expiryTime</span></span> | <span data-ttu-id="cf137-168">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf137-168">DateTimeOffset</span></span> | <span data-ttu-id="cf137-169">目前，结束时间值将被忽略，但在创建**oAuth2PermissionGrant**时需要一个值。</span><span class="sxs-lookup"><span data-stu-id="cf137-169">Currently, the end time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="cf137-170">必填。</span><span class="sxs-lookup"><span data-stu-id="cf137-170">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cf137-171">关系</span><span class="sxs-lookup"><span data-stu-id="cf137-171">Relationships</span></span>

<span data-ttu-id="cf137-172">无。</span><span class="sxs-lookup"><span data-stu-id="cf137-172">None.</span></span>

<span data-ttu-id="cf137-173">该资源支持通过提供 [delta](../api/oauth2permissiongrant-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="cf137-173">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="cf137-174">方法</span><span class="sxs-lookup"><span data-stu-id="cf137-174">Methods</span></span>

| <span data-ttu-id="cf137-175">方法</span><span class="sxs-lookup"><span data-stu-id="cf137-175">Method</span></span>           | <span data-ttu-id="cf137-176">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf137-176">Return Type</span></span>    |<span data-ttu-id="cf137-177">说明</span><span class="sxs-lookup"><span data-stu-id="cf137-177">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cf137-178">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="cf137-178">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="cf137-179">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="cf137-179">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="cf137-180">检索**oauth2PermissionGrant**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="cf137-180">Retrieve a list of **oauth2PermissionGrant** objects.</span></span> |
|[<span data-ttu-id="cf137-181">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-181">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="cf137-182">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-182">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="cf137-183">读取**oAuth2PermissionGrant**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf137-183">Read the properties and relationships of an **oAuth2PermissionGrant** object.</span></span>|
|[<span data-ttu-id="cf137-184">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-184">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="cf137-185">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-185">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="cf137-186">更新**oAuth2PermissionGrant**对象。</span><span class="sxs-lookup"><span data-stu-id="cf137-186">Update an  **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="cf137-187">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-187">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="cf137-188">无</span><span class="sxs-lookup"><span data-stu-id="cf137-188">None</span></span> |<span data-ttu-id="cf137-189">删除**oAuth2PermissionGrant**对象。</span><span class="sxs-lookup"><span data-stu-id="cf137-189">Delete an **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="cf137-190">Get delta</span><span class="sxs-lookup"><span data-stu-id="cf137-190">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="cf137-191">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="cf137-191">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="cf137-192">获取新创建、更新或删除的**oauth2permissiongrant**对象，而不执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="cf137-192">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="cf137-193">属性</span><span class="sxs-lookup"><span data-stu-id="cf137-193">Properties</span></span>
| <span data-ttu-id="cf137-194">属性</span><span class="sxs-lookup"><span data-stu-id="cf137-194">Property</span></span>     | <span data-ttu-id="cf137-195">类型</span><span class="sxs-lookup"><span data-stu-id="cf137-195">Type</span></span>   |<span data-ttu-id="cf137-196">说明</span><span class="sxs-lookup"><span data-stu-id="cf137-196">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cf137-197">clientId</span><span class="sxs-lookup"><span data-stu-id="cf137-197">clientId</span></span>|<span data-ttu-id="cf137-198">字符串</span><span class="sxs-lookup"><span data-stu-id="cf137-198">String</span></span>| <span data-ttu-id="cf137-199">在访问资源（由 resourceId 属性表示）时，授权模拟用户的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="cf137-199">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="cf137-200">consentType</span><span class="sxs-lookup"><span data-stu-id="cf137-200">consentType</span></span>|<span data-ttu-id="cf137-201">String</span><span class="sxs-lookup"><span data-stu-id="cf137-201">String</span></span>| <span data-ttu-id="cf137-202">指示许可是由管理员（代表组织）提供，还是由个人授予。</span><span class="sxs-lookup"><span data-stu-id="cf137-202">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="cf137-203">可能的值为*AllPrincipals*或*Principal*。</span><span class="sxs-lookup"><span data-stu-id="cf137-203">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="cf137-204">expiryTime</span><span class="sxs-lookup"><span data-stu-id="cf137-204">expiryTime</span></span>|<span data-ttu-id="cf137-205">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf137-205">DateTimeOffset</span></span>| <span data-ttu-id="cf137-206">目前，到期时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="cf137-206">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="cf137-207">id</span><span class="sxs-lookup"><span data-stu-id="cf137-207">id</span></span>|<span data-ttu-id="cf137-208">字符串</span><span class="sxs-lookup"><span data-stu-id="cf137-208">String</span></span>| <span data-ttu-id="cf137-209">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="cf137-209">Unique identifier.</span></span> <span data-ttu-id="cf137-210">只读。</span><span class="sxs-lookup"><span data-stu-id="cf137-210">Read-only.</span></span>|
|<span data-ttu-id="cf137-211">principalId</span><span class="sxs-lookup"><span data-stu-id="cf137-211">principalId</span></span>|<span data-ttu-id="cf137-212">String</span><span class="sxs-lookup"><span data-stu-id="cf137-212">String</span></span>| <span data-ttu-id="cf137-213">如果 consentType 为*AllPrincipals* ，则此值为 null，并且同意适用于组织中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="cf137-213">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="cf137-214">如果 consentType 为*Principal*，则此属性指定授予同意的用户的 id，并且仅适用于该用户。</span><span class="sxs-lookup"><span data-stu-id="cf137-214">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="cf137-215">resourceId</span><span class="sxs-lookup"><span data-stu-id="cf137-215">resourceId</span></span>|<span data-ttu-id="cf137-216">String</span><span class="sxs-lookup"><span data-stu-id="cf137-216">String</span></span>| <span data-ttu-id="cf137-217">指定已向其授予访问权限的资源服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="cf137-217">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="cf137-218">scope</span><span class="sxs-lookup"><span data-stu-id="cf137-218">scope</span></span>|<span data-ttu-id="cf137-219">String</span><span class="sxs-lookup"><span data-stu-id="cf137-219">String</span></span>| <span data-ttu-id="cf137-220">指定在 OAuth 2.0 访问令牌中，资源应用程序应预期的[范围](/graph/permissions-reference)声明的值。</span><span class="sxs-lookup"><span data-stu-id="cf137-220">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="cf137-221">例如， *User. Read*</span><span class="sxs-lookup"><span data-stu-id="cf137-221">For example, *User.Read*</span></span> |
|<span data-ttu-id="cf137-222">startTime</span><span class="sxs-lookup"><span data-stu-id="cf137-222">startTime</span></span>|<span data-ttu-id="cf137-223">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cf137-223">DateTimeOffset</span></span>| <span data-ttu-id="cf137-224">目前，开始时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="cf137-224">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cf137-225">关系</span><span class="sxs-lookup"><span data-stu-id="cf137-225">Relationships</span></span>
<span data-ttu-id="cf137-226">无。</span><span class="sxs-lookup"><span data-stu-id="cf137-226">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf137-227">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf137-227">JSON representation</span></span>

<span data-ttu-id="cf137-228">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf137-228">The following is a JSON representation of the resource.</span></span>

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
