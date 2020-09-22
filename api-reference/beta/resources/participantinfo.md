---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: b48c8d9e8e2b7b39a63b919ff30178d8c8ac8536
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998241"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="763bb-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="763bb-103">participantInfo resource type</span></span>

<span data-ttu-id="763bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="763bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="763bb-105">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="763bb-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="763bb-106">属性</span><span class="sxs-lookup"><span data-stu-id="763bb-106">Properties</span></span>

| <span data-ttu-id="763bb-107">属性</span><span class="sxs-lookup"><span data-stu-id="763bb-107">Property</span></span>       | <span data-ttu-id="763bb-108">类型</span><span class="sxs-lookup"><span data-stu-id="763bb-108">Type</span></span>                          | <span data-ttu-id="763bb-109">说明</span><span class="sxs-lookup"><span data-stu-id="763bb-109">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="763bb-110">countryCode</span><span class="sxs-lookup"><span data-stu-id="763bb-110">countryCode</span></span>    | <span data-ttu-id="763bb-111">String</span><span class="sxs-lookup"><span data-stu-id="763bb-111">String</span></span>                        | <span data-ttu-id="763bb-112">呼叫开始时参与者最佳估计物理位置的 ISO 3166-1 Alpha-2 国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="763bb-112">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="763bb-113">只读。</span><span class="sxs-lookup"><span data-stu-id="763bb-113">Read-only.</span></span>                             |
| <span data-ttu-id="763bb-114">endpointType</span><span class="sxs-lookup"><span data-stu-id="763bb-114">endpointType</span></span>   | <span data-ttu-id="763bb-115">String</span><span class="sxs-lookup"><span data-stu-id="763bb-115">String</span></span>                        | <span data-ttu-id="763bb-116">参与者正在使用的终结点的类型。</span><span class="sxs-lookup"><span data-stu-id="763bb-116">The type of endpoint the participant is using.</span></span> <span data-ttu-id="763bb-117">可能的值包括： `default` 、 `skypeForBusiness` 或 `skypeForBusinessVoipPhone` 。</span><span class="sxs-lookup"><span data-stu-id="763bb-117">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="763bb-118">只读。</span><span class="sxs-lookup"><span data-stu-id="763bb-118">Read-only.</span></span>              |
| <span data-ttu-id="763bb-119">窃取</span><span class="sxs-lookup"><span data-stu-id="763bb-119">identity</span></span>       | [<span data-ttu-id="763bb-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="763bb-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="763bb-121">与此参与者关联的 [了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="763bb-121">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="763bb-122">只读。</span><span class="sxs-lookup"><span data-stu-id="763bb-122">Read-only.</span></span>                                                                             |
| <span data-ttu-id="763bb-123">languageId</span><span class="sxs-lookup"><span data-stu-id="763bb-123">languageId</span></span>     | <span data-ttu-id="763bb-124">String</span><span class="sxs-lookup"><span data-stu-id="763bb-124">String</span></span>                        | <span data-ttu-id="763bb-125">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="763bb-125">The language culture string.</span></span> <span data-ttu-id="763bb-126">只读。</span><span class="sxs-lookup"><span data-stu-id="763bb-126">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="763bb-127">范围</span><span class="sxs-lookup"><span data-stu-id="763bb-127">region</span></span>         | <span data-ttu-id="763bb-128">String</span><span class="sxs-lookup"><span data-stu-id="763bb-128">String</span></span>                        | <span data-ttu-id="763bb-129">参与者的家乡区域。</span><span class="sxs-lookup"><span data-stu-id="763bb-129">The home region of the participant.</span></span> <span data-ttu-id="763bb-130">它可以是国家/地区、一个洲或更大的地理区域。</span><span class="sxs-lookup"><span data-stu-id="763bb-130">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="763bb-131">这不会根据参与者的当前物理位置而变化，这与 countryCode 不同。</span><span class="sxs-lookup"><span data-stu-id="763bb-131">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="763bb-132">只读。</span><span class="sxs-lookup"><span data-stu-id="763bb-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="763bb-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="763bb-133">JSON representation</span></span>

<span data-ttu-id="763bb-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="763bb-134">The following is a JSON representation of the resource.</span></span>

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


