---
title: appRole 资源类型
description: 表示客户端应用程序调用另一个应用程序可能请求的应用程序角色，或可能用于将应用程序分配给指定应用程序角色中的用户或组的应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f61eca3971baeb426f4a20697a1e7ffca74e5071
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50132473"
---
# <a name="approle-resource-type"></a><span data-ttu-id="baafd-103">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="baafd-103">appRole resource type</span></span>

<span data-ttu-id="baafd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="baafd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="baafd-105">表示应用程序角色， (并授予) 客户端应用程序，或可用于将应用程序分配给指定角色中的用户或组的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="baafd-105">Represents an application role that can be requested by (and granted to) a client application, or that can be used to assign an application to users or groups in a specified role.</span></span> 

<span data-ttu-id="baafd-106">应用程序和 [servicePrincipal](serviceprincipal.md)实体的 **appRoles** 属性是 **appRole 的集合**。 [](application.md)</span><span class="sxs-lookup"><span data-stu-id="baafd-106">The **appRoles** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities are a collection of **appRole**.</span></span> 

<span data-ttu-id="baafd-107">使用 [appRoleAssignments，](approleassignment.md)可以将应用角色分配给用户、组或其他应用程序的服务主体。</span><span class="sxs-lookup"><span data-stu-id="baafd-107">With [appRoleAssignments](approleassignment.md), app roles can be assigned to users, groups, or other applications' service principals.</span></span>

## <a name="properties"></a><span data-ttu-id="baafd-108">属性</span><span class="sxs-lookup"><span data-stu-id="baafd-108">Properties</span></span>

