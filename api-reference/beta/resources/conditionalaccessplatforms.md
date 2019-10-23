---
title: conditionalAccessPlatforms 资源类型
description: 策略作用域中包含和排除的平台。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9de4d82cac659e73c1b4a898d6de9017c8e3e830
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638503"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="5aa7a-103">conditionalAccessPlatforms 资源类型</span><span class="sxs-lookup"><span data-stu-id="5aa7a-103">conditionalAccessPlatforms resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5aa7a-104">策略作用域中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="5aa7a-104">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="5aa7a-105">属性</span><span class="sxs-lookup"><span data-stu-id="5aa7a-105">Properties</span></span>

| <span data-ttu-id="5aa7a-106">属性</span><span class="sxs-lookup"><span data-stu-id="5aa7a-106">Property</span></span>     | <span data-ttu-id="5aa7a-107">类型</span><span class="sxs-lookup"><span data-stu-id="5aa7a-107">Type</span></span>        | <span data-ttu-id="5aa7a-108">说明</span><span class="sxs-lookup"><span data-stu-id="5aa7a-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5aa7a-109">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="5aa7a-109">includePlatforms</span></span>|<span data-ttu-id="5aa7a-110">String collection</span><span class="sxs-lookup"><span data-stu-id="5aa7a-110">String collection</span></span>| <span data-ttu-id="5aa7a-111">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all`。</span><span class="sxs-lookup"><span data-stu-id="5aa7a-111">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="5aa7a-112">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="5aa7a-112">excludePlatforms</span></span>|<span data-ttu-id="5aa7a-113">String collection</span><span class="sxs-lookup"><span data-stu-id="5aa7a-113">String collection</span></span>| <span data-ttu-id="5aa7a-114">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="5aa7a-114">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5aa7a-115">关系</span><span class="sxs-lookup"><span data-stu-id="5aa7a-115">Relationships</span></span>

<span data-ttu-id="5aa7a-116">无。</span><span class="sxs-lookup"><span data-stu-id="5aa7a-116">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5aa7a-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5aa7a-117">JSON representation</span></span>

<span data-ttu-id="5aa7a-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5aa7a-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessPlatforms",
  "baseType": null
}-->

```json
{
  "includePlatforms": ["String"],
  "excludePlatforms": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conditionalAccessPlatforms resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->