---
title: conditionalAccessSessionControl 资源类型
description: 会话控制基类型。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 856eaa294916bb47022307e3c2252400033c7461
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442175"
---
# <a name="conditionalaccesssessioncontrol-resource-type"></a><span data-ttu-id="2ef82-103">conditionalAccessSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ef82-103">conditionalAccessSessionControl resource type</span></span>

<span data-ttu-id="2ef82-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ef82-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ef82-105">会话控制基类型。</span><span class="sxs-lookup"><span data-stu-id="2ef82-105">Session control base type.</span></span>

## <a name="properties"></a><span data-ttu-id="2ef82-106">属性</span><span class="sxs-lookup"><span data-stu-id="2ef82-106">Properties</span></span>

| <span data-ttu-id="2ef82-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ef82-107">Property</span></span>     | <span data-ttu-id="2ef82-108">类型</span><span class="sxs-lookup"><span data-stu-id="2ef82-108">Type</span></span>        | <span data-ttu-id="2ef82-109">说明</span><span class="sxs-lookup"><span data-stu-id="2ef82-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ef82-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2ef82-110">isEnabled</span></span>     |<span data-ttu-id="2ef82-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="2ef82-111">Boolean</span></span>      | <span data-ttu-id="2ef82-112">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="2ef82-112">Specifies whether the session control is enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2ef82-113">关系</span><span class="sxs-lookup"><span data-stu-id="2ef82-113">Relationships</span></span>

<span data-ttu-id="2ef82-114">无。</span><span class="sxs-lookup"><span data-stu-id="2ef82-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ef82-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ef82-115">JSON representation</span></span>

<span data-ttu-id="2ef82-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ef82-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conditionalAccessSessionControl",
  "baseType": null
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
  "description": "conditionalAccessSessionControl resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->