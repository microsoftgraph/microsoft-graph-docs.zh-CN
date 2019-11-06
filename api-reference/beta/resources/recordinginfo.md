---
title: recordingInfo 资源类型
description: 记录参与者的信息。
author: VinodRavichandran
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 2da0dd44ca1dc7ffd8d6ee13b1289e75c87f7cd6
ms.sourcegitcommit: 9bddc0b7746383e8d05ce50d163af3f4196f12a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/06/2019
ms.locfileid: "38006562"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="64db3-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="64db3-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64db3-104">记录参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="64db3-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="64db3-105">属性</span><span class="sxs-lookup"><span data-stu-id="64db3-105">Properties</span></span>

| <span data-ttu-id="64db3-106">属性</span><span class="sxs-lookup"><span data-stu-id="64db3-106">Property</span></span>       | <span data-ttu-id="64db3-107">类型</span><span class="sxs-lookup"><span data-stu-id="64db3-107">Type</span></span>    | <span data-ttu-id="64db3-108">说明</span><span class="sxs-lookup"><span data-stu-id="64db3-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="64db3-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="64db3-109">initiatedBy</span></span> | [<span data-ttu-id="64db3-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="64db3-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="64db3-111">启动录制的参与者。</span><span class="sxs-lookup"><span data-stu-id="64db3-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="64db3-112">状态</span><span class="sxs-lookup"><span data-stu-id="64db3-112">status</span></span> | <span data-ttu-id="64db3-113">String</span><span class="sxs-lookup"><span data-stu-id="64db3-113">String</span></span> | <span data-ttu-id="64db3-114">可取值为：`recordingCapable`、`notRecording`、`startedRecording`。</span><span class="sxs-lookup"><span data-stu-id="64db3-114">Possible values are: `recordingCapable`, `notRecording`, `startedRecording`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="64db3-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="64db3-115">JSON representation</span></span>

<span data-ttu-id="64db3-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64db3-116">The following is a JSON representation of the resource.</span></span>

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
