---
title: educationAssignmentResource 资源类型
description: 一个包装对象, 该对象存储与工作分配相关联的资源。 该包装添加了**distributeForStudentWork**属性, 并指示该资源将
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 08a716edabc31c83a7fb3e358fbafd023d5fa784
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334406"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="4a6c8-104">educationAssignmentResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="4a6c8-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a6c8-105">一个包装对象, 该对象存储与工作分配相关联的资源。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="4a6c8-106">该包装将添加**distributeForStudentWork**属性, 并指示该资源将被复制到学生提交。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="4a6c8-107">如果不复制该对象, 则每个学生都将看到该工作分配的资源的链接。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="4a6c8-108">学生将不能更新此资源。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="4a6c8-109">这是教师向学生提供的讲义, 无需将其打开。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="4a6c8-110">如果分配资源, 每个学生都会在其提交的资源列表中收到此资源的副本。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="4a6c8-111">每个学生都可以修改其副本并将其提交到评分。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="4a6c8-112">方法</span><span class="sxs-lookup"><span data-stu-id="4a6c8-112">Methods</span></span>

| <span data-ttu-id="4a6c8-113">方法</span><span class="sxs-lookup"><span data-stu-id="4a6c8-113">Method</span></span>           | <span data-ttu-id="4a6c8-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="4a6c8-114">Return Type</span></span>    |<span data-ttu-id="4a6c8-115">说明</span><span class="sxs-lookup"><span data-stu-id="4a6c8-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="4a6c8-116">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="4a6c8-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="4a6c8-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="4a6c8-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="4a6c8-118">读取**educationAssignmentResource**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="4a6c8-119">更新</span><span class="sxs-lookup"><span data-stu-id="4a6c8-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="4a6c8-120">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="4a6c8-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="4a6c8-121">更新**educationAssignmentResource**对象。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="4a6c8-122">删除</span><span class="sxs-lookup"><span data-stu-id="4a6c8-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="4a6c8-123">无</span><span class="sxs-lookup"><span data-stu-id="4a6c8-123">None</span></span> |<span data-ttu-id="4a6c8-124">删除**educationAssignmentResource**对象。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="4a6c8-125">属性</span><span class="sxs-lookup"><span data-stu-id="4a6c8-125">Properties</span></span>
| <span data-ttu-id="4a6c8-126">属性</span><span class="sxs-lookup"><span data-stu-id="4a6c8-126">Property</span></span>     | <span data-ttu-id="4a6c8-127">类型</span><span class="sxs-lookup"><span data-stu-id="4a6c8-127">Type</span></span>   |<span data-ttu-id="4a6c8-128">说明</span><span class="sxs-lookup"><span data-stu-id="4a6c8-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a6c8-129">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="4a6c8-129">distributeForStudentWork</span></span>|<span data-ttu-id="4a6c8-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="4a6c8-130">Boolean</span></span>|<span data-ttu-id="4a6c8-131">指示是否应将此资源复制到每个提交的学生进行修改和提交。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="4a6c8-132">id</span><span class="sxs-lookup"><span data-stu-id="4a6c8-132">id</span></span>|<span data-ttu-id="4a6c8-133">String</span><span class="sxs-lookup"><span data-stu-id="4a6c8-133">String</span></span>| <span data-ttu-id="4a6c8-134">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-134">ID of this resource.</span></span> <span data-ttu-id="4a6c8-135">只读。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-135">Read-only.</span></span>|
|<span data-ttu-id="4a6c8-136">resource</span><span class="sxs-lookup"><span data-stu-id="4a6c8-136">resource</span></span>|[<span data-ttu-id="4a6c8-137">educationResource</span><span class="sxs-lookup"><span data-stu-id="4a6c8-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="4a6c8-138">与此工作分配相关联的资源对象。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4a6c8-139">Relationships</span><span class="sxs-lookup"><span data-stu-id="4a6c8-139">Relationships</span></span>
<span data-ttu-id="4a6c8-140">无。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="4a6c8-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4a6c8-141">JSON representation</span></span>

<span data-ttu-id="4a6c8-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4a6c8-142">The following is a JSON representation of the resource.</span></span>

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
