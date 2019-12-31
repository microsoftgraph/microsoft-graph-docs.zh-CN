---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 9b603d93b2be2fef6a999cf3c1d7663fc7405da9
ms.sourcegitcommit: 636671293b0be89088459c4fc8a5e661341b37cf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/31/2019
ms.locfileid: "40913728"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="0090f-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="0090f-103">participantInfo resource type</span></span>

<span data-ttu-id="0090f-104">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="0090f-104">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="0090f-105">属性</span><span class="sxs-lookup"><span data-stu-id="0090f-105">Properties</span></span>

| <span data-ttu-id="0090f-106">属性</span><span class="sxs-lookup"><span data-stu-id="0090f-106">Property</span></span>       | <span data-ttu-id="0090f-107">类型</span><span class="sxs-lookup"><span data-stu-id="0090f-107">Type</span></span>                          | <span data-ttu-id="0090f-108">说明</span><span class="sxs-lookup"><span data-stu-id="0090f-108">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="0090f-109">窃取</span><span class="sxs-lookup"><span data-stu-id="0090f-109">identity</span></span>       | [<span data-ttu-id="0090f-110">identitySet</span><span class="sxs-lookup"><span data-stu-id="0090f-110">identitySet</span></span>](identityset.md) | <span data-ttu-id="0090f-111">与此参与者关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="0090f-111">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="0090f-112">只读。</span><span class="sxs-lookup"><span data-stu-id="0090f-112">Read-only.</span></span>                                                                             |
| <span data-ttu-id="0090f-113">languageId</span><span class="sxs-lookup"><span data-stu-id="0090f-113">languageId</span></span>     | <span data-ttu-id="0090f-114">String</span><span class="sxs-lookup"><span data-stu-id="0090f-114">String</span></span>                        | <span data-ttu-id="0090f-115">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="0090f-115">The language culture string.</span></span> <span data-ttu-id="0090f-116">只读。</span><span class="sxs-lookup"><span data-stu-id="0090f-116">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="0090f-117">范围</span><span class="sxs-lookup"><span data-stu-id="0090f-117">region</span></span>         | <span data-ttu-id="0090f-118">String</span><span class="sxs-lookup"><span data-stu-id="0090f-118">String</span></span>                        | <span data-ttu-id="0090f-119">参与者的家乡区域。</span><span class="sxs-lookup"><span data-stu-id="0090f-119">The home region of the participant.</span></span> <span data-ttu-id="0090f-120">它可以是国家/地区、一个洲或更大的地理区域。</span><span class="sxs-lookup"><span data-stu-id="0090f-120">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="0090f-121">这不会根据参与者的当前物理位置而更改。</span><span class="sxs-lookup"><span data-stu-id="0090f-121">This does not change based on the participant's current physical location.</span></span> <span data-ttu-id="0090f-122">只读。</span><span class="sxs-lookup"><span data-stu-id="0090f-122">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0090f-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0090f-123">JSON representation</span></span>

<span data-ttu-id="0090f-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0090f-124">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "languageId",
    "region"
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
