---
title: applicationEnforcedRestrictionsSessionControl 资源类型
description: 实施应用程序限制的会话控制。
localization_priority: Normal
author: videor
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 0819b9133e6495bbe6691170ce0c38a2d93302d7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48003365"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="cc7b1-103">applicationEnforcedRestrictionsSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="cc7b1-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="cc7b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc7b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cc7b1-105">实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="cc7b1-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="cc7b1-106">继承自 [条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="cc7b1-106">Inherits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="cc7b1-107">属性</span><span class="sxs-lookup"><span data-stu-id="cc7b1-107">Properties</span></span>

| <span data-ttu-id="cc7b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc7b1-108">Property</span></span>     | <span data-ttu-id="cc7b1-109">类型</span><span class="sxs-lookup"><span data-stu-id="cc7b1-109">Type</span></span>        | <span data-ttu-id="cc7b1-110">说明</span><span class="sxs-lookup"><span data-stu-id="cc7b1-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="cc7b1-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cc7b1-111">isEnabled</span></span>     |<span data-ttu-id="cc7b1-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="cc7b1-112">Boolean</span></span>      | <span data-ttu-id="cc7b1-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="cc7b1-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="cc7b1-114">关系</span><span class="sxs-lookup"><span data-stu-id="cc7b1-114">Relationships</span></span>

<span data-ttu-id="cc7b1-115">无。</span><span class="sxs-lookup"><span data-stu-id="cc7b1-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cc7b1-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cc7b1-116">JSON representation</span></span>

<span data-ttu-id="cc7b1-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc7b1-117">The following is a JSON representation of the resource.</span></span>

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

