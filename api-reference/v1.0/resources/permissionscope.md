---
title: permissionScope 资源类型
description: 表示委派权限的定义，有时称为 OAuth 2.0 权限或 OAuth 2.0 范围。 定义后，客户端应用程序可能会请求委派权限
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: psignoret
ms.openlocfilehash: f98e91da1ff46ef944b2de49add36f174673fad8
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638891"
---
# <a name="permissionscope-resource-type"></a><span data-ttu-id="1fe65-104">permissionScope 资源类型</span><span class="sxs-lookup"><span data-stu-id="1fe65-104">permissionScope resource type</span></span>

<span data-ttu-id="1fe65-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fe65-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1fe65-106">表示委派权限 [的定义](/azure/active-directory/develop/v2-permissions-and-consent#permission-types)。</span><span class="sxs-lookup"><span data-stu-id="1fe65-106">Represents the definition of a [delegated permission](/azure/active-directory/develop/v2-permissions-and-consent#permission-types).</span></span>

<span data-ttu-id="1fe65-107">委派权限可以通过需要访问令牌的客户端应用程序请求，该 API 定义了权限。</span><span class="sxs-lookup"><span data-stu-id="1fe65-107">Delegated permissions can be requested by client applications needing an access token to the API which defined the permissions.</span></span> <span data-ttu-id="1fe65-108">可通过 [](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent)应用程序对象的 `scopes` **requiredResourceAccess**[](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope)集合动态请求委派权限，使用 Microsoft 标识平台的授权请求中的 参数，或静态 [](application.md)请求。</span><span class="sxs-lookup"><span data-stu-id="1fe65-108">Delegated permissions can be requested [dynamically](/azure/active-directory/develop/v2-permissions-and-consent#requesting-individual-user-consent), using the `scopes` parameter in an authorization request to the Microsoft identity platform, or [statically](/azure/active-directory/develop/v2-permissions-and-consent#the-default-scope), through the **requiredResourceAccess** collection on the [application](application.md) object.</span></span>

## <a name="properties"></a><span data-ttu-id="1fe65-109">属性</span><span class="sxs-lookup"><span data-stu-id="1fe65-109">Properties</span></span>

| <span data-ttu-id="1fe65-110">属性</span><span class="sxs-lookup"><span data-stu-id="1fe65-110">Property</span></span> | <span data-ttu-id="1fe65-111">类型</span><span class="sxs-lookup"><span data-stu-id="1fe65-111">Type</span></span> | <span data-ttu-id="1fe65-112">说明</span><span class="sxs-lookup"><span data-stu-id="1fe65-112">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="1fe65-113">adminConsentDescription</span><span class="sxs-lookup"><span data-stu-id="1fe65-113">adminConsentDescription</span></span>|<span data-ttu-id="1fe65-114">String</span><span class="sxs-lookup"><span data-stu-id="1fe65-114">String</span></span>|<span data-ttu-id="1fe65-115">委派权限的说明，供代表所有用户授予权限的管理员读取。</span><span class="sxs-lookup"><span data-stu-id="1fe65-115">A description of the delegated permissions, intended to be read by an administrator granting the permission on behalf of all users.</span></span> <span data-ttu-id="1fe65-116">此文本显示在租户范围的管理员同意体验中。</span><span class="sxs-lookup"><span data-stu-id="1fe65-116">This text appears in tenant-wide admin consent experiences.</span></span>|
|<span data-ttu-id="1fe65-117">adminConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="1fe65-117">adminConsentDisplayName</span></span>|<span data-ttu-id="1fe65-118">String</span><span class="sxs-lookup"><span data-stu-id="1fe65-118">String</span></span>|<span data-ttu-id="1fe65-119">权限的标题，供代表所有用户授予权限的管理员读取。</span><span class="sxs-lookup"><span data-stu-id="1fe65-119">The permission's title, intended to be read by an administrator granting the permission on behalf of all users.</span></span>|
|<span data-ttu-id="1fe65-120">id</span><span class="sxs-lookup"><span data-stu-id="1fe65-120">id</span></span>|<span data-ttu-id="1fe65-121">Guid</span><span class="sxs-lookup"><span data-stu-id="1fe65-121">Guid</span></span>|<span data-ttu-id="1fe65-122">为资源应用程序定义的委派权限集合中的唯一委派权限标识符。</span><span class="sxs-lookup"><span data-stu-id="1fe65-122">Unique delegated permission identifier inside the collection of delegated permissions defined for a resource application.</span></span>|
|<span data-ttu-id="1fe65-123">isEnabled</span><span class="sxs-lookup"><span data-stu-id="1fe65-123">isEnabled</span></span>|<span data-ttu-id="1fe65-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="1fe65-124">Boolean</span></span>|<span data-ttu-id="1fe65-125">创建或更新权限时，必须将此属性设置为 **true** (这是默认) 。</span><span class="sxs-lookup"><span data-stu-id="1fe65-125">When creating or updating a permission, this property must be set to **true** (which is the default).</span></span> <span data-ttu-id="1fe65-126">若要删除权限，必须先将此属性设置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="1fe65-126">To delete a permission, this property must first be set to **false**.</span></span>  <span data-ttu-id="1fe65-127">此时，在后续调用中，可能会删除权限。</span><span class="sxs-lookup"><span data-stu-id="1fe65-127">At that point, in a subsequent call, the permission may be removed.</span></span>|
|<span data-ttu-id="1fe65-128">type</span><span class="sxs-lookup"><span data-stu-id="1fe65-128">type</span></span>|<span data-ttu-id="1fe65-129">String</span><span class="sxs-lookup"><span data-stu-id="1fe65-129">String</span></span>|<span data-ttu-id="1fe65-130">指定非管理员用户代表自己同意此委派权限是否安全，或者是否需要管理员同意这些权限。</span><span class="sxs-lookup"><span data-stu-id="1fe65-130">Specifies whether this delegated permission should be considered safe for non-admin users to consent to on behalf of themselves, or whether an administrator should be required for consent to the permissions.</span></span> <span data-ttu-id="1fe65-131">这是默认行为，但每个客户都可以选择自定义其组织中的行为 (允许、限制或限制用户对此委派权限的同意。) </span><span class="sxs-lookup"><span data-stu-id="1fe65-131">This will be the default behavior, but each customer can choose to customize the behavior in their organization (by allowing, restricting or limiting user consent to this delegated permission.)</span></span>|
|<span data-ttu-id="1fe65-132">userConsentDescription</span><span class="sxs-lookup"><span data-stu-id="1fe65-132">userConsentDescription</span></span>|<span data-ttu-id="1fe65-133">String</span><span class="sxs-lookup"><span data-stu-id="1fe65-133">String</span></span>|<span data-ttu-id="1fe65-134">委派权限的说明，供代表自己授予权限的用户阅读。</span><span class="sxs-lookup"><span data-stu-id="1fe65-134">A description of the delegated permissions, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="1fe65-135">此文本显示在用户仅代表自己同意的同意体验中。</span><span class="sxs-lookup"><span data-stu-id="1fe65-135">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="1fe65-136">userConsentDisplayName</span><span class="sxs-lookup"><span data-stu-id="1fe65-136">userConsentDisplayName</span></span>|<span data-ttu-id="1fe65-137">String</span><span class="sxs-lookup"><span data-stu-id="1fe65-137">String</span></span>|<span data-ttu-id="1fe65-138">权限的标题，供代表自己授予权限的用户读取。</span><span class="sxs-lookup"><span data-stu-id="1fe65-138">A title for the permission, intended to be read by a user granting the permission on their own behalf.</span></span> <span data-ttu-id="1fe65-139">此文本显示在用户仅代表自己同意的同意体验中。</span><span class="sxs-lookup"><span data-stu-id="1fe65-139">This text appears in consent experiences where the user is consenting only on behalf of themselves.</span></span>|
|<span data-ttu-id="1fe65-140">value</span><span class="sxs-lookup"><span data-stu-id="1fe65-140">value</span></span>|<span data-ttu-id="1fe65-141">String</span><span class="sxs-lookup"><span data-stu-id="1fe65-141">String</span></span>|<span data-ttu-id="1fe65-142">指定要包括在访问令牌中声明 (`scp` 作用域) 的值。</span><span class="sxs-lookup"><span data-stu-id="1fe65-142">Specifies the value to include in the `scp` (scope) claim in access tokens.</span></span> <span data-ttu-id="1fe65-143">长度不得超过 120 个字符。</span><span class="sxs-lookup"><span data-stu-id="1fe65-143">Must not exceed 120 characters in length.</span></span> <span data-ttu-id="1fe65-144">允许的字符 `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~` 包括 、 和 范围 `0-9` `A-Z` 中的字符 `a-z` 。</span><span class="sxs-lookup"><span data-stu-id="1fe65-144">Allowed characters are `:` `!` `#` `$` `%` `&` `'` `(` `)` `*` `+` `,` `-` `.` `/` `:` `;` <code>&lt;</code> `=` <code>&gt;</code> `?` `@` `[` `]` `^` `+` `_` <code>&#96;</code> `{` <code>&#124;</code> `}` `~`, as well as characters in the ranges `0-9`, `A-Z` and `a-z`.</span></span> <span data-ttu-id="1fe65-145">不允许任何其他字符，包括空格字符。</span><span class="sxs-lookup"><span data-stu-id="1fe65-145">Any other character, including the space character, are not allowed.</span></span> <span data-ttu-id="1fe65-146">不得以 开头 `.` 。</span><span class="sxs-lookup"><span data-stu-id="1fe65-146">May not begin with `.`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fe65-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1fe65-147">JSON representation</span></span>

<span data-ttu-id="1fe65-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1fe65-148">Here is a JSON representation of the resource</span></span>

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
