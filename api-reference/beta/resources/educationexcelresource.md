---
title: educationExcelResource 资源类型
description: 'EducationResource 一个子类。 此资源类型表示 Excel 文档。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 14d7823f166ca12d202a6561bc9fe7b158ab7476
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522418"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="2a74b-104">educationExcelResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="2a74b-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a74b-105">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="2a74b-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="2a74b-106">此资源类型表示 Excel 文档。</span><span class="sxs-lookup"><span data-stu-id="2a74b-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="2a74b-107">**注意：** Excel 文件必须与此资源所属的工作分配或提交对象关联的资源文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2a74b-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="2a74b-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a74b-108">Properties</span></span>
| <span data-ttu-id="2a74b-109">属性</span><span class="sxs-lookup"><span data-stu-id="2a74b-109">Property</span></span>     | <span data-ttu-id="2a74b-110">类型</span><span class="sxs-lookup"><span data-stu-id="2a74b-110">Type</span></span>   |<span data-ttu-id="2a74b-111">说明</span><span class="sxs-lookup"><span data-stu-id="2a74b-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2a74b-112">FileURL</span><span class="sxs-lookup"><span data-stu-id="2a74b-112">fileUrl</span></span>|<span data-ttu-id="2a74b-113">String</span><span class="sxs-lookup"><span data-stu-id="2a74b-113">String</span></span>|<span data-ttu-id="2a74b-114">Excel 文件对象的指针。</span><span class="sxs-lookup"><span data-stu-id="2a74b-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2a74b-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2a74b-115">JSON representation</span></span>

<span data-ttu-id="2a74b-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a74b-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationExcelResource"
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
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationexcelresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
