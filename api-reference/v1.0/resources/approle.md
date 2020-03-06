---
title: appRole 资源类型
description: 表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 2bda5d65d71873c1427ae99ded550962ad135433
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533143"
---
# <a name="approle-resource-type"></a><span data-ttu-id="91ead-103">appRole 资源类型</span><span class="sxs-lookup"><span data-stu-id="91ead-103">appRole resource type</span></span>

<span data-ttu-id="91ead-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91ead-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91ead-105">表示可能由调用其他应用程序的客户端应用程序请求的应用程序角色，或可用于向指定的应用程序角色中的用户或组分配应用程序的应用程序角色。</span><span class="sxs-lookup"><span data-stu-id="91ead-105">Represents an application role that may be requested by a client application calling another application or that may be used to assign an application to users or groups in a specified application role.</span></span> <span data-ttu-id="91ead-106">**AppRoles**属性</span><span class="sxs-lookup"><span data-stu-id="91ead-106">The **appRoles** property</span></span> <!-- of the [servicePrincipal](serviceprincipal.md) entity and --> <span data-ttu-id="91ead-107">[应用程序](application.md)实体是**appRole**的集合。</span><span class="sxs-lookup"><span data-stu-id="91ead-107">of the [application](application.md) entity is a collection of **appRole**.</span></span>

