---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 0cb09136f4093b290f37ee851cb7d2d0ca10c1bf
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2019
ms.locfileid: "30480542"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="fd8c7-102">SharingInvitation 资源类型</span><span class="sxs-lookup"><span data-stu-id="fd8c7-102">SharingInvitation resource type</span></span>

<span data-ttu-id="fd8c7-103">**SharingInvitation**资源将与邀请相关的数据项分组到一个单一结构中。</span><span class="sxs-lookup"><span data-stu-id="fd8c7-103">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="fd8c7-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fd8c7-104">JSON representation</span></span>

<span data-ttu-id="fd8c7-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd8c7-105">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="fd8c7-106">属性</span><span class="sxs-lookup"><span data-stu-id="fd8c7-106">Properties</span></span>

| <span data-ttu-id="fd8c7-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="fd8c7-107">Property Name</span></span>  | <span data-ttu-id="fd8c7-108">类型</span><span class="sxs-lookup"><span data-stu-id="fd8c7-108">Type</span></span>            | <span data-ttu-id="fd8c7-109">说明</span><span class="sxs-lookup"><span data-stu-id="fd8c7-109">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="fd8c7-110">email</span><span class="sxs-lookup"><span data-stu-id="fd8c7-110">email</span></span>          | <span data-ttu-id="fd8c7-111">String</span><span class="sxs-lookup"><span data-stu-id="fd8c7-111">String</span></span>          | <span data-ttu-id="fd8c7-p101">为共享邀请的收件人提供的电子邮件地址。只读。</span><span class="sxs-lookup"><span data-stu-id="fd8c7-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="fd8c7-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="fd8c7-114">invitedBy</span></span>      | <span data-ttu-id="fd8c7-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="fd8c7-115">[identitySet][]</span></span> | <span data-ttu-id="fd8c7-p102">提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="fd8c7-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="fd8c7-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="fd8c7-118">signInRequired</span></span> | <span data-ttu-id="fd8c7-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="fd8c7-119">Boolean</span></span>         | <span data-ttu-id="fd8c7-p103">如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。</span><span class="sxs-lookup"><span data-stu-id="fd8c7-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="fd8c7-122">注解</span><span class="sxs-lookup"><span data-stu-id="fd8c7-122">Remarks</span></span>

<span data-ttu-id="fd8c7-123">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="fd8c7-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->
