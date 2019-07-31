---
title: educationExcelResource 资源类型
description: 'EducationResource 的子类。 此资源类型代表一个 Excel 文档。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: ef85a92b2629e8a652ce59210018725d6afecb9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972741"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="b3dc3-104">educationExcelResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3dc3-104">educationExcelResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b3dc3-105">[EducationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="b3dc3-105">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="b3dc3-106">此资源类型代表一个 Excel 文档。</span><span class="sxs-lookup"><span data-stu-id="b3dc3-106">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="b3dc3-107">**注意:** Excel 文件必须位于与此资源所属的 "分配" 或 "提交" 对象相关联的资源文件夹中。</span><span class="sxs-lookup"><span data-stu-id="b3dc3-107">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="b3dc3-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3dc3-108">Properties</span></span>
| <span data-ttu-id="b3dc3-109">属性</span><span class="sxs-lookup"><span data-stu-id="b3dc3-109">Property</span></span>     | <span data-ttu-id="b3dc3-110">类型</span><span class="sxs-lookup"><span data-stu-id="b3dc3-110">Type</span></span>   |<span data-ttu-id="b3dc3-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3dc3-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3dc3-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="b3dc3-112">fileUrl</span></span>|<span data-ttu-id="b3dc3-113">String</span><span class="sxs-lookup"><span data-stu-id="b3dc3-113">String</span></span>|<span data-ttu-id="b3dc3-114">指向 Excel 文件对象的指针。</span><span class="sxs-lookup"><span data-stu-id="b3dc3-114">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b3dc3-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3dc3-115">JSON representation</span></span>

<span data-ttu-id="b3dc3-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3dc3-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
