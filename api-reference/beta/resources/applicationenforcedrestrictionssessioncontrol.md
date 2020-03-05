---
title: applicationEnforcedRestrictionsSessionControl 资源类型
description: 实施应用程序限制的会话控制。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: b5f608a2915db80d671ab604ab69d256d6aad0ec
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508287"
---
# <a name="applicationenforcedrestrictionssessioncontrol-resource-type"></a><span data-ttu-id="9a397-103">applicationEnforcedRestrictionsSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="9a397-103">applicationEnforcedRestrictionsSessionControl resource type</span></span>

<span data-ttu-id="9a397-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9a397-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9a397-105">实施应用程序限制的会话控制。</span><span class="sxs-lookup"><span data-stu-id="9a397-105">Session control to enforce application restrictions.</span></span> <span data-ttu-id="9a397-106">Inehrits 来自[条件访问会话控制](conditionalaccesssessioncontrol.md)。</span><span class="sxs-lookup"><span data-stu-id="9a397-106">Inehrits from [Conditional Access Session Control](conditionalaccesssessioncontrol.md).</span></span>

## <a name="properties"></a><span data-ttu-id="9a397-107">属性</span><span class="sxs-lookup"><span data-stu-id="9a397-107">Properties</span></span>

| <span data-ttu-id="9a397-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a397-108">Property</span></span>     | <span data-ttu-id="9a397-109">类型</span><span class="sxs-lookup"><span data-stu-id="9a397-109">Type</span></span>        | <span data-ttu-id="9a397-110">说明</span><span class="sxs-lookup"><span data-stu-id="9a397-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="9a397-111">isEnabled</span><span class="sxs-lookup"><span data-stu-id="9a397-111">isEnabled</span></span>     |<span data-ttu-id="9a397-112">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a397-112">Boolean</span></span>      | <span data-ttu-id="9a397-113">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="9a397-113">Specifies whether the session control is enabled or not.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9a397-114">关系</span><span class="sxs-lookup"><span data-stu-id="9a397-114">Relationships</span></span>

<span data-ttu-id="9a397-115">无。</span><span class="sxs-lookup"><span data-stu-id="9a397-115">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a397-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a397-116">JSON representation</span></span>

<span data-ttu-id="9a397-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a397-117">The following is a JSON representation of the resource.</span></span>

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
