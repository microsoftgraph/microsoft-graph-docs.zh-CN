---
author: JeremyKelley
description: SharingInvitation 资源将与邀请相关的数据项分组到一个单一结构中。
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: eebfa17a08918ec3ac08700577921b1037761086
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008332"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="ee07b-103">SharingInvitation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ee07b-103">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ee07b-104">**SharingInvitation**资源将与邀请相关的数据项分组到一个单一结构中。</span><span class="sxs-lookup"><span data-stu-id="ee07b-104">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ee07b-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ee07b-105">JSON representation</span></span>

<span data-ttu-id="ee07b-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ee07b-106">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="ee07b-107">属性</span><span class="sxs-lookup"><span data-stu-id="ee07b-107">Properties</span></span>

| <span data-ttu-id="ee07b-108">属性名称</span><span class="sxs-lookup"><span data-stu-id="ee07b-108">Property Name</span></span>  | <span data-ttu-id="ee07b-109">类型</span><span class="sxs-lookup"><span data-stu-id="ee07b-109">Type</span></span>                          | <span data-ttu-id="ee07b-110">说明</span><span class="sxs-lookup"><span data-stu-id="ee07b-110">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="ee07b-111">email</span><span class="sxs-lookup"><span data-stu-id="ee07b-111">email</span></span>          | <span data-ttu-id="ee07b-112">String</span><span class="sxs-lookup"><span data-stu-id="ee07b-112">String</span></span>                        | <span data-ttu-id="ee07b-p101">为共享邀请的收件人提供的电子邮件地址。只读。</span><span class="sxs-lookup"><span data-stu-id="ee07b-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="ee07b-115">invitedBy</span><span class="sxs-lookup"><span data-stu-id="ee07b-115">invitedBy</span></span>      | [<span data-ttu-id="ee07b-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="ee07b-116">identitySet</span></span>](identityset.md) | <span data-ttu-id="ee07b-p102">提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="ee07b-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="ee07b-119">signInRequired</span><span class="sxs-lookup"><span data-stu-id="ee07b-119">signInRequired</span></span> | <span data-ttu-id="ee07b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="ee07b-120">Boolean</span></span>                       | <span data-ttu-id="ee07b-p103">如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。</span><span class="sxs-lookup"><span data-stu-id="ee07b-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="ee07b-123">注解</span><span class="sxs-lookup"><span data-stu-id="ee07b-123">Remarks</span></span> 

<span data-ttu-id="ee07b-124">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="ee07b-124">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
