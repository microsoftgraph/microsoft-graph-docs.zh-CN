---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 0316cb1bbe474f8265ed384774183759d29aca0f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447246"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="98678-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="98678-103">participantInfo resource type</span></span>

<span data-ttu-id="98678-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="98678-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="98678-105">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="98678-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="98678-106">属性</span><span class="sxs-lookup"><span data-stu-id="98678-106">Properties</span></span>

| <span data-ttu-id="98678-107">属性</span><span class="sxs-lookup"><span data-stu-id="98678-107">Property</span></span>       | <span data-ttu-id="98678-108">类型</span><span class="sxs-lookup"><span data-stu-id="98678-108">Type</span></span>                          | <span data-ttu-id="98678-109">说明</span><span class="sxs-lookup"><span data-stu-id="98678-109">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="98678-110">窃取</span><span class="sxs-lookup"><span data-stu-id="98678-110">identity</span></span>       | [<span data-ttu-id="98678-111">identitySet</span><span class="sxs-lookup"><span data-stu-id="98678-111">identitySet</span></span>](identityset.md) | <span data-ttu-id="98678-112">与此参与者关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="98678-112">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="98678-113">只读。</span><span class="sxs-lookup"><span data-stu-id="98678-113">Read-only.</span></span>                                                                             |
| <span data-ttu-id="98678-114">languageId</span><span class="sxs-lookup"><span data-stu-id="98678-114">languageId</span></span>     | <span data-ttu-id="98678-115">String</span><span class="sxs-lookup"><span data-stu-id="98678-115">String</span></span>                        | <span data-ttu-id="98678-116">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="98678-116">The language culture string.</span></span> <span data-ttu-id="98678-117">只读。</span><span class="sxs-lookup"><span data-stu-id="98678-117">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="98678-118">范围</span><span class="sxs-lookup"><span data-stu-id="98678-118">region</span></span>         | <span data-ttu-id="98678-119">String</span><span class="sxs-lookup"><span data-stu-id="98678-119">String</span></span>                        | <span data-ttu-id="98678-120">参与者的家乡区域。</span><span class="sxs-lookup"><span data-stu-id="98678-120">The home region of the participant.</span></span> <span data-ttu-id="98678-121">它可以是国家/地区、一个洲或更大的地理区域。</span><span class="sxs-lookup"><span data-stu-id="98678-121">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="98678-122">这不会根据参与者的当前物理位置而更改。</span><span class="sxs-lookup"><span data-stu-id="98678-122">This does not change based on the participant's current physical location.</span></span> <span data-ttu-id="98678-123">只读。</span><span class="sxs-lookup"><span data-stu-id="98678-123">Read-only.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="98678-124">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="98678-124">JSON representation</span></span>

<span data-ttu-id="98678-125">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="98678-125">The following is a JSON representation of the resource.</span></span>

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
