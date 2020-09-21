---
title: applicationEnforcedRestrictionsSessionControl 资源类型
description: 实施应用程序限制的会话控制。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 55e23dead8ea894b57451bf65586672ea125fc35
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48050276"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="63aec-103">applicationEnforcedRestrictionsSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="63aec-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="63aec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63aec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63aec-105">实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="63aec-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="63aec-106">Inehrits 来自 [条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="63aec-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="63aec-107">属性</span><span class="sxs-lookup"><span data-stu-id="63aec-107">Properties</span></span>

| <span data-ttu-id="63aec-108">属性</span><span class="sxs-lookup"><span data-stu-id="63aec-108">Property</span></span>     | <span data-ttu-id="63aec-109">类型</span><span class="sxs-lookup"><span data-stu-id="63aec-109">Type</span></span>        | <span data-ttu-id="63aec-110">说明</span><span class="sxs-lookup"><span data-stu-id="63aec-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="63aec-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="63aec-111">isEnabled</span></span>     |<span data-ttu-id="63aec-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="63aec-112">Boolean</span></span>      | <span data-ttu-id="63aec-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="63aec-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="63aec-114">关系</span><span class="sxs-lookup"><span data-stu-id="63aec-114">Relationships</span></span>

<span data-ttu-id="63aec-115">无。</span><span class="sxs-lookup"><span data-stu-id="63aec-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="63aec-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63aec-116">JSON representation</span></span>

<span data-ttu-id="63aec-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63aec-117">The following is a JSON representation of the resource.</span></span>

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


