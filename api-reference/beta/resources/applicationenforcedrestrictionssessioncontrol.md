---
title: applicationEnforcedRestrictionsSessionControl 资源类型
description: 实施应用程序限制的会话控制。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d29f26ece4ae94562dd1e16c4b9f27c77c142fa1
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638524"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="d55a2-103">applicationEnforcedRestrictionsSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="d55a2-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d55a2-104">实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="d55a2-104">Session control to enforce application restrictions.</span></span> <span data-ttu-id="d55a2-105">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="d55a2-105">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d55a2-106">属性</span><span class="sxs-lookup"><span data-stu-id="d55a2-106">Properties</span></span>

| <span data-ttu-id="d55a2-107">属性</span><span class="sxs-lookup"><span data-stu-id="d55a2-107">Property</span></span>     | <span data-ttu-id="d55a2-108">类型</span><span class="sxs-lookup"><span data-stu-id="d55a2-108">Type</span></span>        | <span data-ttu-id="d55a2-109">说明</span><span class="sxs-lookup"><span data-stu-id="d55a2-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="d55a2-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="d55a2-110">isEnabled</span></span>     |<span data-ttu-id="d55a2-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="d55a2-111">Boolean</span></span>      | <span data-ttu-id="d55a2-112">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="d55a2-112">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="d55a2-113">关系</span><span class="sxs-lookup"><span data-stu-id="d55a2-113">Relationships</span></span>

<span data-ttu-id="d55a2-114">无。</span><span class="sxs-lookup"><span data-stu-id="d55a2-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="d55a2-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d55a2-115">JSON representation</span></span>

<span data-ttu-id="d55a2-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d55a2-116">The following is a JSON representation of the resource.</span></span>

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
