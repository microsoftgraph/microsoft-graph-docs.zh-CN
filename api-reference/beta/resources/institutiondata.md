---
title: institutionData 资源类型
description: institutionData 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: a528bf5bc8800b10deed2c45d84613b5ab4bd6b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986063"
---
# <a name="institutiondata-resource-type"></a><span data-ttu-id="a84a9-103">institutionData 资源类型</span><span class="sxs-lookup"><span data-stu-id="a84a9-103">institutionData resource type</span></span>

<span data-ttu-id="a84a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a84a9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a84a9-105">代表用户已进行并在 [educationalActivity](educationalActivity.md) 资源中使用的 undergraduate、毕业、postgraduate 学位或其他教学活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="a84a9-105">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="a84a9-106">属性</span><span class="sxs-lookup"><span data-stu-id="a84a9-106">Properties</span></span>

| <span data-ttu-id="a84a9-107">属性</span><span class="sxs-lookup"><span data-stu-id="a84a9-107">Property</span></span>     | <span data-ttu-id="a84a9-108">类型</span><span class="sxs-lookup"><span data-stu-id="a84a9-108">Type</span></span>                                 | <span data-ttu-id="a84a9-109">说明</span><span class="sxs-lookup"><span data-stu-id="a84a9-109">Description</span></span>                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="a84a9-110">说明</span><span class="sxs-lookup"><span data-stu-id="a84a9-110">description</span></span>   |<span data-ttu-id="a84a9-111">String</span><span class="sxs-lookup"><span data-stu-id="a84a9-111">String</span></span>                                |<span data-ttu-id="a84a9-112">用户对其进行研究的机构的简短说明。</span><span class="sxs-lookup"><span data-stu-id="a84a9-112">Short description of the institution the user studied at.</span></span> |
|<span data-ttu-id="a84a9-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a84a9-113">displayName</span></span>   |<span data-ttu-id="a84a9-114">String</span><span class="sxs-lookup"><span data-stu-id="a84a9-114">String</span></span>                                |<span data-ttu-id="a84a9-115">用户在其上研究的机构的名称。</span><span class="sxs-lookup"><span data-stu-id="a84a9-115">Name of the institution the user studied at.</span></span>              |
|<span data-ttu-id="a84a9-116">位置</span><span class="sxs-lookup"><span data-stu-id="a84a9-116">location</span></span>      |[<span data-ttu-id="a84a9-117">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a84a9-117">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="a84a9-118">研究院的地址或位置。</span><span class="sxs-lookup"><span data-stu-id="a84a9-118">Address or location of the institute.</span></span>                     |
|<span data-ttu-id="a84a9-119">webUrl</span><span class="sxs-lookup"><span data-stu-id="a84a9-119">webUrl</span></span>        |<span data-ttu-id="a84a9-120">String</span><span class="sxs-lookup"><span data-stu-id="a84a9-120">String</span></span>                                |<span data-ttu-id="a84a9-121">链接到机构或部门主页。</span><span class="sxs-lookup"><span data-stu-id="a84a9-121">Link to the institution or department homepage.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="a84a9-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a84a9-122">JSON representation</span></span>

<span data-ttu-id="a84a9-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a84a9-123">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.institutionData",
  "baseType": null
}-->

```json
{
  "description": "String",
  "displayName": "String",
  "location": {"@odata.type": "microsoft.graph.physicalAddress"},
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "institutionData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

