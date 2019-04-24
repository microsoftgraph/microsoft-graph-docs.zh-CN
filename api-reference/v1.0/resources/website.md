---
title: 网站资源类型
description: 表示一个网站。
localization_priority: Normal
ms.openlocfilehash: 1ffbee8a67527aac97bb4f60b7f8b1637ba1ebe5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457023"
---
# <a name="website-resource-type"></a><span data-ttu-id="abb0b-103">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="abb0b-103">website resource type</span></span>

<span data-ttu-id="abb0b-104">表示一个网站。</span><span class="sxs-lookup"><span data-stu-id="abb0b-104">Represents a website.</span></span>


## <a name="properties"></a><span data-ttu-id="abb0b-105">属性</span><span class="sxs-lookup"><span data-stu-id="abb0b-105">Properties</span></span>
| <span data-ttu-id="abb0b-106">属性</span><span class="sxs-lookup"><span data-stu-id="abb0b-106">Property</span></span>     | <span data-ttu-id="abb0b-107">类型</span><span class="sxs-lookup"><span data-stu-id="abb0b-107">Type</span></span>   |<span data-ttu-id="abb0b-108">描述</span><span class="sxs-lookup"><span data-stu-id="abb0b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="abb0b-109">类型</span><span class="sxs-lookup"><span data-stu-id="abb0b-109">type</span></span>|<span data-ttu-id="abb0b-110">websiteType</span><span class="sxs-lookup"><span data-stu-id="abb0b-110">websiteType</span></span>| <span data-ttu-id="abb0b-111">可能的值包括 `other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="abb0b-111">The possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="abb0b-112">address</span><span class="sxs-lookup"><span data-stu-id="abb0b-112">address</span></span>|<span data-ttu-id="abb0b-113">string</span><span class="sxs-lookup"><span data-stu-id="abb0b-113">string</span></span>|<span data-ttu-id="abb0b-114">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="abb0b-114">The URL of the website.</span></span>|
|<span data-ttu-id="abb0b-115">displayName</span><span class="sxs-lookup"><span data-stu-id="abb0b-115">displayName</span></span>|<span data-ttu-id="abb0b-116">string</span><span class="sxs-lookup"><span data-stu-id="abb0b-116">string</span></span>|<span data-ttu-id="abb0b-117">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="abb0b-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="abb0b-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="abb0b-118">JSON representation</span></span>

<span data-ttu-id="abb0b-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="abb0b-119">The following is a JSON representation of the resource.</span></span>

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
