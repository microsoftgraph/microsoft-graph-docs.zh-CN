---
title: recordingInfo 资源类型
description: 记录参与者的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 644ba7fbd762acde7f5229d15267de5352f03ca8
ms.sourcegitcommit: 6144934d4f6cf8c9797aa19e62285217220c7f45
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268316"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="06f5f-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="06f5f-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="06f5f-104">记录参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="06f5f-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="06f5f-105">属性</span><span class="sxs-lookup"><span data-stu-id="06f5f-105">Properties</span></span>

| <span data-ttu-id="06f5f-106">属性</span><span class="sxs-lookup"><span data-stu-id="06f5f-106">Property</span></span>        | <span data-ttu-id="06f5f-107">类型</span><span class="sxs-lookup"><span data-stu-id="06f5f-107">Type</span></span>    | <span data-ttu-id="06f5f-108">说明</span><span class="sxs-lookup"><span data-stu-id="06f5f-108">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="06f5f-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="06f5f-109">initiatedBy</span></span>     | [<span data-ttu-id="06f5f-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="06f5f-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="06f5f-111">启动录制的参与者。</span><span class="sxs-lookup"><span data-stu-id="06f5f-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="06f5f-112">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="06f5f-112">recordingStatus</span></span> | <span data-ttu-id="06f5f-113">String</span><span class="sxs-lookup"><span data-stu-id="06f5f-113">String</span></span> | <span data-ttu-id="06f5f-114">可能的值包括`unknown`： `notRecording`、 `recording`、或`failed`。</span><span class="sxs-lookup"><span data-stu-id="06f5f-114">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |
| <span data-ttu-id="06f5f-115">initiator</span><span class="sxs-lookup"><span data-stu-id="06f5f-115">initiator</span></span> | [<span data-ttu-id="06f5f-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="06f5f-116">identitySet</span></span>](identitySet.md) | <span data-ttu-id="06f5f-117">记录发起方的标识。</span><span class="sxs-lookup"><span data-stu-id="06f5f-117">The identities of recording initiator.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="06f5f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06f5f-118">JSON representation</span></span>

<span data-ttu-id="06f5f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06f5f-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed",
  "initiator": {"@odata.type": "#microsoft.graph.initiator"}
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
