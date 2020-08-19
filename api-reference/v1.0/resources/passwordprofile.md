---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。用户实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。
localization_priority: Priority
author: eketo-msft
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c776cb21923231cab2701bf3679a2df70a59a928
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808135"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="65c34-104">passwordProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="65c34-104">passwordProfile resource type</span></span>

<span data-ttu-id="65c34-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65c34-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="65c34-p102">包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="65c34-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="65c34-108">属性</span><span class="sxs-lookup"><span data-stu-id="65c34-108">Properties</span></span>
| <span data-ttu-id="65c34-109">属性</span><span class="sxs-lookup"><span data-stu-id="65c34-109">Property</span></span>     | <span data-ttu-id="65c34-110">类型</span><span class="sxs-lookup"><span data-stu-id="65c34-110">Type</span></span>   |<span data-ttu-id="65c34-111">说明</span><span class="sxs-lookup"><span data-stu-id="65c34-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65c34-112">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="65c34-112">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="65c34-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c34-113">Boolean</span></span>| <span data-ttu-id="65c34-114">如果用户在下次登录时必须更改密码，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="65c34-114">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="65c34-115">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="65c34-115">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="65c34-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c34-116">Boolean</span></span>| <span data-ttu-id="65c34-117">如果为 **true**，则在下次登录时，用户必须先执行多重身份验证 (MFA)，然后才会被强制更改密码。</span><span class="sxs-lookup"><span data-stu-id="65c34-117">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="65c34-118">该行为与 **forceChangePasswordNextSignIn** 相同，除了在更改密码之前用户必须先执行多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="65c34-118">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="65c34-119">密码更改后，此属性将自动重置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="65c34-119">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="65c34-120">如未设置，默认值为 **false**。</span><span class="sxs-lookup"><span data-stu-id="65c34-120">If not set, default is **false**.</span></span> |
|<span data-ttu-id="65c34-121">密码</span><span class="sxs-lookup"><span data-stu-id="65c34-121">password</span></span>|<span data-ttu-id="65c34-122">String</span><span class="sxs-lookup"><span data-stu-id="65c34-122">String</span></span>|<span data-ttu-id="65c34-p104">用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="65c34-p104">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="65c34-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65c34-128">JSON representation</span></span>

<span data-ttu-id="65c34-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65c34-129">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
