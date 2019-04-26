---
title: educationWordResource 资源类型
description: 'educationResource 的子类。 这是 Word 文档资源。 必须将 Word 文件上载到与**fileResource**目录关联的 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 9bd9af22c141991efd85fc240a002b5c7a0eac3b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340193"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="a8637-105">educationWordResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8637-105">educationWordResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8637-106">[educationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="a8637-106">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="a8637-107">这是 Word 文档资源。</span><span class="sxs-lookup"><span data-stu-id="a8637-107">This is a Word document resource.</span></span> <span data-ttu-id="a8637-108">必须在与分配或提交相关联的**fileResource**目录中上载 Word 文件。</span><span class="sxs-lookup"><span data-stu-id="a8637-108">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="a8637-109">属性</span><span class="sxs-lookup"><span data-stu-id="a8637-109">Properties</span></span>
| <span data-ttu-id="a8637-110">属性</span><span class="sxs-lookup"><span data-stu-id="a8637-110">Property</span></span>     | <span data-ttu-id="a8637-111">类型</span><span class="sxs-lookup"><span data-stu-id="a8637-111">Type</span></span>   |<span data-ttu-id="a8637-112">说明</span><span class="sxs-lookup"><span data-stu-id="a8637-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8637-113">fileUrl</span><span class="sxs-lookup"><span data-stu-id="a8637-113">fileUrl</span></span>|<span data-ttu-id="a8637-114">String</span><span class="sxs-lookup"><span data-stu-id="a8637-114">String</span></span>|<span data-ttu-id="a8637-115">文件在磁盘上的位置。</span><span class="sxs-lookup"><span data-stu-id="a8637-115">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8637-116">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8637-116">JSON representation</span></span>

<span data-ttu-id="a8637-117">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8637-117">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
