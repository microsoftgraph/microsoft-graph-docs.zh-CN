---
title: stringKeyStringValuePair 资源类型
description: 表示其中的密钥是一个字符串，值为字符串的键 / 值对。
ms.openlocfilehash: 012625d78c8e07b3d38acba063acb57c751ced32
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048526"
---
# <a name="stringkeystringvaluepair-resource-type"></a><span data-ttu-id="c6d0c-103">stringKeyStringValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6d0c-103">stringKeyStringValuePair resource type</span></span>

> <span data-ttu-id="c6d0c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c6d0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c6d0c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c6d0c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c6d0c-106">表示其中的密钥是一个字符串，值为字符串的键 / 值对。</span><span class="sxs-lookup"><span data-stu-id="c6d0c-106">Represents a key-value pair where the key is a string and the value is a string.</span></span>

## <a name="properties"></a><span data-ttu-id="c6d0c-107">属性</span><span class="sxs-lookup"><span data-stu-id="c6d0c-107">Properties</span></span>
| <span data-ttu-id="c6d0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="c6d0c-108">Property</span></span>     | <span data-ttu-id="c6d0c-109">类型</span><span class="sxs-lookup"><span data-stu-id="c6d0c-109">Type</span></span>   |<span data-ttu-id="c6d0c-110">说明</span><span class="sxs-lookup"><span data-stu-id="c6d0c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6d0c-111">Key</span><span class="sxs-lookup"><span data-stu-id="c6d0c-111">key</span></span>|<span data-ttu-id="c6d0c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="c6d0c-112">String</span></span>|<span data-ttu-id="c6d0c-113">键。</span><span class="sxs-lookup"><span data-stu-id="c6d0c-113">Key.</span></span>|
|<span data-ttu-id="c6d0c-114">值</span><span class="sxs-lookup"><span data-stu-id="c6d0c-114">value</span></span>|<span data-ttu-id="c6d0c-115">String</span><span class="sxs-lookup"><span data-stu-id="c6d0c-115">String</span></span>|<span data-ttu-id="c6d0c-116">值。</span><span class="sxs-lookup"><span data-stu-id="c6d0c-116">Value.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6d0c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6d0c-117">JSON representation</span></span>

<span data-ttu-id="c6d0c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6d0c-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyStringValuePair"
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
  "description": "stringKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->