---
title: 操作资源类型
description: 长时间运行的操作的状态。
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 21a49f360ac18ad42ce5530a8cfcbcbea1876bc0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072856"
---
# <a name="operation-resource-type"></a><span data-ttu-id="6229a-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="6229a-103">operation resource type</span></span>

<span data-ttu-id="6229a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6229a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6229a-105">长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="6229a-105">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6229a-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6229a-106">JSON representation</span></span>

<span data-ttu-id="6229a-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6229a-107">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.operation"
}-->

```json
{
  "createdDateTime": "String (timestamp)",
  "lastActionDateTime": "String (timestamp)",
  "status": "notStarted | running | completed | failed"
}

```
## <a name="properties"></a><span data-ttu-id="6229a-108">属性</span><span class="sxs-lookup"><span data-stu-id="6229a-108">Properties</span></span>
| <span data-ttu-id="6229a-109">属性</span><span class="sxs-lookup"><span data-stu-id="6229a-109">Property</span></span>     | <span data-ttu-id="6229a-110">类型</span><span class="sxs-lookup"><span data-stu-id="6229a-110">Type</span></span>   |<span data-ttu-id="6229a-111">说明</span><span class="sxs-lookup"><span data-stu-id="6229a-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6229a-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6229a-112">createdDateTime</span></span>| <span data-ttu-id="6229a-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6229a-113">DateTimeOffset</span></span> |<span data-ttu-id="6229a-114">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="6229a-114">The start time of the operation.</span></span>|
|<span data-ttu-id="6229a-115">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="6229a-115">lastActionDateTime</span></span>| <span data-ttu-id="6229a-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6229a-116">DateTimeOffset</span></span> |<span data-ttu-id="6229a-117">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="6229a-117">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="6229a-118">status</span><span class="sxs-lookup"><span data-stu-id="6229a-118">status</span></span>|<span data-ttu-id="6229a-119">operationStatus</span><span class="sxs-lookup"><span data-stu-id="6229a-119">operationStatus</span></span>|<span data-ttu-id="6229a-120">操作的当前状态： `notStarted` 、 `running` 、 `completed` 、 `failed`</span><span class="sxs-lookup"><span data-stu-id="6229a-120">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

