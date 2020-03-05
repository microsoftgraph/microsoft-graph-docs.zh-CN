---
title: organizerMeetingInfo 资源类型
description: '包含有关会议组织者的详细信息。 '
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 89f487b5edcf1b176a67d10b0ae45d8dd62c46d3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447260"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="9875a-103">organizerMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="9875a-103">organizerMeetingInfo resource type</span></span>

<span data-ttu-id="9875a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9875a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9875a-105">包含有关会议组织者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9875a-105">Contains details about the meeting organizer.</span></span> 

<span data-ttu-id="9875a-106">若要加入现有会议，必须提供 organizerMeetingInfo 和[chatInfo](./chatinfo.md)资源类型或[tokenMeetingInfo](./tokenmeetinginfo.md)资源类型的组合。</span><span class="sxs-lookup"><span data-stu-id="9875a-106">To join an existing meeting, you must either provide a combination of the organizerMeetingInfo and the [chatInfo](./chatinfo.md) resource types, or the [tokenMeetingInfo](./tokenmeetinginfo.md) resource type by itself.</span></span>

## <a name="properties"></a><span data-ttu-id="9875a-107">属性</span><span class="sxs-lookup"><span data-stu-id="9875a-107">Properties</span></span>

| <span data-ttu-id="9875a-108">属性</span><span class="sxs-lookup"><span data-stu-id="9875a-108">Property</span></span>                     | <span data-ttu-id="9875a-109">类型</span><span class="sxs-lookup"><span data-stu-id="9875a-109">Type</span></span>                          | <span data-ttu-id="9875a-110">说明</span><span class="sxs-lookup"><span data-stu-id="9875a-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="9875a-111">组织者</span><span class="sxs-lookup"><span data-stu-id="9875a-111">organizer</span></span>                    | [<span data-ttu-id="9875a-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="9875a-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="9875a-113">组织者 Azure Active Directory 标识。</span><span class="sxs-lookup"><span data-stu-id="9875a-113">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="9875a-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9875a-114">JSON representation</span></span>

<span data-ttu-id="9875a-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9875a-115">The following is a JSON representation of the resource.</span></span>

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
