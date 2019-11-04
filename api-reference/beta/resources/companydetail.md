---
title: companyDetail 资源类型
description: companyDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 04e33c9fdae1eae811ee88e7cdef95b4b97b2c3f
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37936837"
---
# <a name="companydetail-resource-type"></a><span data-ttu-id="21d9f-103">companyDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="21d9f-103">companyDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21d9f-104">表示有关与其[配置文件](profile.md)中的实体相关的公司的信息。</span><span class="sxs-lookup"><span data-stu-id="21d9f-104">Represents information about companies related to entities within their [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="21d9f-105">属性</span><span class="sxs-lookup"><span data-stu-id="21d9f-105">Properties</span></span>

| <span data-ttu-id="21d9f-106">属性</span><span class="sxs-lookup"><span data-stu-id="21d9f-106">Property</span></span>       | <span data-ttu-id="21d9f-107">类型</span><span class="sxs-lookup"><span data-stu-id="21d9f-107">Type</span></span>                                | <span data-ttu-id="21d9f-108">说明</span><span class="sxs-lookup"><span data-stu-id="21d9f-108">Description</span></span>                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|<span data-ttu-id="21d9f-109">address</span><span class="sxs-lookup"><span data-stu-id="21d9f-109">address</span></span>         |[<span data-ttu-id="21d9f-110">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="21d9f-110">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="21d9f-111">公司的地址。</span><span class="sxs-lookup"><span data-stu-id="21d9f-111">Address of the company.</span></span>                     |
|<span data-ttu-id="21d9f-112">department</span><span class="sxs-lookup"><span data-stu-id="21d9f-112">department</span></span>      |<span data-ttu-id="21d9f-113">字符串</span><span class="sxs-lookup"><span data-stu-id="21d9f-113">String</span></span>                               | <span data-ttu-id="21d9f-114">公司内的部门名称。</span><span class="sxs-lookup"><span data-stu-id="21d9f-114">Department Name within a company.</span></span>           |
|<span data-ttu-id="21d9f-115">displayName</span><span class="sxs-lookup"><span data-stu-id="21d9f-115">displayName</span></span>     |<span data-ttu-id="21d9f-116">String</span><span class="sxs-lookup"><span data-stu-id="21d9f-116">String</span></span>                               | <span data-ttu-id="21d9f-117">公司名称。</span><span class="sxs-lookup"><span data-stu-id="21d9f-117">Company name.</span></span>                               |
|<span data-ttu-id="21d9f-118">officeLocation</span><span class="sxs-lookup"><span data-stu-id="21d9f-118">officeLocation</span></span>  |<span data-ttu-id="21d9f-119">字符串</span><span class="sxs-lookup"><span data-stu-id="21d9f-119">String</span></span>                               | <span data-ttu-id="21d9f-120">所引用人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="21d9f-120">Office Location of the person referred to.</span></span>  |
|<span data-ttu-id="21d9f-121">拼音</span><span class="sxs-lookup"><span data-stu-id="21d9f-121">pronunciation</span></span>   |<span data-ttu-id="21d9f-122">字符串</span><span class="sxs-lookup"><span data-stu-id="21d9f-122">String</span></span>                               | <span data-ttu-id="21d9f-123">公司名称的发音指南。</span><span class="sxs-lookup"><span data-stu-id="21d9f-123">Pronunciation guide for the company name.</span></span>   |
|<span data-ttu-id="21d9f-124">webUrl</span><span class="sxs-lookup"><span data-stu-id="21d9f-124">webUrl</span></span>          |<span data-ttu-id="21d9f-125">String</span><span class="sxs-lookup"><span data-stu-id="21d9f-125">String</span></span>                               | <span data-ttu-id="21d9f-126">链接到公司主页。</span><span class="sxs-lookup"><span data-stu-id="21d9f-126">Link to the company home page.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="21d9f-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="21d9f-127">JSON representation</span></span>

<span data-ttu-id="21d9f-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="21d9f-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.companyDetail",
  "baseType": null
}-->

```json
{
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "department": "String",
  "displayName": "String",
  "officeLocation": "String",
  "pronunciation": "String",
  "webUrl": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "companyDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->