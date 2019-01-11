---
title: metadataEntry 资源类型
description: 给定对象的元数据。
localization_priority: Normal
ms.openlocfilehash: ffdb2dd3b6729320b5991b1158e10d145e339968
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27819479"
---
# <a name="metadataentry-resource-type"></a><span data-ttu-id="a904a-103">metadataEntry 资源类型</span><span class="sxs-lookup"><span data-stu-id="a904a-103">metadataEntry resource type</span></span>

> <span data-ttu-id="a904a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a904a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a904a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a904a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a904a-106">给定对象的元数据。</span><span class="sxs-lookup"><span data-stu-id="a904a-106">Metadata for the given object.</span></span>

## <a name="properties"></a><span data-ttu-id="a904a-107">属性</span><span class="sxs-lookup"><span data-stu-id="a904a-107">Properties</span></span>
| <span data-ttu-id="a904a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a904a-108">Property</span></span>     | <span data-ttu-id="a904a-109">类型</span><span class="sxs-lookup"><span data-stu-id="a904a-109">Type</span></span>   |<span data-ttu-id="a904a-110">说明</span><span class="sxs-lookup"><span data-stu-id="a904a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a904a-111">Key</span><span class="sxs-lookup"><span data-stu-id="a904a-111">key</span></span>|<span data-ttu-id="a904a-112">字符串</span><span class="sxs-lookup"><span data-stu-id="a904a-112">String</span></span>|<span data-ttu-id="a904a-113">元数据属性的名称。</span><span class="sxs-lookup"><span data-stu-id="a904a-113">Name of the metadata property.</span></span>|
|<span data-ttu-id="a904a-114">值</span><span class="sxs-lookup"><span data-stu-id="a904a-114">value</span></span>|<span data-ttu-id="a904a-115">字符串</span><span class="sxs-lookup"><span data-stu-id="a904a-115">String</span></span>|<span data-ttu-id="a904a-116">元数据属性的值。</span><span class="sxs-lookup"><span data-stu-id="a904a-116">Value of the metadata property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a904a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a904a-117">JSON representation</span></span>

<span data-ttu-id="a904a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a904a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.metadataEntry"
}-->

```json
{
  "key": "String",
  "value": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "metadataEntry resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
