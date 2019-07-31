---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: ad73ce0bbeaa02b0207f11bbd3f0004857d90506
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966221"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="c4adc-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4adc-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4adc-104">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="c4adc-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="c4adc-105">属性</span><span class="sxs-lookup"><span data-stu-id="c4adc-105">Properties</span></span>

| <span data-ttu-id="c4adc-106">属性</span><span class="sxs-lookup"><span data-stu-id="c4adc-106">Property</span></span>       | <span data-ttu-id="c4adc-107">类型</span><span class="sxs-lookup"><span data-stu-id="c4adc-107">Type</span></span>                          | <span data-ttu-id="c4adc-108">说明</span><span class="sxs-lookup"><span data-stu-id="c4adc-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="c4adc-109">窃取</span><span class="sxs-lookup"><span data-stu-id="c4adc-109">identity</span></span>       | [<span data-ttu-id="c4adc-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="c4adc-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="c4adc-111">与此参与者关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="c4adc-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="c4adc-112">languageId</span><span class="sxs-lookup"><span data-stu-id="c4adc-112">languageId</span></span>     | <span data-ttu-id="c4adc-113">String</span><span class="sxs-lookup"><span data-stu-id="c4adc-113">String</span></span>                        | <span data-ttu-id="c4adc-114">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="c4adc-114">The language culture string.</span></span> |
| <span data-ttu-id="c4adc-115">范围</span><span class="sxs-lookup"><span data-stu-id="c4adc-115">region</span></span>         | <span data-ttu-id="c4adc-116">String</span><span class="sxs-lookup"><span data-stu-id="c4adc-116">String</span></span>                        | <span data-ttu-id="c4adc-117">参与者的地区。</span><span class="sxs-lookup"><span data-stu-id="c4adc-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c4adc-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4adc-118">JSON representation</span></span>

<span data-ttu-id="c4adc-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4adc-119">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId", "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "languageId": "String",
  "region": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "participantInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
