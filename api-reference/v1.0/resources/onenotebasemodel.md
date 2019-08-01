---
title: onenoteEntityBaseModel 资源
description: 这是 OneNote 实体的基本类型。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: be196cff07a33f1debabd71e3e344aee220bf0a2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035838"
---
# <a name="onenoteentitybasemodel-resource"></a><span data-ttu-id="b6094-103">onenoteEntityBaseModel 资源</span><span class="sxs-lookup"><span data-stu-id="b6094-103">onenoteEntityBaseModel resource</span></span>

<span data-ttu-id="b6094-104">这是 OneNote 实体的基本类型。</span><span class="sxs-lookup"><span data-stu-id="b6094-104">This is the base type for OneNote entities.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6094-105">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6094-105">JSON representation</span></span>

<span data-ttu-id="b6094-106">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6094-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="b6094-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6094-107">Properties</span></span>
| <span data-ttu-id="b6094-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6094-108">Property</span></span>     | <span data-ttu-id="b6094-109">类型</span><span class="sxs-lookup"><span data-stu-id="b6094-109">Type</span></span>   |<span data-ttu-id="b6094-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6094-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6094-111">自学</span><span class="sxs-lookup"><span data-stu-id="b6094-111">self</span></span>|<span data-ttu-id="b6094-112">String</span><span class="sxs-lookup"><span data-stu-id="b6094-112">String</span></span>|<span data-ttu-id="b6094-113">可在其中获取有关页面的详细信息的终结点。</span><span class="sxs-lookup"><span data-stu-id="b6094-113">The endpoint where you can get details about the page.</span></span> <span data-ttu-id="b6094-114">只读。</span><span class="sxs-lookup"><span data-stu-id="b6094-114">Read-only.</span></span>|

<!-- uuid: bfb567de-2a2a-4b81-bf47-a55626a0c166
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "page resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
