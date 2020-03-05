---
title: educationWordResource 资源类型
description: 'EducationResource 的子类。 这是 Word 文档资源。 必须将 Word 文件上载到与**fileResource**目录关联的 '
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 06b1f097199bbf188c0bc0a538fe471b07cdec91
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42499944"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="43f29-105">educationWordResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="43f29-105">educationWordResource resource type</span></span>

<span data-ttu-id="43f29-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="43f29-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43f29-107">[EducationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="43f29-107">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="43f29-108">这是 Word 文档资源。</span><span class="sxs-lookup"><span data-stu-id="43f29-108">This is a Word document resource.</span></span> <span data-ttu-id="43f29-109">必须在与分配或提交相关联的**fileResource**目录中上载 Word 文件。</span><span class="sxs-lookup"><span data-stu-id="43f29-109">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="43f29-110">属性</span><span class="sxs-lookup"><span data-stu-id="43f29-110">Properties</span></span>
| <span data-ttu-id="43f29-111">属性</span><span class="sxs-lookup"><span data-stu-id="43f29-111">Property</span></span>     | <span data-ttu-id="43f29-112">类型</span><span class="sxs-lookup"><span data-stu-id="43f29-112">Type</span></span>   |<span data-ttu-id="43f29-113">说明</span><span class="sxs-lookup"><span data-stu-id="43f29-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43f29-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="43f29-114">fileUrl</span></span>|<span data-ttu-id="43f29-115">String</span><span class="sxs-lookup"><span data-stu-id="43f29-115">String</span></span>|<span data-ttu-id="43f29-116">文件在磁盘上的位置。</span><span class="sxs-lookup"><span data-stu-id="43f29-116">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="43f29-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="43f29-117">JSON representation</span></span>

<span data-ttu-id="43f29-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="43f29-118">The following is a JSON representation of the resource.</span></span>

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
