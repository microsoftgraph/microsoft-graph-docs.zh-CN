---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3d040fd5be86068c30e7a63dae50888c4f3ec756
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568568"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="81308-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="81308-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81308-104">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="81308-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="81308-105">属性</span><span class="sxs-lookup"><span data-stu-id="81308-105">Properties</span></span>

| <span data-ttu-id="81308-106">属性</span><span class="sxs-lookup"><span data-stu-id="81308-106">Property</span></span>       | <span data-ttu-id="81308-107">类型</span><span class="sxs-lookup"><span data-stu-id="81308-107">Type</span></span>                          | <span data-ttu-id="81308-108">说明</span><span class="sxs-lookup"><span data-stu-id="81308-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="81308-109">窃取</span><span class="sxs-lookup"><span data-stu-id="81308-109">identity</span></span>       | [<span data-ttu-id="81308-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="81308-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="81308-111">与此参与者关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="81308-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="81308-112">languageId</span><span class="sxs-lookup"><span data-stu-id="81308-112">languageId</span></span>     | <span data-ttu-id="81308-113">String</span><span class="sxs-lookup"><span data-stu-id="81308-113">String</span></span>                        | <span data-ttu-id="81308-114">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="81308-114">The language culture string.</span></span> |
| <span data-ttu-id="81308-115">范围</span><span class="sxs-lookup"><span data-stu-id="81308-115">region</span></span>         | <span data-ttu-id="81308-116">String</span><span class="sxs-lookup"><span data-stu-id="81308-116">String</span></span>                        | <span data-ttu-id="81308-117">参与者的地区。</span><span class="sxs-lookup"><span data-stu-id="81308-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="81308-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81308-118">JSON representation</span></span>

<span data-ttu-id="81308-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81308-119">The following is a JSON representation of the resource.</span></span>

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
