---
title: appRole 资源类型
description: 表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色, 或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。 ServicePrincipal 实体和 application 实体的**appRoles**属性是**appRole**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 35c26e52c5d7eb9529474d08a43b68fceddfc954
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013316"
---
# <a name="approle-resource-type"></a><span data-ttu-id="f193d-104">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="f193d-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f193d-105">表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色, 或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="f193d-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="f193d-106">[ServicePrincipal](serviceprincipal.md)实体和[Application](application.md)实体的**appRoles**属性是**appRole**的集合。</span><span class="sxs-lookup"><span data-stu-id="f193d-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

> <span data-ttu-id="f193d-107">重要说明: 当前版本中禁用了此功能。</span><span class="sxs-lookup"><span data-stu-id="f193d-107">Important: This functionality is disabled in the current release.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f193d-108">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f193d-108">JSON representation</span></span>

<span data-ttu-id="f193d-109">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f193d-109">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f193d-110">属性</span><span class="sxs-lookup"><span data-stu-id="f193d-110">Properties</span></span>
| <span data-ttu-id="f193d-111">属性</span><span class="sxs-lookup"><span data-stu-id="f193d-111">Property</span></span>     | <span data-ttu-id="f193d-112">类型</span><span class="sxs-lookup"><span data-stu-id="f193d-112">Type</span></span>   |<span data-ttu-id="f193d-113">说明</span><span class="sxs-lookup"><span data-stu-id="f193d-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f193d-114">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="f193d-114">allowedMemberTypes</span></span>|<span data-ttu-id="f193d-115">String collection</span><span class="sxs-lookup"><span data-stu-id="f193d-115">String collection</span></span>|<span data-ttu-id="f193d-116">指定是否可以通过设置为 "用户" 或将此应用程序角色定义分配给用户和组, 或通过设置为 "应用程序" 或同时设置为 "应用程序" 来将此应用程序角色定义分配给用户和组。</span><span class="sxs-lookup"><span data-stu-id="f193d-116">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="f193d-117">说明</span><span class="sxs-lookup"><span data-stu-id="f193d-117">description</span></span>|<span data-ttu-id="f193d-118">String</span><span class="sxs-lookup"><span data-stu-id="f193d-118">String</span></span>|<span data-ttu-id="f193d-119">在管理员应用分配和同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="f193d-119">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="f193d-120">displayName</span><span class="sxs-lookup"><span data-stu-id="f193d-120">displayName</span></span>|<span data-ttu-id="f193d-121">字符串</span><span class="sxs-lookup"><span data-stu-id="f193d-121">String</span></span>|<span data-ttu-id="f193d-122">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f193d-122">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="f193d-123">id</span><span class="sxs-lookup"><span data-stu-id="f193d-123">id</span></span>|<span data-ttu-id="f193d-124">Guid</span><span class="sxs-lookup"><span data-stu-id="f193d-124">Guid</span></span>|<span data-ttu-id="f193d-125">**AppRoles**集合中的唯一角色标识符。</span><span class="sxs-lookup"><span data-stu-id="f193d-125">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="f193d-126">创建新的应用程序角色时, 必须提供新的 Guid 标识符。</span><span class="sxs-lookup"><span data-stu-id="f193d-126">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="f193d-127">isEnabled</span><span class="sxs-lookup"><span data-stu-id="f193d-127">isEnabled</span></span>|<span data-ttu-id="f193d-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="f193d-128">Boolean</span></span>|<span data-ttu-id="f193d-129">在创建或更新应用程序角色时, 必须将其设置为**true** (默认值为)。</span><span class="sxs-lookup"><span data-stu-id="f193d-129">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="f193d-130">若要删除角色, 必须首先将此设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="f193d-130">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="f193d-131">此时, 在后续调用中, 可能会删除此角色。</span><span class="sxs-lookup"><span data-stu-id="f193d-131">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="f193d-132">格式</span><span class="sxs-lookup"><span data-stu-id="f193d-132">origin</span></span>|<span data-ttu-id="f193d-133">String</span><span class="sxs-lookup"><span data-stu-id="f193d-133">String</span></span>| <span data-ttu-id="f193d-134">只读。</span><span class="sxs-lookup"><span data-stu-id="f193d-134">Read-only.</span></span> <span data-ttu-id="f193d-135">指定是在 Application 对象上还是在 ServicePrincipal 对象上定义应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="f193d-135">Specifies if the app role is defined on the Application object or on the ServicePrincipal object.</span></span> <span data-ttu-id="f193d-136">不得__ 包含在任何 POST 或 PATCH 请求中。</span><span class="sxs-lookup"><span data-stu-id="f193d-136">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="f193d-137">value</span><span class="sxs-lookup"><span data-stu-id="f193d-137">value</span></span>|<span data-ttu-id="f193d-138">String</span><span class="sxs-lookup"><span data-stu-id="f193d-138">String</span></span>|<span data-ttu-id="f193d-139">指定将包含在 authentication 和 access 令牌中`roles`的声明中的值。</span><span class="sxs-lookup"><span data-stu-id="f193d-139">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="f193d-140">长度不得超过120个字符。</span><span class="sxs-lookup"><span data-stu-id="f193d-140">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="f193d-141">允许的字符`:` `!` `#` `$` `%`为`&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `0-9`中`A-Z`的字符`a-z`和。 `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="f193d-141">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="f193d-142">不允许使用任何其他字符, 包括空格字符。</span><span class="sxs-lookup"><span data-stu-id="f193d-142">Any other character, including the space character, are not allowed.</span></span>  |


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
