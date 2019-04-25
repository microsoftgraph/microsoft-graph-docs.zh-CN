---
title: educationExcelResource 资源类型
description: 'educationResource 的子类。 此资源类型代表一个 Excel 文档。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 14d7823f166ca12d202a6561bc9fe7b158ab7476
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32542816"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="13787-104">educationExcelResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="13787-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13787-105">[educationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="13787-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="13787-106">此资源类型代表一个 Excel 文档。</span><span class="sxs-lookup"><span data-stu-id="13787-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="13787-107">**注意:** Excel 文件必须位于与此资源所属的 "分配" 或 "提交" 对象相关联的资源文件夹中。</span><span class="sxs-lookup"><span data-stu-id="13787-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="13787-108">属性</span><span class="sxs-lookup"><span data-stu-id="13787-108">Properties</span></span>
| <span data-ttu-id="13787-109">属性</span><span class="sxs-lookup"><span data-stu-id="13787-109">Property</span></span>     | <span data-ttu-id="13787-110">类型</span><span class="sxs-lookup"><span data-stu-id="13787-110">Type</span></span>   |<span data-ttu-id="13787-111">说明</span><span class="sxs-lookup"><span data-stu-id="13787-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="13787-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="13787-112">fileUrl</span></span>|<span data-ttu-id="13787-113">String</span><span class="sxs-lookup"><span data-stu-id="13787-113">String</span></span>|<span data-ttu-id="13787-114">指向 Excel 文件对象的指针。</span><span class="sxs-lookup"><span data-stu-id="13787-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="13787-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13787-115">JSON representation</span></span>

<span data-ttu-id="13787-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13787-116">The following is a JSON representation of the resource.</span></span>

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
