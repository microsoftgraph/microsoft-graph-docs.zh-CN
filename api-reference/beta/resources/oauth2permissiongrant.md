---
title: oAuth2PermissionGrant 资源类型
description: 表示已授予应用程序（由服务主体表示）作为用户或管理员同意过程的一部分的 OAuth 2.0 作用域（委派权限）。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: f00d9aa79e6a18e5dddf6881e251b3cbf00172e6
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543413"
---
# <a name="oauth2permissiongrant-resource-type"></a><span data-ttu-id="a45b8-103">oAuth2PermissionGrant 资源类型</span><span class="sxs-lookup"><span data-stu-id="a45b8-103">oAuth2PermissionGrant resource type</span></span>

<span data-ttu-id="a45b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a45b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a45b8-105">表示已授予应用程序（由服务主体表示）作为用户或管理员同意过程的一部分的 OAuth 2.0 作用域（委派权限）。</span><span class="sxs-lookup"><span data-stu-id="a45b8-105">Represents the OAuth 2.0 scopes (delegated permissions) that have been granted to an application (represented by a service principal) as part of the user or admin consent process.</span></span>

<span data-ttu-id="a45b8-106">该资源支持通过提供 [delta](../api/oauth2permissiongrant-delta.md) 函数使用[增量查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="a45b8-106">This resource supports using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/oauth2permissiongrant-delta.md) function.</span></span>

## <a name="methods"></a><span data-ttu-id="a45b8-107">方法</span><span class="sxs-lookup"><span data-stu-id="a45b8-107">Methods</span></span>

