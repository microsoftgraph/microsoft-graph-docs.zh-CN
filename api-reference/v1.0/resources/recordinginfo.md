---
title: recordingInfo 资源类型
description: 表示参与者的录制信息。
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b7044f13f16a9d1126a5b1c72cdc86c3527f6b37
ms.sourcegitcommit: d14e2abb24d9fbab519458b1c9fec890a5e51d70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2020
ms.locfileid: "43543266"
---
# <a name="recordinginfo-resource-type"></a><span data-ttu-id="513d4-103">recordingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="513d4-103">recordingInfo resource type</span></span>

<span data-ttu-id="513d4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="513d4-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="513d4-105">表示参与者的录制信息。</span><span class="sxs-lookup"><span data-stu-id="513d4-105">Represents recording information for a participant.</span></span>

## <a name="properties"></a><span data-ttu-id="513d4-106">属性</span><span class="sxs-lookup"><span data-stu-id="513d4-106">Properties</span></span>

| <span data-ttu-id="513d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="513d4-107">Property</span></span>        | <span data-ttu-id="513d4-108">类型</span><span class="sxs-lookup"><span data-stu-id="513d4-108">Type</span></span>    | <span data-ttu-id="513d4-109">说明</span><span class="sxs-lookup"><span data-stu-id="513d4-109">Description</span></span>|
|:----------------|:--------|:----------|
| <span data-ttu-id="513d4-110">initiator</span><span class="sxs-lookup"><span data-stu-id="513d4-110">initiator</span></span>     | [<span data-ttu-id="513d4-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="513d4-111">identitySet</span></span>](identitySet.md) | <span data-ttu-id="513d4-112">录制发起人的标识。</span><span class="sxs-lookup"><span data-stu-id="513d4-112">The identities of the recording initiator.</span></span> |
| <span data-ttu-id="513d4-113">recordingStatus</span><span class="sxs-lookup"><span data-stu-id="513d4-113">recordingStatus</span></span> | <span data-ttu-id="513d4-114">String</span><span class="sxs-lookup"><span data-stu-id="513d4-114">String</span></span> | <span data-ttu-id="513d4-115">可能的值包括`unknown`： `notRecording`、 `recording`、或`failed`。</span><span class="sxs-lookup"><span data-stu-id="513d4-115">Possible values are: `unknown`, `notRecording`, `recording`, or `failed`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="513d4-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="513d4-116">JSON representation</span></span>

<span data-ttu-id="513d4-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="513d4-117">The following is a JSON representation of the resource.</span></span>

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
