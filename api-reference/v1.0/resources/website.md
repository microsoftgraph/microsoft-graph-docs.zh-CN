---
title: website 资源类型
description: 表示一个网站。
ms.openlocfilehash: 14934aae418581f4c75c880be67bf51fd0bc293c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008162"
---
# <a name="website-resource-type"></a><span data-ttu-id="a5ea7-103">website 资源类型</span><span class="sxs-lookup"><span data-stu-id="a5ea7-103">website resource type</span></span>

<span data-ttu-id="a5ea7-104">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="a5ea7-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="a5ea7-105">属性</span><span class="sxs-lookup"><span data-stu-id="a5ea7-105">Properties</span></span>
| <span data-ttu-id="a5ea7-106">属性</span><span class="sxs-lookup"><span data-stu-id="a5ea7-106">Property</span></span>     | <span data-ttu-id="a5ea7-107">类型</span><span class="sxs-lookup"><span data-stu-id="a5ea7-107">Type</span></span>   |<span data-ttu-id="a5ea7-108">说明</span><span class="sxs-lookup"><span data-stu-id="a5ea7-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a5ea7-109">type</span><span class="sxs-lookup"><span data-stu-id="a5ea7-109">type</span></span>|<span data-ttu-id="a5ea7-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="a5ea7-110">websiteType</span></span>| <span data-ttu-id="a5ea7-111">可能的值为： `other`， `home`， `work`， `blog`， `profile`。</span><span class="sxs-lookup"><span data-stu-id="a5ea7-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="a5ea7-112">address</span><span class="sxs-lookup"><span data-stu-id="a5ea7-112">address</span></span>|<span data-ttu-id="a5ea7-113">string</span><span class="sxs-lookup"><span data-stu-id="a5ea7-113">string</span></span>|<span data-ttu-id="a5ea7-114">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="a5ea7-114">The URL of the website.</span></span>|
|<span data-ttu-id="a5ea7-115">displayName</span><span class="sxs-lookup"><span data-stu-id="a5ea7-115">displayName</span></span>|<span data-ttu-id="a5ea7-116">string</span><span class="sxs-lookup"><span data-stu-id="a5ea7-116">string</span></span>|<span data-ttu-id="a5ea7-117">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="a5ea7-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a5ea7-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a5ea7-118">JSON representation</span></span>

<span data-ttu-id="a5ea7-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a5ea7-119">The following is a JSON representation of the resource.</span></span>

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
