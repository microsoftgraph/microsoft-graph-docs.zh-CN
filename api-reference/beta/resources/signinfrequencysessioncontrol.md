---
title: signInFrequencySessionControl 资源类型
description: 用于强制登录频率的会话控制。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e13a5d46b6dfcd24b24f93e9e9870fbe89f2ee84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42520588"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="b6539-103">signInFrequencySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6539-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="b6539-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="b6539-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6539-105">用于强制登录频率的会话控制。</span><span class="sxs-lookup"><span data-stu-id="b6539-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="b6539-106">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="b6539-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b6539-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6539-107">Properties</span></span>

| <span data-ttu-id="b6539-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6539-108">Property</span></span>     | <span data-ttu-id="b6539-109">类型</span><span class="sxs-lookup"><span data-stu-id="b6539-109">Type</span></span>        | <span data-ttu-id="b6539-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6539-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b6539-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="b6539-111">isEnabled</span></span>     |<span data-ttu-id="b6539-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="b6539-112">Boolean</span></span>      | <span data-ttu-id="b6539-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="b6539-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="b6539-114">type</span><span class="sxs-lookup"><span data-stu-id="b6539-114">type</span></span>          |<span data-ttu-id="b6539-115">String</span><span class="sxs-lookup"><span data-stu-id="b6539-115">String</span></span>       | <span data-ttu-id="b6539-116">可取值为：`days`、`hours`。</span><span class="sxs-lookup"><span data-stu-id="b6539-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="b6539-117">值</span><span class="sxs-lookup"><span data-stu-id="b6539-117">value</span></span>         |<span data-ttu-id="b6539-118">Int32</span><span class="sxs-lookup"><span data-stu-id="b6539-118">Int32</span></span>        | <span data-ttu-id="b6539-119">`days`或`hours`的数目。</span><span class="sxs-lookup"><span data-stu-id="b6539-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6539-120">关系</span><span class="sxs-lookup"><span data-stu-id="b6539-120">Relationships</span></span>

<span data-ttu-id="b6539-121">无。</span><span class="sxs-lookup"><span data-stu-id="b6539-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6539-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6539-122">JSON representation</span></span>

<span data-ttu-id="b6539-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6539-123">The following is a JSON representation of the resource.</span></span>

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