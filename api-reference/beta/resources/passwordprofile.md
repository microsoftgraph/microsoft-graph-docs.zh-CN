---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。用户实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: eketo-msft
ms.openlocfilehash: a597b17d09414a839cb0c8d0ae3c944c255ae8ec
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208321"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="3041b-104">passwordProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="3041b-104">passwordProfile resource type</span></span>

<span data-ttu-id="3041b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3041b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3041b-106">包含与用户关联的密码配置文件。</span><span class="sxs-lookup"><span data-stu-id="3041b-106">Contains the password profile associated with a user.</span></span> <span data-ttu-id="3041b-107">user 实体的 **passwordProfile** [属性是](user.md)**passwordProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="3041b-107">The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span> <span data-ttu-id="3041b-108">请参阅更新用户 [passwordProfile 的示例](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password)。</span><span class="sxs-lookup"><span data-stu-id="3041b-108">See an example to [Update the passwordProfile of a user](../api/user-update.md#example-3-update-the-passwordprofile-of-a-user-to-reset-their-password).</span></span>


## <a name="properties"></a><span data-ttu-id="3041b-109">属性</span><span class="sxs-lookup"><span data-stu-id="3041b-109">Properties</span></span>
| <span data-ttu-id="3041b-110">属性</span><span class="sxs-lookup"><span data-stu-id="3041b-110">Property</span></span>     | <span data-ttu-id="3041b-111">类型</span><span class="sxs-lookup"><span data-stu-id="3041b-111">Type</span></span>   |<span data-ttu-id="3041b-112">说明</span><span class="sxs-lookup"><span data-stu-id="3041b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3041b-113">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="3041b-113">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="3041b-114">Boolean</span><span class="sxs-lookup"><span data-stu-id="3041b-114">Boolean</span></span>|  <span data-ttu-id="3041b-115">如果用户在下次登录时必须更改密码，则为 `true`；否则为 `false`。</span><span class="sxs-lookup"><span data-stu-id="3041b-115">`true` if the user must change her password on the next login; otherwise `false`.</span></span> <span data-ttu-id="3041b-116">如未设置，默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="3041b-116">If not set, default is `false`.</span></span> <span data-ttu-id="3041b-117">**注意：** 对于 Azure B2C 租户，设置为`false`，并在首次登录时改为使用自定义策略和用户流强制重置密码。</span><span class="sxs-lookup"><span data-stu-id="3041b-117">**NOTE:**  For Azure B2C tenants, set to `false` and instead use custom policies and user flows to force password reset at first sign in.</span></span> <span data-ttu-id="3041b-118">请参阅[首次登录时强制密码重置](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon)。</span><span class="sxs-lookup"><span data-stu-id="3041b-118">See [Force password reset at first logon](https://github.com/azure-ad-b2c/samples/tree/master/policies/force-password-reset-first-logon).</span></span> |
|<span data-ttu-id="3041b-119">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="3041b-119">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="3041b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="3041b-120">Boolean</span></span>| <span data-ttu-id="3041b-121">如果为 `true`，则在下次登录时，用户必须先执行多重身份验证 (MFA)，然后才会被强制更改密码。</span><span class="sxs-lookup"><span data-stu-id="3041b-121">If `true`, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="3041b-122">该行为与 **forceChangePasswordNextSignIn** 相同，除了在更改密码之前用户必须先执行多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="3041b-122">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="3041b-123">密码更改后，此属性将自动重置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="3041b-123">After a password change, this property will be automatically reset to `false`.</span></span> <span data-ttu-id="3041b-124">如未设置，默认值为 `false`。</span><span class="sxs-lookup"><span data-stu-id="3041b-124">If not set, default is `false`.</span></span> |
|<span data-ttu-id="3041b-125">密码</span><span class="sxs-lookup"><span data-stu-id="3041b-125">password</span></span>|<span data-ttu-id="3041b-126">String</span><span class="sxs-lookup"><span data-stu-id="3041b-126">String</span></span>|<span data-ttu-id="3041b-p105">用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="3041b-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3041b-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3041b-132">JSON representation</span></span>

<span data-ttu-id="3041b-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3041b-133">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
  "forceChangePasswordNextSignInWithMfa": false,
  "password": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


