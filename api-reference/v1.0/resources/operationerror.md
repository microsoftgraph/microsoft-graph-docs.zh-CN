---
title: operationError 资源类型
description: 描述 teamsAsyncOperation 中的错误。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 8a46943fad974c2e7a12041e9def6a8a6ad6c9a3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035712"
---
# <a name="operationerror-resource-type"></a><span data-ttu-id="fa258-103">operationError 资源类型</span><span class="sxs-lookup"><span data-stu-id="fa258-103">operationError resource type</span></span>



<span data-ttu-id="fa258-104">描述[teamsAsyncOperation](teamsasyncoperation.md)中的错误。</span><span class="sxs-lookup"><span data-stu-id="fa258-104">Describes errors in [teamsAsyncOperation](teamsasyncoperation.md).</span></span>

## <a name="operationerror-properties"></a><span data-ttu-id="fa258-105">operationError 属性</span><span class="sxs-lookup"><span data-stu-id="fa258-105">operationError Properties</span></span>
| <span data-ttu-id="fa258-106">属性</span><span class="sxs-lookup"><span data-stu-id="fa258-106">Property</span></span>     | <span data-ttu-id="fa258-107">类型</span><span class="sxs-lookup"><span data-stu-id="fa258-107">Type</span></span>   |<span data-ttu-id="fa258-108">说明</span><span class="sxs-lookup"><span data-stu-id="fa258-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa258-109">code</span><span class="sxs-lookup"><span data-stu-id="fa258-109">code</span></span>|<span data-ttu-id="fa258-110">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="fa258-110">string (readonly)</span></span>|<span data-ttu-id="fa258-111">操作错误代码。</span><span class="sxs-lookup"><span data-stu-id="fa258-111">Operation error code.</span></span>|
|<span data-ttu-id="fa258-112">message</span><span class="sxs-lookup"><span data-stu-id="fa258-112">message</span></span>|<span data-ttu-id="fa258-113">string (readonly)</span><span class="sxs-lookup"><span data-stu-id="fa258-113">string (readonly)</span></span>|<span data-ttu-id="fa258-114">操作错误消息。</span><span class="sxs-lookup"><span data-stu-id="fa258-114">Operation error message.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fa258-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fa258-115">JSON representation</span></span>

<span data-ttu-id="fa258-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fa258-116">The following is a JSON representation of the resource.</span></span>

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
