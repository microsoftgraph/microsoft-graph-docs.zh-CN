---
title: conditionalAccessSessionControl 资源类型
description: 会话控制基类型。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 3d463c6b3c9a57b40b202e8291890aca20afb909
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42507518"
---
# <a name="conditionalaccesssessioncontrol-resource-type"></a><span data-ttu-id="3d5aa-103">conditionalAccessSessionControl 资源类型</span><span class="sxs-lookup"><span data-stu-id="3d5aa-103">conditionalAccessSessionControl resource type</span></span>

<span data-ttu-id="3d5aa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="3d5aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d5aa-105">会话控制基类型。</span><span class="sxs-lookup"><span data-stu-id="3d5aa-105">Session control base type.</span></span>

## <a name="properties"></a><span data-ttu-id="3d5aa-106">属性</span><span class="sxs-lookup"><span data-stu-id="3d5aa-106">Properties</span></span>

| <span data-ttu-id="3d5aa-107">属性</span><span class="sxs-lookup"><span data-stu-id="3d5aa-107">Property</span></span>     | <span data-ttu-id="3d5aa-108">类型</span><span class="sxs-lookup"><span data-stu-id="3d5aa-108">Type</span></span>        | <span data-ttu-id="3d5aa-109">说明</span><span class="sxs-lookup"><span data-stu-id="3d5aa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3d5aa-110">isEnabled</span><span class="sxs-lookup"><span data-stu-id="3d5aa-110">isEnabled</span></span>     |<span data-ttu-id="3d5aa-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d5aa-111">Boolean</span></span>      | <span data-ttu-id="3d5aa-112">指定是否启用会话控制。</span><span class="sxs-lookup"><span data-stu-id="3d5aa-112">Specifies whether the session control is enabled.</span></span> |

## <a name="relationships"></a><span data-ttu-id="3d5aa-113">关系</span><span class="sxs-lookup"><span data-stu-id="3d5aa-113">Relationships</span></span>

<span data-ttu-id="3d5aa-114">无。</span><span class="sxs-lookup"><span data-stu-id="3d5aa-114">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3d5aa-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3d5aa-115">JSON representation</span></span>

<span data-ttu-id="3d5aa-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d5aa-116">The following is a JSON representation of the resource.</span></span>

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