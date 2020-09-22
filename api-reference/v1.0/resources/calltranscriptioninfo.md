---
title: callTranscriptionInfo 资源类型
description: 表示单个 DTMF 事件。
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b825264623eb74507e43dcd9302499811377f3fb
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48069244"
---
# <a name="calltranscriptioninfo-resource-type"></a><span data-ttu-id="e085b-103">callTranscriptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="e085b-103">callTranscriptionInfo resource type</span></span>

<span data-ttu-id="e085b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e085b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e085b-105">表示单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="e085b-105">Represents a single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="e085b-106">属性</span><span class="sxs-lookup"><span data-stu-id="e085b-106">Properties</span></span>

| <span data-ttu-id="e085b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e085b-107">Property</span></span>       | <span data-ttu-id="e085b-108">类型</span><span class="sxs-lookup"><span data-stu-id="e085b-108">Type</span></span>    | <span data-ttu-id="e085b-109">说明</span><span class="sxs-lookup"><span data-stu-id="e085b-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e085b-110">state</span><span class="sxs-lookup"><span data-stu-id="e085b-110">state</span></span> | <span data-ttu-id="e085b-111">String</span><span class="sxs-lookup"><span data-stu-id="e085b-111">String</span></span> | <span data-ttu-id="e085b-112">可取值为：`notStarted`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="e085b-112">Possible values are: `notStarted`, `active`, `inactive`.</span></span> |
| <span data-ttu-id="e085b-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e085b-113">lastModifiedDateTime</span></span> | <span data-ttu-id="e085b-114">日期时间</span><span class="sxs-lookup"><span data-stu-id="e085b-114">DateTime</span></span> | <span data-ttu-id="e085b-115">以 UTC 表示的状态修改时间。</span><span class="sxs-lookup"><span data-stu-id="e085b-115">The state modified time in UTC.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e085b-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e085b-116">JSON representation</span></span>

<span data-ttu-id="e085b-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e085b-117">The following is a JSON representation of the resource.</span></span>

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

