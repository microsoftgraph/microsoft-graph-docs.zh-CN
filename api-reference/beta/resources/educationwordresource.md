---
title: educationWordResource 资源类型
description: 'EducationResource 一个子类。 这是 Word 文档资源。 必须在与关联的**fileResource**目录中上载的 Word 文件 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9d92b993ab920a894590346bf5fde0ff86c73e8d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529668"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="5f3fb-105">educationWordResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f3fb-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f3fb-106">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="5f3fb-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="5f3fb-107">这是 Word 文档资源。</span><span class="sxs-lookup"><span data-stu-id="5f3fb-107">This is a Word document resource.</span></span> <span data-ttu-id="5f3fb-108">必须与工作分配或提交关联的**fileResource**目录中上载的 Word 文件。</span><span class="sxs-lookup"><span data-stu-id="5f3fb-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="5f3fb-109">属性</span><span class="sxs-lookup"><span data-stu-id="5f3fb-109">Properties</span></span>
| <span data-ttu-id="5f3fb-110">属性</span><span class="sxs-lookup"><span data-stu-id="5f3fb-110">Property</span></span>     | <span data-ttu-id="5f3fb-111">类型</span><span class="sxs-lookup"><span data-stu-id="5f3fb-111">Type</span></span>   |<span data-ttu-id="5f3fb-112">说明</span><span class="sxs-lookup"><span data-stu-id="5f3fb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5f3fb-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="5f3fb-113">fileUrl</span></span>|<span data-ttu-id="5f3fb-114">String</span><span class="sxs-lookup"><span data-stu-id="5f3fb-114">String</span></span>|<span data-ttu-id="5f3fb-115">磁盘上的文件的位置。</span><span class="sxs-lookup"><span data-stu-id="5f3fb-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5f3fb-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f3fb-116">JSON representation</span></span>

<span data-ttu-id="5f3fb-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f3fb-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationWordResource"
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
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationwordresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
