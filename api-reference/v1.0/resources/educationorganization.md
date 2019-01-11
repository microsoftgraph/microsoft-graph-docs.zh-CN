---
title: educationOrganization 资源类型
description: 用于模型之间的教育扇区中的不同组织类型通用性抽象实体。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: b0b65978b3b415af407c886095c4b31c7aaffab9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831931"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="4338c-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="4338c-103">educationOrganization resource type</span></span>

<span data-ttu-id="4338c-104">用于模型之间的教育扇区中的不同组织类型通用性抽象实体。</span><span class="sxs-lookup"><span data-stu-id="4338c-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="4338c-105">属性</span><span class="sxs-lookup"><span data-stu-id="4338c-105">Properties</span></span>
| <span data-ttu-id="4338c-106">属性</span><span class="sxs-lookup"><span data-stu-id="4338c-106">Property</span></span>     | <span data-ttu-id="4338c-107">类型</span><span class="sxs-lookup"><span data-stu-id="4338c-107">Type</span></span>   |<span data-ttu-id="4338c-108">说明</span><span class="sxs-lookup"><span data-stu-id="4338c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4338c-109">说明</span><span class="sxs-lookup"><span data-stu-id="4338c-109">description</span></span>|<span data-ttu-id="4338c-110">字符串</span><span class="sxs-lookup"><span data-stu-id="4338c-110">String</span></span>| <span data-ttu-id="4338c-111">组织说明。</span><span class="sxs-lookup"><span data-stu-id="4338c-111">Organization description.</span></span>|
|<span data-ttu-id="4338c-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4338c-112">displayName</span></span>|<span data-ttu-id="4338c-113">字符串</span><span class="sxs-lookup"><span data-stu-id="4338c-113">String</span></span>| <span data-ttu-id="4338c-114">组织的显示名称。</span><span class="sxs-lookup"><span data-stu-id="4338c-114">Organization display name.</span></span>|
|<span data-ttu-id="4338c-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="4338c-115">externalSource</span></span>|<span data-ttu-id="4338c-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="4338c-116">educationExternalSource</span></span>| <span data-ttu-id="4338c-117">从在其中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="4338c-117">Source where this organization was created from.</span></span> <span data-ttu-id="4338c-118">可能的值为： `sis`， `manual`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="4338c-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4338c-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="4338c-119">Relationships</span></span>
<span data-ttu-id="4338c-120">无。</span><span class="sxs-lookup"><span data-stu-id="4338c-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4338c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4338c-121">JSON representation</span></span>

<span data-ttu-id="4338c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4338c-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOrganization"
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "externalSource": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationOrganization resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
