---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予 (OAuth 2.0) （通常是由于用户或管理员同意过程）的委派权限。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: 27977a758e937312b2d0ea45c84902c275b035ab
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52546880"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="ba167-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="ba167-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="ba167-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba167-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba167-105">表示已授予应用程序的服务主体的委派权限。</span><span class="sxs-lookup"><span data-stu-id="ba167-105">Represents the delegated permissions that have been granted to an application's service principal.</span></span>

<span data-ttu-id="ba167-106">委派权限授予可以在用户同意应用程序访问 API 的请求时创建，也可以直接创建。</span><span class="sxs-lookup"><span data-stu-id="ba167-106">Delegated permissions grants can be created as a result of a user consenting the an application's request to access an API, or created directly.</span></span>

<span data-ttu-id="ba167-107">委派权限有时称为"OAuth 2.0 范围"或"范围"。</span><span class="sxs-lookup"><span data-stu-id="ba167-107">Delegated permissions are sometimes referred to as "OAuth 2.0 scopes" or "scopes".</span></span>

## <a name="methods"></a><span data-ttu-id="ba167-108">方法</span><span class="sxs-lookup"><span data-stu-id="ba167-108">Methods</span></span>

| <span data-ttu-id="ba167-109">方法</span><span class="sxs-lookup"><span data-stu-id="ba167-109">Method</span></span> | <span data-ttu-id="ba167-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="ba167-110">Return Type</span></span> | <span data-ttu-id="ba167-111">说明</span><span class="sxs-lookup"><span data-stu-id="ba167-111">Description</span></span> |
|:---------------|:--------|:----------|
| [<span data-ttu-id="ba167-112">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="ba167-112">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="ba167-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba167-113">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="ba167-114">检索委派权限授予的列表。</span><span class="sxs-lookup"><span data-stu-id="ba167-114">Retrieve a list of delegated permission grants.</span></span> |
| [<span data-ttu-id="ba167-115">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ba167-115">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="ba167-116">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ba167-116">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)  | <span data-ttu-id="ba167-117">读取单个委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="ba167-117">Read a single delegated permission grant.</span></span>|
| [<span data-ttu-id="ba167-118">创建 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ba167-118">Create oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-post.md) | [<span data-ttu-id="ba167-119">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ba167-119">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) | <span data-ttu-id="ba167-120">创建委派权限授予。</span><span class="sxs-lookup"><span data-stu-id="ba167-120">Create a delegated permission grant.</span></span> |
| [<span data-ttu-id="ba167-121">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ba167-121">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | <span data-ttu-id="ba167-122">无</span><span class="sxs-lookup"><span data-stu-id="ba167-122">None</span></span> | <span data-ttu-id="ba167-123">更新 oAuth2PermissionGrant 对象。</span><span class="sxs-lookup"><span data-stu-id="ba167-123">Update oAuth2PermissionGrant object.</span></span> |
| [<span data-ttu-id="ba167-124">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="ba167-124">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="ba167-125">无</span><span class="sxs-lookup"><span data-stu-id="ba167-125">None</span></span>  | <span data-ttu-id="ba167-126">删除委派的权限授予。</span><span class="sxs-lookup"><span data-stu-id="ba167-126">Delete a delegated permission grant.</span></span> |
| [<span data-ttu-id="ba167-127">delta</span><span class="sxs-lookup"><span data-stu-id="ba167-127">Delta</span></span>](../api/oauth2permissiongrant-delta.md) | <span data-ttu-id="ba167-128">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ba167-128">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> |<span data-ttu-id="ba167-129">获取新创建、更新或删除的 **oauth2permissiongrant** 对象，而无需执行整个资源集合的完整读取。</span><span class="sxs-lookup"><span data-stu-id="ba167-129">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span> |

## <a name="properties"></a><span data-ttu-id="ba167-130">属性</span><span class="sxs-lookup"><span data-stu-id="ba167-130">Properties</span></span>

| <span data-ttu-id="ba167-131">属性</span><span class="sxs-lookup"><span data-stu-id="ba167-131">Property</span></span> | <span data-ttu-id="ba167-132">类型</span><span class="sxs-lookup"><span data-stu-id="ba167-132">Type</span></span> | <span data-ttu-id="ba167-133">说明</span><span class="sxs-lookup"><span data-stu-id="ba167-133">Description</span></span> |
|:---------------|:--------|:----------|
| <span data-ttu-id="ba167-134">id</span><span class="sxs-lookup"><span data-stu-id="ba167-134">id</span></span> | <span data-ttu-id="ba167-135">String</span><span class="sxs-lookup"><span data-stu-id="ba167-135">String</span></span> | <span data-ttu-id="ba167-136">**oAuth2PermissionGrant 的唯一标识符**。</span><span class="sxs-lookup"><span data-stu-id="ba167-136">Unique identifier for the **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="ba167-137">只读。</span><span class="sxs-lookup"><span data-stu-id="ba167-137">Read-only.</span></span>|
| <span data-ttu-id="ba167-138">clientId</span><span class="sxs-lookup"><span data-stu-id="ba167-138">clientId</span></span> | <span data-ttu-id="ba167-139">字符串</span><span class="sxs-lookup"><span data-stu-id="ba167-139">String</span></span> | <span data-ttu-id="ba167-140">**授权** 在访问 API [](serviceprincipal.md)时代表已登录用户操作的应用程序的客户端服务主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="ba167-140">The **id** of the client [service principal](serviceprincipal.md) for the application which is authorized to act on behalf of a signed-in user when accessing an API.</span></span> <span data-ttu-id="ba167-141">必填。</span><span class="sxs-lookup"><span data-stu-id="ba167-141">Required.</span></span> <span data-ttu-id="ba167-142">支持 `$filter`（仅 `eq`）。</span><span class="sxs-lookup"><span data-stu-id="ba167-142">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="ba167-143">consentType</span><span class="sxs-lookup"><span data-stu-id="ba167-143">consentType</span></span> | <span data-ttu-id="ba167-144">String</span><span class="sxs-lookup"><span data-stu-id="ba167-144">String</span></span> | <span data-ttu-id="ba167-145">指示是否向客户端应用程序授予了模拟所有用户或仅模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="ba167-145">Indicates whether authorization is granted for the client application to impersonate all users or only a specific user.</span></span> <span data-ttu-id="ba167-146">*AllPrincipals* 指示对模拟所有用户的授权。</span><span class="sxs-lookup"><span data-stu-id="ba167-146">*AllPrincipals* indicates authorization to impersonate all users.</span></span> <span data-ttu-id="ba167-147">*主体* 指示对模拟特定用户的授权。</span><span class="sxs-lookup"><span data-stu-id="ba167-147">*Principal* indicates authorization to impersonate a specific user.</span></span> <span data-ttu-id="ba167-148">管理员可以代表所有用户授予同意。</span><span class="sxs-lookup"><span data-stu-id="ba167-148">Consent on behalf of all users can be granted by an administrator.</span></span> <span data-ttu-id="ba167-149">在某些情况下，可能会授权非管理员用户代表自己同意某些委派权限。</span><span class="sxs-lookup"><span data-stu-id="ba167-149">Non-admin users may be authorized to consent on behalf of themselves in some cases, for some delegated permissions.</span></span> <span data-ttu-id="ba167-150">必填。</span><span class="sxs-lookup"><span data-stu-id="ba167-150">Required.</span></span> <span data-ttu-id="ba167-151">支持 `$filter`（仅 `eq`）。</span><span class="sxs-lookup"><span data-stu-id="ba167-151">Supports `$filter` (`eq` only).</span></span> |
| <span data-ttu-id="ba167-152">principalId</span><span class="sxs-lookup"><span data-stu-id="ba167-152">principalId</span></span> | <span data-ttu-id="ba167-153">String</span><span class="sxs-lookup"><span data-stu-id="ba167-153">String</span></span> | <span data-ttu-id="ba167-154">当 **consentType** [为 Principal](user.md)时，客户端有权访问资源的用户的 **ID。** </span><span class="sxs-lookup"><span data-stu-id="ba167-154">The **id** of the [user](user.md) on behalf of whom the client is authorized to access the resource, when **consentType** is *Principal*.</span></span> <span data-ttu-id="ba167-155">如果 **consentType** 为 *AllPrincipals，* 则此值为 null。</span><span class="sxs-lookup"><span data-stu-id="ba167-155">If **consentType** is *AllPrincipals* this value is null.</span></span> <span data-ttu-id="ba167-156">当 **consentType** 为 Principal 时 *是必需的*。</span><span class="sxs-lookup"><span data-stu-id="ba167-156">Required when **consentType** is *Principal*.</span></span> |
| <span data-ttu-id="ba167-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="ba167-157">resourceId</span></span> | <span data-ttu-id="ba167-158">String</span><span class="sxs-lookup"><span data-stu-id="ba167-158">String</span></span> | <span data-ttu-id="ba167-159">**有权访问** 的资源 [服务主体](serviceprincipal.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="ba167-159">The **id** of the resource [service principal](serviceprincipal.md) to which access is authorized.</span></span> <span data-ttu-id="ba167-160">这标识了客户端有权尝试代表登录用户调用的 API。</span><span class="sxs-lookup"><span data-stu-id="ba167-160">This identifies the API which the client is authorized to attempt to call on behalf of a signed-in user.</span></span> |
| <span data-ttu-id="ba167-161">scope</span><span class="sxs-lookup"><span data-stu-id="ba167-161">scope</span></span> | <span data-ttu-id="ba167-162">String</span><span class="sxs-lookup"><span data-stu-id="ba167-162">String</span></span> | <span data-ttu-id="ba167-163">委派权限声明值的列表（以空格分隔）应包含在 API (访问令牌) 。</span><span class="sxs-lookup"><span data-stu-id="ba167-163">A space-separated list of the claim values for delegated permissions which should be included in access tokens for the resource application (the API).</span></span> <span data-ttu-id="ba167-164">例如，`openid User.Read GroupMember.Read.All`。</span><span class="sxs-lookup"><span data-stu-id="ba167-164">For example, `openid User.Read GroupMember.Read.All`.</span></span> <span data-ttu-id="ba167-165">每个声明值都应与资源服务主体 的 **publishedPermissionScopes** 属性中列出的 API 定义的委派权限之一的值 [字段匹配](serviceprincipal.md)。</span><span class="sxs-lookup"><span data-stu-id="ba167-165">Each claim value should match the **value** field of one of the delegated permissions defined by the API, listed in the **publishedPermissionScopes** property of the resource [service principal](serviceprincipal.md).</span></span> |
| <span data-ttu-id="ba167-166">startTime</span><span class="sxs-lookup"><span data-stu-id="ba167-166">startTime</span></span> | <span data-ttu-id="ba167-167">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba167-167">DateTimeOffset</span></span> | <span data-ttu-id="ba167-168">目前，将忽略开始时间值，但创建 **oAuth2PermissionGrant** 时需要一个值。</span><span class="sxs-lookup"><span data-stu-id="ba167-168">Currently, the start time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="ba167-169">必填。</span><span class="sxs-lookup"><span data-stu-id="ba167-169">Required.</span></span> |
| <span data-ttu-id="ba167-170">expiryTime</span><span class="sxs-lookup"><span data-stu-id="ba167-170">expiryTime</span></span> | <span data-ttu-id="ba167-171">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ba167-171">DateTimeOffset</span></span> | <span data-ttu-id="ba167-172">目前，将忽略结束时间值，但创建 **oAuth2PermissionGrant** 时需要一个值。</span><span class="sxs-lookup"><span data-stu-id="ba167-172">Currently, the end time value is ignored, but a value is required when creating an **oAuth2PermissionGrant**.</span></span> <span data-ttu-id="ba167-173">必填。</span><span class="sxs-lookup"><span data-stu-id="ba167-173">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ba167-174">关系</span><span class="sxs-lookup"><span data-stu-id="ba167-174">Relationships</span></span>
<span data-ttu-id="ba167-175">无。</span><span class="sxs-lookup"><span data-stu-id="ba167-175">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba167-176">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ba167-176">JSON representation</span></span>

<span data-ttu-id="ba167-177">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ba167-177">The following is a JSON representation of the resource.</span></span>

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


