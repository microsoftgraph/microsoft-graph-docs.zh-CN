---
title: website 资源类型
description: 表示一个网站。
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851364"
---
# <a name="website-resource-type"></a><span data-ttu-id="ca853-103">website 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca853-103">website resource type</span></span>

<span data-ttu-id="ca853-104">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="ca853-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="ca853-105">属性</span><span class="sxs-lookup"><span data-stu-id="ca853-105">Properties</span></span>
| <span data-ttu-id="ca853-106">属性</span><span class="sxs-lookup"><span data-stu-id="ca853-106">Property</span></span>     | <span data-ttu-id="ca853-107">类型</span><span class="sxs-lookup"><span data-stu-id="ca853-107">Type</span></span>   |<span data-ttu-id="ca853-108">说明</span><span class="sxs-lookup"><span data-stu-id="ca853-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca853-109">type</span><span class="sxs-lookup"><span data-stu-id="ca853-109">type</span></span>|<span data-ttu-id="ca853-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="ca853-110">websiteType</span></span>| <span data-ttu-id="ca853-111">可能的值为： `other`， `home`， `work`， `blog`， `profile`。</span><span class="sxs-lookup"><span data-stu-id="ca853-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="ca853-112">address</span><span class="sxs-lookup"><span data-stu-id="ca853-112">address</span></span>|<span data-ttu-id="ca853-113">string</span><span class="sxs-lookup"><span data-stu-id="ca853-113">string</span></span>|<span data-ttu-id="ca853-114">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="ca853-114">The URL of the website.</span></span>|
|<span data-ttu-id="ca853-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ca853-115">displayName</span></span>|<span data-ttu-id="ca853-116">string</span><span class="sxs-lookup"><span data-stu-id="ca853-116">string</span></span>|<span data-ttu-id="ca853-117">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ca853-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ca853-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca853-118">JSON representation</span></span>

<span data-ttu-id="ca853-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca853-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.website"
}-->

```json
{
  "type": "String",
  "address": "string",
  "displayName": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
