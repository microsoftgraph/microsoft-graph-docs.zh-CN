---
title: conditionalAccessSessionControl 资源类型
description: 会话控制基类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 74163ae0a5e76aa72841760857c40e14ca5a9685
ms.sourcegitcommit: 3ee6a3a949be7f0a9028bde90092a10a42e0f1fc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2019
ms.locfileid: "37638489"
---
# <a name="conditionalaccesssessioncontrol-resource-type"></a><span data-ttu-id="2b94c-103">conditionalAccessSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="2b94c-103">conditionalAccessSessionControl resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b94c-104">会话控制基类型。</span><span class="sxs-lookup"><span data-stu-id="2b94c-104">Session control base type.</span></span>

## <a name="properties"></a><span data-ttu-id="2b94c-105">属性</span><span class="sxs-lookup"><span data-stu-id="2b94c-105">Properties</span></span>

| <span data-ttu-id="2b94c-106">属性</span><span class="sxs-lookup"><span data-stu-id="2b94c-106">Property</span></span>     | <span data-ttu-id="2b94c-107">类型</span><span class="sxs-lookup"><span data-stu-id="2b94c-107">Type</span></span>        | <span data-ttu-id="2b94c-108">说明</span><span class="sxs-lookup"><span data-stu-id="2b94c-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2b94c-109">isEnabled</span><span class="sxs-lookup"><span data-stu-id="2b94c-109">isEnabled</span></span>     |<span data-ttu-id="2b94c-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b94c-110">Boolean</span></span>      | <span data-ttu-id="2b94c-111">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="2b94c-111">Specifies whether the session control is enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="2b94c-112">关系</span><span class="sxs-lookup"><span data-stu-id="2b94c-112">Relationships</span></span>

<span data-ttu-id="2b94c-113">无。</span><span class="sxs-lookup"><span data-stu-id="2b94c-113">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b94c-114">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2b94c-114">JSON representation</span></span>

<span data-ttu-id="2b94c-115">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b94c-115">The following is a JSON representation of the resource.</span></span>

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