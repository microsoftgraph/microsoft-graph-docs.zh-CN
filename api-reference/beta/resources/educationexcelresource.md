---
title: educationExcelResource 资源类型
description: 'EducationResource 一个子类。 此资源类型表示 Excel 文档。  '
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 7f772f7911667c76e64c31a856f3a9f8b6f3e6ff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858098"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="713a0-104">educationExcelResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="713a0-104">educationExcelResource resource type</span></span>

> <span data-ttu-id="713a0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="713a0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="713a0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="713a0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="713a0-107">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="713a0-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="713a0-108">此资源类型表示 Excel 文档。</span><span class="sxs-lookup"><span data-stu-id="713a0-108">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="713a0-109">**注意：** Excel 文件必须与此资源所属的工作分配或提交对象关联的资源文件夹中。</span><span class="sxs-lookup"><span data-stu-id="713a0-109">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="713a0-110">属性</span><span class="sxs-lookup"><span data-stu-id="713a0-110">Properties</span></span>
| <span data-ttu-id="713a0-111">属性</span><span class="sxs-lookup"><span data-stu-id="713a0-111">Property</span></span>     | <span data-ttu-id="713a0-112">类型</span><span class="sxs-lookup"><span data-stu-id="713a0-112">Type</span></span>   |<span data-ttu-id="713a0-113">Description</span><span class="sxs-lookup"><span data-stu-id="713a0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="713a0-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="713a0-114">fileUrl</span></span>|<span data-ttu-id="713a0-115">字符串</span><span class="sxs-lookup"><span data-stu-id="713a0-115">String</span></span>|<span data-ttu-id="713a0-116">Excel 文件对象的指针。</span><span class="sxs-lookup"><span data-stu-id="713a0-116">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="713a0-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="713a0-117">JSON representation</span></span>

<span data-ttu-id="713a0-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="713a0-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationExcelResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
