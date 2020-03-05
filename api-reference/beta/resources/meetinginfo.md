---
title: meetingInfo 资源类型
description: 指定用于创建或加入会议的会议信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 1c6bda0463b2762122695ed84ecc02c1b5dd3d1b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522734"
---
# <a name="meetinginfo-resource-type"></a><span data-ttu-id="78527-103">meetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="78527-103">meetingInfo resource type</span></span>

<span data-ttu-id="78527-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="78527-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="78527-105">这是一个包含会议特定信息的抽象类。</span><span class="sxs-lookup"><span data-stu-id="78527-105">This is an abstract class that contains meeting specific information.</span></span>
 
<span data-ttu-id="78527-106">若要加入现有会议，必须将[organizerMeetingInfo](organizermeetinginfo.md)与[chatInfo](./chatinfo.md)或仅指定[tokenMeetingInfo](tokenmeetinginfo.md)一起指定。</span><span class="sxs-lookup"><span data-stu-id="78527-106">To join an existing meeting, you must either specify the [organizerMeetingInfo](organizermeetinginfo.md) in combination with the [chatInfo](./chatinfo.md), or just the the [tokenMeetingInfo](tokenmeetinginfo.md).</span></span>


## <a name="derived-types"></a><span data-ttu-id="78527-107">派生类型</span><span class="sxs-lookup"><span data-stu-id="78527-107">Derived types</span></span>

| <span data-ttu-id="78527-108">类型</span><span class="sxs-lookup"><span data-stu-id="78527-108">Type</span></span>                                                 | <span data-ttu-id="78527-109">说明</span><span class="sxs-lookup"><span data-stu-id="78527-109">Description</span></span>                                                         |
|:-----------------------------------------------------|:--------------------------------------------------------------------|
| [<span data-ttu-id="78527-110">organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="78527-110">organizerMeetingInfo</span></span>](./organizermeetinginfo.md)    | <span data-ttu-id="78527-111">有关会议组织者的详细信息</span><span class="sxs-lookup"><span data-stu-id="78527-111">Details about the organizer of the meeting</span></span>                          |
| [<span data-ttu-id="78527-112">tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="78527-112">tokenMeetingInfo</span></span>](tokenmeetinginfo.md)              | <span data-ttu-id="78527-113">包含有关会议的信息的加密令牌</span><span class="sxs-lookup"><span data-stu-id="78527-113">An encrypted token that contains the information about the meeting</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="78527-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78527-114">JSON representation</span></span>

<span data-ttu-id="78527-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78527-115">The following is a JSON representation of the resource.</span></span>

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
