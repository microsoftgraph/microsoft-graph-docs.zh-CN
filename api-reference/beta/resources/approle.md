---
title: appRole 资源类型
description: 表示应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: psignoret
ms.openlocfilehash: 06a5f97048be74388b49a79c8661b49043ddf727
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638837"
---
# <a name="approle-resource-type"></a><span data-ttu-id="182fc-103">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="182fc-103">appRole resource type</span></span>

<span data-ttu-id="182fc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="182fc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="182fc-105">表示应用程序角色， (请求并授予) 客户端应用程序，或可用于将应用程序分配给指定角色中的用户或组。</span><span class="sxs-lookup"><span data-stu-id="182fc-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="182fc-106">若要添加、更新或删除应用程序的应用程序角色，请 [更新](../api/application-update.md) 应用程序或服务的应用程序。</span><span class="sxs-lookup"><span data-stu-id="182fc-106">To add, update, or remove app roles for an application, [update the application](../api/application-update.md) for the app or service.</span></span> <span data-ttu-id="182fc-107">应用程序实体上的应用程序角色将在使用应用程序的所有租户中可用。</span><span class="sxs-lookup"><span data-stu-id="182fc-107">App roles on the application entity will be available in all tenants where the application is used.</span></span> <span data-ttu-id="182fc-108">若要定义仅适用于租户 (例如，代表多租户应用程序) 实例中的自定义角色的应用角色，还可以更新应用的服务主体，以向 **appRoles** 集合添加或更新应用 [](../api/serviceprincipal-update.md)角色。</span><span class="sxs-lookup"><span data-stu-id="182fc-108">To define app roles that are only applicable in your tenant (for example, app roles representing custom roles in your instance of a multi-tenant application), you can also [update the service principal](../api/serviceprincipal-update.md) for the app, to add or update app roles to the **appRoles** collection.</span></span>

<span data-ttu-id="182fc-109">使用 [appRoleAssignments，](approleassignment.md)可以将应用角色分配给用户、组或其他应用程序的服务主体。</span><span class="sxs-lookup"><span data-stu-id="182fc-109">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="182fc-110">属性</span><span class="sxs-lookup"><span data-stu-id="182fc-110">Properties</span></span>

