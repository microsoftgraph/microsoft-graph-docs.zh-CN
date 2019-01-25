---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: SharingInvitation
localization_priority: Normal
ms.openlocfilehash: 009dcf77492d8ec77230413dc628076ef0d557fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523391"
---
# <a name="sharinginvitation-resource-type"></a><span data-ttu-id="079fc-102">SharingInvitation 资源类型</span><span class="sxs-lookup"><span data-stu-id="079fc-102">SharingInvitation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="079fc-103">**SharingInvitation** 资源将与邀请相关的数据项分组到一个单一结构。</span><span class="sxs-lookup"><span data-stu-id="079fc-103">The **SharingInvitation** resource groups invitation-related data items into a single strucutre.</span></span>

## <a name="json-representation"></a><span data-ttu-id="079fc-104">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="079fc-104">JSON representation</span></span>

<span data-ttu-id="079fc-105">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="079fc-105">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="079fc-106">属性</span><span class="sxs-lookup"><span data-stu-id="079fc-106">Properties</span></span>

| <span data-ttu-id="079fc-107">属性名称</span><span class="sxs-lookup"><span data-stu-id="079fc-107">Property Name</span></span>  | <span data-ttu-id="079fc-108">类型</span><span class="sxs-lookup"><span data-stu-id="079fc-108">Type</span></span>                          | <span data-ttu-id="079fc-109">说明</span><span class="sxs-lookup"><span data-stu-id="079fc-109">Description</span></span>                                                                                                                   |
|:---------------|:------------------------------|:------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="079fc-110">email</span><span class="sxs-lookup"><span data-stu-id="079fc-110">email</span></span>          | <span data-ttu-id="079fc-111">String</span><span class="sxs-lookup"><span data-stu-id="079fc-111">String</span></span>                        | <span data-ttu-id="079fc-p101">为共享邀请的收件人提供的电子邮件地址。只读。</span><span class="sxs-lookup"><span data-stu-id="079fc-p101">The email address provided for the recipient of the sharing invitation. Read-only.</span></span>                                          |
| <span data-ttu-id="079fc-114">invitedBy</span><span class="sxs-lookup"><span data-stu-id="079fc-114">invitedBy</span></span>      | [<span data-ttu-id="079fc-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="079fc-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="079fc-p102">提供创建了此权限的邀请发送者的相关信息（如果信息可用）。只读。</span><span class="sxs-lookup"><span data-stu-id="079fc-p102">Provides information about who sent the invitation that created this permission, if that information is available. Read-only.</span></span> |
| <span data-ttu-id="079fc-118">signInRequired</span><span class="sxs-lookup"><span data-stu-id="079fc-118">signInRequired</span></span> | <span data-ttu-id="079fc-119">布尔</span><span class="sxs-lookup"><span data-stu-id="079fc-119">Boolean</span></span>                       | <span data-ttu-id="079fc-p103">如果 `true`，邀请接收者需要登录才能访问共享的项目。只读。</span><span class="sxs-lookup"><span data-stu-id="079fc-p103">If `true` the recipient of the invitation needs to sign in in order to access the shared item. Read-only.</span></span>                     |

## <a name="remarks"></a><span data-ttu-id="079fc-122">注解</span><span class="sxs-lookup"><span data-stu-id="079fc-122">Remarks</span></span> 

<span data-ttu-id="079fc-123">有关 DriveItem 上 facet 的详细信息，请参阅 [DriveItem](driveitem.md)。</span><span class="sxs-lookup"><span data-stu-id="079fc-123">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The sharing invitation facet describes details of a sharing invitation associated with a permission.",
  "keywords": "image,width,height,item,facet",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/sharinginvitation.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
