---
title: operationError 资源类型
description: 介绍 teamsAsyncOperation 中的错误。
localization_priority: Normal
ms.openlocfilehash: 22590d7d955cf01385292d2796ad960b1c0ced41
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824582"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="9d635-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d635-103">operationError resource type</span></span>



<span data-ttu-id="9d635-104">介绍[teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="9d635-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="9d635-105">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="9d635-105">operationError Properties</span></span>
| <span data-ttu-id="9d635-106">属性</span><span class="sxs-lookup"><span data-stu-id="9d635-106">Property</span></span>     | <span data-ttu-id="9d635-107">类型</span><span class="sxs-lookup"><span data-stu-id="9d635-107">Type</span></span>   |<span data-ttu-id="9d635-108">说明</span><span class="sxs-lookup"><span data-stu-id="9d635-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d635-109">code</span><span class="sxs-lookup"><span data-stu-id="9d635-109">code</span></span>|<span data-ttu-id="9d635-110">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="9d635-110">string (readonly)</span></span>|<span data-ttu-id="9d635-111">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="9d635-111">Operation error code.</span></span>|
|<span data-ttu-id="9d635-112">message</span><span class="sxs-lookup"><span data-stu-id="9d635-112">message</span></span>|<span data-ttu-id="9d635-113">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="9d635-113">string (readonly)</span></span>|<span data-ttu-id="9d635-114">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="9d635-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9d635-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d635-115">JSON representation</span></span>

<span data-ttu-id="9d635-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d635-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.operationError"
}-->

```json
{
    "code": "TeamUnavailable",
    "message": "The team was not found."
}
```

<!-- uuid: 069fadaa-52db-4ced-85d5-74f7caa2c66f
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
