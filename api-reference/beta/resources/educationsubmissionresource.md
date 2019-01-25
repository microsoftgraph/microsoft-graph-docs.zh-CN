---
title: educationSubmissionResource 资源类型
description: '用于在提交资源周围的包装。 包装将指针添加到工作分配的资源，如果这从工作分配复制。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: ef231de49d3871ec877c279b4e77585343e1a85e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522075"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="aed6d-104">educationSubmissionResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="aed6d-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aed6d-105">用于在提交资源周围的包装。</span><span class="sxs-lookup"><span data-stu-id="aed6d-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="aed6d-106">包装将指针添加到工作分配的资源，如果这从工作分配复制。</span><span class="sxs-lookup"><span data-stu-id="aed6d-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="aed6d-107">方法</span><span class="sxs-lookup"><span data-stu-id="aed6d-107">Methods</span></span>

| <span data-ttu-id="aed6d-108">方法</span><span class="sxs-lookup"><span data-stu-id="aed6d-108">Method</span></span>           | <span data-ttu-id="aed6d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="aed6d-109">Return Type</span></span>    |<span data-ttu-id="aed6d-110">说明</span><span class="sxs-lookup"><span data-stu-id="aed6d-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aed6d-111">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="aed6d-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="aed6d-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="aed6d-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="aed6d-113">读取属性和**educationSubmissionResource**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="aed6d-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="aed6d-114">删除</span><span class="sxs-lookup"><span data-stu-id="aed6d-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="aed6d-115">无</span><span class="sxs-lookup"><span data-stu-id="aed6d-115">None</span></span> |<span data-ttu-id="aed6d-116">删除**educationSubmissionResource**对象。</span><span class="sxs-lookup"><span data-stu-id="aed6d-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="aed6d-117">属性</span><span class="sxs-lookup"><span data-stu-id="aed6d-117">Properties</span></span>
| <span data-ttu-id="aed6d-118">属性</span><span class="sxs-lookup"><span data-stu-id="aed6d-118">Property</span></span>     | <span data-ttu-id="aed6d-119">类型</span><span class="sxs-lookup"><span data-stu-id="aed6d-119">Type</span></span>   |<span data-ttu-id="aed6d-120">说明</span><span class="sxs-lookup"><span data-stu-id="aed6d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aed6d-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="aed6d-121">assignmentResourceUrl</span></span>|<span data-ttu-id="aed6d-122">String</span><span class="sxs-lookup"><span data-stu-id="aed6d-122">String</span></span>|<span data-ttu-id="aed6d-123">到从中复制此资源分配的指针。</span><span class="sxs-lookup"><span data-stu-id="aed6d-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="aed6d-124">如果这是 null，则学生上载资源。</span><span class="sxs-lookup"><span data-stu-id="aed6d-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="aed6d-125">id</span><span class="sxs-lookup"><span data-stu-id="aed6d-125">id</span></span>|<span data-ttu-id="aed6d-126">String</span><span class="sxs-lookup"><span data-stu-id="aed6d-126">String</span></span>| <span data-ttu-id="aed6d-127">只读。</span><span class="sxs-lookup"><span data-stu-id="aed6d-127">Read-only.</span></span>|
|<span data-ttu-id="aed6d-128">资源</span><span class="sxs-lookup"><span data-stu-id="aed6d-128">resource</span></span>|[<span data-ttu-id="aed6d-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="aed6d-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="aed6d-130">Resource 对象</span><span class="sxs-lookup"><span data-stu-id="aed6d-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aed6d-131">关系</span><span class="sxs-lookup"><span data-stu-id="aed6d-131">Relationships</span></span>
<span data-ttu-id="aed6d-132">无</span><span class="sxs-lookup"><span data-stu-id="aed6d-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="aed6d-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aed6d-133">JSON representation</span></span>

<span data-ttu-id="aed6d-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aed6d-134">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationSubmissionResource"
}-->

```json
{
  "assignmentResourceUrl": "String",
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationsubmissionresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
