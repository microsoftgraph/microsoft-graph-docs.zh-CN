---
title: educationFileResource 资源类型
description: 代表与分配或提交相关联的 file 对象的 educationResource 的子类。  在这种情况下，该文件不是特殊文件（Word、Excel 等）之一，而是在系统中没有特殊处理的文件。 文件资源必须存储在与此资源附加到的工作分配或提交相关联的**resourceFolder**中。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d232e664cd7977f0f62d40adebeabaa357ea362d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502037"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="18e29-105">educationFileResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="18e29-105">educationFileResource resource type</span></span>

<span data-ttu-id="18e29-106">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="18e29-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18e29-107">代表与分配或提交相关联的 file 对象的[educationResource](educationresource.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="18e29-107">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>  <span data-ttu-id="18e29-108">在这种情况下，该文件不是特殊文件（Word、Excel 等）之一，而是在系统中没有特殊处理的文件。</span><span class="sxs-lookup"><span data-stu-id="18e29-108">In this case, the file is not one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="18e29-109">文件资源必须存储在与此资源附加到的工作分配或提交相关联的**resourceFolder**中。</span><span class="sxs-lookup"><span data-stu-id="18e29-109">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="18e29-110">属性</span><span class="sxs-lookup"><span data-stu-id="18e29-110">Properties</span></span>
| <span data-ttu-id="18e29-111">属性</span><span class="sxs-lookup"><span data-stu-id="18e29-111">Property</span></span>     | <span data-ttu-id="18e29-112">类型</span><span class="sxs-lookup"><span data-stu-id="18e29-112">Type</span></span>   |<span data-ttu-id="18e29-113">说明</span><span class="sxs-lookup"><span data-stu-id="18e29-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="18e29-114">fileUrl</span><span class="sxs-lookup"><span data-stu-id="18e29-114">fileUrl</span></span>|<span data-ttu-id="18e29-115">String</span><span class="sxs-lookup"><span data-stu-id="18e29-115">String</span></span>|<span data-ttu-id="18e29-116">文件资源在磁盘上的位置。</span><span class="sxs-lookup"><span data-stu-id="18e29-116">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18e29-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="18e29-117">JSON representation</span></span>

<span data-ttu-id="18e29-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="18e29-118">The following is a JSON representation of the resource.</span></span>

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
