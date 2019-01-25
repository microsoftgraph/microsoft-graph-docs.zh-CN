---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3d040fd5be86068c30e7a63dae50888c4f3ec756
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528345"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="2fc36-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="2fc36-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2fc36-104">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="2fc36-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="2fc36-105">属性</span><span class="sxs-lookup"><span data-stu-id="2fc36-105">Properties</span></span>

| <span data-ttu-id="2fc36-106">属性</span><span class="sxs-lookup"><span data-stu-id="2fc36-106">Property</span></span>       | <span data-ttu-id="2fc36-107">类型</span><span class="sxs-lookup"><span data-stu-id="2fc36-107">Type</span></span>                          | <span data-ttu-id="2fc36-108">说明</span><span class="sxs-lookup"><span data-stu-id="2fc36-108">Description</span></span>  |
|:---------------|:------------------------------|:-------------|
| <span data-ttu-id="2fc36-109">Identity</span><span class="sxs-lookup"><span data-stu-id="2fc36-109">identity</span></span>       | [<span data-ttu-id="2fc36-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="2fc36-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="2fc36-111">与此参与者关联[identitySet](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="2fc36-111">The [identitySet](identityset.md) associated with this participant.</span></span> |
| <span data-ttu-id="2fc36-112">languageId</span><span class="sxs-lookup"><span data-stu-id="2fc36-112">languageId</span></span>     | <span data-ttu-id="2fc36-113">String</span><span class="sxs-lookup"><span data-stu-id="2fc36-113">String</span></span>                        | <span data-ttu-id="2fc36-114">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="2fc36-114">The language culture string.</span></span> |
| <span data-ttu-id="2fc36-115">地区</span><span class="sxs-lookup"><span data-stu-id="2fc36-115">region</span></span>         | <span data-ttu-id="2fc36-116">String</span><span class="sxs-lookup"><span data-stu-id="2fc36-116">String</span></span>                        | <span data-ttu-id="2fc36-117">参与者的区域。</span><span class="sxs-lookup"><span data-stu-id="2fc36-117">Region of the participant.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2fc36-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fc36-118">JSON representation</span></span>

<span data-ttu-id="2fc36-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fc36-119">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/participantinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
