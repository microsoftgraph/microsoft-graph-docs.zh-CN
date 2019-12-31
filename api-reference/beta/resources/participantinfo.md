---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b3d8671c33a0040fde8671a2d97b67dae0e94b28
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913581"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="b70c1-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="b70c1-103">participantInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b70c1-104">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="b70c1-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="b70c1-105">属性</span><span class="sxs-lookup"><span data-stu-id="b70c1-105">Properties</span></span>

| <span data-ttu-id="b70c1-106">属性</span><span class="sxs-lookup"><span data-stu-id="b70c1-106">Property</span></span>       | <span data-ttu-id="b70c1-107">类型</span><span class="sxs-lookup"><span data-stu-id="b70c1-107">Type</span></span>                          | <span data-ttu-id="b70c1-108">说明</span><span class="sxs-lookup"><span data-stu-id="b70c1-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b70c1-109">countryCode</span><span class="sxs-lookup"><span data-stu-id="b70c1-109">countryCode</span></span>    | <span data-ttu-id="b70c1-110">String</span><span class="sxs-lookup"><span data-stu-id="b70c1-110">String</span></span>                        | <span data-ttu-id="b70c1-111">呼叫开始时参与者最佳估计物理位置的 ISO 3166-1 Alpha-2 国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="b70c1-111">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="b70c1-112">只读。</span><span class="sxs-lookup"><span data-stu-id="b70c1-112">Read-only.</span></span>                             |
| <span data-ttu-id="b70c1-113">endpointType</span><span class="sxs-lookup"><span data-stu-id="b70c1-113">endpointType</span></span>   | <span data-ttu-id="b70c1-114">String</span><span class="sxs-lookup"><span data-stu-id="b70c1-114">String</span></span>                        | <span data-ttu-id="b70c1-115">参与者正在使用的终结点的类型。</span><span class="sxs-lookup"><span data-stu-id="b70c1-115">The type of endpoint the participant is using.</span></span> <span data-ttu-id="b70c1-116">可能的值包括`default`： `skypeForBusiness`、或`skypeForBusinessVoipPhone`。</span><span class="sxs-lookup"><span data-stu-id="b70c1-116">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="b70c1-117">只读。</span><span class="sxs-lookup"><span data-stu-id="b70c1-117">Read-only.</span></span>              |
| <span data-ttu-id="b70c1-118">窃取</span><span class="sxs-lookup"><span data-stu-id="b70c1-118">identity</span></span>       | [<span data-ttu-id="b70c1-119">identitySet</span><span class="sxs-lookup"><span data-stu-id="b70c1-119">identitySet</span></span>](identityset.md) | <span data-ttu-id="b70c1-120">与此参与者关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="b70c1-120">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="b70c1-121">只读。</span><span class="sxs-lookup"><span data-stu-id="b70c1-121">Read-only.</span></span>                                                                             |
| <span data-ttu-id="b70c1-122">languageId</span><span class="sxs-lookup"><span data-stu-id="b70c1-122">languageId</span></span>     | <span data-ttu-id="b70c1-123">String</span><span class="sxs-lookup"><span data-stu-id="b70c1-123">String</span></span>                        | <span data-ttu-id="b70c1-124">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="b70c1-124">The language culture string.</span></span> <span data-ttu-id="b70c1-125">只读。</span><span class="sxs-lookup"><span data-stu-id="b70c1-125">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="b70c1-126">范围</span><span class="sxs-lookup"><span data-stu-id="b70c1-126">region</span></span>         | <span data-ttu-id="b70c1-127">String</span><span class="sxs-lookup"><span data-stu-id="b70c1-127">String</span></span>                        | <span data-ttu-id="b70c1-128">参与者的家乡区域。</span><span class="sxs-lookup"><span data-stu-id="b70c1-128">The home region of the participant.</span></span> <span data-ttu-id="b70c1-129">它可以是国家/地区、一个洲或更大的地理区域。</span><span class="sxs-lookup"><span data-stu-id="b70c1-129">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="b70c1-130">这不会根据参与者的当前物理位置而变化，这与 countryCode 不同。</span><span class="sxs-lookup"><span data-stu-id="b70c1-130">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="b70c1-131">只读。</span><span class="sxs-lookup"><span data-stu-id="b70c1-131">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b70c1-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b70c1-132">JSON representation</span></span>

<span data-ttu-id="b70c1-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b70c1-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "countryCode",
    "endpointType",
    "languageId",
    "region"
  ],
  "@odata.type": "microsoft.graph.participantInfo"
}-->
```json
{
  "countryCode": "String",
  "identity": { "@odata.type": "#microsoft.graph.identitySet" },
  "endpointType": "default | skypeForBusiness | skypeForBusinessVoipPhone",
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
