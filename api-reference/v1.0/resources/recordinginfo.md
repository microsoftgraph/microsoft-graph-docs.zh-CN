---
title: recordingInfo 资源类型
description: 表示参与者的录制信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 6a41195705a46ac46bd085f3b4a655943b730ad3
ms.sourcegitcommit: 115890bc7e7a54db8a2befeb8f720a9ca94f42b5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2020
ms.locfileid: "42962539"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="78ef7-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="78ef7-103">recordingInfo resource type</span></span>

<span data-ttu-id="78ef7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78ef7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="78ef7-105">表示参与者的录制信息。</span><span class="sxs-lookup"><span data-stu-id="78ef7-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="78ef7-106">属性</span><span class="sxs-lookup"><span data-stu-id="78ef7-106">Properties</span></span>

| <span data-ttu-id="78ef7-107">属性</span><span class="sxs-lookup"><span data-stu-id="78ef7-107">Property</span></span>        | <span data-ttu-id="78ef7-108">类型</span><span class="sxs-lookup"><span data-stu-id="78ef7-108">Type</span></span>    | <span data-ttu-id="78ef7-109">说明</span><span class="sxs-lookup"><span data-stu-id="78ef7-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="78ef7-110">initiator</span><span class="sxs-lookup"><span data-stu-id="78ef7-110">initiator</span></span>     | [<span data-ttu-id="78ef7-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="78ef7-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="78ef7-112">录制发起人的标识。</span><span class="sxs-lookup"><span data-stu-id="78ef7-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="78ef7-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="78ef7-113">recordingStatus</span></span> | <span data-ttu-id="78ef7-114">String</span><span class="sxs-lookup"><span data-stu-id="78ef7-114">String</span></span> | <span data-ttu-id="78ef7-115">可能的值包括`unknown`： `notRecording`、 `recording`、或`failed`。</span><span class="sxs-lookup"><span data-stu-id="78ef7-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="78ef7-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78ef7-116">JSON representation</span></span>

<span data-ttu-id="78ef7-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78ef7-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
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
