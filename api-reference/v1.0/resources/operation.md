---
title: 操作资源类型
description: 长时间运行操作的状态。
ms.openlocfilehash: 622a17233a25709047ea852b7df5020aee3ae343
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008123"
---
# <a name="operation-resource-type"></a><span data-ttu-id="7fd33-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="7fd33-103">operation resource type</span></span>

<span data-ttu-id="7fd33-104">长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="7fd33-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7fd33-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7fd33-105">JSON representation</span></span>

<span data-ttu-id="7fd33-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7fd33-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="7fd33-107">属性</span><span class="sxs-lookup"><span data-stu-id="7fd33-107">Properties</span></span>
| <span data-ttu-id="7fd33-108">属性</span><span class="sxs-lookup"><span data-stu-id="7fd33-108">Property</span></span>     | <span data-ttu-id="7fd33-109">类型</span><span class="sxs-lookup"><span data-stu-id="7fd33-109">Type</span></span>   |<span data-ttu-id="7fd33-110">说明</span><span class="sxs-lookup"><span data-stu-id="7fd33-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7fd33-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7fd33-111">createdDateTime</span></span>| <span data-ttu-id="7fd33-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fd33-112">DateTimeOffset</span></span> |<span data-ttu-id="7fd33-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="7fd33-113">The start time of the operation.</span></span>|
|<span data-ttu-id="7fd33-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="7fd33-114">lastActionDateTime</span></span>| <span data-ttu-id="7fd33-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7fd33-115">DateTimeOffset</span></span> |<span data-ttu-id="7fd33-116">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="7fd33-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="7fd33-117">状态</span><span class="sxs-lookup"><span data-stu-id="7fd33-117">status</span></span>|<span data-ttu-id="7fd33-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="7fd33-118">operationStatus</span></span>|<span data-ttu-id="7fd33-119">操作的当前状态：`notStarted`、`running`、`completed`、`failed`</span><span class="sxs-lookup"><span data-stu-id="7fd33-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
