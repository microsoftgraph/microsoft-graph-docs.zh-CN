---
title: educationFileResource 资源类型
description: EducationResource 代表相关联的工作分配或提交文件对象的一个子类。  在这种情况下，文件不是一个特殊的文件 （Word、 Excel 和等等），但没有在系统中的特殊处理文件。 文件资源必须存储在与工作分配或提交此资源附加到关联的**资源**。
localization_priority: Normal
ms.openlocfilehash: 5fda86b80030a2bc0c885b4dd90a384b7ede7fff
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858084"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="54e55-105">educationFileResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="54e55-105">educationFileResource resource type</span></span>

> <span data-ttu-id="54e55-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="54e55-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="54e55-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="54e55-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="54e55-108">[EducationResource](educationresource.md)代表相关联的工作分配或提交文件对象的一个子类。</span><span class="sxs-lookup"><span data-stu-id="54e55-108">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="54e55-109">在这种情况下，文件不是一个特殊的文件 （Word、 Excel 和等等），但没有在系统中的特殊处理文件。</span><span class="sxs-lookup"><span data-stu-id="54e55-109">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="54e55-110">文件资源必须存储在与工作分配或提交此资源附加到关联的**资源**。</span><span class="sxs-lookup"><span data-stu-id="54e55-110">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="54e55-111">属性</span><span class="sxs-lookup"><span data-stu-id="54e55-111">Properties</span></span>
| <span data-ttu-id="54e55-112">属性</span><span class="sxs-lookup"><span data-stu-id="54e55-112">Property</span></span>     | <span data-ttu-id="54e55-113">类型</span><span class="sxs-lookup"><span data-stu-id="54e55-113">Type</span></span>   |<span data-ttu-id="54e55-114">Description</span><span class="sxs-lookup"><span data-stu-id="54e55-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="54e55-115">fileUrl</span><span class="sxs-lookup"><span data-stu-id="54e55-115">fileUrl</span></span>|<span data-ttu-id="54e55-116">字符串</span><span class="sxs-lookup"><span data-stu-id="54e55-116">String</span></span>|<span data-ttu-id="54e55-117">在磁盘上的文件资源的位置。</span><span class="sxs-lookup"><span data-stu-id="54e55-117">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="54e55-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="54e55-118">JSON representation</span></span>

<span data-ttu-id="54e55-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="54e55-119">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationFileResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
