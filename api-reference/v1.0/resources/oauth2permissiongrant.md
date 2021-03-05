---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予 (OAuth 2.0) （通常是由于用户或管理员同意过程）的委派权限。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: d0c9e78d22a882998c0e17ba521cc76a611697af
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50432842"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="1df70-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="1df70-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="1df70-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1df70-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1df70-105">表示已授予应用程序的服务主体的委派权限。</span><span class="sxs-lookup"><span data-stu-id="1df70-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="1df70-106">委派的权限授予可以是用户同意应用程序访问 API 请求的结果，也可以直接创建。</span><span class="sxs-lookup"><span data-stu-id="1df70-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="1df70-107">委派的权限有时称为"OAuth 2.0 范围"或"作用域"。</span><span class="sxs-lookup"><span data-stu-id="1df70-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="1df70-108">Methods</span><span class="sxs-lookup"><span data-stu-id="1df70-108">Methods</span></span>

| <span data-ttu-id="1df70-109">方法</span><span class="sxs-lookup"><span data-stu-id="1df70-109">Method</span></span> | <span data-ttu-id="1df70-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="1df70-110">Return Type</span></span> | <span data-ttu-id="1df70-111">说明</span><span class="sxs-lookup"><span data-stu-id="1df70-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="1df70-112">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="1df70-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="1df70-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1df70-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="1df70-114">检索委派权限授予的列表。</span><span class="sxs-lookup"><span data-stu-id="1df70-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="1df70-115">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1df70-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="1df70-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1df70-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="1df70-117">读取单个委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="1df70-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="1df70-118">创建 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1df70-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="1df70-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1df70-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="1df70-120">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="1df70-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="1df70-121">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1df70-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="1df70-122">无</span><span class="sxs-lookup"><span data-stu-id="1df70-122">None</span></span> | <span data-ttu-id="1df70-123">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="1df70-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="1df70-124">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1df70-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="1df70-125">无</span><span class="sxs-lookup"><span data-stu-id="1df70-125">None</span></span>  | <span data-ttu-id="1df70-126">删除委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="1df70-126">Delete a delegated permission grant.</span></span> |
|[<span data-ttu-id="1df70-127">获取 delta</span><span class="sxs-lookup"><span data-stu-id="1df70-127">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="1df70-128">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="1df70-128">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="1df70-129">获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而无需执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="1df70-129">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="1df70-130">属性</span><span class="sxs-lookup"><span data-stu-id="1df70-130">Properties</span></span>

| <span data-ttu-id="1df70-131">属性</span><span class="sxs-lookup"><span data-stu-id="1df70-131">Property</span></span> | <span data-ttu-id="1df70-132">类型</span><span class="sxs-lookup"><span data-stu-id="1df70-132">Type</span></span> | <span data-ttu-id="1df70-133">说明</span><span class="sxs-lookup"><span data-stu-id="1df70-133">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="1df70-134">id</span><span class="sxs-lookup"><span data-stu-id="1df70-134">id</span></span> | <span data-ttu-id="1df70-135">String</span><span class="sxs-lookup"><span data-stu-id="1df70-135">String</span></span> | <span data-ttu-id="1df70-136">**oAuth2PermissionGrant 的唯一标识符**。</span><span class="sxs-lookup"><span data-stu-id="1df70-136">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="1df70-137">只读。</span><span class="sxs-lookup"><span data-stu-id="1df70-137">Read-only.</span></span>|
| <span data-ttu-id="1df70-138">clientId</span><span class="sxs-lookup"><span data-stu-id="1df70-138">clientId</span></span> | <span data-ttu-id="1df70-139">字符串</span><span class="sxs-lookup"><span data-stu-id="1df70-139">String</span></span> | <span data-ttu-id="1df70-140">**应用程序** 客户端 [服务](serviceprincipal.md)主体的 ID，授权在访问 API 时代表登录用户操作。</span><span class="sxs-lookup"><span data-stu-id="1df70-140">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="1df70-141">必填。</span><span class="sxs-lookup"><span data-stu-id="1df70-141">Required.</span></span> <span data-ttu-id="1df70-142">支持 `$filter`（仅 `eq`）。</span><span class="sxs-lookup"><span data-stu-id="1df70-142">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="1df70-143">consentType</span><span class="sxs-lookup"><span data-stu-id="1df70-143">consentType</span></span> | <span data-ttu-id="1df70-144">String</span><span class="sxs-lookup"><span data-stu-id="1df70-144">String</span></span> | <span data-ttu-id="1df70-145">指示是否向客户端应用程序授予了模拟所有用户或仅模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="1df70-145">Indicates if authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="1df70-146">*AllPrincipals* 指示对模拟所有用户的授权。</span><span class="sxs-lookup"><span data-stu-id="1df70-146">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="1df70-147">*主体* 指示对模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="1df70-147">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="1df70-148">管理员可以代表所有用户授予同意。</span><span class="sxs-lookup"><span data-stu-id="1df70-148">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="1df70-149">在某些情况下，对于某些委派权限，非管理员用户可能有权代表自己同意。</span><span class="sxs-lookup"><span data-stu-id="1df70-149">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="1df70-150">必填。</span><span class="sxs-lookup"><span data-stu-id="1df70-150">Required.</span></span> <span data-ttu-id="1df70-151">支持 `$filter`（仅 `eq`）。</span><span class="sxs-lookup"><span data-stu-id="1df70-151">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="1df70-152">principalId</span><span class="sxs-lookup"><span data-stu-id="1df70-152">principalId</span></span> | <span data-ttu-id="1df70-153">String</span><span class="sxs-lookup"><span data-stu-id="1df70-153">String</span></span> | <span data-ttu-id="1df70-154">**consentType** 为 [Principal](user.md)时，客户端有权访问资源的用户的 *ID。*</span><span class="sxs-lookup"><span data-stu-id="1df70-154">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="1df70-155">如果 **consentType** *为 AllPrincipals，* 则此值为 null。</span><span class="sxs-lookup"><span data-stu-id="1df70-155">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="1df70-156">consentType 为 **主体** 时 *必需*。</span><span class="sxs-lookup"><span data-stu-id="1df70-156">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="1df70-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="1df70-157">resourceId</span></span> | <span data-ttu-id="1df70-158">String</span><span class="sxs-lookup"><span data-stu-id="1df70-158">String</span></span> | <span data-ttu-id="1df70-159">**有权访问** 的资源 [服务](serviceprincipal.md)主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="1df70-159">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="1df70-160">这标识了客户端有权尝试代表登录用户调用的 API。</span><span class="sxs-lookup"><span data-stu-id="1df70-160">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="1df70-161">scope</span><span class="sxs-lookup"><span data-stu-id="1df70-161">scope</span></span> | <span data-ttu-id="1df70-162">String</span><span class="sxs-lookup"><span data-stu-id="1df70-162">String</span></span> | <span data-ttu-id="1df70-163">委派权限声明值的列表（以空格分隔）应包含在 API (访问令牌) 。</span><span class="sxs-lookup"><span data-stu-id="1df70-163">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="1df70-164">例如，`openid User.Read GroupMember.Read.All`。</span><span class="sxs-lookup"><span data-stu-id="1df70-164">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="1df70-165">每个声明值应匹配由API 定义的委派权限之一的值字段，在资源服务主体的 **publishedPermissionScopes** 属性 [中列出](serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="1df70-165">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |

## <a name="relationships"></a><span data-ttu-id="1df70-166">关系</span><span class="sxs-lookup"><span data-stu-id="1df70-166">Relationships</span></span>

<span data-ttu-id="1df70-167">无。</span><span class="sxs-lookup"><span data-stu-id="1df70-167">None.</span></span>

<span data-ttu-id="1df70-168">该资源支持通过提供 [delta](../api/oauth2permissiongrant-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="1df70-168">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1df70-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1df70-169">JSON representation</span></span>

<span data-ttu-id="1df70-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1df70-170">The following is a JSON representation of the resource.</span></span>

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

