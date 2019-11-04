---
title: appRole 资源类型
description: 表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色，或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。 ServicePrincipal 实体和 application 实体的**appRoles**属性是**appRole**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: febf5beb135e907680b8a038b9ca21c86abe9dfe
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939136"
---
# <a name="approle-resource-type"></a><span data-ttu-id="693b6-104">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="693b6-104">appRole resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="693b6-105">表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色，或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="693b6-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="693b6-106">[ServicePrincipal](serviceprincipal.md)实体和[Application](application.md)实体的**appRoles**属性是**appRole**的集合。</span><span class="sxs-lookup"><span data-stu-id="693b6-106">The **appRoles** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **appRole**.</span></span>

## <a name="properties"></a><span data-ttu-id="693b6-107">属性</span><span class="sxs-lookup"><span data-stu-id="693b6-107">Properties</span></span>
| <span data-ttu-id="693b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="693b6-108">Property</span></span>     | <span data-ttu-id="693b6-109">类型</span><span class="sxs-lookup"><span data-stu-id="693b6-109">Type</span></span>   |<span data-ttu-id="693b6-110">描述</span><span class="sxs-lookup"><span data-stu-id="693b6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="693b6-111">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="693b6-111">allowedMemberTypes</span></span>|<span data-ttu-id="693b6-112">String collection</span><span class="sxs-lookup"><span data-stu-id="693b6-112">String collection</span></span>|<span data-ttu-id="693b6-113">指定是否可以通过设置为 "用户" 或将此应用程序角色定义分配给用户和组，或通过设置为 "应用程序" 或同时设置为 "应用程序" 来将此应用程序角色定义分配给用户和组。</span><span class="sxs-lookup"><span data-stu-id="693b6-113">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="693b6-114">description</span><span class="sxs-lookup"><span data-stu-id="693b6-114">description</span></span>|<span data-ttu-id="693b6-115">字符串</span><span class="sxs-lookup"><span data-stu-id="693b6-115">String</span></span>|<span data-ttu-id="693b6-116">在管理员应用分配和同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="693b6-116">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="693b6-117">displayName</span><span class="sxs-lookup"><span data-stu-id="693b6-117">displayName</span></span>|<span data-ttu-id="693b6-118">字符串</span><span class="sxs-lookup"><span data-stu-id="693b6-118">String</span></span>|<span data-ttu-id="693b6-119">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="693b6-119">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="693b6-120">id</span><span class="sxs-lookup"><span data-stu-id="693b6-120">id</span></span>|<span data-ttu-id="693b6-121">Guid</span><span class="sxs-lookup"><span data-stu-id="693b6-121">Guid</span></span>|<span data-ttu-id="693b6-122">**AppRoles**集合中的唯一角色标识符。</span><span class="sxs-lookup"><span data-stu-id="693b6-122">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="693b6-123">创建新的应用程序角色时，必须提供新的 Guid 标识符。</span><span class="sxs-lookup"><span data-stu-id="693b6-123">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="693b6-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="693b6-124">isEnabled</span></span>|<span data-ttu-id="693b6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="693b6-125">Boolean</span></span>|<span data-ttu-id="693b6-126">在创建或更新应用程序角色时，必须将其设置为**true** （默认值为）。</span><span class="sxs-lookup"><span data-stu-id="693b6-126">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="693b6-127">若要删除角色，必须首先将此设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="693b6-127">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="693b6-128">此时，在后续调用中，可能会删除此角色。</span><span class="sxs-lookup"><span data-stu-id="693b6-128">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="693b6-129">格式</span><span class="sxs-lookup"><span data-stu-id="693b6-129">origin</span></span>|<span data-ttu-id="693b6-130">字符串</span><span class="sxs-lookup"><span data-stu-id="693b6-130">String</span></span>| <span data-ttu-id="693b6-131">只读。</span><span class="sxs-lookup"><span data-stu-id="693b6-131">Read-only.</span></span> <span data-ttu-id="693b6-132">指定是在 Application 对象上还是在 ServicePrincipal 对象上定义应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="693b6-132">Specifies if the app role is defined on the Application object or on the ServicePrincipal object.</span></span> <span data-ttu-id="693b6-133">不得_包含_在任何 POST 或 PATCH 请求中。</span><span class="sxs-lookup"><span data-stu-id="693b6-133">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="693b6-134">value</span><span class="sxs-lookup"><span data-stu-id="693b6-134">value</span></span>|<span data-ttu-id="693b6-135">String</span><span class="sxs-lookup"><span data-stu-id="693b6-135">String</span></span>|<span data-ttu-id="693b6-136">指定将包含在 authentication 和 access 令牌中`roles`的声明中的值。</span><span class="sxs-lookup"><span data-stu-id="693b6-136">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="693b6-137">长度不得超过120个字符。</span><span class="sxs-lookup"><span data-stu-id="693b6-137">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="693b6-138">允许的字符`:` `!` `#` `$` `%`为`&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `0-9`中`A-Z`的字符`a-z`和。 `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="693b6-138">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="693b6-139">不允许使用任何其他字符，包括空格字符。</span><span class="sxs-lookup"><span data-stu-id="693b6-139">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="693b6-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="693b6-140">JSON representation</span></span>

<span data-ttu-id="693b6-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="693b6-141">Here is a JSON representation of the resource</span></span>

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
