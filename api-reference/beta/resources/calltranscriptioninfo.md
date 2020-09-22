---
title: callTranscriptionInfo 资源类型
description: 表示单个 DTMF 事件。
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bd95ebf165bad8cde296d54e5b0a06f969f1c903
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042707"
---
# <a name="calltranscriptioninfo-resource-type"></a><span data-ttu-id="c59d3-103">callTranscriptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c59d3-103">callTranscriptionInfo resource type</span></span>

<span data-ttu-id="c59d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c59d3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c59d3-105">表示单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="c59d3-105">Represents a single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="c59d3-106">属性</span><span class="sxs-lookup"><span data-stu-id="c59d3-106">Properties</span></span>

| <span data-ttu-id="c59d3-107">属性</span><span class="sxs-lookup"><span data-stu-id="c59d3-107">Property</span></span>       | <span data-ttu-id="c59d3-108">类型</span><span class="sxs-lookup"><span data-stu-id="c59d3-108">Type</span></span>    | <span data-ttu-id="c59d3-109">说明</span><span class="sxs-lookup"><span data-stu-id="c59d3-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="c59d3-110">state</span><span class="sxs-lookup"><span data-stu-id="c59d3-110">state</span></span> | <span data-ttu-id="c59d3-111">String</span><span class="sxs-lookup"><span data-stu-id="c59d3-111">String</span></span> | <span data-ttu-id="c59d3-112">可取值为：`notStarted`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="c59d3-112">Possible values are: `notStarted`, `active`, `inactive`.</span></span> |
| <span data-ttu-id="c59d3-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c59d3-113">lastModifiedDateTime</span></span> | <span data-ttu-id="c59d3-114">日期时间</span><span class="sxs-lookup"><span data-stu-id="c59d3-114">DateTime</span></span> | <span data-ttu-id="c59d3-115">以 UTC 表示的状态修改时间。</span><span class="sxs-lookup"><span data-stu-id="c59d3-115">The state modified time in UTC.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c59d3-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c59d3-116">JSON representation</span></span>

<span data-ttu-id="c59d3-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c59d3-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.callTranscriptionInfo"
}-->
```json
{
  "state": "notStarted | active | inactive",
  "lastModifiedDateTime": "String (timestamp)"
}
```


