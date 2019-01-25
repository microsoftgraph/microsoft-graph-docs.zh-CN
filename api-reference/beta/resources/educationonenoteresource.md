---
title: educationOneNoteResource 资源类型
description: 'EducationResource 一个子类。 这表示在 OneNote 页面的位置。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 60b0e4647f1a601d3cbe206e264f7d288ee2110c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521416"
---
# <a name="educationonenoteresource-resource-type"></a><span data-ttu-id="a47fb-104">educationOneNoteResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="a47fb-104">educationOneNoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a47fb-105">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="a47fb-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="a47fb-106">这表示在 OneNote 页面的位置。</span><span class="sxs-lookup"><span data-stu-id="a47fb-106">This represents the location of the OneNote page.</span></span>  

## <a name="properties"></a><span data-ttu-id="a47fb-107">属性</span><span class="sxs-lookup"><span data-stu-id="a47fb-107">Properties</span></span>
| <span data-ttu-id="a47fb-108">属性</span><span class="sxs-lookup"><span data-stu-id="a47fb-108">Property</span></span>     | <span data-ttu-id="a47fb-109">类型</span><span class="sxs-lookup"><span data-stu-id="a47fb-109">Type</span></span>   |<span data-ttu-id="a47fb-110">说明</span><span class="sxs-lookup"><span data-stu-id="a47fb-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a47fb-111">pageUrl</span><span class="sxs-lookup"><span data-stu-id="a47fb-111">pageUrl</span></span>|<span data-ttu-id="a47fb-112">String</span><span class="sxs-lookup"><span data-stu-id="a47fb-112">String</span></span>|<span data-ttu-id="a47fb-113">在 OneNote 中页的 Microsoft Graph URL。</span><span class="sxs-lookup"><span data-stu-id="a47fb-113">The Microsoft Graph URL to the page in OneNote.</span></span>|
|<span data-ttu-id="a47fb-114">sectionName</span><span class="sxs-lookup"><span data-stu-id="a47fb-114">sectionName</span></span>|<span data-ttu-id="a47fb-115">String</span><span class="sxs-lookup"><span data-stu-id="a47fb-115">String</span></span>|<span data-ttu-id="a47fb-116">分配应复制到或已复制到的部分名称。</span><span class="sxs-lookup"><span data-stu-id="a47fb-116">Section name that distributions should be copied into or were copied into.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a47fb-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a47fb-117">JSON representation</span></span>

<span data-ttu-id="a47fb-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a47fb-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationOneNoteResource"
}-->

```json
{
  "pageUrl": "String",
  "sectionName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationOneNoteResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationonenoteresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
