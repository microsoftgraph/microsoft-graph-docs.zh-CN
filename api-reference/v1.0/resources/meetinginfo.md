---
title: meetingInfo 资源类型
description: 指定用于创建或加入会议的会议信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 8ef003db89ea676b4415a90c27913add49aad6e1
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913175"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="e45e5-103">meetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e45e5-103">meetingInfo resource type</span></span>

<span data-ttu-id="e45e5-104">这是一个包含会议特定信息的抽象类。</span><span class="sxs-lookup"><span data-stu-id="e45e5-104">This is an abstract class that contains meeting specific information.</span></span>
 
<span data-ttu-id="e45e5-105">若要加入现有会议，必须将[organizerMeetingInfo](organizermeetinginfo.md)与[chatInfo](./chatinfo.md)或仅指定[tokenMeetingInfo](tokenmeetinginfo.md)一起指定。</span><span class="sxs-lookup"><span data-stu-id="e45e5-105">To join an existing meeting, you must either specify the [organizerMeetingInfo](organizermeetinginfo.md) in combination with the [chatInfo](./chatinfo.md), or just the [tokenMeetingInfo](tokenmeetinginfo.md).</span></span>


## <a name="derived-types"></a><span data-ttu-id="e45e5-106">派生类型</span><span class="sxs-lookup"><span data-stu-id="e45e5-106">Derived types</span></span>

| <span data-ttu-id="e45e5-107">类型</span><span class="sxs-lookup"><span data-stu-id="e45e5-107">Type</span></span>                                                 | <span data-ttu-id="e45e5-108">说明</span><span class="sxs-lookup"><span data-stu-id="e45e5-108">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="e45e5-109">organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="e45e5-109">organizerMeetingInfo</span></span>](./organizermeetinginfo.md)    | <span data-ttu-id="e45e5-110">有关会议组织者的详细信息</span><span class="sxs-lookup"><span data-stu-id="e45e5-110">Details about the organizer of the meeting</span></span>                          |
| [<span data-ttu-id="e45e5-111">tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="e45e5-111">tokenMeetingInfo</span></span>](tokenmeetinginfo.md)              | <span data-ttu-id="e45e5-112">包含有关会议的信息的加密令牌</span><span class="sxs-lookup"><span data-stu-id="e45e5-112">An encrypted token that contains the information about the meeting</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="e45e5-113">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e45e5-113">JSON representation</span></span>

<span data-ttu-id="e45e5-114">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e45e5-114">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingInfo"
}-->
```json
{
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "meetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
