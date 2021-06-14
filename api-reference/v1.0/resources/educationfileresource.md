---
title: educationFileResource 资源类型
description: educationResource 的子类，表示与作业或提交关联的文件对象。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 814ea6119210184356c561ac4f6a3dee5d3eac10
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912169"
---
# <a name="educationfileresource-resource-type"></a><span data-ttu-id="af358-103">educationFileResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="af358-103">educationFileResource resource type</span></span>

<span data-ttu-id="af358-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af358-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="af358-105">[educationResource](educationresource.md)的子类，表示与作业或提交关联的文件对象。</span><span class="sxs-lookup"><span data-stu-id="af358-105">A subclass of [educationResource](educationresource.md) that represents a file object that is associated with the assignment or submission.</span></span>

<span data-ttu-id="af358-106">在这种情况下，文件不是 Word、 (Excel 等特殊文件之一) 而是在系统中没有特殊处理的文件。</span><span class="sxs-lookup"><span data-stu-id="af358-106">In this case, the file isn't one of the special files (Word, Excel, and so on) but is a file that does not have special handling within the system.</span></span> <span data-ttu-id="af358-107">文件资源必须存储在与此资源所附加到的工作分配或提交关联的 **resourceFolder** 中。</span><span class="sxs-lookup"><span data-stu-id="af358-107">The file resource must be stored in the **resourceFolder** that is associated with the assignment or submission this resource is attached to.</span></span>

## <a name="properties"></a><span data-ttu-id="af358-108">属性</span><span class="sxs-lookup"><span data-stu-id="af358-108">Properties</span></span>
| <span data-ttu-id="af358-109">属性</span><span class="sxs-lookup"><span data-stu-id="af358-109">Property</span></span>     | <span data-ttu-id="af358-110">类型</span><span class="sxs-lookup"><span data-stu-id="af358-110">Type</span></span>   |<span data-ttu-id="af358-111">说明</span><span class="sxs-lookup"><span data-stu-id="af358-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="af358-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="af358-112">fileUrl</span></span>|<span data-ttu-id="af358-113">String</span><span class="sxs-lookup"><span data-stu-id="af358-113">String</span></span>|<span data-ttu-id="af358-114">文件资源的磁盘上的位置。</span><span class="sxs-lookup"><span data-stu-id="af358-114">Location on disk of the file resource.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="af358-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af358-115">JSON representation</span></span>

<span data-ttu-id="af358-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af358-116">The following is a JSON representation of the resource.</span></span>

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


