---
title: educationOrganization 资源类型
description: 用于模型之间的教育扇区中的不同组织类型通用性抽象实体。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 99f3294f76a246e4e78f0f61b0fc1f62532c3a03
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977421"
---
# <a name="educationorganization-resource-type"></a><span data-ttu-id="fad36-103">educationOrganization 资源类型</span><span class="sxs-lookup"><span data-stu-id="fad36-103">educationOrganization resource type</span></span>

<span data-ttu-id="fad36-104">用于模型之间的教育扇区中的不同组织类型通用性抽象实体。</span><span class="sxs-lookup"><span data-stu-id="fad36-104">Abstract entity used to model the commonality between different organization types within the education sector.</span></span>

## <a name="properties"></a><span data-ttu-id="fad36-105">属性</span><span class="sxs-lookup"><span data-stu-id="fad36-105">Properties</span></span>
| <span data-ttu-id="fad36-106">属性</span><span class="sxs-lookup"><span data-stu-id="fad36-106">Property</span></span>     | <span data-ttu-id="fad36-107">类型</span><span class="sxs-lookup"><span data-stu-id="fad36-107">Type</span></span>   |<span data-ttu-id="fad36-108">说明</span><span class="sxs-lookup"><span data-stu-id="fad36-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fad36-109">说明</span><span class="sxs-lookup"><span data-stu-id="fad36-109">description</span></span>|<span data-ttu-id="fad36-110">字符串</span><span class="sxs-lookup"><span data-stu-id="fad36-110">String</span></span>| <span data-ttu-id="fad36-111">组织说明。</span><span class="sxs-lookup"><span data-stu-id="fad36-111">Organization description.</span></span>|
|<span data-ttu-id="fad36-112">displayName</span><span class="sxs-lookup"><span data-stu-id="fad36-112">displayName</span></span>|<span data-ttu-id="fad36-113">字符串</span><span class="sxs-lookup"><span data-stu-id="fad36-113">String</span></span>| <span data-ttu-id="fad36-114">组织的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fad36-114">Organization display name.</span></span>|
|<span data-ttu-id="fad36-115">externalSource</span><span class="sxs-lookup"><span data-stu-id="fad36-115">externalSource</span></span>|<span data-ttu-id="fad36-116">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="fad36-116">educationExternalSource</span></span>| <span data-ttu-id="fad36-117">从在其中创建此组织的源。</span><span class="sxs-lookup"><span data-stu-id="fad36-117">Source where this organization was created from.</span></span> <span data-ttu-id="fad36-118">可能的值为： `sis`， `manual`， `unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="fad36-118">The possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fad36-119">Relationships</span><span class="sxs-lookup"><span data-stu-id="fad36-119">Relationships</span></span>
<span data-ttu-id="fad36-120">无。</span><span class="sxs-lookup"><span data-stu-id="fad36-120">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="fad36-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fad36-121">JSON representation</span></span>

<span data-ttu-id="fad36-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fad36-122">The following is a JSON representation of the resource.</span></span>

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
