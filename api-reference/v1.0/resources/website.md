---
title: 网站资源类型
description: 表示一个网站。
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: fbdb96a9a19a9edef98d73916dcbd01dd6ba9e66
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015237"
---
# <a name="website-resource-type"></a><span data-ttu-id="6366a-103">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="6366a-103">website resource type</span></span>

<span data-ttu-id="6366a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6366a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6366a-105">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="6366a-105">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="6366a-106">属性</span><span class="sxs-lookup"><span data-stu-id="6366a-106">Properties</span></span>
| <span data-ttu-id="6366a-107">属性</span><span class="sxs-lookup"><span data-stu-id="6366a-107">Property</span></span>     | <span data-ttu-id="6366a-108">类型</span><span class="sxs-lookup"><span data-stu-id="6366a-108">Type</span></span>   |<span data-ttu-id="6366a-109">说明</span><span class="sxs-lookup"><span data-stu-id="6366a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6366a-110">类型</span><span class="sxs-lookup"><span data-stu-id="6366a-110">type</span></span>|<span data-ttu-id="6366a-111">websiteType</span><span class="sxs-lookup"><span data-stu-id="6366a-111">websiteType</span></span>| <span data-ttu-id="6366a-112">可能的值包括 `other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="6366a-112">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="6366a-113">address</span><span class="sxs-lookup"><span data-stu-id="6366a-113">address</span></span>|<span data-ttu-id="6366a-114">string</span><span class="sxs-lookup"><span data-stu-id="6366a-114">string</span></span>|<span data-ttu-id="6366a-115">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="6366a-115">The URL of the website.</span></span>|
|<span data-ttu-id="6366a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="6366a-116">displayName</span></span>|<span data-ttu-id="6366a-117">string</span><span class="sxs-lookup"><span data-stu-id="6366a-117">string</span></span>|<span data-ttu-id="6366a-118">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="6366a-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6366a-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6366a-119">JSON representation</span></span>

<span data-ttu-id="6366a-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6366a-120">The following is a JSON representation of the resource.</span></span>

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

