---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。用户实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。
localization_priority: Priority
ms.openlocfilehash: cea8dcc114cb599a2d857ced67ac25c9eb275497
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462499"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="37b42-104">passwordProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="37b42-104">passwordProfile resource type</span></span>

<span data-ttu-id="37b42-p102">包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="37b42-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="37b42-107">属性</span><span class="sxs-lookup"><span data-stu-id="37b42-107">Properties</span></span>
| <span data-ttu-id="37b42-108">属性</span><span class="sxs-lookup"><span data-stu-id="37b42-108">Property</span></span>     | <span data-ttu-id="37b42-109">类型</span><span class="sxs-lookup"><span data-stu-id="37b42-109">Type</span></span>   |<span data-ttu-id="37b42-110">说明</span><span class="sxs-lookup"><span data-stu-id="37b42-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="37b42-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="37b42-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="37b42-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="37b42-112">Boolean</span></span>| <span data-ttu-id="37b42-113">如果用户在下次登录时必须更改密码，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="37b42-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="37b42-114">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="37b42-114">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="37b42-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="37b42-115">Boolean</span></span>| <span data-ttu-id="37b42-116">如果为 **true**，则在下次登录时，用户必须先执行多重身份验证 (MFA)，然后才会被强制更改密码。</span><span class="sxs-lookup"><span data-stu-id="37b42-116">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="37b42-117">该行为与 **forceChangePasswordNextSignIn** 相同，除了在更改密码之前用户必须先执行多重身份验证。</span><span class="sxs-lookup"><span data-stu-id="37b42-117">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="37b42-118">密码更改后，此属性将自动重置为 **false**。</span><span class="sxs-lookup"><span data-stu-id="37b42-118">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="37b42-119">如未设置，默认值为 **false**。</span><span class="sxs-lookup"><span data-stu-id="37b42-119">If not set, default is **false**.</span></span> |
|<span data-ttu-id="37b42-120">密码</span><span class="sxs-lookup"><span data-stu-id="37b42-120">password</span></span>|<span data-ttu-id="37b42-121">String</span><span class="sxs-lookup"><span data-stu-id="37b42-121">String</span></span>|<span data-ttu-id="37b42-p104">用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="37b42-p104">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="37b42-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37b42-127">JSON representation</span></span>

<span data-ttu-id="37b42-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37b42-128">Here is a JSON representation of the resource</span></span>

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
