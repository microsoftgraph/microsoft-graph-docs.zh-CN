---
title: educationExcelResource 资源类型
description: 'EducationResource 的子类。 此资源类型代表一个 Excel 文档。  '
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 96fc84227bc7c8e5140ef06ce62ea2d485badab7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095518"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="2f3f5-104">educationExcelResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f3f5-104">educationExcelResource resource type</span></span>

<span data-ttu-id="2f3f5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f3f5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f3f5-106">[EducationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="2f3f5-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="2f3f5-107">此资源类型代表一个 Excel 文档。</span><span class="sxs-lookup"><span data-stu-id="2f3f5-107">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="2f3f5-108">**注意：** Excel 文件必须位于与此资源所属的 "分配" 或 "提交" 对象相关联的资源文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2f3f5-108">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="2f3f5-109">属性</span><span class="sxs-lookup"><span data-stu-id="2f3f5-109">Properties</span></span>
| <span data-ttu-id="2f3f5-110">属性</span><span class="sxs-lookup"><span data-stu-id="2f3f5-110">Property</span></span>     | <span data-ttu-id="2f3f5-111">类型</span><span class="sxs-lookup"><span data-stu-id="2f3f5-111">Type</span></span>   |<span data-ttu-id="2f3f5-112">说明</span><span class="sxs-lookup"><span data-stu-id="2f3f5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f3f5-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="2f3f5-113">fileUrl</span></span>|<span data-ttu-id="2f3f5-114">字符串</span><span class="sxs-lookup"><span data-stu-id="2f3f5-114">String</span></span>|<span data-ttu-id="2f3f5-115">指向 Excel 文件对象的指针。</span><span class="sxs-lookup"><span data-stu-id="2f3f5-115">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f3f5-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f3f5-116">JSON representation</span></span>

<span data-ttu-id="2f3f5-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f3f5-117">The following is a JSON representation of the resource.</span></span>

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


