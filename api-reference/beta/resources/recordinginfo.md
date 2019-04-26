---
title: recordingInfo 资源类型
description: 记录参与者的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 6025259bafdcff78c3c7dbfa19aa39f5f6648f84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563095"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="82d5f-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="82d5f-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82d5f-104">记录参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="82d5f-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="82d5f-105">属性</span><span class="sxs-lookup"><span data-stu-id="82d5f-105">Properties</span></span>

| <span data-ttu-id="82d5f-106">属性</span><span class="sxs-lookup"><span data-stu-id="82d5f-106">Property</span></span>       | <span data-ttu-id="82d5f-107">类型</span><span class="sxs-lookup"><span data-stu-id="82d5f-107">Type</span></span>    | <span data-ttu-id="82d5f-108">说明</span><span class="sxs-lookup"><span data-stu-id="82d5f-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="82d5f-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="82d5f-109">initiatedBy</span></span> | [<span data-ttu-id="82d5f-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="82d5f-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="82d5f-111">启动录制的参与者。</span><span class="sxs-lookup"><span data-stu-id="82d5f-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="82d5f-112">状态</span><span class="sxs-lookup"><span data-stu-id="82d5f-112">status</span></span> | <span data-ttu-id="82d5f-113">字符串</span><span class="sxs-lookup"><span data-stu-id="82d5f-113">String</span></span> | <span data-ttu-id="82d5f-114">可取值为：`recordingCapable`、`notRecording`、`startedRecording`。</span><span class="sxs-lookup"><span data-stu-id="82d5f-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="82d5f-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82d5f-115">JSON representation</span></span>

<span data-ttu-id="82d5f-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82d5f-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recordingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
