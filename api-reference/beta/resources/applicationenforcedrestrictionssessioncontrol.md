---
title: applicationEnforcedRestrictionsSessionControl 资源类型
description: 强制实施应用程序限制的会话控制。
localization_priority: Normal
author: sureshja
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f7f20950b3773e660cfc1b0ed4fdec338546e09a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50134764"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="dea5e-103">applicationEnforcedRestrictionsSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="dea5e-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="dea5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dea5e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dea5e-105">强制实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="dea5e-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="dea5e-106">条件访问会话 [控件中的指令](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="dea5e-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="dea5e-107">属性</span><span class="sxs-lookup"><span data-stu-id="dea5e-107">Properties</span></span>

| <span data-ttu-id="dea5e-108">属性</span><span class="sxs-lookup"><span data-stu-id="dea5e-108">Property</span></span>     | <span data-ttu-id="dea5e-109">类型</span><span class="sxs-lookup"><span data-stu-id="dea5e-109">Type</span></span>        | <span data-ttu-id="dea5e-110">说明</span><span class="sxs-lookup"><span data-stu-id="dea5e-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="dea5e-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="dea5e-111">isEnabled</span></span>     |<span data-ttu-id="dea5e-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="dea5e-112">Boolean</span></span>      | <span data-ttu-id="dea5e-113">指定是否启用会话控件。</span><span class="sxs-lookup"><span data-stu-id="dea5e-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="dea5e-114">关系</span><span class="sxs-lookup"><span data-stu-id="dea5e-114">Relationships</span></span>

<span data-ttu-id="dea5e-115">无。</span><span class="sxs-lookup"><span data-stu-id="dea5e-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dea5e-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dea5e-116">JSON representation</span></span>

<span data-ttu-id="dea5e-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dea5e-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.applicationEnforcedRestrictionsSessionControl",
  "baseType": "microsoft.graph.conditionalAccessSessionControl"
}-->

```json
{
  "isEnabled": true
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "applicationEnforcedRestrictionsSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


