---
title: 操作资源类型
description: 长时间运行的操作的状态。
localization_priority: Normal
ms.openlocfilehash: 4f2e2c9a6fb9eb6d26a3511c637e79822919e2f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462674"
---
# <a name="operation-resource-type"></a><span data-ttu-id="74b8a-103">操作资源类型</span><span class="sxs-lookup"><span data-stu-id="74b8a-103">operation resource type</span></span>

<span data-ttu-id="74b8a-104">长时间运行的操作的状态。</span><span class="sxs-lookup"><span data-stu-id="74b8a-104">The status of a long-running operation.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74b8a-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74b8a-105">JSON representation</span></span>

<span data-ttu-id="74b8a-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74b8a-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="74b8a-107">属性</span><span class="sxs-lookup"><span data-stu-id="74b8a-107">Properties</span></span>
| <span data-ttu-id="74b8a-108">属性</span><span class="sxs-lookup"><span data-stu-id="74b8a-108">Property</span></span>     | <span data-ttu-id="74b8a-109">类型</span><span class="sxs-lookup"><span data-stu-id="74b8a-109">Type</span></span>   |<span data-ttu-id="74b8a-110">说明</span><span class="sxs-lookup"><span data-stu-id="74b8a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="74b8a-111">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="74b8a-111">createdDateTime</span></span>| <span data-ttu-id="74b8a-112">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74b8a-112">DateTimeOffset</span></span> |<span data-ttu-id="74b8a-113">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="74b8a-113">The start time of the operation.</span></span>|
|<span data-ttu-id="74b8a-114">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="74b8a-114">lastActionDateTime</span></span>| <span data-ttu-id="74b8a-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74b8a-115">DateTimeOffset</span></span> |<span data-ttu-id="74b8a-116">操作的上一操作的时间。</span><span class="sxs-lookup"><span data-stu-id="74b8a-116">The time of the last action of the operation.</span></span>|
|<span data-ttu-id="74b8a-117">status</span><span class="sxs-lookup"><span data-stu-id="74b8a-117">status</span></span>|<span data-ttu-id="74b8a-118">operationStatus</span><span class="sxs-lookup"><span data-stu-id="74b8a-118">operationStatus</span></span>|<span data-ttu-id="74b8a-119">操作的当前状态: `notStarted`、 `running`、、 `completed``failed`</span><span class="sxs-lookup"><span data-stu-id="74b8a-119">The current status of the operation: `notStarted`, `running`, `completed`, `failed`</span></span> |

<!-- uuid: 13fa92b1-3b41-498b-aab1-f943464a124f
2018-03-30 10:29:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
