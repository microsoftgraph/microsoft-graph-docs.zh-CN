---
title: 网站资源类型
description: 表示一个网站。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 6a59022426392bbf3a94c6fb82b941131db3c1d8
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033381"
---
# <a name="website-resource-type"></a><span data-ttu-id="bc9b3-103">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="bc9b3-103">website resource type</span></span>

<span data-ttu-id="bc9b3-104">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="bc9b3-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="bc9b3-105">属性</span><span class="sxs-lookup"><span data-stu-id="bc9b3-105">Properties</span></span>
| <span data-ttu-id="bc9b3-106">属性</span><span class="sxs-lookup"><span data-stu-id="bc9b3-106">Property</span></span>     | <span data-ttu-id="bc9b3-107">类型</span><span class="sxs-lookup"><span data-stu-id="bc9b3-107">Type</span></span>   |<span data-ttu-id="bc9b3-108">说明</span><span class="sxs-lookup"><span data-stu-id="bc9b3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bc9b3-109">类型</span><span class="sxs-lookup"><span data-stu-id="bc9b3-109">type</span></span>|<span data-ttu-id="bc9b3-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="bc9b3-110">websiteType</span></span>| <span data-ttu-id="bc9b3-111">可能的值包括 `other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="bc9b3-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="bc9b3-112">address</span><span class="sxs-lookup"><span data-stu-id="bc9b3-112">address</span></span>|<span data-ttu-id="bc9b3-113">string</span><span class="sxs-lookup"><span data-stu-id="bc9b3-113">string</span></span>|<span data-ttu-id="bc9b3-114">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="bc9b3-114">The URL of the website.</span></span>|
|<span data-ttu-id="bc9b3-115">displayName</span><span class="sxs-lookup"><span data-stu-id="bc9b3-115">displayName</span></span>|<span data-ttu-id="bc9b3-116">string</span><span class="sxs-lookup"><span data-stu-id="bc9b3-116">string</span></span>|<span data-ttu-id="bc9b3-117">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="bc9b3-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bc9b3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bc9b3-118">JSON representation</span></span>

<span data-ttu-id="bc9b3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bc9b3-119">The following is a JSON representation of the resource.</span></span>

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