| <span data-ttu-id="a45b8-108">方法</span><span class="sxs-lookup"><span data-stu-id="a45b8-108">Method</span></span>           | <span data-ttu-id="a45b8-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a45b8-109">Return Type</span></span>    |<span data-ttu-id="a45b8-110">说明</span><span class="sxs-lookup"><span data-stu-id="a45b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a45b8-111">列出 oAuth2PermissionGrants</span><span class="sxs-lookup"><span data-stu-id="a45b8-111">List oAuth2PermissionGrants</span></span>](../api/oauth2permissiongrant-list.md) | <span data-ttu-id="a45b8-112">[oAuth2PermissionGrant](oauth2permissiongrant.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a45b8-112">[oAuth2PermissionGrant](oauth2permissiongrant.md) collection</span></span> | <span data-ttu-id="a45b8-113">检索**oauth2PermissionGrant**对象的列表。</span><span class="sxs-lookup"><span data-stu-id="a45b8-113">Retrieve a list of **oauth2PermissionGrant** objects.</span></span> |
|[<span data-ttu-id="a45b8-114">获取 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a45b8-114">Get oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-get.md) | [<span data-ttu-id="a45b8-115">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a45b8-115">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a45b8-116">读取**oAuth2PermissionGrant**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a45b8-116">Read the properties and relationships of an **oAuth2PermissionGrant** object.</span></span>|
|[<span data-ttu-id="a45b8-117">更新 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a45b8-117">Update oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-update.md) | [<span data-ttu-id="a45b8-118">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a45b8-118">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md) |<span data-ttu-id="a45b8-119">更新**oAuth2PermissionGrant**对象。</span><span class="sxs-lookup"><span data-stu-id="a45b8-119">Update an  **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="a45b8-120">删除 oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a45b8-120">Delete oAuth2PermissionGrant</span></span>](../api/oauth2permissiongrant-delete.md) | <span data-ttu-id="a45b8-121">无</span><span class="sxs-lookup"><span data-stu-id="a45b8-121">None</span></span> |<span data-ttu-id="a45b8-122">删除**oAuth2PermissionGrant**对象。</span><span class="sxs-lookup"><span data-stu-id="a45b8-122">Delete an **oAuth2PermissionGrant** object.</span></span> |
|[<span data-ttu-id="a45b8-123">获取增量</span><span class="sxs-lookup"><span data-stu-id="a45b8-123">Get delta</span></span>](../api/oauth2permissiongrant-delta.md)|[<span data-ttu-id="a45b8-124">oAuth2PermissionGrant</span><span class="sxs-lookup"><span data-stu-id="a45b8-124">oAuth2PermissionGrant</span></span>](oauth2permissiongrant.md)|<span data-ttu-id="a45b8-125">获取新创建、更新或删除的**oauth2permissiongrant**对象，而不执行整个资源集合的完全读取。</span><span class="sxs-lookup"><span data-stu-id="a45b8-125">Get newly created, updated, or deleted **oauth2permissiongrant** objects without performing a full read of the entire resource collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="a45b8-126">属性</span><span class="sxs-lookup"><span data-stu-id="a45b8-126">Properties</span></span>
| <span data-ttu-id="a45b8-127">属性</span><span class="sxs-lookup"><span data-stu-id="a45b8-127">Property</span></span>     | <span data-ttu-id="a45b8-128">类型</span><span class="sxs-lookup"><span data-stu-id="a45b8-128">Type</span></span>   |<span data-ttu-id="a45b8-129">说明</span><span class="sxs-lookup"><span data-stu-id="a45b8-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a45b8-130">clientId</span><span class="sxs-lookup"><span data-stu-id="a45b8-130">clientId</span></span>|<span data-ttu-id="a45b8-131">字符串</span><span class="sxs-lookup"><span data-stu-id="a45b8-131">String</span></span>| <span data-ttu-id="a45b8-132">在访问资源（由 resourceId 属性表示）时，授权模拟用户的服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="a45b8-132">The id of the service principal granted consent to impersonate the user when accessing the resource (represented by the resourceId property).</span></span> |
|<span data-ttu-id="a45b8-133">consentType</span><span class="sxs-lookup"><span data-stu-id="a45b8-133">consentType</span></span>|<span data-ttu-id="a45b8-134">String</span><span class="sxs-lookup"><span data-stu-id="a45b8-134">String</span></span>| <span data-ttu-id="a45b8-135">指示许可是由管理员（代表组织）提供，还是由个人授予。</span><span class="sxs-lookup"><span data-stu-id="a45b8-135">Indicates if consent was provided by the administrator (on behalf of the organization) or by an individual.</span></span> <span data-ttu-id="a45b8-136">可能的值为*AllPrincipals*或*Principal*。</span><span class="sxs-lookup"><span data-stu-id="a45b8-136">The possible values are *AllPrincipals* or *Principal*.</span></span> |
|<span data-ttu-id="a45b8-137">expiryTime</span><span class="sxs-lookup"><span data-stu-id="a45b8-137">expiryTime</span></span>|<span data-ttu-id="a45b8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a45b8-138">DateTimeOffset</span></span>| <span data-ttu-id="a45b8-139">目前，到期时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="a45b8-139">Currently, the expiry time value is ignored.</span></span> |
|<span data-ttu-id="a45b8-140">id</span><span class="sxs-lookup"><span data-stu-id="a45b8-140">id</span></span>|<span data-ttu-id="a45b8-141">String</span><span class="sxs-lookup"><span data-stu-id="a45b8-141">String</span></span>| <span data-ttu-id="a45b8-142">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a45b8-142">Unique identifier.</span></span> <span data-ttu-id="a45b8-143">只读。</span><span class="sxs-lookup"><span data-stu-id="a45b8-143">Read-only.</span></span>|
|<span data-ttu-id="a45b8-144">principalId</span><span class="sxs-lookup"><span data-stu-id="a45b8-144">principalId</span></span>|<span data-ttu-id="a45b8-145">String</span><span class="sxs-lookup"><span data-stu-id="a45b8-145">String</span></span>| <span data-ttu-id="a45b8-146">如果 consentType 为*AllPrincipals* ，则此值为 null，并且同意适用于组织中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="a45b8-146">If consentType is *AllPrincipals* this value is null, and the consent applies to all users in the organization.</span></span> <span data-ttu-id="a45b8-147">如果 consentType 为*Principal*，则此属性指定授予同意的用户的 id，并且仅适用于该用户。</span><span class="sxs-lookup"><span data-stu-id="a45b8-147">If consentType is *Principal*, then this property specifies the id of the user that granted consent and applies only for that user.</span></span> |
|<span data-ttu-id="a45b8-148">resourceId</span><span class="sxs-lookup"><span data-stu-id="a45b8-148">resourceId</span></span>|<span data-ttu-id="a45b8-149">String</span><span class="sxs-lookup"><span data-stu-id="a45b8-149">String</span></span>| <span data-ttu-id="a45b8-150">指定已向其授予访问权限的资源服务主体的 id。</span><span class="sxs-lookup"><span data-stu-id="a45b8-150">Specifies the id of the resource service principal to which access has been granted.</span></span> |
|<span data-ttu-id="a45b8-151">scope</span><span class="sxs-lookup"><span data-stu-id="a45b8-151">scope</span></span>|<span data-ttu-id="a45b8-152">String</span><span class="sxs-lookup"><span data-stu-id="a45b8-152">String</span></span>| <span data-ttu-id="a45b8-153">指定在 OAuth 2.0 访问令牌中，资源应用程序应预期的[范围](/graph/permissions-reference)声明的值。</span><span class="sxs-lookup"><span data-stu-id="a45b8-153">Specifies the value of the [scope](/graph/permissions-reference) claim that the resource application should expect in the OAuth 2.0 access token.</span></span> <span data-ttu-id="a45b8-154">例如， *User. Read*</span><span class="sxs-lookup"><span data-stu-id="a45b8-154">For example, *User.Read*</span></span> |
|<span data-ttu-id="a45b8-155">startTime</span><span class="sxs-lookup"><span data-stu-id="a45b8-155">startTime</span></span>|<span data-ttu-id="a45b8-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a45b8-156">DateTimeOffset</span></span>| <span data-ttu-id="a45b8-157">目前，开始时间值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="a45b8-157">Currently, the start time value is ignored.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a45b8-158">关系</span><span class="sxs-lookup"><span data-stu-id="a45b8-158">Relationships</span></span>
<span data-ttu-id="a45b8-159">无。</span><span class="sxs-lookup"><span data-stu-id="a45b8-159">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a45b8-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a45b8-160">JSON representation</span></span>

<span data-ttu-id="a45b8-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a45b8-161">The following is a JSON representation of the resource.</span></span>

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
  "expiryTime": "String (timestamp)",
  "id": "string (identifier)",
  "principalId": "string",
  "resourceId": "string",
  "scope": "string",
  "startTime": "String (timestamp)"
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
