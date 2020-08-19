---
title: 操作资源类型
description: 长时间运行的操作的状态。
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c9b920bbf696e80923c1d37756d7c27e1f06ab3a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808149"
---
# <a name="operation-resource-type"></a><span data-ttu-id="0e863-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="0e863-103">operation resource type</span></span>

<span data-ttu-id="0e863-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e863-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0e863-105">长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="0e863-105">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e863-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e863-106">JSON representation</span></span>

<span data-ttu-id="0e863-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e863-107">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0e863-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e863-108">Properties</span></span>
| <span data-ttu-id="0e863-109">属性</span><span class="sxs-lookup"><span data-stu-id="0e863-109">Property</span></span>     | <span data-ttu-id="0e863-110">类型</span><span class="sxs-lookup"><span data-stu-id="0e863-110">Type</span></span>   |<span data-ttu-id="0e863-111">说明</span><span class="sxs-lookup"><span data-stu-id="0e863-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0e863-112">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0e863-112">createdDateTime</span></span>| <span data-ttu-id="0e863-113">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e863-113">DateTimeOffset</span></span> |<span data-ttu-id="0e863-114">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="0e863-114">The start time of the operation.</span></span>|
|<span data-ttu-id="0e863-115">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="0e863-115">lastActionDateTime</span></span>| <span data-ttu-id="0e863-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e863-116">DateTimeOffset</span></span> |<span data-ttu-id="0e863-117">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="0e863-117">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="0e863-118">status</span><span class="sxs-lookup"><span data-stu-id="0e863-118">status</span></span>|<span data-ttu-id="0e863-119">operationStatus</span><span class="sxs-lookup"><span data-stu-id="0e863-119">operationStatus</span></span>|<span data-ttu-id="0e863-120">操作的当前状态： `notStarted` 、 `running` 、 `completed` 、 `failed`</span><span class="sxs-lookup"><span data-stu-id="0e863-120">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
