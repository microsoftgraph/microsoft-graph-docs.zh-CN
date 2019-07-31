---
title: 网站资源类型
description: 代表网站。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0f822c38c57d5e47d39a40b3285773e0e36fd2ee
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964130"
---
# <a name="website-resource-type"></a><span data-ttu-id="0055f-103">网站资源类型</span><span class="sxs-lookup"><span data-stu-id="0055f-103">website resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0055f-104">代表网站。</span><span class="sxs-lookup"><span data-stu-id="0055f-104">Represents a web site.</span></span>


## <a name="properties"></a><span data-ttu-id="0055f-105">属性</span><span class="sxs-lookup"><span data-stu-id="0055f-105">Properties</span></span>
| <span data-ttu-id="0055f-106">属性</span><span class="sxs-lookup"><span data-stu-id="0055f-106">Property</span></span>     | <span data-ttu-id="0055f-107">类型</span><span class="sxs-lookup"><span data-stu-id="0055f-107">Type</span></span>   |<span data-ttu-id="0055f-108">说明</span><span class="sxs-lookup"><span data-stu-id="0055f-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0055f-109">type</span><span class="sxs-lookup"><span data-stu-id="0055f-109">type</span></span>|<span data-ttu-id="0055f-110">String</span><span class="sxs-lookup"><span data-stu-id="0055f-110">String</span></span>| <span data-ttu-id="0055f-111">可取值为：`other`、`home`、`work`、`blog`、`profile`。</span><span class="sxs-lookup"><span data-stu-id="0055f-111">Possible values are: `other`, `home`, `work`, `blog`, `profile`.</span></span>|
|<span data-ttu-id="0055f-112">address</span><span class="sxs-lookup"><span data-stu-id="0055f-112">address</span></span>|<span data-ttu-id="0055f-113">string</span><span class="sxs-lookup"><span data-stu-id="0055f-113">string</span></span>|<span data-ttu-id="0055f-114">网站的 URL。</span><span class="sxs-lookup"><span data-stu-id="0055f-114">The URL of the website.</span></span>|
|<span data-ttu-id="0055f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0055f-115">displayName</span></span>|<span data-ttu-id="0055f-116">string</span><span class="sxs-lookup"><span data-stu-id="0055f-116">string</span></span>|<span data-ttu-id="0055f-117">网站的显示名称。</span><span class="sxs-lookup"><span data-stu-id="0055f-117">The display name of the web site.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0055f-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0055f-118">JSON representation</span></span>

<span data-ttu-id="0055f-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0055f-119">Here is a JSON representation of the resource.</span></span>

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
