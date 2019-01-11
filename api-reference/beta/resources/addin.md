---
title: 外接程序资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 6e76b8f7981be5da9a2ac8437ff21d4a59dbbe73
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27884212"
---
# <a name="addin-resource-type"></a><span data-ttu-id="3a69c-103">外接程序资源类型</span><span class="sxs-lookup"><span data-stu-id="3a69c-103">addIn resource type</span></span>

> <span data-ttu-id="3a69c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3a69c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a69c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3a69c-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3a69c-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3a69c-106">JSON representation</span></span>

<span data-ttu-id="3a69c-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a69c-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.addIn"
}-->

```json
{
  "id": "guid",
  "properties": [{"@odata.type": "microsoft.graph.keyvalue"}],
  "type": "string"
}

```
## <a name="properties"></a><span data-ttu-id="3a69c-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a69c-108">Properties</span></span>
| <span data-ttu-id="3a69c-109">属性</span><span class="sxs-lookup"><span data-stu-id="3a69c-109">Property</span></span>     | <span data-ttu-id="3a69c-110">类型</span><span class="sxs-lookup"><span data-stu-id="3a69c-110">Type</span></span>   |<span data-ttu-id="3a69c-111">说明</span><span class="sxs-lookup"><span data-stu-id="3a69c-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3a69c-112">ID</span><span class="sxs-lookup"><span data-stu-id="3a69c-112">id</span></span>|<span data-ttu-id="3a69c-113">guid</span><span class="sxs-lookup"><span data-stu-id="3a69c-113">guid</span></span>||
|<span data-ttu-id="3a69c-114">properties</span><span class="sxs-lookup"><span data-stu-id="3a69c-114">properties</span></span>|<span data-ttu-id="3a69c-115">[keyValue](keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="3a69c-115">[keyValue](keyvalue.md) collection</span></span>||
|<span data-ttu-id="3a69c-116">type</span><span class="sxs-lookup"><span data-stu-id="3a69c-116">type</span></span>|<span data-ttu-id="3a69c-117">字符串</span><span class="sxs-lookup"><span data-stu-id="3a69c-117">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "addIn resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
