---
title: callTranscriptionInfo 资源类型
description: 表示单个 DTMF 事件。
author: rzhang
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0f2f91b8aadfd9f819e87eff839090aa37166cf2
ms.sourcegitcommit: ae2e4b8963edcdcc8ce572c06a531db4769d7779
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/29/2020
ms.locfileid: "47312207"
---
# <a name="calltranscriptioninfo-resource-type"></a><span data-ttu-id="83afb-103">callTranscriptionInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="83afb-103">callTranscriptionInfo resource type</span></span>

<span data-ttu-id="83afb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83afb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="83afb-105">表示单个 DTMF 事件。</span><span class="sxs-lookup"><span data-stu-id="83afb-105">Represents a single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="83afb-106">属性</span><span class="sxs-lookup"><span data-stu-id="83afb-106">Properties</span></span>

| <span data-ttu-id="83afb-107">属性</span><span class="sxs-lookup"><span data-stu-id="83afb-107">Property</span></span>       | <span data-ttu-id="83afb-108">类型</span><span class="sxs-lookup"><span data-stu-id="83afb-108">Type</span></span>    | <span data-ttu-id="83afb-109">说明</span><span class="sxs-lookup"><span data-stu-id="83afb-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="83afb-110">state</span><span class="sxs-lookup"><span data-stu-id="83afb-110">state</span></span> | <span data-ttu-id="83afb-111">String</span><span class="sxs-lookup"><span data-stu-id="83afb-111">String</span></span> | <span data-ttu-id="83afb-112">可取值为：`notStarted`、`active`、`inactive`。</span><span class="sxs-lookup"><span data-stu-id="83afb-112">Possible values are: `notStarted`, `active`, `inactive`.</span></span> |
| <span data-ttu-id="83afb-113">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="83afb-113">lastModifiedDateTime</span></span> | <span data-ttu-id="83afb-114">日期时间</span><span class="sxs-lookup"><span data-stu-id="83afb-114">DateTime</span></span> | <span data-ttu-id="83afb-115">以 UTC 表示的状态修改时间。</span><span class="sxs-lookup"><span data-stu-id="83afb-115">The state modified time in UTC.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="83afb-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="83afb-116">JSON representation</span></span>

<span data-ttu-id="83afb-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83afb-117">The following is a JSON representation of the resource.</span></span>

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
