---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。用户 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。
ms.openlocfilehash: 71a91f0848ba8218d16a59c9e1f867d14e5cad9b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049325"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="37545-104">passwordProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="37545-104">passwordProfile resource type</span></span>

> <span data-ttu-id="37545-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="37545-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="37545-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="37545-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="37545-p103">包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="37545-p103">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="37545-109">属性</span><span class="sxs-lookup"><span data-stu-id="37545-109">Properties</span></span>
| <span data-ttu-id="37545-110">属性</span><span class="sxs-lookup"><span data-stu-id="37545-110">Property</span></span>     | <span data-ttu-id="37545-111">类型</span><span class="sxs-lookup"><span data-stu-id="37545-111">Type</span></span>   |<span data-ttu-id="37545-112">说明</span><span class="sxs-lookup"><span data-stu-id="37545-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37545-113">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="37545-113">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="37545-114">布尔</span><span class="sxs-lookup"><span data-stu-id="37545-114">Boolean</span></span>| <span data-ttu-id="37545-115">如果**true**，在下一步登录，用户必须更改其密码。</span><span class="sxs-lookup"><span data-stu-id="37545-115">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="37545-116">密码更改之后，此属性将自动重置为 \***false**。</span><span class="sxs-lookup"><span data-stu-id="37545-116">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="37545-117">如果不设置，默认值为**false**。</span><span class="sxs-lookup"><span data-stu-id="37545-117">If not set, default is **false**.</span></span> |
|<span data-ttu-id="37545-118">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="37545-118">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="37545-119">布尔</span><span class="sxs-lookup"><span data-stu-id="37545-119">Boolean</span></span>| <span data-ttu-id="37545-120">如果**true**，在下一步登录，用户必须执行在之前的多因素身份验证 (MFA) 强制更改其密码。</span><span class="sxs-lookup"><span data-stu-id="37545-120">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="37545-121">行为等同于**forceChangePasswordNextSignIn**之处在于密码更改之前先执行多因素身份验证所需的用户。</span><span class="sxs-lookup"><span data-stu-id="37545-121">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="37545-122">密码更改之后，此属性将自动重置为**false**。</span><span class="sxs-lookup"><span data-stu-id="37545-122">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="37545-123">如果不设置，默认值为**false**。</span><span class="sxs-lookup"><span data-stu-id="37545-123">If not set, default is **false**.</span></span> |
|<span data-ttu-id="37545-124">password</span><span class="sxs-lookup"><span data-stu-id="37545-124">password</span></span>|<span data-ttu-id="37545-125">String</span><span class="sxs-lookup"><span data-stu-id="37545-125">String</span></span>|<span data-ttu-id="37545-p106">用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="37545-p106">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37545-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37545-131">JSON representation</span></span>

<span data-ttu-id="37545-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37545-132">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordprofile"
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
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->