---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予应用程序的 (OAuth 2.0 作用域) 的委派权限，这通常是由用户或管理员同意流程导致的。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: 557bd9973a3a04ffedb2104a480823de21c95499
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48041195"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="e7e8a-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="e7e8a-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="e7e8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7e8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e7e8a-105">表示已授予应用程序的服务主体的委派权限。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="e7e8a-106">委派权限授予可因用户同意应用程序的访问 API 的请求而创建，或直接创建。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="e7e8a-107">委派权限有时称为 "OAuth 2.0 作用域" 或 "作用域"。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="e7e8a-108">方法</span><span class="sxs-lookup"><span data-stu-id="e7e8a-108">Methods</span></span>

| <span data-ttu-id="e7e8a-109">方法</span><span class="sxs-lookup"><span data-stu-id="e7e8a-109">Method</span></span> | <span data-ttu-id="e7e8a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e7e8a-110">Return Type</span></span> | <span data-ttu-id="e7e8a-111">说明</span><span class="sxs-lookup"><span data-stu-id="e7e8a-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="e7e8a-112">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="e7e8a-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="e7e8a-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e7e8a-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="e7e8a-114">检索委派权限授予的列表。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="e7e8a-115">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e7e8a-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="e7e8a-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e7e8a-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="e7e8a-117">阅读单个委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="e7e8a-118">创建 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e7e8a-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="e7e8a-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e7e8a-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="e7e8a-120">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="e7e8a-121">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e7e8a-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="e7e8a-122">无</span><span class="sxs-lookup"><span data-stu-id="e7e8a-122">None</span></span> | <span data-ttu-id="e7e8a-123">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="e7e8a-124">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e7e8a-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="e7e8a-125">无</span><span class="sxs-lookup"><span data-stu-id="e7e8a-125">None</span></span>  | <span data-ttu-id="e7e8a-126">删除委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-126">Delete a delegated permission grant.</span></span> |
|[<span data-ttu-id="e7e8a-127">Get delta</span><span class="sxs-lookup"><span data-stu-id="e7e8a-127">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="e7e8a-128">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="e7e8a-128">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="e7e8a-129">获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而不执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-129">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e7e8a-130">属性</span><span class="sxs-lookup"><span data-stu-id="e7e8a-130">Properties</span></span>

| <span data-ttu-id="e7e8a-131">属性</span><span class="sxs-lookup"><span data-stu-id="e7e8a-131">Property</span></span> | <span data-ttu-id="e7e8a-132">类型</span><span class="sxs-lookup"><span data-stu-id="e7e8a-132">Type</span></span> | <span data-ttu-id="e7e8a-133">说明</span><span class="sxs-lookup"><span data-stu-id="e7e8a-133">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="e7e8a-134">id</span><span class="sxs-lookup"><span data-stu-id="e7e8a-134">id</span></span> | <span data-ttu-id="e7e8a-135">String</span><span class="sxs-lookup"><span data-stu-id="e7e8a-135">String</span></span> | <span data-ttu-id="e7e8a-136">**OAuth2PermissionGrant**的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-136">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="e7e8a-137">只读。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-137">Read-only.</span></span>|
| <span data-ttu-id="e7e8a-138">clientId</span><span class="sxs-lookup"><span data-stu-id="e7e8a-138">clientId</span></span> | <span data-ttu-id="e7e8a-139">字符串</span><span class="sxs-lookup"><span data-stu-id="e7e8a-139">String</span></span> | <span data-ttu-id="e7e8a-140">授权在访问 API 时代表登录用户执行操作的应用程序的客户端[服务主体](serviceprincipal.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-140">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="e7e8a-141">必需。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-141">Required.</span></span> <span data-ttu-id="e7e8a-142">`$filter`仅支持 `eq`)  (。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-142">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="e7e8a-143">consentType</span><span class="sxs-lookup"><span data-stu-id="e7e8a-143">consentType</span></span> | <span data-ttu-id="e7e8a-144">String</span><span class="sxs-lookup"><span data-stu-id="e7e8a-144">String</span></span> | <span data-ttu-id="e7e8a-145">指示是否向客户端应用程序授予了授权以模拟所有用户或仅模拟特定用户。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-145">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="e7e8a-146">*AllPrincipals* 表示模拟所有用户的授权。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-146">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="e7e8a-147">*主体* 指示模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-147">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="e7e8a-148">管理员可以授予代表所有用户的同意。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-148">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="e7e8a-149">在某些情况下，对于某些委派权限，非管理员用户可能有权代表自己同意代表自己。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-149">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="e7e8a-150">必需。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-150">Required.</span></span> <span data-ttu-id="e7e8a-151">`$filter`仅支持 `eq`)  (。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-151">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="e7e8a-152">principalId</span><span class="sxs-lookup"><span data-stu-id="e7e8a-152">principalId</span></span> | <span data-ttu-id="e7e8a-153">String</span><span class="sxs-lookup"><span data-stu-id="e7e8a-153">String</span></span> | <span data-ttu-id="e7e8a-154">当**consentType**为*Principal*时，代表其授权客户端访问该资源的[用户](user.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-154">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="e7e8a-155">如果 **consentType** 为 *AllPrincipals* ，则此值为 null。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-155">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="e7e8a-156">当 **consentType** 为 *Principal*时是必需的。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-156">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="e7e8a-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="e7e8a-157">resourceId</span></span> | <span data-ttu-id="e7e8a-158">String</span><span class="sxs-lookup"><span data-stu-id="e7e8a-158">String</span></span> | <span data-ttu-id="e7e8a-159">向其授予访问权限的资源[服务主体](serviceprincipal.md)的**id** 。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-159">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="e7e8a-160">这将标识客户端授权尝试代表已登录用户呼叫的 API。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-160">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="e7e8a-161">scope</span><span class="sxs-lookup"><span data-stu-id="e7e8a-161">scope</span></span> | <span data-ttu-id="e7e8a-162">String</span><span class="sxs-lookup"><span data-stu-id="e7e8a-162">String</span></span> | <span data-ttu-id="e7e8a-163">委派权限的声明值列表，应包含在 API)  (的资源应用程序的访问令牌中。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-163">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="e7e8a-164">例如，`openid User.Read GroupMember.Read.All`。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-164">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="e7e8a-165">每个声明值都应与 API 定义的某个委派权限的**值**字段相匹配，这些权限在资源[服务主体](serviceprincipal.md)的**publishedPermissionScopes**属性中列出。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-165">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="e7e8a-166">关系</span><span class="sxs-lookup"><span data-stu-id="e7e8a-166">Relationships</span></span>

<span data-ttu-id="e7e8a-167">无。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-167">None.</span></span>

<span data-ttu-id="e7e8a-168">该资源支持通过提供 [delta](../api/oauth2permissiongrant-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-168">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e7e8a-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e7e8a-169">JSON representation</span></span>

<span data-ttu-id="e7e8a-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7e8a-170">The following is a JSON representation of the resource.</span></span>

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
  "scope": "string"
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

