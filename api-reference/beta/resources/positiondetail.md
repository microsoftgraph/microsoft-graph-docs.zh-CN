---
title: positionDetail 资源类型
description: positionDetail 资源类型
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: f4094da9c3ffc6a000fc0f7954ca8838a2d659af
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939787"
---
# <a name="positiondetail-resource-type"></a><span data-ttu-id="d944f-103">positionDetail 资源类型</span><span class="sxs-lookup"><span data-stu-id="d944f-103">positionDetail resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d944f-104">表示有关与用户[配置文件](profile.md)中的实体相关的位置的信息。</span><span class="sxs-lookup"><span data-stu-id="d944f-104">Represents information about positions related to entities within a user's [profile](profile.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d944f-105">属性</span><span class="sxs-lookup"><span data-stu-id="d944f-105">Properties</span></span>

| <span data-ttu-id="d944f-106">属性</span><span class="sxs-lookup"><span data-stu-id="d944f-106">Property</span></span>       | <span data-ttu-id="d944f-107">类型</span><span class="sxs-lookup"><span data-stu-id="d944f-107">Type</span></span>                             | <span data-ttu-id="d944f-108">描述</span><span class="sxs-lookup"><span data-stu-id="d944f-108">Description</span></span>                                            |
|:---------------|:---------------------------------|:-------------------------------------------------------|
|<span data-ttu-id="d944f-109">公司</span><span class="sxs-lookup"><span data-stu-id="d944f-109">company</span></span>         |[<span data-ttu-id="d944f-110">companyDetail</span><span class="sxs-lookup"><span data-stu-id="d944f-110">companyDetail</span></span>](companydetail.md) | <span data-ttu-id="d944f-111">有关公司或雇主的详细信息。</span><span class="sxs-lookup"><span data-stu-id="d944f-111">Detail about the company or employer.</span></span>                  |
|<span data-ttu-id="d944f-112">description</span><span class="sxs-lookup"><span data-stu-id="d944f-112">description</span></span>     |<span data-ttu-id="d944f-113">字符串</span><span class="sxs-lookup"><span data-stu-id="d944f-113">String</span></span>                            | <span data-ttu-id="d944f-114">相关职位的描述。</span><span class="sxs-lookup"><span data-stu-id="d944f-114">Description of the position in question.</span></span>               |
|<span data-ttu-id="d944f-115">endMonthYear</span><span class="sxs-lookup"><span data-stu-id="d944f-115">endMonthYear</span></span>    |<span data-ttu-id="d944f-116">日期</span><span class="sxs-lookup"><span data-stu-id="d944f-116">Date</span></span>                              | <span data-ttu-id="d944f-117">位置结束时。</span><span class="sxs-lookup"><span data-stu-id="d944f-117">When the position ended.</span></span>                               |
|<span data-ttu-id="d944f-118">jobTitle</span><span class="sxs-lookup"><span data-stu-id="d944f-118">jobTitle</span></span>        |<span data-ttu-id="d944f-119">String</span><span class="sxs-lookup"><span data-stu-id="d944f-119">String</span></span>                            | <span data-ttu-id="d944f-120">在该位置保留的标题。</span><span class="sxs-lookup"><span data-stu-id="d944f-120">The title held when in that position.</span></span>                  |
|<span data-ttu-id="d944f-121">role</span><span class="sxs-lookup"><span data-stu-id="d944f-121">role</span></span>            |<span data-ttu-id="d944f-122">字符串</span><span class="sxs-lookup"><span data-stu-id="d944f-122">String</span></span>                            | <span data-ttu-id="d944f-123">位置 entailed 的角色。</span><span class="sxs-lookup"><span data-stu-id="d944f-123">The role the position entailed.</span></span>                        |
|<span data-ttu-id="d944f-124">startMonthYear</span><span class="sxs-lookup"><span data-stu-id="d944f-124">startMonthYear</span></span>  |<span data-ttu-id="d944f-125">日期</span><span class="sxs-lookup"><span data-stu-id="d944f-125">Date</span></span>                              | <span data-ttu-id="d944f-126">开始月份和位置的年。</span><span class="sxs-lookup"><span data-stu-id="d944f-126">The start month and year of the position.</span></span>              |
|<span data-ttu-id="d944f-127">摘要</span><span class="sxs-lookup"><span data-stu-id="d944f-127">summary</span></span>         |<span data-ttu-id="d944f-128">字符串</span><span class="sxs-lookup"><span data-stu-id="d944f-128">String</span></span>                            |<span data-ttu-id="d944f-129">职位的简短摘要。</span><span class="sxs-lookup"><span data-stu-id="d944f-129">Short summary of the position.</span></span>                          |

## <a name="json-representation"></a><span data-ttu-id="d944f-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d944f-130">JSON representation</span></span>

<span data-ttu-id="d944f-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d944f-131">The following is a JSON representation of the resource.</span></span>

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