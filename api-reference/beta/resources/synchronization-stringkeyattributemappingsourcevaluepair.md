---
title: stringKeyAttributeMappingSourceValuePair 资源类型
description: 表示其中的密钥是一个字符串，并且值为 attributeMappingSource 的键 / 值对。
ms.openlocfilehash: 875c593ae652ce763f420d29e5dd4e5e2601bc88
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048527"
---
# <a name="stringkeyattributemappingsourcevaluepair-resource-type"></a><span data-ttu-id="7513f-103">stringKeyAttributeMappingSourceValuePair 资源类型</span><span class="sxs-lookup"><span data-stu-id="7513f-103">stringKeyAttributeMappingSourceValuePair resource type</span></span>

> <span data-ttu-id="7513f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7513f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7513f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7513f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7513f-106">表示其中的密钥是一个字符串，并且值为[attributeMappingSource](synchronization-attributemappingsource.md)的键 / 值对。</span><span class="sxs-lookup"><span data-stu-id="7513f-106">Represents a key-value pair where the key is a string and the value is [attributeMappingSource](synchronization-attributemappingsource.md).</span></span>

## <a name="properties"></a><span data-ttu-id="7513f-107">属性</span><span class="sxs-lookup"><span data-stu-id="7513f-107">Properties</span></span>
| <span data-ttu-id="7513f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7513f-108">Property</span></span>     | <span data-ttu-id="7513f-109">类型</span><span class="sxs-lookup"><span data-stu-id="7513f-109">Type</span></span>   |<span data-ttu-id="7513f-110">说明</span><span class="sxs-lookup"><span data-stu-id="7513f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7513f-111">Key</span><span class="sxs-lookup"><span data-stu-id="7513f-111">key</span></span>|<span data-ttu-id="7513f-112">字符串</span><span class="sxs-lookup"><span data-stu-id="7513f-112">String</span></span>|<span data-ttu-id="7513f-113">参数的名称。</span><span class="sxs-lookup"><span data-stu-id="7513f-113">The name of the parameter.</span></span>|
|<span data-ttu-id="7513f-114">值</span><span class="sxs-lookup"><span data-stu-id="7513f-114">value</span></span>|[<span data-ttu-id="7513f-115">attributeMappingSource</span><span class="sxs-lookup"><span data-stu-id="7513f-115">attributeMappingSource</span></span>](synchronization-attributemappingsource.md)|<span data-ttu-id="7513f-116">参数的值。</span><span class="sxs-lookup"><span data-stu-id="7513f-116">The value of the parameter.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7513f-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7513f-117">JSON representation</span></span>

<span data-ttu-id="7513f-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7513f-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.stringKeyAttributeMappingSourceValuePair"
}-->

```json
{
  "key": "String",
  "value": {"@odata.type": "microsoft.graph.attributeMappingSource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "stringKeyAttributeMappingSourceValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
