---
title: companyDetail 资源类型
description: companyDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 93b5490048c149ca526a9c3d0024175c1c20d7e7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48033928"
---
# <a name="companydetail-resource-type"></a><span data-ttu-id="af051-103">companyDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="af051-103">companyDetail resource type</span></span>

<span data-ttu-id="af051-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af051-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af051-105">表示有关与其 [配置文件](profile.md)中的实体相关的公司的信息。</span><span class="sxs-lookup"><span data-stu-id="af051-105">Represents information about companies related to entities within their [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="af051-106">属性</span><span class="sxs-lookup"><span data-stu-id="af051-106">Properties</span></span>

| <span data-ttu-id="af051-107">属性</span><span class="sxs-lookup"><span data-stu-id="af051-107">Property</span></span>       | <span data-ttu-id="af051-108">类型</span><span class="sxs-lookup"><span data-stu-id="af051-108">Type</span></span>                                | <span data-ttu-id="af051-109">说明</span><span class="sxs-lookup"><span data-stu-id="af051-109">Description</span></span>                                 |
|:---------------|:------------------------------------|:--------------------------------------------|
|<span data-ttu-id="af051-110">address</span><span class="sxs-lookup"><span data-stu-id="af051-110">address</span></span>         |[<span data-ttu-id="af051-111">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="af051-111">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="af051-112">公司的地址。</span><span class="sxs-lookup"><span data-stu-id="af051-112">Address of the company.</span></span>                     |
|<span data-ttu-id="af051-113">department</span><span class="sxs-lookup"><span data-stu-id="af051-113">department</span></span>      |<span data-ttu-id="af051-114">String</span><span class="sxs-lookup"><span data-stu-id="af051-114">String</span></span>                               | <span data-ttu-id="af051-115">公司内的部门名称。</span><span class="sxs-lookup"><span data-stu-id="af051-115">Department Name within a company.</span></span>           |
|<span data-ttu-id="af051-116">displayName</span><span class="sxs-lookup"><span data-stu-id="af051-116">displayName</span></span>     |<span data-ttu-id="af051-117">String</span><span class="sxs-lookup"><span data-stu-id="af051-117">String</span></span>                               | <span data-ttu-id="af051-118">公司名称。</span><span class="sxs-lookup"><span data-stu-id="af051-118">Company name.</span></span>                               |
|<span data-ttu-id="af051-119">officeLocation</span><span class="sxs-lookup"><span data-stu-id="af051-119">officeLocation</span></span>  |<span data-ttu-id="af051-120">String</span><span class="sxs-lookup"><span data-stu-id="af051-120">String</span></span>                               | <span data-ttu-id="af051-121">所引用人员的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="af051-121">Office Location of the person referred to.</span></span>  |
|<span data-ttu-id="af051-122">拼音</span><span class="sxs-lookup"><span data-stu-id="af051-122">pronunciation</span></span>   |<span data-ttu-id="af051-123">String</span><span class="sxs-lookup"><span data-stu-id="af051-123">String</span></span>                               | <span data-ttu-id="af051-124">公司名称的发音指南。</span><span class="sxs-lookup"><span data-stu-id="af051-124">Pronunciation guide for the company name.</span></span>   |
|<span data-ttu-id="af051-125">WebUrl</span><span class="sxs-lookup"><span data-stu-id="af051-125">webUrl</span></span>          |<span data-ttu-id="af051-126">String</span><span class="sxs-lookup"><span data-stu-id="af051-126">String</span></span>                               | <span data-ttu-id="af051-127">链接到公司主页。</span><span class="sxs-lookup"><span data-stu-id="af051-127">Link to the company home page.</span></span>              |

## <a name="json-representation"></a><span data-ttu-id="af051-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af051-128">JSON representation</span></span>

<span data-ttu-id="af051-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af051-129">The following is a JSON representation of the resource.</span></span>

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

