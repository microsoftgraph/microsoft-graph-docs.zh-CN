---
title: stringKeyLongValuePair 资源类型
description: 表示其中的密钥是一个字符串，并且值为 Int64 的键 / 值对。
localization_priority: Normal
ms.openlocfilehash: 21d081dcb488c406bc0971f6b1aeadacfcc8c208
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812234"
---
# <a name="stringkeylongvaluepair-resource-type"></a><span data-ttu-id="c891f-103">stringKeyLongValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="c891f-103">stringKeyLongValuePair resource type</span></span>

> <span data-ttu-id="c891f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c891f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c891f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c891f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c891f-106">表示其中的密钥是一个字符串，并且值为 Int64 的键 / 值对。</span><span class="sxs-lookup"><span data-stu-id="c891f-106">Represents a key-value pair where the key is a string and the value is an Int64.</span></span>

## <a name="properties"></a><span data-ttu-id="c891f-107">属性</span><span class="sxs-lookup"><span data-stu-id="c891f-107">Properties</span></span>
| <span data-ttu-id="c891f-108">属性</span><span class="sxs-lookup"><span data-stu-id="c891f-108">Property</span></span>     | <span data-ttu-id="c891f-109">类型</span><span class="sxs-lookup"><span data-stu-id="c891f-109">Type</span></span>   |<span data-ttu-id="c891f-110">说明</span><span class="sxs-lookup"><span data-stu-id="c891f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c891f-111">Key</span><span class="sxs-lookup"><span data-stu-id="c891f-111">key</span></span>|<span data-ttu-id="c891f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c891f-112">String</span></span>|<span data-ttu-id="c891f-113">键。</span><span class="sxs-lookup"><span data-stu-id="c891f-113">Key.</span></span>|
|<span data-ttu-id="c891f-114">值</span><span class="sxs-lookup"><span data-stu-id="c891f-114">value</span></span>|<span data-ttu-id="c891f-115">Int64</span><span class="sxs-lookup"><span data-stu-id="c891f-115">Int64</span></span>|<span data-ttu-id="c891f-116">值。</span><span class="sxs-lookup"><span data-stu-id="c891f-116">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c891f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c891f-117">JSON representation</span></span>

<span data-ttu-id="c891f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c891f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyLongValuePair"
}-->

```json
{
  "key": "String",
  "value": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyLongValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
