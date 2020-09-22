---
title: educationPowerPointResource 资源类型
description: 'EducationResource 的子类。 这是一种 PowerPoint 资源。 必须将 PowerPoint 文件上传到与 **fileResource** 目录关联的 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e7dabc312e0e8db58624651436e8c04f742d51d4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081704"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="573ef-105">educationPowerPointResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="573ef-105">educationPowerPointResource resource type</span></span>

<span data-ttu-id="573ef-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="573ef-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="573ef-107">[EducationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="573ef-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="573ef-108">这是一种 PowerPoint 资源。</span><span class="sxs-lookup"><span data-stu-id="573ef-108">This is a PowerPoint resource.</span></span> <span data-ttu-id="573ef-109">必须在与分配或提交相关联的 **fileResource** 目录中上载 PowerPoint 文件。</span><span class="sxs-lookup"><span data-stu-id="573ef-109">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="573ef-110">属性</span><span class="sxs-lookup"><span data-stu-id="573ef-110">Properties</span></span>
| <span data-ttu-id="573ef-111">属性</span><span class="sxs-lookup"><span data-stu-id="573ef-111">Property</span></span>     | <span data-ttu-id="573ef-112">类型</span><span class="sxs-lookup"><span data-stu-id="573ef-112">Type</span></span>   |<span data-ttu-id="573ef-113">说明</span><span class="sxs-lookup"><span data-stu-id="573ef-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="573ef-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="573ef-114">fileUrl</span></span>|<span data-ttu-id="573ef-115">字符串</span><span class="sxs-lookup"><span data-stu-id="573ef-115">String</span></span>|<span data-ttu-id="573ef-116">文件在磁盘上的位置。</span><span class="sxs-lookup"><span data-stu-id="573ef-116">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="573ef-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="573ef-117">JSON representation</span></span>

<span data-ttu-id="573ef-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="573ef-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationPowerPointResource"
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
  "description": "educationPowerPointResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


