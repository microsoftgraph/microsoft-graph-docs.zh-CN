---
title: signInFrequencySessionControl 资源类型
description: 用于强制登录频率的会话控制。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: af2d23c26d2911c8abc36c8a9e66fb776edd43e0
ms.sourcegitcommit: 2856a818ef3be0d4cfcbc9253906603bcc3d6325
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434846"
---
# <a name="signinfrequencysessioncontrol-resource-type"></a><span data-ttu-id="45f4f-103">signInFrequencySessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="45f4f-103">signInFrequencySessionControl resource type</span></span>

<span data-ttu-id="45f4f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45f4f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45f4f-105">用于强制登录频率的会话控制。</span><span class="sxs-lookup"><span data-stu-id="45f4f-105">Session control to enforce sign-in frequency.</span></span> <span data-ttu-id="45f4f-106">继承自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="45f4f-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="45f4f-107">属性</span><span class="sxs-lookup"><span data-stu-id="45f4f-107">Properties</span></span>

| <span data-ttu-id="45f4f-108">属性</span><span class="sxs-lookup"><span data-stu-id="45f4f-108">Property</span></span>     | <span data-ttu-id="45f4f-109">类型</span><span class="sxs-lookup"><span data-stu-id="45f4f-109">Type</span></span>        | <span data-ttu-id="45f4f-110">说明</span><span class="sxs-lookup"><span data-stu-id="45f4f-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="45f4f-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="45f4f-111">isEnabled</span></span>     |<span data-ttu-id="45f4f-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="45f4f-112">Boolean</span></span>      | <span data-ttu-id="45f4f-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="45f4f-113">Specifies whether the session control is enabled.</span></span> |
|<span data-ttu-id="45f4f-114">type</span><span class="sxs-lookup"><span data-stu-id="45f4f-114">type</span></span>          |<span data-ttu-id="45f4f-115">String</span><span class="sxs-lookup"><span data-stu-id="45f4f-115">String</span></span>       | <span data-ttu-id="45f4f-116">可取值为：`days`、`hours`。</span><span class="sxs-lookup"><span data-stu-id="45f4f-116">Possible values are: `days`, `hours`.</span></span>|
|<span data-ttu-id="45f4f-117">值</span><span class="sxs-lookup"><span data-stu-id="45f4f-117">value</span></span>         |<span data-ttu-id="45f4f-118">Int32</span><span class="sxs-lookup"><span data-stu-id="45f4f-118">Int32</span></span>        | <span data-ttu-id="45f4f-119">或的数目 `days` `hours` 。</span><span class="sxs-lookup"><span data-stu-id="45f4f-119">The number of `days` or `hours`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="45f4f-120">关系</span><span class="sxs-lookup"><span data-stu-id="45f4f-120">Relationships</span></span>

<span data-ttu-id="45f4f-121">无。</span><span class="sxs-lookup"><span data-stu-id="45f4f-121">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="45f4f-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45f4f-122">JSON representation</span></span>

<span data-ttu-id="45f4f-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45f4f-123">The following is a JSON representation of the resource.</span></span>

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
