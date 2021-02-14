---
author: JeremyKelley
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
description: SharingInvitation 资源将邀请相关的数据项分组到一个结构中。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f90382fa2f65ed2c56afc53ef0a142913eb05579
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240078"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="77e2f-103">SharingInvitation 资源类型</span><span class="sxs-lookup"><span data-stu-id="77e2f-103">SharingInvitation resource type</span></span>

<span data-ttu-id="77e2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77e2f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="77e2f-105">**SharingInvitation** 资源将邀请相关的数据项分组到一个结构中。</span><span class="sxs-lookup"><span data-stu-id="77e2f-105">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="77e2f-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77e2f-106">JSON representation</span></span>

<span data-ttu-id="77e2f-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77e2f-107">Here is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="77e2f-108">属性</span><span class="sxs-lookup"><span data-stu-id="77e2f-108">Properties</span></span>

| <span data-ttu-id="77e2f-109">属性名</span><span class="sxs-lookup"><span data-stu-id="77e2f-109">Property Name</span></span>  | <span data-ttu-id="77e2f-110">类型</span><span class="sxs-lookup"><span data-stu-id="77e2f-110">Type</span></span>            | <span data-ttu-id="77e2f-111">说明</span><span class="sxs-lookup"><span data-stu-id="77e2f-111">Description</span></span>
|:---------------|:----------------|:------------------------------------------
| <span data-ttu-id="77e2f-112">email</span><span class="sxs-lookup"><span data-stu-id="77e2f-112">email</span></span>          | <span data-ttu-id="77e2f-113">String</span><span class="sxs-lookup"><span data-stu-id="77e2f-113">String</span></span>          | <span data-ttu-id="77e2f-p101">为共享邀请的收件人提供的电子邮件地址。只读。</span><span class="sxs-lookup"><span data-stu-id="77e2f-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>
| <span data-ttu-id="77e2f-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="77e2f-116">invitedBy</span></span>      | <span data-ttu-id="77e2f-117">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="77e2f-117">[identitySet][]</span></span> | <span data-ttu-id="77e2f-p102">提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="77e2f-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span>
| <span data-ttu-id="77e2f-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="77e2f-120">signInRequired</span></span> | <span data-ttu-id="77e2f-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="77e2f-121">Boolean</span></span>         | <span data-ttu-id="77e2f-p103">如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。</span><span class="sxs-lookup"><span data-stu-id="77e2f-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>

## <a name="remarks"></a><span data-ttu-id="77e2f-124">注解</span><span class="sxs-lookup"><span data-stu-id="77e2f-124">Remarks</span></span>

<span data-ttu-id="77e2f-125">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="77e2f-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

[DriveItem]: driveitem.md
[IdentitySet]: identityset.md

<!-- {
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "Facets/SharingInvitation"
} -->

