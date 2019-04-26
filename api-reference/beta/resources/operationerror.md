---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
localization_priority: Normal
ms.openlocfilehash: 957f1ed2960c33f2e7bc07f79e7f749a3b9f15a5
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341758"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="6cee5-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="6cee5-103">operationError resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6cee5-104">描述[teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="6cee5-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="6cee5-105">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="6cee5-105">operationError Properties</span></span>
| <span data-ttu-id="6cee5-106">属性</span><span class="sxs-lookup"><span data-stu-id="6cee5-106">Property</span></span>     | <span data-ttu-id="6cee5-107">类型</span><span class="sxs-lookup"><span data-stu-id="6cee5-107">Type</span></span>   |<span data-ttu-id="6cee5-108">说明</span><span class="sxs-lookup"><span data-stu-id="6cee5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6cee5-109">code</span><span class="sxs-lookup"><span data-stu-id="6cee5-109">code</span></span>|<span data-ttu-id="6cee5-110">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="6cee5-110">string (readonly)</span></span>|<span data-ttu-id="6cee5-111">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="6cee5-111">Operation error code.</span></span>|
|<span data-ttu-id="6cee5-112">message</span><span class="sxs-lookup"><span data-stu-id="6cee5-112">message</span></span>|<span data-ttu-id="6cee5-113">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="6cee5-113">string (readonly)</span></span>|<span data-ttu-id="6cee5-114">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="6cee5-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6cee5-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6cee5-115">JSON representation</span></span>

<span data-ttu-id="6cee5-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6cee5-116">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "operation error resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
