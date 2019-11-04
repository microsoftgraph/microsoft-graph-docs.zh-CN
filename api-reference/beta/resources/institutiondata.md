---
title: institutionData 资源类型
description: institutionData 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 5724f56a5e68c059126eaac910d34999dcded632
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939451"
---
# <a name="institutiondata-resource-type"></a><span data-ttu-id="d0a79-103">institutionData 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0a79-103">institutionData resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0a79-104">代表用户已进行并在[educationalActivity](educationalActivity.md)资源中使用的 undergraduate、毕业、postgraduate 学位或其他教学活动的其他详细信息。</span><span class="sxs-lookup"><span data-stu-id="d0a79-104">Represents additional detail about an undergraduate, graduate, postgraduate degree or other educational activity that a user has undertaken and is used within an [educationalActivity](educationalActivity.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="d0a79-105">属性</span><span class="sxs-lookup"><span data-stu-id="d0a79-105">Properties</span></span>

| <span data-ttu-id="d0a79-106">属性</span><span class="sxs-lookup"><span data-stu-id="d0a79-106">Property</span></span>     | <span data-ttu-id="d0a79-107">类型</span><span class="sxs-lookup"><span data-stu-id="d0a79-107">Type</span></span>                                 | <span data-ttu-id="d0a79-108">说明</span><span class="sxs-lookup"><span data-stu-id="d0a79-108">Description</span></span>                                              |
|:-------------|:-------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0a79-109">说明</span><span class="sxs-lookup"><span data-stu-id="d0a79-109">description</span></span>   |<span data-ttu-id="d0a79-110">字符串</span><span class="sxs-lookup"><span data-stu-id="d0a79-110">String</span></span>                                |<span data-ttu-id="d0a79-111">用户对其进行研究的机构的简短说明。</span><span class="sxs-lookup"><span data-stu-id="d0a79-111">Short description of the institution the user studied at.</span></span> |
|<span data-ttu-id="d0a79-112">displayName</span><span class="sxs-lookup"><span data-stu-id="d0a79-112">displayName</span></span>   |<span data-ttu-id="d0a79-113">String</span><span class="sxs-lookup"><span data-stu-id="d0a79-113">String</span></span>                                |<span data-ttu-id="d0a79-114">用户在其上研究的机构的名称。</span><span class="sxs-lookup"><span data-stu-id="d0a79-114">Name of the institution the user studied at.</span></span>              |
|<span data-ttu-id="d0a79-115">位置</span><span class="sxs-lookup"><span data-stu-id="d0a79-115">location</span></span>      |[<span data-ttu-id="d0a79-116">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="d0a79-116">physicalAddress</span></span>](physicaladdress.md) |<span data-ttu-id="d0a79-117">研究院的地址或位置。</span><span class="sxs-lookup"><span data-stu-id="d0a79-117">Address or location of the institute.</span></span>                     |
|<span data-ttu-id="d0a79-118">webUrl</span><span class="sxs-lookup"><span data-stu-id="d0a79-118">webUrl</span></span>        |<span data-ttu-id="d0a79-119">String</span><span class="sxs-lookup"><span data-stu-id="d0a79-119">String</span></span>                                |<span data-ttu-id="d0a79-120">链接到机构或部门主页。</span><span class="sxs-lookup"><span data-stu-id="d0a79-120">Link to the institution or department homepage.</span></span>           |

## <a name="json-representation"></a><span data-ttu-id="d0a79-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0a79-121">JSON representation</span></span>

<span data-ttu-id="d0a79-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0a79-122">The following is a JSON representation of the resource.</span></span>

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