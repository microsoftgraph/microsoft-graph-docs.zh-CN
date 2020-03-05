---
author: JeremyKelley
description: SharingInvitation 资源将与邀请相关的数据项分组到一个单一结构中。
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 6bbe39603ed4daad9c354b1c14ed6a68b3638c6d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520651"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="f414a-103">SharingInvitation 资源类型</span><span class="sxs-lookup"><span data-stu-id="f414a-103">SharingInvitation resource type</span></span>

<span data-ttu-id="f414a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f414a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f414a-105">**SharingInvitation**资源将与邀请相关的数据项分组到一个单一结构中。</span><span class="sxs-lookup"><span data-stu-id="f414a-105">The **SharingInvitation** resource groups invitation-related data items into a single structure.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f414a-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f414a-106">JSON representation</span></span>

<span data-ttu-id="f414a-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f414a-107">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="f414a-108">属性</span><span class="sxs-lookup"><span data-stu-id="f414a-108">Properties</span></span>

| <span data-ttu-id="f414a-109">属性名</span><span class="sxs-lookup"><span data-stu-id="f414a-109">Property Name</span></span>  | <span data-ttu-id="f414a-110">类型</span><span class="sxs-lookup"><span data-stu-id="f414a-110">Type</span></span>                          | <span data-ttu-id="f414a-111">说明</span><span class="sxs-lookup"><span data-stu-id="f414a-111">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f414a-112">email</span><span class="sxs-lookup"><span data-stu-id="f414a-112">email</span></span>          | <span data-ttu-id="f414a-113">String</span><span class="sxs-lookup"><span data-stu-id="f414a-113">String</span></span>                        | <span data-ttu-id="f414a-p101">为共享邀请的收件人提供的电子邮件地址。只读。</span><span class="sxs-lookup"><span data-stu-id="f414a-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="f414a-116">invitedBy</span><span class="sxs-lookup"><span data-stu-id="f414a-116">invitedBy</span></span>      | [<span data-ttu-id="f414a-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="f414a-117">identitySet</span></span>](identityset.md) | <span data-ttu-id="f414a-p102">提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="f414a-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="f414a-120">signInRequired</span><span class="sxs-lookup"><span data-stu-id="f414a-120">signInRequired</span></span> | <span data-ttu-id="f414a-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="f414a-121">Boolean</span></span>                       | <span data-ttu-id="f414a-p103">如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。</span><span class="sxs-lookup"><span data-stu-id="f414a-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="f414a-124">注解</span><span class="sxs-lookup"><span data-stu-id="f414a-124">Remarks</span></span> 

<span data-ttu-id="f414a-125">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="f414a-125">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


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
