---
title: onenoteEntityBaseModel 资源
description: 这是 OneNote 实体的基类型。
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 0c6a3d4916bf54eeec5856f51af87fa79e1f6e6c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821229"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="1a8d9-103">onenoteEntityBaseModel 资源</span><span class="sxs-lookup"><span data-stu-id="1a8d9-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="1a8d9-104">这是 OneNote 实体的基类型。</span><span class="sxs-lookup"><span data-stu-id="1a8d9-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a8d9-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a8d9-105">JSON representation</span></span>

<span data-ttu-id="1a8d9-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a8d9-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [
    "self"
  ],
  "@odata.type": "microsoft.graph.onenoteEntityBaseModel"
}-->

```json
{
  "self": "string"
}

```
## <a name="properties"></a><span data-ttu-id="1a8d9-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a8d9-107">Properties</span></span>
| <span data-ttu-id="1a8d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="1a8d9-108">Property</span></span>     | <span data-ttu-id="1a8d9-109">类型</span><span class="sxs-lookup"><span data-stu-id="1a8d9-109">Type</span></span>   |<span data-ttu-id="1a8d9-110">Description</span><span class="sxs-lookup"><span data-stu-id="1a8d9-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1a8d9-111">self</span><span class="sxs-lookup"><span data-stu-id="1a8d9-111">self</span></span>|<span data-ttu-id="1a8d9-112">字符串</span><span class="sxs-lookup"><span data-stu-id="1a8d9-112">String</span></span>|<span data-ttu-id="1a8d9-p101">可以在其中获取关于页面的详细信息的终结点。只读。</span><span class="sxs-lookup"><span data-stu-id="1a8d9-p101">The endpoint where you can get details about the page. Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
