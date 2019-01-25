---
title: educationPowerPointResource 资源类型
description: 'EducationResource 一个子类。 这是 PowerPoint 资源。 必须在与关联的**fileResource**目录中上载 PowerPoint 文件 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: b61f210ce0efde36b83632268e12d18d3b96b661
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512197"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="c6a7a-105">educationPowerPointResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="c6a7a-105">educationPowerPointResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c6a7a-106">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="c6a7a-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="c6a7a-107">这是 PowerPoint 资源。</span><span class="sxs-lookup"><span data-stu-id="c6a7a-107">This is a PowerPoint resource.</span></span> <span data-ttu-id="c6a7a-108">必须与工作分配或提交关联的**fileResource**目录中上载 PowerPoint 文件。</span><span class="sxs-lookup"><span data-stu-id="c6a7a-108">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="c6a7a-109">属性</span><span class="sxs-lookup"><span data-stu-id="c6a7a-109">Properties</span></span>
| <span data-ttu-id="c6a7a-110">属性</span><span class="sxs-lookup"><span data-stu-id="c6a7a-110">Property</span></span>     | <span data-ttu-id="c6a7a-111">类型</span><span class="sxs-lookup"><span data-stu-id="c6a7a-111">Type</span></span>   |<span data-ttu-id="c6a7a-112">说明</span><span class="sxs-lookup"><span data-stu-id="c6a7a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6a7a-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="c6a7a-113">fileUrl</span></span>|<span data-ttu-id="c6a7a-114">String</span><span class="sxs-lookup"><span data-stu-id="c6a7a-114">String</span></span>|<span data-ttu-id="c6a7a-115">磁盘上的文件的位置。</span><span class="sxs-lookup"><span data-stu-id="c6a7a-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c6a7a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c6a7a-116">JSON representation</span></span>

<span data-ttu-id="c6a7a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c6a7a-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
}-->

```json
{
  "fileUrl": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationpowerpointresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
