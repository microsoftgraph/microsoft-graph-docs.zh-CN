---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
localization_priority: Normal
author: billbliss
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6ae6215d00bc573e6c8d004de743b10c0d381e43
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808160"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="2e1a8-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e1a8-103">operationError resource type</span></span>

<span data-ttu-id="2e1a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e1a8-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="2e1a8-105">描述 [teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="2e1a8-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="2e1a8-106">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="2e1a8-106">operationError Properties</span></span>
| <span data-ttu-id="2e1a8-107">属性</span><span class="sxs-lookup"><span data-stu-id="2e1a8-107">Property</span></span>     | <span data-ttu-id="2e1a8-108">类型</span><span class="sxs-lookup"><span data-stu-id="2e1a8-108">Type</span></span>   |<span data-ttu-id="2e1a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="2e1a8-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e1a8-110">code</span><span class="sxs-lookup"><span data-stu-id="2e1a8-110">code</span></span>|<span data-ttu-id="2e1a8-111">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="2e1a8-111">string (readonly)</span></span>|<span data-ttu-id="2e1a8-112">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="2e1a8-112">Operation error code.</span></span>|
|<span data-ttu-id="2e1a8-113">message</span><span class="sxs-lookup"><span data-stu-id="2e1a8-113">message</span></span>|<span data-ttu-id="2e1a8-114">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="2e1a8-114">string (readonly)</span></span>|<span data-ttu-id="2e1a8-115">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="2e1a8-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e1a8-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e1a8-116">JSON representation</span></span>

<span data-ttu-id="2e1a8-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e1a8-117">The following is a JSON representation of the resource.</span></span>

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
