---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0cf550b0c15d5bd6632490d40eae04c0b4f5f3f1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447281"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="b00bd-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="b00bd-103">operationError resource type</span></span>

<span data-ttu-id="b00bd-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b00bd-104">Namespace: microsoft.graph</span></span>



<span data-ttu-id="b00bd-105">描述[teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="b00bd-105">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="b00bd-106">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="b00bd-106">operationError Properties</span></span>
| <span data-ttu-id="b00bd-107">属性</span><span class="sxs-lookup"><span data-stu-id="b00bd-107">Property</span></span>     | <span data-ttu-id="b00bd-108">类型</span><span class="sxs-lookup"><span data-stu-id="b00bd-108">Type</span></span>   |<span data-ttu-id="b00bd-109">说明</span><span class="sxs-lookup"><span data-stu-id="b00bd-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b00bd-110">code</span><span class="sxs-lookup"><span data-stu-id="b00bd-110">code</span></span>|<span data-ttu-id="b00bd-111">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="b00bd-111">string (readonly)</span></span>|<span data-ttu-id="b00bd-112">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="b00bd-112">Operation error code.</span></span>|
|<span data-ttu-id="b00bd-113">message</span><span class="sxs-lookup"><span data-stu-id="b00bd-113">message</span></span>|<span data-ttu-id="b00bd-114">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="b00bd-114">string (readonly)</span></span>|<span data-ttu-id="b00bd-115">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="b00bd-115">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b00bd-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b00bd-116">JSON representation</span></span>

<span data-ttu-id="b00bd-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b00bd-117">The following is a JSON representation of the resource.</span></span>

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
