---
title: educationExcelResource 资源类型
description: educationResource 的子类。 此资源类型表示Excel文档。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9345bb39f16066b4c5eee688d781e99563147ef2
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912239"
---
# <a name="educationexcelresource-resource-type"></a><span data-ttu-id="f6a8f-104">educationExcelResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6a8f-104">educationExcelResource resource type</span></span>

<span data-ttu-id="f6a8f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6a8f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f6a8f-106">educationResource 的 [子类](educationresource.md)。</span><span class="sxs-lookup"><span data-stu-id="f6a8f-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="f6a8f-107">此资源类型表示Excel文档。</span><span class="sxs-lookup"><span data-stu-id="f6a8f-107">This resource type represents an Excel document.</span></span>  
 
><span data-ttu-id="f6a8f-108">**注意：** 该Excel文件必须在此资源所属的工作分配或提交对象关联的资源文件夹中。</span><span class="sxs-lookup"><span data-stu-id="f6a8f-108">**Note:** The Excel file must be in the resource folder associated with the assignment or submission object to which this resource belongs.</span></span>


## <a name="properties"></a><span data-ttu-id="f6a8f-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6a8f-109">Properties</span></span>
| <span data-ttu-id="f6a8f-110">属性</span><span class="sxs-lookup"><span data-stu-id="f6a8f-110">Property</span></span>     | <span data-ttu-id="f6a8f-111">类型</span><span class="sxs-lookup"><span data-stu-id="f6a8f-111">Type</span></span>   |<span data-ttu-id="f6a8f-112">说明</span><span class="sxs-lookup"><span data-stu-id="f6a8f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6a8f-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="f6a8f-113">fileUrl</span></span>|<span data-ttu-id="f6a8f-114">String</span><span class="sxs-lookup"><span data-stu-id="f6a8f-114">String</span></span>|<span data-ttu-id="f6a8f-115">指向文件Excel指针。</span><span class="sxs-lookup"><span data-stu-id="f6a8f-115">Pointer to the Excel file object.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f6a8f-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6a8f-116">JSON representation</span></span>

<span data-ttu-id="f6a8f-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6a8f-117">The following is a JSON representation of the resource.</span></span>

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


