---
title: organizerMeetingInfo 资源类型
description: '包含有关会议组织者的详细信息。 '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 3f011870422abb255c895b389a959554cd44ddfa
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913511"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="902c0-103">organizerMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="902c0-103">organizerMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="902c0-104">包含有关会议组织者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="902c0-104">Contains details about the meeting organizer.</span></span> 

<span data-ttu-id="902c0-105">若要加入现有会议，必须提供 organizerMeetingInfo 和[chatInfo](./chatinfo.md)资源类型或[tokenMeetingInfo](./tokenmeetinginfo.md)资源类型的组合。</span><span class="sxs-lookup"><span data-stu-id="902c0-105">To join an existing meeting, you must either provide a combination of the organizerMeetingInfo and the [chatInfo](./chatinfo.md) resource types, or the [tokenMeetingInfo](./tokenmeetinginfo.md) resource type by itself.</span></span>

## <a name="properties"></a><span data-ttu-id="902c0-106">属性</span><span class="sxs-lookup"><span data-stu-id="902c0-106">Properties</span></span>

| <span data-ttu-id="902c0-107">属性</span><span class="sxs-lookup"><span data-stu-id="902c0-107">Property</span></span>                     | <span data-ttu-id="902c0-108">类型</span><span class="sxs-lookup"><span data-stu-id="902c0-108">Type</span></span>                          | <span data-ttu-id="902c0-109">说明</span><span class="sxs-lookup"><span data-stu-id="902c0-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="902c0-110">organizer － 组织者</span><span class="sxs-lookup"><span data-stu-id="902c0-110">organizer</span></span>                    | [<span data-ttu-id="902c0-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="902c0-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="902c0-112">组织者 Azure Active Directory 标识。</span><span class="sxs-lookup"><span data-stu-id="902c0-112">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="902c0-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="902c0-113">JSON representation</span></span>

<span data-ttu-id="902c0-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="902c0-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
