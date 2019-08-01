---
title: 操作资源类型
description: 长时间运行的操作的状态。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8088d704d5a075131d5ee1b2c3b9edf75785708b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035726"
---
# <a name="operation-resource-type"></a><span data-ttu-id="7df24-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="7df24-103">operation resource type</span></span>

<span data-ttu-id="7df24-104">长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7df24-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7df24-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7df24-105">JSON representation</span></span>

<span data-ttu-id="7df24-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7df24-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7df24-107">属性</span><span class="sxs-lookup"><span data-stu-id="7df24-107">Properties</span></span>
| <span data-ttu-id="7df24-108">属性</span><span class="sxs-lookup"><span data-stu-id="7df24-108">Property</span></span>     | <span data-ttu-id="7df24-109">类型</span><span class="sxs-lookup"><span data-stu-id="7df24-109">Type</span></span>   |<span data-ttu-id="7df24-110">说明</span><span class="sxs-lookup"><span data-stu-id="7df24-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7df24-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7df24-111">createdDateTime</span></span>| <span data-ttu-id="7df24-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df24-112">DateTimeOffset</span></span> |<span data-ttu-id="7df24-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="7df24-113">The start time of the operation.</span></span>|
|<span data-ttu-id="7df24-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7df24-114">lastActionDateTime</span></span>| <span data-ttu-id="7df24-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7df24-115">DateTimeOffset</span></span> |<span data-ttu-id="7df24-116">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="7df24-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="7df24-117">status</span><span class="sxs-lookup"><span data-stu-id="7df24-117">status</span></span>|<span data-ttu-id="7df24-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="7df24-118">operationStatus</span></span>|<span data-ttu-id="7df24-119">操作的当前状态: `notStarted`、 `running`、、 `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="7df24-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
