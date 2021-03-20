---
title: signInFrequencySessionControl 资源类型
description: 强制执行登录频率的会话控制。
localization_priority: Normal
author: dkershaw10
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 1f224c1e9ba72e114fd9c9bcacdd74670713837d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945625"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="c2bf6-103">signInFrequencySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="c2bf6-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="c2bf6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2bf6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2bf6-105">强制执行登录频率的会话控制。</span><span class="sxs-lookup"><span data-stu-id="c2bf6-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="c2bf6-106">继承自 [条件访问会话控件](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="c2bf6-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="c2bf6-107">属性</span><span class="sxs-lookup"><span data-stu-id="c2bf6-107">Properties</span></span>

| <span data-ttu-id="c2bf6-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2bf6-108">Property</span></span>     | <span data-ttu-id="c2bf6-109">类型</span><span class="sxs-lookup"><span data-stu-id="c2bf6-109">Type</span></span>        | <span data-ttu-id="c2bf6-110">说明</span><span class="sxs-lookup"><span data-stu-id="c2bf6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="c2bf6-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="c2bf6-111">isEnabled</span></span>     |<span data-ttu-id="c2bf6-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="c2bf6-112">Boolean</span></span>      | <span data-ttu-id="c2bf6-113">指定是否启用会话控件。</span><span class="sxs-lookup"><span data-stu-id="c2bf6-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="c2bf6-114">type</span><span class="sxs-lookup"><span data-stu-id="c2bf6-114">type</span></span>          |<span data-ttu-id="c2bf6-115">signinFrequencyType</span><span class="sxs-lookup"><span data-stu-id="c2bf6-115">signinFrequencyType</span></span>       | <span data-ttu-id="c2bf6-116">可取值为：`days`、`hours`。</span><span class="sxs-lookup"><span data-stu-id="c2bf6-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="c2bf6-117">值</span><span class="sxs-lookup"><span data-stu-id="c2bf6-117">value</span></span>         |<span data-ttu-id="c2bf6-118">Int32</span><span class="sxs-lookup"><span data-stu-id="c2bf6-118">Int32</span></span>        | <span data-ttu-id="c2bf6-119">或 `days` 的编号 `hours` 。</span><span class="sxs-lookup"><span data-stu-id="c2bf6-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2bf6-120">关系</span><span class="sxs-lookup"><span data-stu-id="c2bf6-120">Relationships</span></span>

<span data-ttu-id="c2bf6-121">无。</span><span class="sxs-lookup"><span data-stu-id="c2bf6-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c2bf6-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c2bf6-122">JSON representation</span></span>

<span data-ttu-id="c2bf6-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2bf6-123">The following is a JSON representation of the resource.</span></span>

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


