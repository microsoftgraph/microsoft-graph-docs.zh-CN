---
title: educationFileResource 资源类型
description: 代表与分配或提交相关联的 file 对象的 educationResource 的子类。  在这种情况下, 该文件不是特殊文件 (Word、Excel 等) 之一, 而是在系统中没有特殊处理的文件。 文件资源必须存储在与此资源附加到的工作分配或提交相关联的**resourceFolder**中。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9a851c66e137da1941df9b0268657c9e1b7392b3
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334242"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="a220a-105">educationFileResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="a220a-105">educationFileResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a220a-106">代表与分配或提交相关联的 file 对象的[educationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="a220a-106">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="a220a-107">在这种情况下, 该文件不是特殊文件 (Word、Excel 等) 之一, 而是在系统中没有特殊处理的文件。</span><span class="sxs-lookup"><span data-stu-id="a220a-107">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="a220a-108">文件资源必须存储在与此资源附加到的工作分配或提交相关联的**resourceFolder**中。</span><span class="sxs-lookup"><span data-stu-id="a220a-108">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="a220a-109">属性</span><span class="sxs-lookup"><span data-stu-id="a220a-109">Properties</span></span>
| <span data-ttu-id="a220a-110">属性</span><span class="sxs-lookup"><span data-stu-id="a220a-110">Property</span></span>     | <span data-ttu-id="a220a-111">类型</span><span class="sxs-lookup"><span data-stu-id="a220a-111">Type</span></span>   |<span data-ttu-id="a220a-112">说明</span><span class="sxs-lookup"><span data-stu-id="a220a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a220a-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="a220a-113">fileUrl</span></span>|<span data-ttu-id="a220a-114">String</span><span class="sxs-lookup"><span data-stu-id="a220a-114">String</span></span>|<span data-ttu-id="a220a-115">文件资源在磁盘上的位置。</span><span class="sxs-lookup"><span data-stu-id="a220a-115">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a220a-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a220a-116">JSON representation</span></span>

<span data-ttu-id="a220a-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a220a-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
