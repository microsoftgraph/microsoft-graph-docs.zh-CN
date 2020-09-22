---
title: educationAssignmentResource 资源类型
description: 一个包装对象，该对象存储与工作分配相关联的资源。 该包装添加了 **distributeForStudentWork** 属性，并指示该资源将
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 462433a24b8515146303505865b3d356d025d6c4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095546"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="e0456-104">educationAssignmentResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="e0456-104">educationAssignmentResource resource type</span></span>

<span data-ttu-id="e0456-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0456-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e0456-106">一个包装对象，该对象存储与工作分配相关联的资源。</span><span class="sxs-lookup"><span data-stu-id="e0456-106">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="e0456-107">该包装将添加 **distributeForStudentWork** 属性，并指示该资源将被复制到学生提交。</span><span class="sxs-lookup"><span data-stu-id="e0456-107">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="e0456-108">如果不复制该对象，则每个学生都将看到该工作分配的资源的链接。</span><span class="sxs-lookup"><span data-stu-id="e0456-108">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="e0456-109">学生将不能更新此资源。</span><span class="sxs-lookup"><span data-stu-id="e0456-109">The student will not be able to update this resource.</span></span> <span data-ttu-id="e0456-110">这是教师向学生提供的讲义，无需将其打开。</span><span class="sxs-lookup"><span data-stu-id="e0456-110">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="e0456-111">如果分配资源，每个学生都会在其提交的资源列表中收到此资源的副本。</span><span class="sxs-lookup"><span data-stu-id="e0456-111">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="e0456-112">每个学生都可以修改其副本并将其提交到评分。</span><span class="sxs-lookup"><span data-stu-id="e0456-112">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="e0456-113">方法</span><span class="sxs-lookup"><span data-stu-id="e0456-113">Methods</span></span>

| <span data-ttu-id="e0456-114">方法</span><span class="sxs-lookup"><span data-stu-id="e0456-114">Method</span></span>           | <span data-ttu-id="e0456-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="e0456-115">Return Type</span></span>    |<span data-ttu-id="e0456-116">说明</span><span class="sxs-lookup"><span data-stu-id="e0456-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e0456-117">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e0456-117">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="e0456-118">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e0456-118">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="e0456-119">读取 **educationAssignmentResource** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e0456-119">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="e0456-120">更新</span><span class="sxs-lookup"><span data-stu-id="e0456-120">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="e0456-121">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="e0456-121">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="e0456-122">更新 **educationAssignmentResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="e0456-122">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="e0456-123">删除</span><span class="sxs-lookup"><span data-stu-id="e0456-123">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="e0456-124">无</span><span class="sxs-lookup"><span data-stu-id="e0456-124">None</span></span> |<span data-ttu-id="e0456-125">删除 **educationAssignmentResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="e0456-125">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e0456-126">属性</span><span class="sxs-lookup"><span data-stu-id="e0456-126">Properties</span></span>
| <span data-ttu-id="e0456-127">属性</span><span class="sxs-lookup"><span data-stu-id="e0456-127">Property</span></span>     | <span data-ttu-id="e0456-128">类型</span><span class="sxs-lookup"><span data-stu-id="e0456-128">Type</span></span>   |<span data-ttu-id="e0456-129">说明</span><span class="sxs-lookup"><span data-stu-id="e0456-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e0456-130">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="e0456-130">distributeForStudentWork</span></span>|<span data-ttu-id="e0456-131">布尔</span><span class="sxs-lookup"><span data-stu-id="e0456-131">Boolean</span></span>|<span data-ttu-id="e0456-132">指示是否应将此资源复制到每个提交的学生进行修改和提交。</span><span class="sxs-lookup"><span data-stu-id="e0456-132">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="e0456-133">id</span><span class="sxs-lookup"><span data-stu-id="e0456-133">id</span></span>|<span data-ttu-id="e0456-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e0456-134">String</span></span>| <span data-ttu-id="e0456-135">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="e0456-135">ID of this resource.</span></span> <span data-ttu-id="e0456-136">只读。</span><span class="sxs-lookup"><span data-stu-id="e0456-136">Read-only.</span></span>|
|<span data-ttu-id="e0456-137">resource</span><span class="sxs-lookup"><span data-stu-id="e0456-137">resource</span></span>|[<span data-ttu-id="e0456-138">educationResource</span><span class="sxs-lookup"><span data-stu-id="e0456-138">educationResource</span></span>](educationresource.md)|<span data-ttu-id="e0456-139">与此工作分配相关联的资源对象。</span><span class="sxs-lookup"><span data-stu-id="e0456-139">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e0456-140">关系</span><span class="sxs-lookup"><span data-stu-id="e0456-140">Relationships</span></span>
<span data-ttu-id="e0456-141">无。</span><span class="sxs-lookup"><span data-stu-id="e0456-141">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e0456-142">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e0456-142">JSON representation</span></span>

<span data-ttu-id="e0456-143">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0456-143">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentResource"
}-->

```json
{
  "distributeForStudentWork": true,
  "id": "String (identifier)",
  "resource": {"@odata.type": "microsoft.graph.educationResource"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


