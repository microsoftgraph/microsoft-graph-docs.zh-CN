---
title: keyValue 资源类型
description: 下面是资源的 JSON 表示形式。
localization_priority: Normal
ms.openlocfilehash: 6f81d5aaef6e045abec02ebb5a55c4eb19db2665
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833843"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="60f7e-103">keyValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="60f7e-103">keyValue resource type</span></span>

> <span data-ttu-id="60f7e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="60f7e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="60f7e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="60f7e-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="json-representation"></a><span data-ttu-id="60f7e-106">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="60f7e-106">JSON representation</span></span>

<span data-ttu-id="60f7e-107">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60f7e-107">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyvalue"
}-->

```json
{
  "key": "string",
  "value": "string"
}

```
## <a name="properties"></a><span data-ttu-id="60f7e-108">属性</span><span class="sxs-lookup"><span data-stu-id="60f7e-108">Properties</span></span>
| <span data-ttu-id="60f7e-109">属性</span><span class="sxs-lookup"><span data-stu-id="60f7e-109">Property</span></span>     | <span data-ttu-id="60f7e-110">类型</span><span class="sxs-lookup"><span data-stu-id="60f7e-110">Type</span></span>   |<span data-ttu-id="60f7e-111">说明</span><span class="sxs-lookup"><span data-stu-id="60f7e-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60f7e-112">Key</span><span class="sxs-lookup"><span data-stu-id="60f7e-112">key</span></span>|<span data-ttu-id="60f7e-113">string</span><span class="sxs-lookup"><span data-stu-id="60f7e-113">string</span></span>||
|<span data-ttu-id="60f7e-114">值</span><span class="sxs-lookup"><span data-stu-id="60f7e-114">value</span></span>|<span data-ttu-id="60f7e-115">字符串</span><span class="sxs-lookup"><span data-stu-id="60f7e-115">string</span></span>||

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyValue resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
