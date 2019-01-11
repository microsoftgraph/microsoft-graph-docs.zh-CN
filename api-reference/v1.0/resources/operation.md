---
title: 操作资源类型
description: 长时间运行操作的状态。
localization_priority: Normal
ms.openlocfilehash: 4f2e2c9a6fb9eb6d26a3511c637e79822919e2f5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884964"
---
# <a name="operation-resource-type"></a><span data-ttu-id="cbdff-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="cbdff-103">operation resource type</span></span>

<span data-ttu-id="cbdff-104">长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="cbdff-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cbdff-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cbdff-105">JSON representation</span></span>

<span data-ttu-id="cbdff-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cbdff-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="cbdff-107">属性</span><span class="sxs-lookup"><span data-stu-id="cbdff-107">Properties</span></span>
| <span data-ttu-id="cbdff-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbdff-108">Property</span></span>     | <span data-ttu-id="cbdff-109">类型</span><span class="sxs-lookup"><span data-stu-id="cbdff-109">Type</span></span>   |<span data-ttu-id="cbdff-110">说明</span><span class="sxs-lookup"><span data-stu-id="cbdff-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cbdff-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cbdff-111">createdDateTime</span></span>| <span data-ttu-id="cbdff-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbdff-112">DateTimeOffset</span></span> |<span data-ttu-id="cbdff-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="cbdff-113">The start time of the operation.</span></span>|
|<span data-ttu-id="cbdff-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="cbdff-114">lastActionDateTime</span></span>| <span data-ttu-id="cbdff-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cbdff-115">DateTimeOffset</span></span> |<span data-ttu-id="cbdff-116">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="cbdff-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="cbdff-117">status</span><span class="sxs-lookup"><span data-stu-id="cbdff-117">status</span></span>|<span data-ttu-id="cbdff-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="cbdff-118">operationStatus</span></span>|<span data-ttu-id="cbdff-119">操作的当前状态：`notStarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="cbdff-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
