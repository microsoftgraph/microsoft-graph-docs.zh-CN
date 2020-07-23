---
title: conditionalAccessPlatforms 资源类型
description: 策略作用域中包含和排除的平台。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 88d40fa1557102bc04ef9a46bba93a50097d66cd
ms.sourcegitcommit: fec7d5002dbeb8d58587c89f1b678d4a54645422
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/23/2020
ms.locfileid: "45384462"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="1a146-103">conditionalAccessPlatforms 资源类型</span><span class="sxs-lookup"><span data-stu-id="1a146-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="1a146-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a146-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1a146-105">策略作用域中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="1a146-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="1a146-106">属性</span><span class="sxs-lookup"><span data-stu-id="1a146-106">Properties</span></span>

| <span data-ttu-id="1a146-107">属性</span><span class="sxs-lookup"><span data-stu-id="1a146-107">Property</span></span>     | <span data-ttu-id="1a146-108">类型</span><span class="sxs-lookup"><span data-stu-id="1a146-108">Type</span></span>        | <span data-ttu-id="1a146-109">说明</span><span class="sxs-lookup"><span data-stu-id="1a146-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="1a146-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="1a146-110">includePlatforms</span></span>|<span data-ttu-id="1a146-111">String collection</span><span class="sxs-lookup"><span data-stu-id="1a146-111">String collection</span></span>| <span data-ttu-id="1a146-112">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all` 或 `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1a146-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="1a146-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="1a146-113">excludePlatforms</span></span>|<span data-ttu-id="1a146-114">String collection</span><span class="sxs-lookup"><span data-stu-id="1a146-114">String collection</span></span>| <span data-ttu-id="1a146-115">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="1a146-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1a146-116">关系</span><span class="sxs-lookup"><span data-stu-id="1a146-116">Relationships</span></span>

<span data-ttu-id="1a146-117">无。</span><span class="sxs-lookup"><span data-stu-id="1a146-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1a146-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1a146-118">JSON representation</span></span>

<span data-ttu-id="1a146-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a146-119">The following is a JSON representation of the resource.</span></span>

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
