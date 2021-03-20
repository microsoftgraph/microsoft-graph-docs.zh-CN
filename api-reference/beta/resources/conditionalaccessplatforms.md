---
title: conditionalAccessPlatforms 资源类型
description: 策略作用域中包含和排除的平台。
localization_priority: Normal
author: videor
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 71c8b38b59d30ce1e8e1fa1c7668c41a5d2288c2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945702"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="9b299-103">conditionalAccessPlatforms 资源类型</span><span class="sxs-lookup"><span data-stu-id="9b299-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="9b299-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b299-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b299-105">策略作用域中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="9b299-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="9b299-106">属性</span><span class="sxs-lookup"><span data-stu-id="9b299-106">Properties</span></span>

| <span data-ttu-id="9b299-107">属性</span><span class="sxs-lookup"><span data-stu-id="9b299-107">Property</span></span>     | <span data-ttu-id="9b299-108">类型</span><span class="sxs-lookup"><span data-stu-id="9b299-108">Type</span></span>        | <span data-ttu-id="9b299-109">说明</span><span class="sxs-lookup"><span data-stu-id="9b299-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9b299-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="9b299-110">includePlatforms</span></span>|<span data-ttu-id="9b299-111">conditionalAccessDevicePlatform 集合</span><span class="sxs-lookup"><span data-stu-id="9b299-111">conditionalAccessDevicePlatform collection</span></span>| <span data-ttu-id="9b299-112">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9b299-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9b299-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="9b299-113">excludePlatforms</span></span>|<span data-ttu-id="9b299-114">conditionalAccessDevicePlatform 集合</span><span class="sxs-lookup"><span data-stu-id="9b299-114">conditionalAccessDevicePlatform collection</span></span>| <span data-ttu-id="9b299-115">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9b299-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b299-116">关系</span><span class="sxs-lookup"><span data-stu-id="9b299-116">Relationships</span></span>

<span data-ttu-id="9b299-117">无。</span><span class="sxs-lookup"><span data-stu-id="9b299-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b299-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9b299-118">JSON representation</span></span>

<span data-ttu-id="9b299-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9b299-119">The following is a JSON representation of the resource.</span></span>

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

