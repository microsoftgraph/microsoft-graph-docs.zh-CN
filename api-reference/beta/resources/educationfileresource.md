---
title: educationFileResource 资源类型
description: EducationResource 代表相关联的工作分配或提交文件对象的一个子类。  在这种情况下，文件不是一个特殊的文件 （Word、 Excel 和等等），但没有在系统中的特殊处理文件。 文件资源必须存储在与工作分配或提交此资源附加到关联的**资源**。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 15ca31576618f15e64b85d860077785160c25989
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520793"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="94914-105">educationFileResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="94914-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94914-106">[EducationResource](educationresource.md)代表相关联的工作分配或提交文件对象的一个子类。</span><span class="sxs-lookup"><span data-stu-id="94914-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="94914-107">在这种情况下，文件不是一个特殊的文件 （Word、 Excel 和等等），但没有在系统中的特殊处理文件。</span><span class="sxs-lookup"><span data-stu-id="94914-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="94914-108">文件资源必须存储在与工作分配或提交此资源附加到关联的**资源**。</span><span class="sxs-lookup"><span data-stu-id="94914-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="94914-109">属性</span><span class="sxs-lookup"><span data-stu-id="94914-109">Properties</span></span>
| <span data-ttu-id="94914-110">属性</span><span class="sxs-lookup"><span data-stu-id="94914-110">Property</span></span>     | <span data-ttu-id="94914-111">类型</span><span class="sxs-lookup"><span data-stu-id="94914-111">Type</span></span>   |<span data-ttu-id="94914-112">说明</span><span class="sxs-lookup"><span data-stu-id="94914-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94914-113">FileURL</span><span class="sxs-lookup"><span data-stu-id="94914-113">fileUrl</span></span>|<span data-ttu-id="94914-114">String</span><span class="sxs-lookup"><span data-stu-id="94914-114">String</span></span>|<span data-ttu-id="94914-115">在磁盘上的文件资源的位置。</span><span class="sxs-lookup"><span data-stu-id="94914-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94914-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94914-116">JSON representation</span></span>

<span data-ttu-id="94914-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94914-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationFileResource"
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
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationfileresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
