---
title: positionDetail 资源类型
description: positionDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 6c77c116f013000ec4d419ec20c1e45c07187a22
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521591"
---
# <a name="positiondetail-resource-type"></a><span data-ttu-id="d66ab-103">positionDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d66ab-103">positionDetail resource type</span></span>

<span data-ttu-id="d66ab-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d66ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d66ab-105">表示有关与用户[配置文件](profile.md)中的实体相关的位置的信息。</span><span class="sxs-lookup"><span data-stu-id="d66ab-105">Represents information about positions related to entities within a user's [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d66ab-106">属性</span><span class="sxs-lookup"><span data-stu-id="d66ab-106">Properties</span></span>

| <span data-ttu-id="d66ab-107">属性</span><span class="sxs-lookup"><span data-stu-id="d66ab-107">Property</span></span>       | <span data-ttu-id="d66ab-108">类型</span><span class="sxs-lookup"><span data-stu-id="d66ab-108">Type</span></span>                             | <span data-ttu-id="d66ab-109">说明</span><span class="sxs-lookup"><span data-stu-id="d66ab-109">Description</span></span>                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|<span data-ttu-id="d66ab-110">公司</span><span class="sxs-lookup"><span data-stu-id="d66ab-110">company</span></span>         |[<span data-ttu-id="d66ab-111">companyDetail</span><span class="sxs-lookup"><span data-stu-id="d66ab-111">companyDetail</span></span>](companydetail.md) | <span data-ttu-id="d66ab-112">有关公司或雇主的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d66ab-112">Detail about the company or employer.</span></span>                  |
|<span data-ttu-id="d66ab-113">说明</span><span class="sxs-lookup"><span data-stu-id="d66ab-113">description</span></span>     |<span data-ttu-id="d66ab-114">String</span><span class="sxs-lookup"><span data-stu-id="d66ab-114">String</span></span>                            | <span data-ttu-id="d66ab-115">相关职位的描述。</span><span class="sxs-lookup"><span data-stu-id="d66ab-115">Description of the position in question.</span></span>               |
|<span data-ttu-id="d66ab-116">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="d66ab-116">endMonthYear</span></span>    |<span data-ttu-id="d66ab-117">日期</span><span class="sxs-lookup"><span data-stu-id="d66ab-117">Date</span></span>                              | <span data-ttu-id="d66ab-118">位置结束时。</span><span class="sxs-lookup"><span data-stu-id="d66ab-118">When the position ended.</span></span>                               |
|<span data-ttu-id="d66ab-119">jobTitle</span><span class="sxs-lookup"><span data-stu-id="d66ab-119">jobTitle</span></span>        |<span data-ttu-id="d66ab-120">String</span><span class="sxs-lookup"><span data-stu-id="d66ab-120">String</span></span>                            | <span data-ttu-id="d66ab-121">在该位置保留的标题。</span><span class="sxs-lookup"><span data-stu-id="d66ab-121">The title held when in that position.</span></span>                  |
|<span data-ttu-id="d66ab-122">role</span><span class="sxs-lookup"><span data-stu-id="d66ab-122">role</span></span>            |<span data-ttu-id="d66ab-123">String</span><span class="sxs-lookup"><span data-stu-id="d66ab-123">String</span></span>                            | <span data-ttu-id="d66ab-124">位置 entailed 的角色。</span><span class="sxs-lookup"><span data-stu-id="d66ab-124">The role the position entailed.</span></span>                        |
|<span data-ttu-id="d66ab-125">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="d66ab-125">startMonthYear</span></span>  |<span data-ttu-id="d66ab-126">日期</span><span class="sxs-lookup"><span data-stu-id="d66ab-126">Date</span></span>                              | <span data-ttu-id="d66ab-127">开始月份和位置的年。</span><span class="sxs-lookup"><span data-stu-id="d66ab-127">The start month and year of the position.</span></span>              |
|<span data-ttu-id="d66ab-128">摘要</span><span class="sxs-lookup"><span data-stu-id="d66ab-128">summary</span></span>         |<span data-ttu-id="d66ab-129">String</span><span class="sxs-lookup"><span data-stu-id="d66ab-129">String</span></span>                            |<span data-ttu-id="d66ab-130">职位的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="d66ab-130">Short summary of the position.</span></span>                          |

## <a name="json-representation"></a><span data-ttu-id="d66ab-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d66ab-131">JSON representation</span></span>

<span data-ttu-id="d66ab-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d66ab-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.positionDetail",
  "baseType": null
}-->

```json
{
  "company": {"@odata.type": "microsoft.graph.companyDetail"},
  "description": "String",
  "endMonthYear": "String (timestamp)",
  "jobTitle": "String",
  "role": "String",
  "startMonthYear": "String (timestamp)",
  "summary": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "positionDetail resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->