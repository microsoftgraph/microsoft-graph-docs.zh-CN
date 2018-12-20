---
title: meetingParticipantInfo 资源类型
description: 有关会议中的参与者的信息。
author: VinodRavichandran
ms.openlocfilehash: 2bbb410ea26640ec05d66b5beb0c4b4ea24a42bd
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380196"
---
# <a name="meetingparticipantinfo-resource-type"></a><span data-ttu-id="00d24-103">meetingParticipantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="00d24-103">meetingParticipantInfo resource type</span></span>

> <span data-ttu-id="00d24-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="00d24-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="00d24-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="00d24-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="00d24-106">有关会议中的参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="00d24-106">Information about a participant in a meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="00d24-107">属性</span><span class="sxs-lookup"><span data-stu-id="00d24-107">Properties</span></span>

| <span data-ttu-id="00d24-108">属性</span><span class="sxs-lookup"><span data-stu-id="00d24-108">Property</span></span>       | <span data-ttu-id="00d24-109">类型</span><span class="sxs-lookup"><span data-stu-id="00d24-109">Type</span></span>                          | <span data-ttu-id="00d24-110">说明</span><span class="sxs-lookup"><span data-stu-id="00d24-110">Description</span></span>                              |
|:---------------|:------------------------------|:-----------------------------------------|
| <span data-ttu-id="00d24-111">标识</span><span class="sxs-lookup"><span data-stu-id="00d24-111">identity</span></span>       | [<span data-ttu-id="00d24-112">identitySet</span><span class="sxs-lookup"><span data-stu-id="00d24-112">identitySet</span></span>](identityset.md) | <span data-ttu-id="00d24-113">参与者的标识信息。</span><span class="sxs-lookup"><span data-stu-id="00d24-113">Identity information of the participant.</span></span> |
| <span data-ttu-id="00d24-114">upn</span><span class="sxs-lookup"><span data-stu-id="00d24-114">upn</span></span>            | <span data-ttu-id="00d24-115">字符串</span><span class="sxs-lookup"><span data-stu-id="00d24-115">String</span></span>                        | <span data-ttu-id="00d24-116">参与者的用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="00d24-116">User principal name of the participant.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="00d24-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00d24-117">JSON representation</span></span>

<span data-ttu-id="00d24-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00d24-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.meetingParticipantInfo"
}-->
```json
{
  "identity": {"@odata.type": "#microsoft.graph.identitySet"},
  "upn": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "meetingParticipantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
