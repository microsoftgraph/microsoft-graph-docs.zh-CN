---
title: visualProperties 资源类型
description: '表示面向用户的视觉通知的可视内容（即标题和正文）。  '
localization_priority: Normal
author: merzink
ms.prod: notifications
doc_type: resourcePageType
ms.openlocfilehash: f03563549cc1b2f42a274032dab7b310511c70c7
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939178"
---
# <a name="visualproperties-resource-type"></a><span data-ttu-id="328e5-103">visualProperties 资源类型</span><span class="sxs-lookup"><span data-stu-id="328e5-103">visualProperties resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="328e5-104">表示面向用户的视觉通知的可视内容（即标题和正文）。</span><span class="sxs-lookup"><span data-stu-id="328e5-104">Represents the visual content, namely title and body, of a visual notification targeted to a user.</span></span> 

## <a name="properties"></a><span data-ttu-id="328e5-105">属性</span><span class="sxs-lookup"><span data-stu-id="328e5-105">Properties</span></span>

| <span data-ttu-id="328e5-106">属性</span><span class="sxs-lookup"><span data-stu-id="328e5-106">Property</span></span>     | <span data-ttu-id="328e5-107">类型</span><span class="sxs-lookup"><span data-stu-id="328e5-107">Type</span></span>        | <span data-ttu-id="328e5-108">说明</span><span class="sxs-lookup"><span data-stu-id="328e5-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="328e5-109">title</span><span class="sxs-lookup"><span data-stu-id="328e5-109">title</span></span>|<span data-ttu-id="328e5-110">String</span><span class="sxs-lookup"><span data-stu-id="328e5-110">String</span></span>|<span data-ttu-id="328e5-111">可视用户通知的标题。</span><span class="sxs-lookup"><span data-stu-id="328e5-111">The title of a visual user notification.</span></span> <span data-ttu-id="328e5-112">此字段对于 visual 通知负载来说是必需的。</span><span class="sxs-lookup"><span data-stu-id="328e5-112">This field is required for visual notification payloads.</span></span> |
|<span data-ttu-id="328e5-113">body</span><span class="sxs-lookup"><span data-stu-id="328e5-113">body</span></span>|<span data-ttu-id="328e5-114">字符串</span><span class="sxs-lookup"><span data-stu-id="328e5-114">String</span></span>|<span data-ttu-id="328e5-115">可视化用户通知的正文。</span><span class="sxs-lookup"><span data-stu-id="328e5-115">The body of a visual user notification.</span></span> <span data-ttu-id="328e5-116">正文是可选的。</span><span class="sxs-lookup"><span data-stu-id="328e5-116">Body is optional.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="328e5-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="328e5-117">JSON representation</span></span>

<span data-ttu-id="328e5-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="328e5-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.visualProperties",
  "baseType": null
}-->

```json
{
  "title": "String",
  "body": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "visualProperties resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->