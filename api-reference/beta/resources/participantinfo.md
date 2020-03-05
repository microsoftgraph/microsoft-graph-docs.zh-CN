---
title: participantInfo 资源类型
description: 包含有关参与者标识的其他属性
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: bd9c57961bee93e7d01e504bccb8671a8f1dd449
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522030"
---
# <a name="participantinfo-resource-type"></a><span data-ttu-id="f88fb-103">participantInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="f88fb-103">participantInfo resource type</span></span>

<span data-ttu-id="f88fb-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f88fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f88fb-105">包含有关参与者标识的其他属性</span><span class="sxs-lookup"><span data-stu-id="f88fb-105">Contains additional properties about the participant identity</span></span>

## <a name="properties"></a><span data-ttu-id="f88fb-106">属性</span><span class="sxs-lookup"><span data-stu-id="f88fb-106">Properties</span></span>

| <span data-ttu-id="f88fb-107">属性</span><span class="sxs-lookup"><span data-stu-id="f88fb-107">Property</span></span>       | <span data-ttu-id="f88fb-108">类型</span><span class="sxs-lookup"><span data-stu-id="f88fb-108">Type</span></span>                          | <span data-ttu-id="f88fb-109">说明</span><span class="sxs-lookup"><span data-stu-id="f88fb-109">Description</span></span>                                                                                                                                                |
|:---------------|:------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="f88fb-110">countryCode</span><span class="sxs-lookup"><span data-stu-id="f88fb-110">countryCode</span></span>    | <span data-ttu-id="f88fb-111">String</span><span class="sxs-lookup"><span data-stu-id="f88fb-111">String</span></span>                        | <span data-ttu-id="f88fb-112">呼叫开始时参与者最佳估计物理位置的 ISO 3166-1 Alpha-2 国家/地区代码。</span><span class="sxs-lookup"><span data-stu-id="f88fb-112">The ISO 3166-1 Alpha-2 country code of the participant's best estimated physical location at the start of the call.</span></span> <span data-ttu-id="f88fb-113">只读。</span><span class="sxs-lookup"><span data-stu-id="f88fb-113">Read-only.</span></span>                             |
| <span data-ttu-id="f88fb-114">endpointType</span><span class="sxs-lookup"><span data-stu-id="f88fb-114">endpointType</span></span>   | <span data-ttu-id="f88fb-115">String</span><span class="sxs-lookup"><span data-stu-id="f88fb-115">String</span></span>                        | <span data-ttu-id="f88fb-116">参与者正在使用的终结点的类型。</span><span class="sxs-lookup"><span data-stu-id="f88fb-116">The type of endpoint the participant is using.</span></span> <span data-ttu-id="f88fb-117">可能的值包括`default`： `skypeForBusiness`、或`skypeForBusinessVoipPhone`。</span><span class="sxs-lookup"><span data-stu-id="f88fb-117">Possible values are: `default`, `skypeForBusiness`, or `skypeForBusinessVoipPhone`.</span></span> <span data-ttu-id="f88fb-118">只读。</span><span class="sxs-lookup"><span data-stu-id="f88fb-118">Read-only.</span></span>              |
| <span data-ttu-id="f88fb-119">窃取</span><span class="sxs-lookup"><span data-stu-id="f88fb-119">identity</span></span>       | [<span data-ttu-id="f88fb-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="f88fb-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="f88fb-121">与此参与者关联的[了解 identityset](identityset.md) 。</span><span class="sxs-lookup"><span data-stu-id="f88fb-121">The [identitySet](identityset.md) associated with this participant.</span></span> <span data-ttu-id="f88fb-122">只读。</span><span class="sxs-lookup"><span data-stu-id="f88fb-122">Read-only.</span></span>                                                                             |
| <span data-ttu-id="f88fb-123">languageId</span><span class="sxs-lookup"><span data-stu-id="f88fb-123">languageId</span></span>     | <span data-ttu-id="f88fb-124">String</span><span class="sxs-lookup"><span data-stu-id="f88fb-124">String</span></span>                        | <span data-ttu-id="f88fb-125">语言区域性字符串。</span><span class="sxs-lookup"><span data-stu-id="f88fb-125">The language culture string.</span></span> <span data-ttu-id="f88fb-126">只读。</span><span class="sxs-lookup"><span data-stu-id="f88fb-126">Read-only.</span></span>                                                                                                                    |
| <span data-ttu-id="f88fb-127">范围</span><span class="sxs-lookup"><span data-stu-id="f88fb-127">region</span></span>         | <span data-ttu-id="f88fb-128">String</span><span class="sxs-lookup"><span data-stu-id="f88fb-128">String</span></span>                        | <span data-ttu-id="f88fb-129">参与者的家乡区域。</span><span class="sxs-lookup"><span data-stu-id="f88fb-129">The home region of the participant.</span></span> <span data-ttu-id="f88fb-130">它可以是国家/地区、一个洲或更大的地理区域。</span><span class="sxs-lookup"><span data-stu-id="f88fb-130">This can be a country, a continent, or a larger geographic region.</span></span> <span data-ttu-id="f88fb-131">这不会根据参与者的当前物理位置而变化，这与 countryCode 不同。</span><span class="sxs-lookup"><span data-stu-id="f88fb-131">This does not change based on the participant's current physical location, unlike countryCode.</span></span> <span data-ttu-id="f88fb-132">只读。</span><span class="sxs-lookup"><span data-stu-id="f88fb-132">Read-only.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f88fb-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f88fb-133">JSON representation</span></span>

<span data-ttu-id="f88fb-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f88fb-134">The following is a JSON representation of the resource.</span></span>

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
