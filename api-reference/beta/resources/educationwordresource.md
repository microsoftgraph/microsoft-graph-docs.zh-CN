---
title: educationWordResource 资源类型
description: 'EducationResource 一个子类。 这是 Word 文档资源。 必须在与关联的**fileResource**目录中上载的 Word 文件 '
ms.openlocfilehash: 28df3278a0d97f440014c342d592d2701b348d94
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046866"
---
# <a name="educationwordresource-resource-type"></a><span data-ttu-id="271fd-105">educationWordResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="271fd-105">educationWordResource resource type</span></span>

> <span data-ttu-id="271fd-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="271fd-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="271fd-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="271fd-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="271fd-108">[EducationResource](educationresource.md)一个子类。</span><span class="sxs-lookup"><span data-stu-id="271fd-108">A subclass of [educationResource](educationresource.md).</span></span> <span data-ttu-id="271fd-109">这是 Word 文档资源。</span><span class="sxs-lookup"><span data-stu-id="271fd-109">This is a Word document resource.</span></span> <span data-ttu-id="271fd-110">必须与工作分配或提交关联的**fileResource**目录中上载的 Word 文件。</span><span class="sxs-lookup"><span data-stu-id="271fd-110">The Word file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="271fd-111">属性</span><span class="sxs-lookup"><span data-stu-id="271fd-111">Properties</span></span>
| <span data-ttu-id="271fd-112">属性</span><span class="sxs-lookup"><span data-stu-id="271fd-112">Property</span></span>     | <span data-ttu-id="271fd-113">类型</span><span class="sxs-lookup"><span data-stu-id="271fd-113">Type</span></span>   |<span data-ttu-id="271fd-114">说明</span><span class="sxs-lookup"><span data-stu-id="271fd-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="271fd-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="271fd-115">fileUrl</span></span>|<span data-ttu-id="271fd-116">字符串</span><span class="sxs-lookup"><span data-stu-id="271fd-116">String</span></span>|<span data-ttu-id="271fd-117">磁盘上的文件的位置。</span><span class="sxs-lookup"><span data-stu-id="271fd-117">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="271fd-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="271fd-118">JSON representation</span></span>

<span data-ttu-id="271fd-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="271fd-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationWordResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->