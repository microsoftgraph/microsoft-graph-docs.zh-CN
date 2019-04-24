---
title: educationTerm 资源类型
description: 一个学期。 它表示学年的指定部分。 在 educationClass 中使用。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b5cfe363922fe466eef7a7333ce81249311b4063
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506865"
---
# <a name="educationterm-resource-type"></a><span data-ttu-id="b5b30-105">educationTerm 资源类型</span><span class="sxs-lookup"><span data-stu-id="b5b30-105">educationTerm resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5b30-106">一个学期。</span><span class="sxs-lookup"><span data-stu-id="b5b30-106">A term.</span></span> <span data-ttu-id="b5b30-107">它表示学年的指定部分。</span><span class="sxs-lookup"><span data-stu-id="b5b30-107">This represents a designated portion of the academic year.</span></span> <span data-ttu-id="b5b30-108">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="b5b30-108">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="b5b30-109">属性</span><span class="sxs-lookup"><span data-stu-id="b5b30-109">Properties</span></span>
| <span data-ttu-id="b5b30-110">属性</span><span class="sxs-lookup"><span data-stu-id="b5b30-110">Property</span></span>     | <span data-ttu-id="b5b30-111">类型</span><span class="sxs-lookup"><span data-stu-id="b5b30-111">Type</span></span>   |<span data-ttu-id="b5b30-112">说明</span><span class="sxs-lookup"><span data-stu-id="b5b30-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5b30-113">displayName</span><span class="sxs-lookup"><span data-stu-id="b5b30-113">displayName</span></span>| <span data-ttu-id="b5b30-114">String</span><span class="sxs-lookup"><span data-stu-id="b5b30-114">String</span></span>| <span data-ttu-id="b5b30-115">学期的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b5b30-115">Display name of the term.</span></span>| 
|<span data-ttu-id="b5b30-116">externalId</span><span class="sxs-lookup"><span data-stu-id="b5b30-116">externalId</span></span>|<span data-ttu-id="b5b30-117">String</span><span class="sxs-lookup"><span data-stu-id="b5b30-117">String</span></span>| <span data-ttu-id="b5b30-118">同步系统中的学期 ID。</span><span class="sxs-lookup"><span data-stu-id="b5b30-118">ID of term in the syncing system.</span></span>|
|<span data-ttu-id="b5b30-119">startDate</span><span class="sxs-lookup"><span data-stu-id="b5b30-119">startDate</span></span>|<span data-ttu-id="b5b30-120">日期</span><span class="sxs-lookup"><span data-stu-id="b5b30-120">Date</span></span>|<span data-ttu-id="b5b30-121">学期开始日期。</span><span class="sxs-lookup"><span data-stu-id="b5b30-121">Start of the term.</span></span>|
|<span data-ttu-id="b5b30-122">endDate</span><span class="sxs-lookup"><span data-stu-id="b5b30-122">endDate</span></span>|<span data-ttu-id="b5b30-123">Date</span><span class="sxs-lookup"><span data-stu-id="b5b30-123">Date</span></span>|<span data-ttu-id="b5b30-124">学期结束日期。</span><span class="sxs-lookup"><span data-stu-id="b5b30-124">End of the term.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b5b30-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b5b30-125">JSON representation</span></span>

<span data-ttu-id="b5b30-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5b30-126">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationTerm"
}-->

```json
{
  "displayName": "String",
  "externalId": "String",
  "startDate": "Date",
  "endDate": "Date"
}
```

<!-- uuid: 4e9d671f-3068-4e09-aba2-b39e81a0e452
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationTerm resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationterm.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
