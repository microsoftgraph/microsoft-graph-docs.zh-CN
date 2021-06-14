---
title: educationPowerPointResource 资源类型
description: educationResource 的子类。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 860387ea966061077929781f667a9cac5d3d2107
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912309"
---
# <a name="educationpowerpointresource-resource-type"></a><span data-ttu-id="febd8-103">educationPowerPointResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="febd8-103">educationPowerPointResource resource type</span></span>

<span data-ttu-id="febd8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="febd8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="febd8-105">educationResource 的 [子类](educationresource.md)。</span><span class="sxs-lookup"><span data-stu-id="febd8-105">A subclass of [educationResource](educationresource.md).</span></span> 

<span data-ttu-id="febd8-106">这是一个PowerPoint资源。</span><span class="sxs-lookup"><span data-stu-id="febd8-106">This is a PowerPoint resource.</span></span> <span data-ttu-id="febd8-107">必须将PowerPoint文件上传到与作业或提交关联的 **fileResource** 目录中。</span><span class="sxs-lookup"><span data-stu-id="febd8-107">The PowerPoint file must be uploaded in the **fileResource** directory associated with the assignment or submission.</span></span>


## <a name="properties"></a><span data-ttu-id="febd8-108">属性</span><span class="sxs-lookup"><span data-stu-id="febd8-108">Properties</span></span>
| <span data-ttu-id="febd8-109">属性</span><span class="sxs-lookup"><span data-stu-id="febd8-109">Property</span></span>     | <span data-ttu-id="febd8-110">类型</span><span class="sxs-lookup"><span data-stu-id="febd8-110">Type</span></span>   |<span data-ttu-id="febd8-111">说明</span><span class="sxs-lookup"><span data-stu-id="febd8-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="febd8-112">fileUrl</span><span class="sxs-lookup"><span data-stu-id="febd8-112">fileUrl</span></span>|<span data-ttu-id="febd8-113">String</span><span class="sxs-lookup"><span data-stu-id="febd8-113">String</span></span>|<span data-ttu-id="febd8-114">文件在磁盘上的位置。</span><span class="sxs-lookup"><span data-stu-id="febd8-114">Location of the file on disk.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="febd8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="febd8-115">JSON representation</span></span>

<span data-ttu-id="febd8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="febd8-116">The following is a JSON representation of the resource.</span></span>

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


