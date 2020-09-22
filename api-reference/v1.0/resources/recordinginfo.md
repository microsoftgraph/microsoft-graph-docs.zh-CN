---
title: recordingInfo 资源类型
description: 表示参与者的录制信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: dd640e3ddef6b88f17449c31611ad6bd956ca0b8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078974"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="5a655-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="5a655-103">recordingInfo resource type</span></span>

<span data-ttu-id="5a655-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a655-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5a655-105">表示参与者的录制信息。</span><span class="sxs-lookup"><span data-stu-id="5a655-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="5a655-106">属性</span><span class="sxs-lookup"><span data-stu-id="5a655-106">Properties</span></span>

| <span data-ttu-id="5a655-107">属性</span><span class="sxs-lookup"><span data-stu-id="5a655-107">Property</span></span>        | <span data-ttu-id="5a655-108">类型</span><span class="sxs-lookup"><span data-stu-id="5a655-108">Type</span></span>    | <span data-ttu-id="5a655-109">说明</span><span class="sxs-lookup"><span data-stu-id="5a655-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="5a655-110">initiator</span><span class="sxs-lookup"><span data-stu-id="5a655-110">initiator</span></span>     | [<span data-ttu-id="5a655-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="5a655-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="5a655-112">录制发起人的标识。</span><span class="sxs-lookup"><span data-stu-id="5a655-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="5a655-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="5a655-113">recordingStatus</span></span> | <span data-ttu-id="5a655-114">String</span><span class="sxs-lookup"><span data-stu-id="5a655-114">String</span></span> | <span data-ttu-id="5a655-115">可能的值包括： `unknown` 、 `notRecording` 、 `recording` 或 `failed` 。</span><span class="sxs-lookup"><span data-stu-id="5a655-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="5a655-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5a655-116">JSON representation</span></span>

<span data-ttu-id="5a655-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a655-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "initiator"
  ],
  "@odata.type": "microsoft.graph.recordingInfo"
}-->
```json
{
  "initiator": {"@odata.type": "#microsoft.graph.identitySet"},
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

