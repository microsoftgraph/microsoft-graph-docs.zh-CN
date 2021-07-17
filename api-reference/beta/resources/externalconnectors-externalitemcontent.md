---
title: externalItemContent 资源类型
description: 通过连接建立索引的项目Microsoft 搜索内容。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d895d0056da71ea065dbc62d08c9deda054a6f29
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467664"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="fdf64-103">externalItemContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="fdf64-103">externalItemContent resource type</span></span>

<span data-ttu-id="fdf64-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="fdf64-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fdf64-105">通过连接[建立索引的 externalItem](externalconnectors-externalitem.md) Microsoft 搜索[内容](externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="fdf64-105">The content of an [externalItem](externalconnectors-externalitem.md) indexed via a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="fdf64-106">属性</span><span class="sxs-lookup"><span data-stu-id="fdf64-106">Properties</span></span>

| <span data-ttu-id="fdf64-107">属性</span><span class="sxs-lookup"><span data-stu-id="fdf64-107">Property</span></span> | <span data-ttu-id="fdf64-108">类型</span><span class="sxs-lookup"><span data-stu-id="fdf64-108">Type</span></span>   | <span data-ttu-id="fdf64-109">说明</span><span class="sxs-lookup"><span data-stu-id="fdf64-109">Description</span></span>                                                                                 |
|:---------|:-------|:--------------------------------------------------------------------------------------------|
| <span data-ttu-id="fdf64-110">值</span><span class="sxs-lookup"><span data-stu-id="fdf64-110">value</span></span>    | <span data-ttu-id="fdf64-111">String</span><span class="sxs-lookup"><span data-stu-id="fdf64-111">String</span></span> | <span data-ttu-id="fdf64-112">externalItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="fdf64-112">The content for the externalItem.</span></span> <span data-ttu-id="fdf64-113">此为必需属性。</span><span class="sxs-lookup"><span data-stu-id="fdf64-113">Required.</span></span>                                                 |
| <span data-ttu-id="fdf64-114">type</span><span class="sxs-lookup"><span data-stu-id="fdf64-114">type</span></span>     | <span data-ttu-id="fdf64-115">String</span><span class="sxs-lookup"><span data-stu-id="fdf64-115">String</span></span> | <span data-ttu-id="fdf64-116">value 属性中的内容类型。</span><span class="sxs-lookup"><span data-stu-id="fdf64-116">The type of content in the value property.</span></span> <span data-ttu-id="fdf64-117">可能的值为 `text` 和 `html`。</span><span class="sxs-lookup"><span data-stu-id="fdf64-117">Possible values are `text` and `html`.</span></span> <span data-ttu-id="fdf64-118">必填。</span><span class="sxs-lookup"><span data-stu-id="fdf64-118">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="fdf64-119">关系</span><span class="sxs-lookup"><span data-stu-id="fdf64-119">Relationships</span></span>

<span data-ttu-id="fdf64-120">无</span><span class="sxs-lookup"><span data-stu-id="fdf64-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fdf64-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fdf64-121">JSON representation</span></span>

<span data-ttu-id="fdf64-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdf64-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}-->

```json
{
  "value": "String",
  "type": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItemContent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->