---
title: 网站资源类型
description: 表示一个网站。
localization_priority: Normal
author: AAmatino
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ec3642ea513ae054e22537c86426df365cd41ba9
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807666"
---
# <a name="website-resource-type"></a><span data-ttu-id="00fa0-103">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="00fa0-103">website resource type</span></span>

<span data-ttu-id="00fa0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00fa0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00fa0-105">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="00fa0-105">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="00fa0-106">属性</span><span class="sxs-lookup"><span data-stu-id="00fa0-106">Properties</span></span>
| <span data-ttu-id="00fa0-107">属性</span><span class="sxs-lookup"><span data-stu-id="00fa0-107">Property</span></span>     | <span data-ttu-id="00fa0-108">类型</span><span class="sxs-lookup"><span data-stu-id="00fa0-108">Type</span></span>   |<span data-ttu-id="00fa0-109">说明</span><span class="sxs-lookup"><span data-stu-id="00fa0-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00fa0-110">类型</span><span class="sxs-lookup"><span data-stu-id="00fa0-110">type</span></span>|<span data-ttu-id="00fa0-111">websiteType</span><span class="sxs-lookup"><span data-stu-id="00fa0-111">websiteType</span></span>| <span data-ttu-id="00fa0-112">可能的值包括 `other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="00fa0-112">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="00fa0-113">address</span><span class="sxs-lookup"><span data-stu-id="00fa0-113">address</span></span>|<span data-ttu-id="00fa0-114">string</span><span class="sxs-lookup"><span data-stu-id="00fa0-114">string</span></span>|<span data-ttu-id="00fa0-115">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="00fa0-115">The URL of the website.</span></span>|
|<span data-ttu-id="00fa0-116">displayName</span><span class="sxs-lookup"><span data-stu-id="00fa0-116">displayName</span></span>|<span data-ttu-id="00fa0-117">string</span><span class="sxs-lookup"><span data-stu-id="00fa0-117">string</span></span>|<span data-ttu-id="00fa0-118">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="00fa0-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00fa0-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00fa0-119">JSON representation</span></span>

<span data-ttu-id="00fa0-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00fa0-120">The following is a JSON representation of the resource.</span></span>

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
