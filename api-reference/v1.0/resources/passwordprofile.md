---
title: passwordProfile 资源类型
description: 包含与用户关联的密码配置文件。用户 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。
ms.openlocfilehash: ee933b75b3dc536cbfcb33502cdda0d63680174c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010388"
---
# <a name="passwordprofile-resource-type"></a><span data-ttu-id="c3d06-104">passwordProfile 资源类型</span><span class="sxs-lookup"><span data-stu-id="c3d06-104">passwordProfile resource type</span></span>

<span data-ttu-id="c3d06-p102">包含与用户关联的密码配置文件。[用户](user.md) 实体的 **passwordProfile** 属性是一个 **passwordProfile** 对象。</span><span class="sxs-lookup"><span data-stu-id="c3d06-p102">Contains the password profile associated with a user. The **passwordProfile** property of the [user](user.md) entity is a **passwordProfile** object.</span></span>


## <a name="properties"></a><span data-ttu-id="c3d06-107">属性</span><span class="sxs-lookup"><span data-stu-id="c3d06-107">Properties</span></span>
| <span data-ttu-id="c3d06-108">属性</span><span class="sxs-lookup"><span data-stu-id="c3d06-108">Property</span></span>     | <span data-ttu-id="c3d06-109">类型</span><span class="sxs-lookup"><span data-stu-id="c3d06-109">Type</span></span>   |<span data-ttu-id="c3d06-110">说明</span><span class="sxs-lookup"><span data-stu-id="c3d06-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c3d06-111">forceChangePasswordNextSignIn</span><span class="sxs-lookup"><span data-stu-id="c3d06-111">forceChangePasswordNextSignIn</span></span>|<span data-ttu-id="c3d06-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c3d06-112">Boolean</span></span>| <span data-ttu-id="c3d06-113">如果用户在下次登录时必须更改密码，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="c3d06-113">**true** if the user must change her password on the next login; otherwise **false**.</span></span> |
|<span data-ttu-id="c3d06-114">密码</span><span class="sxs-lookup"><span data-stu-id="c3d06-114">password</span></span>|<span data-ttu-id="c3d06-115">String</span><span class="sxs-lookup"><span data-stu-id="c3d06-115">String</span></span>|<span data-ttu-id="c3d06-p103">用户的密码。创建用户时此属性是必需的。此属性可以更新，但用户在下次登录时必须更改密码。密码必须满足用户的 **passwordPolicies** 属性指定的最低要求。默认情况下，必须使用强密码。</span><span class="sxs-lookup"><span data-stu-id="c3d06-p103">The password for the user. This property is required when a user is created. It can be updated, but the user will be required to change the password on the next login. The password must satisfy minimum requirements as specified by the user’s **passwordPolicies** property. By default, a strong password is required.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c3d06-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c3d06-121">JSON representation</span></span>

<span data-ttu-id="c3d06-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3d06-122">Here is a JSON representation of the resource</span></span>

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