---
title: permissionScope 资源类型
description: 表示委派权限（有时称为 OAuth 2.0 权限或 OAuth 2.0 作用域）的定义。 一旦定义，客户端应用程序可能会请求委派权限
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: psignoret
ms.openlocfilehash: ea3205139bffa11ff8fbe67d1ab6abb426bc65ca
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48406173"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="85f57-104">permissionScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="85f57-104">permissionScope resource type</span></span>

<span data-ttu-id="85f57-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85f57-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85f57-106">表示 [委派权限](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)的定义。</span><span class="sxs-lookup"><span data-stu-id="85f57-106">Represents the definition of a [delegated permission](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span>

<span data-ttu-id="85f57-107">需要对定义了权限的 API 拥有访问令牌的客户端应用程序可以请求委派权限。</span><span class="sxs-lookup"><span data-stu-id="85f57-107">Delegated permissions can be requested by client applications needing an access token to the API which defined the permissions.</span></span> <span data-ttu-id="85f57-108">可以[dynamically](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)使用 `scopes` 对 Microsoft identity 平台的授权请求中的参数（或[静态](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)）通过[application](application.md)对象上的**requiredResourceAccess**集合来动态请求委派权限。</span><span class="sxs-lookup"><span data-stu-id="85f57-108">Delegated permissions can be requested [dynamically](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), using the `scopes` parameter in an authorization request to the Microsoft identity platform, or [statically](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), through the **requiredResourceAccess** collection on the [application](application.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="85f57-109">属性</span><span class="sxs-lookup"><span data-stu-id="85f57-109">Properties</span></span>

| <span data-ttu-id="85f57-110">属性</span><span class="sxs-lookup"><span data-stu-id="85f57-110">Property</span></span> | <span data-ttu-id="85f57-111">类型</span><span class="sxs-lookup"><span data-stu-id="85f57-111">Type</span></span> | <span data-ttu-id="85f57-112">说明</span><span class="sxs-lookup"><span data-stu-id="85f57-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="85f57-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="85f57-113">adminConsentDescription</span></span>|<span data-ttu-id="85f57-114">字符串</span><span class="sxs-lookup"><span data-stu-id="85f57-114">String</span></span>|<span data-ttu-id="85f57-115">委派权限的说明，供管理员用来代表所有用户授予权限来阅读。</span><span class="sxs-lookup"><span data-stu-id="85f57-115">A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.</span></span> <span data-ttu-id="85f57-116">此文本显示在租户范围内的管理员同意体验中。</span><span class="sxs-lookup"><span data-stu-id="85f57-116">This text appears in tenant-wide admin consent experiences.</span></span>|
|<span data-ttu-id="85f57-117">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="85f57-117">adminConsentDisplayName</span></span>|<span data-ttu-id="85f57-118">字符串</span><span class="sxs-lookup"><span data-stu-id="85f57-118">String</span></span>|<span data-ttu-id="85f57-119">权限的标题，由管理员代表授予所有用户的权限来读取。</span><span class="sxs-lookup"><span data-stu-id="85f57-119">The permission's title, intended to be read by an administrator granting the permission on behalf of all users.</span></span>|
|<span data-ttu-id="85f57-120">id</span><span class="sxs-lookup"><span data-stu-id="85f57-120">id</span></span>|<span data-ttu-id="85f57-121">Guid</span><span class="sxs-lookup"><span data-stu-id="85f57-121">Guid</span></span>|<span data-ttu-id="85f57-122">为资源应用程序定义的委派权限集合中的唯一委派权限标识符。</span><span class="sxs-lookup"><span data-stu-id="85f57-122">Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.</span></span>|
|<span data-ttu-id="85f57-123">isEnabled</span><span class="sxs-lookup"><span data-stu-id="85f57-123">isEnabled</span></span>|<span data-ttu-id="85f57-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="85f57-124">Boolean</span></span>|<span data-ttu-id="85f57-125">在创建或更新权限时，此属性必须设置为 **true** (这是默认) 。</span><span class="sxs-lookup"><span data-stu-id="85f57-125">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="85f57-126">若要删除权限，必须首先将此属性设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="85f57-126">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="85f57-127">此时，在后续调用中，可能会删除该权限。</span><span class="sxs-lookup"><span data-stu-id="85f57-127">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="85f57-128">type</span><span class="sxs-lookup"><span data-stu-id="85f57-128">type</span></span>|<span data-ttu-id="85f57-129">字符串</span><span class="sxs-lookup"><span data-stu-id="85f57-129">String</span></span>|<span data-ttu-id="85f57-130">指定是否应将此委派权限视为非管理员用户同意代表自己同意，或者是否需要管理员同意权限才能。</span><span class="sxs-lookup"><span data-stu-id="85f57-130">Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions.</span></span> <span data-ttu-id="85f57-131">这将是默认行为，但每个客户可以通过允许、限制或限制用户同意此委派权限来选择自定义其组织中的行为 (。 ) </span><span class="sxs-lookup"><span data-stu-id="85f57-131">This will be the default behavior, but each customer can choose to customize the behavior in their organization (by allowing, restricting or limiting user consent to this delegated permission.)</span></span>|
|<span data-ttu-id="85f57-132">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="85f57-132">userConsentDescription</span></span>|<span data-ttu-id="85f57-133">字符串</span><span class="sxs-lookup"><span data-stu-id="85f57-133">String</span></span>|<span data-ttu-id="85f57-134">委派权限的说明，用于代表自己授予权限的用户阅读。</span><span class="sxs-lookup"><span data-stu-id="85f57-134">A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="85f57-135">此文本在同意体验中显示，其中用户仅代表自己。</span><span class="sxs-lookup"><span data-stu-id="85f57-135">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="85f57-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="85f57-136">userConsentDisplayName</span></span>|<span data-ttu-id="85f57-137">字符串</span><span class="sxs-lookup"><span data-stu-id="85f57-137">String</span></span>|<span data-ttu-id="85f57-138">权限的标题，旨在供代表自己授予权限的用户阅读。</span><span class="sxs-lookup"><span data-stu-id="85f57-138">A title for the permission, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="85f57-139">此文本在同意体验中显示，其中用户仅代表自己。</span><span class="sxs-lookup"><span data-stu-id="85f57-139">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="85f57-140">value</span><span class="sxs-lookup"><span data-stu-id="85f57-140">value</span></span>|<span data-ttu-id="85f57-141">String</span><span class="sxs-lookup"><span data-stu-id="85f57-141">String</span></span>|<span data-ttu-id="85f57-142">指定要包含在 `scp` access 令牌中) 声明的 (范围中的值。</span><span class="sxs-lookup"><span data-stu-id="85f57-142">Specifies the value to include in the `scp` (scope) claim in access tokens.</span></span> <span data-ttu-id="85f57-143">长度不得超过120个字符。</span><span class="sxs-lookup"><span data-stu-id="85f57-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="85f57-144">允许的字符包括 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` ，以及范围中的字符 `0-9` `A-Z` 和 `a-z` 。</span><span class="sxs-lookup"><span data-stu-id="85f57-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="85f57-145">不允许使用任何其他字符，包括空格字符。</span><span class="sxs-lookup"><span data-stu-id="85f57-145">Any other character, including the space character, are not allowed.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="85f57-146">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="85f57-146">JSON representation</span></span>

<span data-ttu-id="85f57-147">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="85f57-147">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.permissionScope"
}-->

```json
{
  "id": "guid",
  "adminConsentDisplayName": "string",
  "adminConsentDescription": "string",
  "userConsentDisplayName": "string",
  "userConsentDescription": "string",
  "value": "string",
  "type": "string",
  "isEnabled": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "oAuth2Permission resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->