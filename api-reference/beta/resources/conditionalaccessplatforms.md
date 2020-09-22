---
title: conditionalAccessPlatforms 资源类型
description: 策略作用域中包含和排除的平台。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3b835d5a9ab348a7786211f51f3b4f39c100efaf
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47994265"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="be6b8-103">conditionalAccessPlatforms 资源类型</span><span class="sxs-lookup"><span data-stu-id="be6b8-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="be6b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be6b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be6b8-105">策略作用域中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="be6b8-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="be6b8-106">属性</span><span class="sxs-lookup"><span data-stu-id="be6b8-106">Properties</span></span>

| <span data-ttu-id="be6b8-107">属性</span><span class="sxs-lookup"><span data-stu-id="be6b8-107">Property</span></span>     | <span data-ttu-id="be6b8-108">类型</span><span class="sxs-lookup"><span data-stu-id="be6b8-108">Type</span></span>        | <span data-ttu-id="be6b8-109">说明</span><span class="sxs-lookup"><span data-stu-id="be6b8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="be6b8-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="be6b8-110">includePlatforms</span></span>|<span data-ttu-id="be6b8-111">String collection</span><span class="sxs-lookup"><span data-stu-id="be6b8-111">String collection</span></span>| <span data-ttu-id="be6b8-112">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all`。</span><span class="sxs-lookup"><span data-stu-id="be6b8-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="be6b8-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="be6b8-113">excludePlatforms</span></span>|<span data-ttu-id="be6b8-114">String collection</span><span class="sxs-lookup"><span data-stu-id="be6b8-114">String collection</span></span>| <span data-ttu-id="be6b8-115">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="be6b8-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be6b8-116">关系</span><span class="sxs-lookup"><span data-stu-id="be6b8-116">Relationships</span></span>

<span data-ttu-id="be6b8-117">无。</span><span class="sxs-lookup"><span data-stu-id="be6b8-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be6b8-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be6b8-118">JSON representation</span></span>

<span data-ttu-id="be6b8-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be6b8-119">The following is a JSON representation of the resource.</span></span>

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

