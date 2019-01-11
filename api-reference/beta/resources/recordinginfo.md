---
title: recordingInfo 资源类型
description: 参与者录制信息。
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: 85c2710452905f97235928bae71ff60c2d22983f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27891936"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="7d596-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="7d596-103">recordingInfo resource type</span></span>

> <span data-ttu-id="7d596-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7d596-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d596-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7d596-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7d596-106">参与者录制信息。</span><span class="sxs-lookup"><span data-stu-id="7d596-106">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="7d596-107">属性</span><span class="sxs-lookup"><span data-stu-id="7d596-107">Properties</span></span>

| <span data-ttu-id="7d596-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d596-108">Property</span></span>       | <span data-ttu-id="7d596-109">类型</span><span class="sxs-lookup"><span data-stu-id="7d596-109">Type</span></span>    | <span data-ttu-id="7d596-110">Description</span><span class="sxs-lookup"><span data-stu-id="7d596-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7d596-111">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="7d596-111">initiatedBy</span></span> | [<span data-ttu-id="7d596-112">participantInfo</span><span class="sxs-lookup"><span data-stu-id="7d596-112">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="7d596-113">参与者发起录制。</span><span class="sxs-lookup"><span data-stu-id="7d596-113">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="7d596-114">status</span><span class="sxs-lookup"><span data-stu-id="7d596-114">status</span></span> | <span data-ttu-id="7d596-115">字符串</span><span class="sxs-lookup"><span data-stu-id="7d596-115">String</span></span> | <span data-ttu-id="7d596-116">可取值为：`recordingCapable`、`notRecording`、`startedRecording`。</span><span class="sxs-lookup"><span data-stu-id="7d596-116">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7d596-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7d596-117">JSON representation</span></span>

<span data-ttu-id="7d596-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d596-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "status": "recordingCapable | notRecording | startedRecording"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
