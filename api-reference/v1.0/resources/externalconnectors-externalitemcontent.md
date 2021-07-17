---
title: externalItemContent 资源类型
description: 通过连接建立索引的项目Microsoft 搜索内容。
author: mecampos
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 4dd853ca32c918988f2f99e1f1238d9ac937da02
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467253"
---
# <a name="externalitemcontent-resource-type"></a><span data-ttu-id="74811-103">externalItemContent 资源类型</span><span class="sxs-lookup"><span data-stu-id="74811-103">externalItemContent resource type</span></span>

<span data-ttu-id="74811-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="74811-104">Namespace: microsoft.graph.externalConnectors</span></span>

<span data-ttu-id="74811-105">通过连接[建立索引的 externalItem](externalconnectors-externalitem.md) Microsoft 搜索[内容](externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="74811-105">The content of an [externalItem](externalconnectors-externalitem.md) indexed via a Microsoft Search [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="properties"></a><span data-ttu-id="74811-106">属性</span><span class="sxs-lookup"><span data-stu-id="74811-106">Properties</span></span>
|<span data-ttu-id="74811-107">属性</span><span class="sxs-lookup"><span data-stu-id="74811-107">Property</span></span>|<span data-ttu-id="74811-108">类型</span><span class="sxs-lookup"><span data-stu-id="74811-108">Type</span></span>|<span data-ttu-id="74811-109">说明</span><span class="sxs-lookup"><span data-stu-id="74811-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74811-110">类型</span><span class="sxs-lookup"><span data-stu-id="74811-110">type</span></span>|<span data-ttu-id="74811-111">microsoft.graph.externalConnectors.externalItemContentType</span><span class="sxs-lookup"><span data-stu-id="74811-111">microsoft.graph.externalConnectors.externalItemContentType</span></span>|<span data-ttu-id="74811-112">value 属性中的内容类型。</span><span class="sxs-lookup"><span data-stu-id="74811-112">The type of content in the value property.</span></span> <span data-ttu-id="74811-113">可取值为：`text`、`html`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="74811-113">Possible values are: `text`, `html`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="74811-114">value</span><span class="sxs-lookup"><span data-stu-id="74811-114">value</span></span>|<span data-ttu-id="74811-115">String</span><span class="sxs-lookup"><span data-stu-id="74811-115">String</span></span>|<span data-ttu-id="74811-116">externalItem 的内容。</span><span class="sxs-lookup"><span data-stu-id="74811-116">The content for the externalItem.</span></span> <span data-ttu-id="74811-117">必填。</span><span class="sxs-lookup"><span data-stu-id="74811-117">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="74811-118">关系</span><span class="sxs-lookup"><span data-stu-id="74811-118">Relationships</span></span>
<span data-ttu-id="74811-119">无。</span><span class="sxs-lookup"><span data-stu-id="74811-119">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="74811-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74811-120">JSON representation</span></span>
<span data-ttu-id="74811-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74811-121">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.externalConnectors.externalItemContent"
}
-->
``` json
{
  "value": "String",
  "type": "String"
}
```