| <span data-ttu-id="182fc-111">属性</span><span class="sxs-lookup"><span data-stu-id="182fc-111">Property</span></span>   | <span data-ttu-id="182fc-112">类型</span><span class="sxs-lookup"><span data-stu-id="182fc-112">Type</span></span> |<span data-ttu-id="182fc-113">说明</span><span class="sxs-lookup"><span data-stu-id="182fc-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="182fc-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="182fc-114">allowedMemberTypes</span></span>|<span data-ttu-id="182fc-115">String 集合</span><span class="sxs-lookup"><span data-stu-id="182fc-115">String collection</span></span>|<span data-ttu-id="182fc-116">通过设置为) ，指定此应用角色是否可分配给用户和组 (，或者通过设置为) 将此应用程序角色设置为 或同时将两 (分配给应用程序的 `["User"]` `["Application"]` `["User", "Application"]` (。</span><span class="sxs-lookup"><span data-stu-id="182fc-116">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="182fc-117">支持向其他应用程序的服务主体分配的应用程序角色也称为应用程序 [权限](/graph/auth/auth-concepts#microsoft-graph-permissions)。</span><span class="sxs-lookup"><span data-stu-id="182fc-117">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="182fc-118">"Application"值仅受应用程序实体上定义的 **应用角色** 支持。</span><span class="sxs-lookup"><span data-stu-id="182fc-118">The "Application" value is only supported for app roles defined on **application** entities.</span></span> |
|<span data-ttu-id="182fc-119">说明</span><span class="sxs-lookup"><span data-stu-id="182fc-119">description</span></span>|<span data-ttu-id="182fc-120">String</span><span class="sxs-lookup"><span data-stu-id="182fc-120">String</span></span>|<span data-ttu-id="182fc-121">应用角色的说明。</span><span class="sxs-lookup"><span data-stu-id="182fc-121">The description for the app role.</span></span> <span data-ttu-id="182fc-122">在分配应用角色时显示，如果应用角色在同意体验期间用作应用程序权限，则显示此状态。</span><span class="sxs-lookup"><span data-stu-id="182fc-122">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="182fc-123">displayName</span><span class="sxs-lookup"><span data-stu-id="182fc-123">displayName</span></span>|<span data-ttu-id="182fc-124">String</span><span class="sxs-lookup"><span data-stu-id="182fc-124">String</span></span>|<span data-ttu-id="182fc-125">应用和许可体验中显示的权限角色分配名称。</span><span class="sxs-lookup"><span data-stu-id="182fc-125">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="182fc-126">id</span><span class="sxs-lookup"><span data-stu-id="182fc-126">id</span></span>|<span data-ttu-id="182fc-127">Guid</span><span class="sxs-lookup"><span data-stu-id="182fc-127">Guid</span></span>|<span data-ttu-id="182fc-128">**appRoles 集合内的唯一角色** 标识符。</span><span class="sxs-lookup"><span data-stu-id="182fc-128">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="182fc-129">创建新的应用角色时，必须提供新的 Guid 标识符。</span><span class="sxs-lookup"><span data-stu-id="182fc-129">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="182fc-130">isEnabled</span><span class="sxs-lookup"><span data-stu-id="182fc-130">isEnabled</span></span>|<span data-ttu-id="182fc-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="182fc-131">Boolean</span></span>|<span data-ttu-id="182fc-132">在创建或更新应用角色时，必须设置为 **true** (这是默认角色) 。</span><span class="sxs-lookup"><span data-stu-id="182fc-132">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="182fc-133">若要删除角色，必须先将其设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="182fc-133">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="182fc-134">此时，在后续调用中，可能会删除此角色。</span><span class="sxs-lookup"><span data-stu-id="182fc-134">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="182fc-135">origin</span><span class="sxs-lookup"><span data-stu-id="182fc-135">origin</span></span>|<span data-ttu-id="182fc-136">String</span><span class="sxs-lookup"><span data-stu-id="182fc-136">String</span></span>| <span data-ttu-id="182fc-137">指定应用程序角色是在 [application](application.md) 对象上还是 [servicePrincipal](serviceprincipal.md) 实体上定义。</span><span class="sxs-lookup"><span data-stu-id="182fc-137">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="182fc-138">_不得_ 包含在任何 POST 或 PATCH 请求中。</span><span class="sxs-lookup"><span data-stu-id="182fc-138">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="182fc-139">只读。</span><span class="sxs-lookup"><span data-stu-id="182fc-139">Read-only.</span></span> |
|<span data-ttu-id="182fc-140">value</span><span class="sxs-lookup"><span data-stu-id="182fc-140">value</span></span>|<span data-ttu-id="182fc-141">String</span><span class="sxs-lookup"><span data-stu-id="182fc-141">String</span></span>|<span data-ttu-id="182fc-142">指定要包括在 ID 令牌和访问令牌中的声明中的值，对分配的用户和服务主体 `roles` 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="182fc-142">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="182fc-143">长度不得超过 120 个字符。</span><span class="sxs-lookup"><span data-stu-id="182fc-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="182fc-144">允许的字符 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` 包括 、 和 范围 `0-9` `A-Z` 中的字符 `a-z` 。</span><span class="sxs-lookup"><span data-stu-id="182fc-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="182fc-145">不允许任何其他字符，包括空格字符。</span><span class="sxs-lookup"><span data-stu-id="182fc-145">Any other character, including the space character, are not allowed.</span></span> <span data-ttu-id="182fc-146">不得以 开头 `.` 。</span><span class="sxs-lookup"><span data-stu-id="182fc-146">May not begin with `.`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="182fc-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="182fc-147">JSON representation</span></span>

<span data-ttu-id="182fc-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="182fc-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.appRole"
}-->

```json
{
  "allowedMemberTypes": ["string"],
  "description": "string",
  "displayName": "string",
  "id": "guid",
  "isEnabled": true,
  "origin": "string",
  "value": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "appRole resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


