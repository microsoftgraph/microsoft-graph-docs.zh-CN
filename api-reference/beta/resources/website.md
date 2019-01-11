---
title: website 资源类型
description: 代表一个网站。
localization_priority: Normal
ms.openlocfilehash: 15cc926ad1c251fd169ccdb0b1374df7f434a645
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826115"
---
# <a name="website-resource-type"></a><span data-ttu-id="5f893-103">website 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f893-103">website resource type</span></span>

> <span data-ttu-id="5f893-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5f893-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5f893-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5f893-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5f893-106">代表一个网站。</span><span class="sxs-lookup"><span data-stu-id="5f893-106">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="5f893-107">属性</span><span class="sxs-lookup"><span data-stu-id="5f893-107">Properties</span></span>
| <span data-ttu-id="5f893-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f893-108">Property</span></span>     | <span data-ttu-id="5f893-109">类型</span><span class="sxs-lookup"><span data-stu-id="5f893-109">Type</span></span>   |<span data-ttu-id="5f893-110">说明</span><span class="sxs-lookup"><span data-stu-id="5f893-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f893-111">type</span><span class="sxs-lookup"><span data-stu-id="5f893-111">type</span></span>|<span data-ttu-id="5f893-112">String</span><span class="sxs-lookup"><span data-stu-id="5f893-112">String</span></span>| <span data-ttu-id="5f893-113">可能的值是：`other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="5f893-113">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="5f893-114">address</span><span class="sxs-lookup"><span data-stu-id="5f893-114">address</span></span>|<span data-ttu-id="5f893-115">string</span><span class="sxs-lookup"><span data-stu-id="5f893-115">string</span></span>|<span data-ttu-id="5f893-116">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="5f893-116">The URL of the website.</span></span>|
|<span data-ttu-id="5f893-117">displayName</span><span class="sxs-lookup"><span data-stu-id="5f893-117">displayName</span></span>|<span data-ttu-id="5f893-118">string</span><span class="sxs-lookup"><span data-stu-id="5f893-118">string</span></span>|<span data-ttu-id="5f893-119">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5f893-119">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f893-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f893-120">JSON representation</span></span>

<span data-ttu-id="5f893-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f893-121">Here is a JSON representation of the resource.</span></span>

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
