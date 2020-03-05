---
title: conditionalAccessPlatforms 资源类型
description: 策略作用域中包含和排除的平台。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 2612b352f512d1177bc9137603b6ecda1ad96f66
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507532"
---
# <a name="conditionalaccessplatforms-resource-type"></a><span data-ttu-id="5e2f2-103">conditionalAccessPlatforms 资源类型</span><span class="sxs-lookup"><span data-stu-id="5e2f2-103">conditionalAccessPlatforms resource type</span></span>

<span data-ttu-id="5e2f2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5e2f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5e2f2-105">策略作用域中包含和排除的平台。</span><span class="sxs-lookup"><span data-stu-id="5e2f2-105">Platforms included in and excluded from the policy scope.</span></span>

## <a name="properties"></a><span data-ttu-id="5e2f2-106">属性</span><span class="sxs-lookup"><span data-stu-id="5e2f2-106">Properties</span></span>

| <span data-ttu-id="5e2f2-107">属性</span><span class="sxs-lookup"><span data-stu-id="5e2f2-107">Property</span></span>     | <span data-ttu-id="5e2f2-108">类型</span><span class="sxs-lookup"><span data-stu-id="5e2f2-108">Type</span></span>        | <span data-ttu-id="5e2f2-109">说明</span><span class="sxs-lookup"><span data-stu-id="5e2f2-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5e2f2-110">includePlatforms</span><span class="sxs-lookup"><span data-stu-id="5e2f2-110">includePlatforms</span></span>|<span data-ttu-id="5e2f2-111">String 集合</span><span class="sxs-lookup"><span data-stu-id="5e2f2-111">String collection</span></span>| <span data-ttu-id="5e2f2-112">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`、`all`。</span><span class="sxs-lookup"><span data-stu-id="5e2f2-112">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`, `all`.</span></span>|
|<span data-ttu-id="5e2f2-113">excludePlatforms</span><span class="sxs-lookup"><span data-stu-id="5e2f2-113">excludePlatforms</span></span>|<span data-ttu-id="5e2f2-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="5e2f2-114">String collection</span></span>| <span data-ttu-id="5e2f2-115">可取值为：`android`、`iOS`、`windows`、`windowsPhone`、`macOS`。</span><span class="sxs-lookup"><span data-stu-id="5e2f2-115">Possible values are: `android`, `iOS`, `windows`, `windowsPhone`, `macOS`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5e2f2-116">关系</span><span class="sxs-lookup"><span data-stu-id="5e2f2-116">Relationships</span></span>

<span data-ttu-id="5e2f2-117">无。</span><span class="sxs-lookup"><span data-stu-id="5e2f2-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5e2f2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5e2f2-118">JSON representation</span></span>

<span data-ttu-id="5e2f2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e2f2-119">The following is a JSON representation of the resource.</span></span>

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