| <span data-ttu-id="baafd-109">属性</span><span class="sxs-lookup"><span data-stu-id="baafd-109">Property</span></span>   | <span data-ttu-id="baafd-110">类型</span><span class="sxs-lookup"><span data-stu-id="baafd-110">Type</span></span> |<span data-ttu-id="baafd-111">说明</span><span class="sxs-lookup"><span data-stu-id="baafd-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="baafd-112">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="baafd-112">allowedMemberTypes</span></span>|<span data-ttu-id="baafd-113">String collection</span><span class="sxs-lookup"><span data-stu-id="baafd-113">String collection</span></span>|<span data-ttu-id="baafd-114">指定是否可以通过将此应用程序角色设置为 (来分配给用户和组) ，通过设置为 (或将两者设置为 (来分配给应用程序的 `["User"]` `["Application"]` `["User", "Application"]`) 。</span><span class="sxs-lookup"><span data-stu-id="baafd-114">Specifies whether this app role can be assigned to users and groups (by setting to `["User"]`), to other application's (by setting to `["Application"]`, or both (by setting to `["User", "Application"]`).</span></span> <span data-ttu-id="baafd-115">支持向其他应用程序的服务主体分配的应用程序角色也称为 [应用程序权限](/graph/auth/auth-concepts#microsoft-graph-permissions)。</span><span class="sxs-lookup"><span data-stu-id="baafd-115">App roles supporting assignment to other applications' service principals are also known as [application permissions](/graph/auth/auth-concepts#microsoft-graph-permissions).</span></span> <span data-ttu-id="baafd-116">"Application"值仅支持在应用程序实体上 **定义的应用** 角色。</span><span class="sxs-lookup"><span data-stu-id="baafd-116">The "Application" value is only supported for app roles defined on **application** entities.</span></span>|
|<span data-ttu-id="baafd-117">说明</span><span class="sxs-lookup"><span data-stu-id="baafd-117">description</span></span>|<span data-ttu-id="baafd-118">String</span><span class="sxs-lookup"><span data-stu-id="baafd-118">String</span></span>|<span data-ttu-id="baafd-119">应用角色的说明。</span><span class="sxs-lookup"><span data-stu-id="baafd-119">The description for the app role.</span></span> <span data-ttu-id="baafd-120">在分配应用角色时显示此状态，如果应用角色用作应用程序权限，将在同意体验期间显示。</span><span class="sxs-lookup"><span data-stu-id="baafd-120">This is displayed when the app role is being assigned and, if the app role functions as an application permission, during  consent experiences.</span></span>|
|<span data-ttu-id="baafd-121">displayName</span><span class="sxs-lookup"><span data-stu-id="baafd-121">displayName</span></span>|<span data-ttu-id="baafd-122">String</span><span class="sxs-lookup"><span data-stu-id="baafd-122">String</span></span>|<span data-ttu-id="baafd-123">应用和许可体验中显示的权限角色分配名称。</span><span class="sxs-lookup"><span data-stu-id="baafd-123">Display name for the permission that appears in the app role assignment and consent experiences.</span></span>|
|<span data-ttu-id="baafd-124">id</span><span class="sxs-lookup"><span data-stu-id="baafd-124">id</span></span>|<span data-ttu-id="baafd-125">Guid</span><span class="sxs-lookup"><span data-stu-id="baafd-125">Guid</span></span>|<span data-ttu-id="baafd-126">**appRoles 集合内的唯一角色** 标识符。</span><span class="sxs-lookup"><span data-stu-id="baafd-126">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="baafd-127">创建新的应用角色时，必须提供新的 Guid 标识符。</span><span class="sxs-lookup"><span data-stu-id="baafd-127">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="baafd-128">isEnabled</span><span class="sxs-lookup"><span data-stu-id="baafd-128">isEnabled</span></span>|<span data-ttu-id="baafd-129">Boolean</span><span class="sxs-lookup"><span data-stu-id="baafd-129">Boolean</span></span>|<span data-ttu-id="baafd-130">在创建或更新应用角色时，必须设置为 **true** (默认角色) 。</span><span class="sxs-lookup"><span data-stu-id="baafd-130">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="baafd-131">若要删除角色，必须先将其设置为 **false。**</span><span class="sxs-lookup"><span data-stu-id="baafd-131">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="baafd-132">此时，在后续调用中，可能会删除此角色。</span><span class="sxs-lookup"><span data-stu-id="baafd-132">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="baafd-133">origin</span><span class="sxs-lookup"><span data-stu-id="baafd-133">origin</span></span>|<span data-ttu-id="baafd-134">String</span><span class="sxs-lookup"><span data-stu-id="baafd-134">String</span></span>| <span data-ttu-id="baafd-135">指定应用程序角色是在 [应用程序](application.md) 对象上还是 [servicePrincipal 实体上](serviceprincipal.md) 定义。</span><span class="sxs-lookup"><span data-stu-id="baafd-135">Specifies if the app role is defined on the [application](application.md) object or on the [servicePrincipal](serviceprincipal.md) entity.</span></span> <span data-ttu-id="baafd-136">_不得包含在_ 任何 POST 或 PATCH 请求中。</span><span class="sxs-lookup"><span data-stu-id="baafd-136">Must _not_ be included in any POST or PATCH requests.</span></span> <span data-ttu-id="baafd-137">只读。</span><span class="sxs-lookup"><span data-stu-id="baafd-137">Read-only.</span></span> |
|<span data-ttu-id="baafd-138">value</span><span class="sxs-lookup"><span data-stu-id="baafd-138">value</span></span>|<span data-ttu-id="baafd-139">String</span><span class="sxs-lookup"><span data-stu-id="baafd-139">String</span></span>|<span data-ttu-id="baafd-140">指定要包括在 ID 令牌和访问令牌中的声明中的值，对分配的用户和服务主体 `roles` 进行身份验证。</span><span class="sxs-lookup"><span data-stu-id="baafd-140">Specifies the value to include in the `roles` claim in ID tokens and access tokens authenticating an assigned user or service principal.</span></span> <span data-ttu-id="baafd-141">长度不得超过 120 个字符。</span><span class="sxs-lookup"><span data-stu-id="baafd-141">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="baafd-142">允许的字符 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` 以及范围中的字符 `0-9` 和 `A-Z` `a-z` 。</span><span class="sxs-lookup"><span data-stu-id="baafd-142">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="baafd-143">不允许任何其他字符，包括空格字符。</span><span class="sxs-lookup"><span data-stu-id="baafd-143">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="baafd-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="baafd-144">JSON representation</span></span>

<span data-ttu-id="baafd-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="baafd-145">The following is a JSON representation of the resource.</span></span>

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

