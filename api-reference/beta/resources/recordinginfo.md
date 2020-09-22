---
title: recordingInfo 资源类型
description: 记录参与者的信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 45d844329688e663c27ef5ecdf94282312baa53d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48055173"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="184cc-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="184cc-103">recordingInfo resource type</span></span>

<span data-ttu-id="184cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="184cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="184cc-105">记录参与者的信息。</span><span class="sxs-lookup"><span data-stu-id="184cc-105">Recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="184cc-106">属性</span><span class="sxs-lookup"><span data-stu-id="184cc-106">Properties</span></span>

| <span data-ttu-id="184cc-107">属性</span><span class="sxs-lookup"><span data-stu-id="184cc-107">Property</span></span>        | <span data-ttu-id="184cc-108">类型</span><span class="sxs-lookup"><span data-stu-id="184cc-108">Type</span></span>    | <span data-ttu-id="184cc-109">说明</span><span class="sxs-lookup"><span data-stu-id="184cc-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="184cc-110">initiatedBy</span><span class="sxs-lookup"><span data-stu-id="184cc-110">initiatedBy</span></span>     | [<span data-ttu-id="184cc-111">participantInfo</span><span class="sxs-lookup"><span data-stu-id="184cc-111">participantInfo</span></span>](participantinfo.md) | <span data-ttu-id="184cc-112">启动录制的参与者。</span><span class="sxs-lookup"><span data-stu-id="184cc-112">The participant who initiated the recording.</span></span> |
| <span data-ttu-id="184cc-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="184cc-113">recordingStatus</span></span> | <span data-ttu-id="184cc-114">String</span><span class="sxs-lookup"><span data-stu-id="184cc-114">String</span></span> | <span data-ttu-id="184cc-115">可能的值包括： `unknown` 、 `notRecording` 、 `recording` 或 `failed` 。</span><span class="sxs-lookup"><span data-stu-id="184cc-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |
| <span data-ttu-id="184cc-116">initiator</span><span class="sxs-lookup"><span data-stu-id="184cc-116">initiator</span></span> | [<span data-ttu-id="184cc-117">identitySet</span><span class="sxs-lookup"><span data-stu-id="184cc-117">identitySet</span></span>](identitySet.md) | <span data-ttu-id="184cc-118">记录发起方的标识。</span><span class="sxs-lookup"><span data-stu-id="184cc-118">The identities of recording initiator.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="184cc-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="184cc-119">JSON representation</span></span>

<span data-ttu-id="184cc-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="184cc-120">The following is a JSON representation of the resource.</span></span>

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


