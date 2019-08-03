---
title: educationMakeCodeResource 资源类型
description: 一个 MakeCode 资源
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e983f217af71b6e27f750599ee2f8db295da5fec
ms.sourcegitcommit: 129e58f83fc566f9d9f36e26b0c0b8cdf81d27d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/03/2019
ms.locfileid: "36173368"
---
# <a name="educationmakecoderesource-resource-type"></a><span data-ttu-id="97420-103">educationMakeCodeResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="97420-103">educationMakeCodeResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="97420-104">一个代表[MakeCode](https://www.microsoft.com/en-us/makecode)项目的资源。</span><span class="sxs-lookup"><span data-stu-id="97420-104">A resource representing a [MakeCode](https://www.microsoft.com/en-us/makecode) project.</span></span>

## <a name="properties"></a><span data-ttu-id="97420-105">属性</span><span class="sxs-lookup"><span data-stu-id="97420-105">Properties</span></span>

| <span data-ttu-id="97420-106">属性</span><span class="sxs-lookup"><span data-stu-id="97420-106">Property</span></span>     | <span data-ttu-id="97420-107">类型</span><span class="sxs-lookup"><span data-stu-id="97420-107">Type</span></span>        | <span data-ttu-id="97420-108">说明</span><span class="sxs-lookup"><span data-stu-id="97420-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="97420-109">mkcd</span><span class="sxs-lookup"><span data-stu-id="97420-109">mkcd</span></span>|<span data-ttu-id="97420-110">String</span><span class="sxs-lookup"><span data-stu-id="97420-110">String</span></span>|<span data-ttu-id="97420-111">MakeCode 项目的 ID</span><span class="sxs-lookup"><span data-stu-id="97420-111">ID of the MakeCode project</span></span>|
|<span data-ttu-id="97420-112">url</span><span class="sxs-lookup"><span data-stu-id="97420-112">url</span></span>|<span data-ttu-id="97420-113">String</span><span class="sxs-lookup"><span data-stu-id="97420-113">String</span></span>|<span data-ttu-id="97420-114">MakeCode 资源类型的主机 (例如, arcade、microbit)</span><span class="sxs-lookup"><span data-stu-id="97420-114">Host for the type of MakeCode resource (for example, arcade, microbit)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="97420-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="97420-115">JSON representation</span></span>

<span data-ttu-id="97420-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="97420-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationMakeCodeResource",
  "baseType": "microsoft.graph.educationResource"
}-->

```json
{
  "mkcd": "String",
  "url": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationMakeCodeResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->