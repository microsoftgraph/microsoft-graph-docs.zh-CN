---
title: signInFrequencySessionControl 资源类型
description: 用于强制登录频率的会话控制。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 8c0c0eca971c6d9df8bde348787029cb5aa98320
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47970619"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="e0382-103">signInFrequencySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0382-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="e0382-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0382-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e0382-105">用于强制登录频率的会话控制。</span><span class="sxs-lookup"><span data-stu-id="e0382-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="e0382-106">继承自 [条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="e0382-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e0382-107">属性</span><span class="sxs-lookup"><span data-stu-id="e0382-107">Properties</span></span>

| <span data-ttu-id="e0382-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0382-108">Property</span></span>     | <span data-ttu-id="e0382-109">类型</span><span class="sxs-lookup"><span data-stu-id="e0382-109">Type</span></span>        | <span data-ttu-id="e0382-110">说明</span><span class="sxs-lookup"><span data-stu-id="e0382-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e0382-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="e0382-111">isEnabled</span></span>     |<span data-ttu-id="e0382-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0382-112">Boolean</span></span>      | <span data-ttu-id="e0382-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="e0382-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="e0382-114">type</span><span class="sxs-lookup"><span data-stu-id="e0382-114">type</span></span>          |<span data-ttu-id="e0382-115">String</span><span class="sxs-lookup"><span data-stu-id="e0382-115">String</span></span>       | <span data-ttu-id="e0382-116">可取值为：`days`、`hours`。</span><span class="sxs-lookup"><span data-stu-id="e0382-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="e0382-117">值</span><span class="sxs-lookup"><span data-stu-id="e0382-117">value</span></span>         |<span data-ttu-id="e0382-118">Int32</span><span class="sxs-lookup"><span data-stu-id="e0382-118">Int32</span></span>        | <span data-ttu-id="e0382-119">或的数目 `days` `hours` 。</span><span class="sxs-lookup"><span data-stu-id="e0382-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0382-120">关系</span><span class="sxs-lookup"><span data-stu-id="e0382-120">Relationships</span></span>

<span data-ttu-id="e0382-121">无。</span><span class="sxs-lookup"><span data-stu-id="e0382-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e0382-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0382-122">JSON representation</span></span>

<span data-ttu-id="e0382-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0382-123">The following is a JSON representation of the resource.</span></span>

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

