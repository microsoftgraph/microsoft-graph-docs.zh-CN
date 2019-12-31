---
title: recordingInfo 资源类型
description: 记录参与者的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: e924ea98bb0f9ac8e0b610a4672cbed83d83d0bc
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913441"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="d6c21-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6c21-103">recordingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d6c21-104">记录参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="d6c21-104">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="d6c21-105">属性</span><span class="sxs-lookup"><span data-stu-id="d6c21-105">Properties</span></span>

| <span data-ttu-id="d6c21-106">属性</span><span class="sxs-lookup"><span data-stu-id="d6c21-106">Property</span></span>        | <span data-ttu-id="d6c21-107">类型</span><span class="sxs-lookup"><span data-stu-id="d6c21-107">Type</span></span>    | <span data-ttu-id="d6c21-108">说明</span><span class="sxs-lookup"><span data-stu-id="d6c21-108">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="d6c21-109">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="d6c21-109">initiatedBy</span></span>     | [<span data-ttu-id="d6c21-110">participantInfo</span><span class="sxs-lookup"><span data-stu-id="d6c21-110">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="d6c21-111">启动录制的参与者。</span><span class="sxs-lookup"><span data-stu-id="d6c21-111">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="d6c21-112">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="d6c21-112">recordingStatus</span></span> | <span data-ttu-id="d6c21-113">String</span><span class="sxs-lookup"><span data-stu-id="d6c21-113">String</span></span> | <span data-ttu-id="d6c21-114">可能的值包括`unknown`： `notRecording`、 `recording`、或`failed`。</span><span class="sxs-lookup"><span data-stu-id="d6c21-114">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="d6c21-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6c21-115">JSON representation</span></span>

<span data-ttu-id="d6c21-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6c21-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiatedBy": {"@odata.type": "#microsoft.graph.participantInfo"},
  "recordingStatus": "unknown | notRecording | recording | failed"
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
