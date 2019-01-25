---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。**用户** 实体的 **passwordProfile** 属性是一个 passwordProfile 对象。
localization_priority: Normal
ms.openlocfilehash: 3caff59c8fd0838b91f9fdfb79bdbb154aa83b9f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518931"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="6cab8-104">passwordProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="6cab8-104">passwordProfile resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cab8-p102">包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="6cab8-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="6cab8-107">属性</span><span class="sxs-lookup"><span data-stu-id="6cab8-107">Properties</span></span>
| <span data-ttu-id="6cab8-108">属性</span><span class="sxs-lookup"><span data-stu-id="6cab8-108">Property</span></span>     | <span data-ttu-id="6cab8-109">类型</span><span class="sxs-lookup"><span data-stu-id="6cab8-109">Type</span></span>   |<span data-ttu-id="6cab8-110">说明</span><span class="sxs-lookup"><span data-stu-id="6cab8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cab8-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="6cab8-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="6cab8-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cab8-112">Boolean</span></span>| <span data-ttu-id="6cab8-113">如果**true**，在下一步登录，用户必须更改其密码。</span><span class="sxs-lookup"><span data-stu-id="6cab8-113">If **true**, at next sign-in, the user must change their password.</span></span> <span data-ttu-id="6cab8-114">密码更改之后，此属性将自动重置为 \***false**。</span><span class="sxs-lookup"><span data-stu-id="6cab8-114">After a password change, this property will be automatically reset to \***false**.</span></span> <span data-ttu-id="6cab8-115">如果不设置，默认值为**false**。</span><span class="sxs-lookup"><span data-stu-id="6cab8-115">If not set, default is **false**.</span></span> |
|<span data-ttu-id="6cab8-116">forceChangePasswordNextSignInWithMfa</span><span class="sxs-lookup"><span data-stu-id="6cab8-116">forceChangePasswordNextSignInWithMfa</span></span>|<span data-ttu-id="6cab8-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="6cab8-117">Boolean</span></span>| <span data-ttu-id="6cab8-118">如果**true**，在下一步登录，用户必须执行在之前的多因素身份验证 (MFA) 强制更改其密码。</span><span class="sxs-lookup"><span data-stu-id="6cab8-118">If **true**, at next sign-in, the user must perform a multi-factor authentication (MFA) before being forced to change their password.</span></span> <span data-ttu-id="6cab8-119">行为等同于**forceChangePasswordNextSignIn**之处在于密码更改之前先执行多因素身份验证所需的用户。</span><span class="sxs-lookup"><span data-stu-id="6cab8-119">The behavior is identical to **forceChangePasswordNextSignIn** except that the user is required to first perform a multi-factor authentication before password change.</span></span> <span data-ttu-id="6cab8-120">密码更改之后，此属性将自动重置为**false**。</span><span class="sxs-lookup"><span data-stu-id="6cab8-120">After a password change, this property will be automatically reset to **false**.</span></span> <span data-ttu-id="6cab8-121">如果不设置，默认值为**false**。</span><span class="sxs-lookup"><span data-stu-id="6cab8-121">If not set, default is **false**.</span></span> |
|<span data-ttu-id="6cab8-122">password</span><span class="sxs-lookup"><span data-stu-id="6cab8-122">password</span></span>|<span data-ttu-id="6cab8-123">String</span><span class="sxs-lookup"><span data-stu-id="6cab8-123">String</span></span>|<span data-ttu-id="6cab8-p105">用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="6cab8-p105">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cab8-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6cab8-129">JSON representation</span></span>

<span data-ttu-id="6cab8-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6cab8-130">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "passwordProfile resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordprofile.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
