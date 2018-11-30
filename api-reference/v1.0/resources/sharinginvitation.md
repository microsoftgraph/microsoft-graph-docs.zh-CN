---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
ms.openlocfilehash: 187a7bd8fe51be57b663c215436272ee711512e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009507"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="3681b-102">SharingInvitation 资源类型</span><span class="sxs-lookup"><span data-stu-id="3681b-102">SharingInvitation resource type</span></span>

<span data-ttu-id="3681b-103">**SharingInvitation**资源组合到单个结构邀请相关的数据项。</span><span class="sxs-lookup"><span data-stu-id="3681b-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3681b-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3681b-104">JSON representation</span></span>

<span data-ttu-id="3681b-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3681b-105">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sharingInvitation"
}-->

```json
{
  "email": "string",
  "invitedBy": {"@odata.type": "microsoft.graph.identitySet" },
  "signInRequired": true
}
```

## <a name="properties"></a><span data-ttu-id="3681b-106">属性</span><span class="sxs-lookup"><span data-stu-id="3681b-106">Properties</span></span>

| <span data-ttu-id="3681b-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="3681b-107">Property Name</span></span>  | <span data-ttu-id="3681b-108">类型</span><span class="sxs-lookup"><span data-stu-id="3681b-108">Type</span></span>            | <span data-ttu-id="3681b-109">说明</span><span class="sxs-lookup"><span data-stu-id="3681b-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="3681b-110">email</span><span class="sxs-lookup"><span data-stu-id="3681b-110">email</span></span>          | <span data-ttu-id="3681b-111">String</span><span class="sxs-lookup"><span data-stu-id="3681b-111">String</span></span>          | <span data-ttu-id="3681b-p101">为共享邀请的收件人提供的电子邮件地址。只读。</span><span class="sxs-lookup"><span data-stu-id="3681b-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="3681b-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="3681b-114">invitedBy</span></span>      | <span data-ttu-id="3681b-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="3681b-115">[identitySet][]</span></span> | <span data-ttu-id="3681b-p102">提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="3681b-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="3681b-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="3681b-118">signInRequired</span></span> | <span data-ttu-id="3681b-119">布尔</span><span class="sxs-lookup"><span data-stu-id="3681b-119">Boolean</span></span>         | <span data-ttu-id="3681b-p103">如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。</span><span class="sxs-lookup"><span data-stu-id="3681b-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="3681b-122">注解</span><span class="sxs-lookup"><span data-stu-id="3681b-122">Remarks</span></span>

<span data-ttu-id="3681b-123">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="3681b-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
