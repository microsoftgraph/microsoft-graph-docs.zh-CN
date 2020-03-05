---
title: 网站资源类型
description: 表示一个网站。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: f6d630a2cde87415cb8229f7d320cb32bc6260d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446735"
---
# <a name="website-resource-type"></a><span data-ttu-id="5c650-103">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="5c650-103">website resource type</span></span>

<span data-ttu-id="5c650-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5c650-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5c650-105">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="5c650-105">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="5c650-106">属性</span><span class="sxs-lookup"><span data-stu-id="5c650-106">Properties</span></span>
| <span data-ttu-id="5c650-107">属性</span><span class="sxs-lookup"><span data-stu-id="5c650-107">Property</span></span>     | <span data-ttu-id="5c650-108">类型</span><span class="sxs-lookup"><span data-stu-id="5c650-108">Type</span></span>   |<span data-ttu-id="5c650-109">说明</span><span class="sxs-lookup"><span data-stu-id="5c650-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5c650-110">类型</span><span class="sxs-lookup"><span data-stu-id="5c650-110">type</span></span>|<span data-ttu-id="5c650-111">websiteType</span><span class="sxs-lookup"><span data-stu-id="5c650-111">websiteType</span></span>| <span data-ttu-id="5c650-112">可能的值包括 `other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="5c650-112">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="5c650-113">address</span><span class="sxs-lookup"><span data-stu-id="5c650-113">address</span></span>|<span data-ttu-id="5c650-114">string</span><span class="sxs-lookup"><span data-stu-id="5c650-114">string</span></span>|<span data-ttu-id="5c650-115">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="5c650-115">The URL of the website.</span></span>|
|<span data-ttu-id="5c650-116">displayName</span><span class="sxs-lookup"><span data-stu-id="5c650-116">displayName</span></span>|<span data-ttu-id="5c650-117">string</span><span class="sxs-lookup"><span data-stu-id="5c650-117">string</span></span>|<span data-ttu-id="5c650-118">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5c650-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5c650-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5c650-119">JSON representation</span></span>

<span data-ttu-id="5c650-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c650-120">The following is a JSON representation of the resource.</span></span>

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