## <a name="properties"></a><span data-ttu-id="91ead-108">属性</span><span class="sxs-lookup"><span data-stu-id="91ead-108">Properties</span></span>
| <span data-ttu-id="91ead-109">属性</span><span class="sxs-lookup"><span data-stu-id="91ead-109">Property</span></span>     | <span data-ttu-id="91ead-110">类型</span><span class="sxs-lookup"><span data-stu-id="91ead-110">Type</span></span>   |<span data-ttu-id="91ead-111">说明</span><span class="sxs-lookup"><span data-stu-id="91ead-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91ead-112">allowedMemberTypes</span><span class="sxs-lookup"><span data-stu-id="91ead-112">allowedMemberTypes</span></span>|<span data-ttu-id="91ead-113">String collection</span><span class="sxs-lookup"><span data-stu-id="91ead-113">String collection</span></span>|<span data-ttu-id="91ead-114">指定是否可以通过设置为 "用户" 或将此应用程序角色定义分配给用户和组，或通过设置为 "应用程序" 或同时设置为 "应用程序" 来将此应用程序角色定义分配给用户和组。</span><span class="sxs-lookup"><span data-stu-id="91ead-114">Specifies whether this app role definition can be assigned to users and groups by setting to "User", or to other applications (that are accessing this application in daemon service scenarios) by setting to "Application", or to both.</span></span>|
|<span data-ttu-id="91ead-115">说明</span><span class="sxs-lookup"><span data-stu-id="91ead-115">description</span></span>|<span data-ttu-id="91ead-116">字符串</span><span class="sxs-lookup"><span data-stu-id="91ead-116">String</span></span>|<span data-ttu-id="91ead-117">在管理员应用分配和同意体验中显示的权限帮助文本。</span><span class="sxs-lookup"><span data-stu-id="91ead-117">Permission help text that appears in the admin app assignment and consent experiences.</span></span>|
|<span data-ttu-id="91ead-118">displayName</span><span class="sxs-lookup"><span data-stu-id="91ead-118">displayName</span></span>|<span data-ttu-id="91ead-119">字符串</span><span class="sxs-lookup"><span data-stu-id="91ead-119">String</span></span>|<span data-ttu-id="91ead-120">管理员同意和应用工作分配体验中显示的权限的显示名称。</span><span class="sxs-lookup"><span data-stu-id="91ead-120">Display name for the permission that appears in the admin consent and app assignment experiences.</span></span>|
|<span data-ttu-id="91ead-121">id</span><span class="sxs-lookup"><span data-stu-id="91ead-121">id</span></span>|<span data-ttu-id="91ead-122">Guid</span><span class="sxs-lookup"><span data-stu-id="91ead-122">Guid</span></span>|<span data-ttu-id="91ead-123">**AppRoles**集合中的唯一角色标识符。</span><span class="sxs-lookup"><span data-stu-id="91ead-123">Unique role identifier inside the **appRoles** collection.</span></span> <span data-ttu-id="91ead-124">创建新的应用程序角色时，必须提供新的 Guid 标识符。</span><span class="sxs-lookup"><span data-stu-id="91ead-124">When creating a new app role, a new Guid identifier must be provided.</span></span> |
|<span data-ttu-id="91ead-125">isEnabled</span><span class="sxs-lookup"><span data-stu-id="91ead-125">isEnabled</span></span>|<span data-ttu-id="91ead-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="91ead-126">Boolean</span></span>|<span data-ttu-id="91ead-127">在创建或更新应用程序角色时，必须将其设置为**true** （默认值为）。</span><span class="sxs-lookup"><span data-stu-id="91ead-127">When creating or updating an app role, this must be set to **true** (which is the default).</span></span> <span data-ttu-id="91ead-128">若要删除角色，必须首先将此设置为**false**。</span><span class="sxs-lookup"><span data-stu-id="91ead-128">To delete a role, this must first be set to **false**.</span></span>  <span data-ttu-id="91ead-129">此时，在后续调用中，可能会删除此角色。</span><span class="sxs-lookup"><span data-stu-id="91ead-129">At that point, in a subsequent call, this role may be removed.</span></span>|
|<span data-ttu-id="91ead-130">格式</span><span class="sxs-lookup"><span data-stu-id="91ead-130">origin</span></span>|<span data-ttu-id="91ead-131">字符串</span><span class="sxs-lookup"><span data-stu-id="91ead-131">String</span></span>| <span data-ttu-id="91ead-132">只读。</span><span class="sxs-lookup"><span data-stu-id="91ead-132">Read-only.</span></span> <span data-ttu-id="91ead-133">指定是否在 Application 对象上定义应用程序角色</span><span class="sxs-lookup"><span data-stu-id="91ead-133">Specifies if the app role is defined on the Application object</span></span> <!-- or on the ServicePrincipal object --><span data-ttu-id="91ead-134">.</span><span class="sxs-lookup"><span data-stu-id="91ead-134">.</span></span> <span data-ttu-id="91ead-135">不得_包含_在任何 POST 或 PATCH 请求中。</span><span class="sxs-lookup"><span data-stu-id="91ead-135">Must _not_ be included in any POST or PATCH requests.</span></span> |
|<span data-ttu-id="91ead-136">value</span><span class="sxs-lookup"><span data-stu-id="91ead-136">value</span></span>|<span data-ttu-id="91ead-137">String</span><span class="sxs-lookup"><span data-stu-id="91ead-137">String</span></span>|<span data-ttu-id="91ead-138">指定将包含在 authentication 和 access 令牌中`roles`的声明中的值。</span><span class="sxs-lookup"><span data-stu-id="91ead-138">Specifies the value which will be included in the `roles` claim in authentication and access tokens.</span></span> <span data-ttu-id="91ead-139">长度不得超过120个字符。</span><span class="sxs-lookup"><span data-stu-id="91ead-139">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="91ead-140">允许的字符`:` `!` `#` `$` `%`包括`&` `'` `(` `a-z`，以及`0-9`范围中`A-Z`的字符和。 `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`</span><span class="sxs-lookup"><span data-stu-id="91ead-140">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="91ead-141">不允许使用任何其他字符，包括空格字符。</span><span class="sxs-lookup"><span data-stu-id="91ead-141">Any other character, including the space character, are not allowed.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="91ead-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91ead-142">JSON representation</span></span>

<span data-ttu-id="91ead-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91ead-143">Here is a JSON representation of the resource</span></span>

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
