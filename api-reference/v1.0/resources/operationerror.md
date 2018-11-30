---
title: operationError 资源类型
description: 介绍 teamsAsyncOperation 中的错误。
ms.openlocfilehash: bcd8c989c4c69336165ef1ca29e1d114d524aa9e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010607"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="7c7ae-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c7ae-103">operationError resource type</span></span>



<span data-ttu-id="7c7ae-104">介绍[teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="7c7ae-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="7c7ae-105">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="7c7ae-105">operationError Properties</span></span>
| <span data-ttu-id="7c7ae-106">属性</span><span class="sxs-lookup"><span data-stu-id="7c7ae-106">Property</span></span>     | <span data-ttu-id="7c7ae-107">类型</span><span class="sxs-lookup"><span data-stu-id="7c7ae-107">Type</span></span>   |<span data-ttu-id="7c7ae-108">说明</span><span class="sxs-lookup"><span data-stu-id="7c7ae-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7c7ae-109">code</span><span class="sxs-lookup"><span data-stu-id="7c7ae-109">code</span></span>|<span data-ttu-id="7c7ae-110">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="7c7ae-110">string (readonly)</span></span>|<span data-ttu-id="7c7ae-111">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="7c7ae-111">Operation error code.</span></span>|
|<span data-ttu-id="7c7ae-112">message</span><span class="sxs-lookup"><span data-stu-id="7c7ae-112">message</span></span>|<span data-ttu-id="7c7ae-113">字符串 （只读）</span><span class="sxs-lookup"><span data-stu-id="7c7ae-113">string (readonly)</span></span>|<span data-ttu-id="7c7ae-114">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="7c7ae-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7c7ae-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c7ae-115">JSON representation</span></span>

<span data-ttu-id="7c7ae-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c7ae-116">The following is a JSON representation of the resource.</span></span>

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
