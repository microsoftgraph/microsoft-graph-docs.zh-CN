---
title: signInFrequencySessionControl 资源类型
description: 用于强制登录频率的会话控制。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ab4eaa619117aa350dcb28be9afd43e1aa2fbc8a
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638776"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="e1d17-103">signInFrequencySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="e1d17-103">signInFrequencySessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1d17-104">用于强制登录频率的会话控制。</span><span class="sxs-lookup"><span data-stu-id="e1d17-104">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="e1d17-105">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="e1d17-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e1d17-106">属性</span><span class="sxs-lookup"><span data-stu-id="e1d17-106">Properties</span></span>

| <span data-ttu-id="e1d17-107">属性</span><span class="sxs-lookup"><span data-stu-id="e1d17-107">Property</span></span>     | <span data-ttu-id="e1d17-108">类型</span><span class="sxs-lookup"><span data-stu-id="e1d17-108">Type</span></span>        | <span data-ttu-id="e1d17-109">说明</span><span class="sxs-lookup"><span data-stu-id="e1d17-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e1d17-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e1d17-110">isEnabled</span></span>     |<span data-ttu-id="e1d17-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="e1d17-111">Boolean</span></span>      | <span data-ttu-id="e1d17-112">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="e1d17-112">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="e1d17-113">type</span><span class="sxs-lookup"><span data-stu-id="e1d17-113">type</span></span>          |<span data-ttu-id="e1d17-114">String</span><span class="sxs-lookup"><span data-stu-id="e1d17-114">String</span></span>       | <span data-ttu-id="e1d17-115">可取值为：`days`、`hours`。</span><span class="sxs-lookup"><span data-stu-id="e1d17-115">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="e1d17-116">值</span><span class="sxs-lookup"><span data-stu-id="e1d17-116">value</span></span>         |<span data-ttu-id="e1d17-117">Int32</span><span class="sxs-lookup"><span data-stu-id="e1d17-117">Int32</span></span>        | <span data-ttu-id="e1d17-118">`days`或`hours`的数目。</span><span class="sxs-lookup"><span data-stu-id="e1d17-118">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1d17-119">关系</span><span class="sxs-lookup"><span data-stu-id="e1d17-119">Relationships</span></span>

<span data-ttu-id="e1d17-120">无。</span><span class="sxs-lookup"><span data-stu-id="e1d17-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e1d17-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e1d17-121">JSON representation</span></span>

<span data-ttu-id="e1d17-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1d17-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInFrequencySessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true,
  "type": "String",
  "value": 1024
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInFrequencySessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->