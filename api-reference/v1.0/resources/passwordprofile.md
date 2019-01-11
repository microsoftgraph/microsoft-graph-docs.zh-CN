---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。用户 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。
localization_priority: Priority
ms.openlocfilehash: 80d774906fb4897f57b943af827cfbc32e90511f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819661"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="a647b-104">passwordProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="a647b-104">passwordProfile resource type</span></span>

<span data-ttu-id="a647b-p102">包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="a647b-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="a647b-107">属性</span><span class="sxs-lookup"><span data-stu-id="a647b-107">Properties</span></span>
| <span data-ttu-id="a647b-108">属性</span><span class="sxs-lookup"><span data-stu-id="a647b-108">Property</span></span>     | <span data-ttu-id="a647b-109">类型</span><span class="sxs-lookup"><span data-stu-id="a647b-109">Type</span></span>   |<span data-ttu-id="a647b-110">说明</span><span class="sxs-lookup"><span data-stu-id="a647b-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a647b-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="a647b-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="a647b-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="a647b-112">Boolean</span></span>| <span data-ttu-id="a647b-113">如果用户在下次登录时必须更改密码，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="a647b-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="a647b-114">密码</span><span class="sxs-lookup"><span data-stu-id="a647b-114">password</span></span>|<span data-ttu-id="a647b-115">String</span><span class="sxs-lookup"><span data-stu-id="a647b-115">String</span></span>|<span data-ttu-id="a647b-p103">用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="a647b-p103">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a647b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a647b-121">JSON representation</span></span>

<span data-ttu-id="a647b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a647b-122">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordProfile"
}-->

```json
{
  "forceChangePasswordNextSignIn": true,
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
