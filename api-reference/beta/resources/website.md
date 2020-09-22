---
title: 网站资源类型
description: 代表网站。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: AAmatino
ms.openlocfilehash: 4c283d77119c0272aaafa964db62bb35ad747a10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973469"
---
# <a name="website-resource-type"></a><span data-ttu-id="73663-103">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="73663-103">website resource type</span></span>

<span data-ttu-id="73663-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73663-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73663-105">代表网站。</span><span class="sxs-lookup"><span data-stu-id="73663-105">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="73663-106">属性</span><span class="sxs-lookup"><span data-stu-id="73663-106">Properties</span></span>
| <span data-ttu-id="73663-107">属性</span><span class="sxs-lookup"><span data-stu-id="73663-107">Property</span></span>     | <span data-ttu-id="73663-108">类型</span><span class="sxs-lookup"><span data-stu-id="73663-108">Type</span></span>   |<span data-ttu-id="73663-109">说明</span><span class="sxs-lookup"><span data-stu-id="73663-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73663-110">type</span><span class="sxs-lookup"><span data-stu-id="73663-110">type</span></span>|<span data-ttu-id="73663-111">String</span><span class="sxs-lookup"><span data-stu-id="73663-111">String</span></span>| <span data-ttu-id="73663-112">可取值为：`other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="73663-112">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="73663-113">address</span><span class="sxs-lookup"><span data-stu-id="73663-113">address</span></span>|<span data-ttu-id="73663-114">string</span><span class="sxs-lookup"><span data-stu-id="73663-114">string</span></span>|<span data-ttu-id="73663-115">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="73663-115">The URL of the website.</span></span>|
|<span data-ttu-id="73663-116">displayName</span><span class="sxs-lookup"><span data-stu-id="73663-116">displayName</span></span>|<span data-ttu-id="73663-117">string</span><span class="sxs-lookup"><span data-stu-id="73663-117">string</span></span>|<span data-ttu-id="73663-118">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="73663-118">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73663-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73663-119">JSON representation</span></span>

<span data-ttu-id="73663-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73663-120">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "webSite resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


