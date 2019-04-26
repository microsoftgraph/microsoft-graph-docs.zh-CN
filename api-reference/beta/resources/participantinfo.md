---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9869cf1154735742630edf75ea3e4d5303d45bc9
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33344910"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="20f33-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="20f33-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="20f33-104">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="20f33-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="20f33-105">属性</span><span class="sxs-lookup"><span data-stu-id="20f33-105">Properties</span></span>

| <span data-ttu-id="20f33-106">属性</span><span class="sxs-lookup"><span data-stu-id="20f33-106">Property</span></span>       | <span data-ttu-id="20f33-107">类型</span><span class="sxs-lookup"><span data-stu-id="20f33-107">Type</span></span>                          | <span data-ttu-id="20f33-108">说明</span><span class="sxs-lookup"><span data-stu-id="20f33-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="20f33-109">窃取</span><span class="sxs-lookup"><span data-stu-id="20f33-109">identity</span></span>       | [<span data-ttu-id="20f33-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="20f33-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="20f33-111">与此参与者关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="20f33-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="20f33-112">languageId</span><span class="sxs-lookup"><span data-stu-id="20f33-112">languageId</span></span>     | <span data-ttu-id="20f33-113">String</span><span class="sxs-lookup"><span data-stu-id="20f33-113">String</span></span>                        | <span data-ttu-id="20f33-114">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="20f33-114">The language culture string.</span></span> |
| <span data-ttu-id="20f33-115">范围</span><span class="sxs-lookup"><span data-stu-id="20f33-115">region</span></span>         | <span data-ttu-id="20f33-116">String</span><span class="sxs-lookup"><span data-stu-id="20f33-116">String</span></span>                        | <span data-ttu-id="20f33-117">参与者的地区。</span><span class="sxs-lookup"><span data-stu-id="20f33-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="20f33-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20f33-118">JSON representation</span></span>

<span data-ttu-id="20f33-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20f33-119">The following is a JSON representation of the resource.</span></span>

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
