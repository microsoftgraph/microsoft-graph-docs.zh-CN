---
title: appRole 资源类型
description: 表示应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: fe3753a0743a5cf1faac84b4fb102e1ffd702fed
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291011"
---
# <a name="approle-resource-type"></a><span data-ttu-id="cb7f5-103">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb7f5-103">appRole resource type</span></span>

<span data-ttu-id="cb7f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb7f5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cb7f5-105">表示可由客户端应用程序请求的应用程序角色，或可用于向指定角色中的用户或组分配应用程序的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="cb7f5-106">[Application](application.md)和[ServicePrincipal](serviceprincipal.md)实体的**appRoles**属性是**appRole**的集合。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-106">The **appRoles** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities are a collection of **appRole**.</span></span> 

<span data-ttu-id="cb7f5-107">使用[appRoleAssignments](approleassignment.md)，可以将应用程序角色分配给用户、组或其他应用程序的服务主体。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-107">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="cb7f5-108">属性</span><span class="sxs-lookup"><span data-stu-id="cb7f5-108">Properties</span></span>

| <span data-ttu-id="cb7f5-109">属性</span><span class="sxs-lookup"><span data-stu-id="cb7f5-109">Property</span></span>   | <span data-ttu-id="cb7f5-110">类型</span><span class="sxs-lookup"><span data-stu-id="cb7f5-110">Type</span></span> |<span data-ttu-id="cb7f5-111">说明</span><span class="sxs-lookup"><span data-stu-id="cb7f5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb7f5-112">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="cb7f5-112">allowedMemberTypes</span></span>|<span data-ttu-id="cb7f5-113">String collection</span><span class="sxs-lookup"><span data-stu-id="cb7f5-113">String collection</span></span>|<span data-ttu-id="cb7f5-114">指定是否可以将此应用程序角色分配给用户和组（通过设置为 `["User"]` ）到其他应用程序（通过设置为 `["Application"]` 或同时设置为两者）（通过设置为 `["User", "Application"]` ）。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-114">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="cb7f5-115">支持分配其他应用程序服务主体的应用程序角色也称为 "[应用程序权限](/graph/auth/auth-concepts#microsoft-graph-permissions)"。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-115">App roles supporting assignment of other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span>|
|<span data-ttu-id="cb7f5-116">说明</span><span class="sxs-lookup"><span data-stu-id="cb7f5-116">description</span></span>|<span data-ttu-id="cb7f5-117">String</span><span class="sxs-lookup"><span data-stu-id="cb7f5-117">String</span></span>|<span data-ttu-id="cb7f5-118">应用程序角色的说明。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-118">The description for the app role.</span></span> <span data-ttu-id="cb7f5-119">在授权体验期间，如果应用程序角色是作为应用程序的权限运行的，则会显示此情况。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-119">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="cb7f5-120">displayName</span><span class="sxs-lookup"><span data-stu-id="cb7f5-120">displayName</span></span>|<span data-ttu-id="cb7f5-121">字符串</span><span class="sxs-lookup"><span data-stu-id="cb7f5-121">String</span></span>|<span data-ttu-id="cb7f5-122">显示在应用程序角色分配和同意体验中的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-122">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="cb7f5-123">id</span><span class="sxs-lookup"><span data-stu-id="cb7f5-123">id</span></span>|<span data-ttu-id="cb7f5-124">Guid</span><span class="sxs-lookup"><span data-stu-id="cb7f5-124">Guid</span></span>|<span data-ttu-id="cb7f5-125">**AppRoles**集合中的唯一角色标识符。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-125">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="cb7f5-126">创建新的应用程序角色时，必须提供新的 Guid 标识符。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-126">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="cb7f5-127">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cb7f5-127">isEnabled</span></span>|<span data-ttu-id="cb7f5-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb7f5-128">Boolean</span></span>|<span data-ttu-id="cb7f5-129">在创建或更新应用程序角色时，必须将其设置为**true** （默认值为）。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-129">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="cb7f5-130">若要删除角色，必须首先将此设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-130">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="cb7f5-131">此时，在后续调用中，可能会删除此角色。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-131">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="cb7f5-132">格式</span><span class="sxs-lookup"><span data-stu-id="cb7f5-132">origin</span></span>|<span data-ttu-id="cb7f5-133">String</span><span class="sxs-lookup"><span data-stu-id="cb7f5-133">String</span></span>| <span data-ttu-id="cb7f5-134">指定是在[application](application.md)对象上还是在[servicePrincipal](serviceprincipal.md)实体上定义应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-134">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="cb7f5-135">不得_包含_在任何 POST 或 PATCH 请求中。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-135">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="cb7f5-136">只读。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-136">Read-only.</span></span> |
|<span data-ttu-id="cb7f5-137">value</span><span class="sxs-lookup"><span data-stu-id="cb7f5-137">value</span></span>|<span data-ttu-id="cb7f5-138">String</span><span class="sxs-lookup"><span data-stu-id="cb7f5-138">String</span></span>|<span data-ttu-id="cb7f5-139">指定要包含在 `roles` ID 令牌中的声明中的值，以及对分配的用户或服务主体进行身份验证的访问令牌。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-139">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="cb7f5-140">长度不得超过120个字符。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-140">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="cb7f5-141">允许的字符包括 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` ，以及范围中的字符 `0-9` `A-Z` 和 `a-z` 。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-141">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="cb7f5-142">不允许使用任何其他字符，包括空格字符。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-142">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="cb7f5-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb7f5-143">JSON representation</span></span>

<span data-ttu-id="cb7f5-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb7f5-144">The following is a JSON representation of the resource.</span></span>

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
