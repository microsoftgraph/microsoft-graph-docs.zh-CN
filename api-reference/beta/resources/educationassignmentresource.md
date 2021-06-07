---
title: educationAssignmentResource 资源类型
description: 一个包装对象，用于存储与工作分配关联的资源。 包装器将添加 **distributeForStudentWork** 属性并指示此资源将
localization_priority: Normal
author: dipakboyed
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: a4f4e96c4b08eed4584d6357a8c903c080b2d16d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750369"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="652b4-104">educationAssignmentResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="652b4-104">educationAssignmentResource resource type</span></span>

<span data-ttu-id="652b4-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="652b4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="652b4-106">一个包装对象，用于存储与工作分配关联的资源。</span><span class="sxs-lookup"><span data-stu-id="652b4-106">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="652b4-107">包装器将 **添加 distributeForStudentWork** 属性，并指示此资源将复制到学生提交。</span><span class="sxs-lookup"><span data-stu-id="652b4-107">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="652b4-108">如果未复制对象，则每个学生将在作业中看到指向资源的链接。</span><span class="sxs-lookup"><span data-stu-id="652b4-108">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="652b4-109">学生将无法更新此资源。</span><span class="sxs-lookup"><span data-stu-id="652b4-109">The student will not be able to update this resource.</span></span> <span data-ttu-id="652b4-110">这是教师向学生发的讲义，没有要打开的讲义。</span><span class="sxs-lookup"><span data-stu-id="652b4-110">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="652b4-111">如果分配了资源，则每个学生都将在提交的资源列表中收到此资源的副本。</span><span class="sxs-lookup"><span data-stu-id="652b4-111">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="652b4-112">每个学生将能够修改其副本并提交它进行评分。</span><span class="sxs-lookup"><span data-stu-id="652b4-112">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="652b4-113">Methods</span><span class="sxs-lookup"><span data-stu-id="652b4-113">Methods</span></span>

| <span data-ttu-id="652b4-114">方法</span><span class="sxs-lookup"><span data-stu-id="652b4-114">Method</span></span>           | <span data-ttu-id="652b4-115">返回类型</span><span class="sxs-lookup"><span data-stu-id="652b4-115">Return Type</span></span>    |<span data-ttu-id="652b4-116">Description</span><span class="sxs-lookup"><span data-stu-id="652b4-116">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="652b4-117">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="652b4-117">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="652b4-118">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="652b4-118">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="652b4-119">读取 **educationAssignmentResource 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="652b4-119">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="652b4-120">删除</span><span class="sxs-lookup"><span data-stu-id="652b4-120">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="652b4-121">无</span><span class="sxs-lookup"><span data-stu-id="652b4-121">None</span></span> |<span data-ttu-id="652b4-122">删除 **educationAssignmentResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="652b4-122">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="652b4-123">属性</span><span class="sxs-lookup"><span data-stu-id="652b4-123">Properties</span></span>
| <span data-ttu-id="652b4-124">属性</span><span class="sxs-lookup"><span data-stu-id="652b4-124">Property</span></span>     | <span data-ttu-id="652b4-125">类型</span><span class="sxs-lookup"><span data-stu-id="652b4-125">Type</span></span>   |<span data-ttu-id="652b4-126">Description</span><span class="sxs-lookup"><span data-stu-id="652b4-126">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="652b4-127">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="652b4-127">distributeForStudentWork</span></span>|<span data-ttu-id="652b4-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="652b4-128">Boolean</span></span>|<span data-ttu-id="652b4-129">指示是否应该将此资源复制到每个学生提交以进行修改和提交。</span><span class="sxs-lookup"><span data-stu-id="652b4-129">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="652b4-130">id</span><span class="sxs-lookup"><span data-stu-id="652b4-130">id</span></span>|<span data-ttu-id="652b4-131">String</span><span class="sxs-lookup"><span data-stu-id="652b4-131">String</span></span>| <span data-ttu-id="652b4-132">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="652b4-132">ID of this resource.</span></span> <span data-ttu-id="652b4-133">只读。</span><span class="sxs-lookup"><span data-stu-id="652b4-133">Read-only.</span></span>|
|<span data-ttu-id="652b4-134">resource</span><span class="sxs-lookup"><span data-stu-id="652b4-134">resource</span></span>|[<span data-ttu-id="652b4-135">educationResource</span><span class="sxs-lookup"><span data-stu-id="652b4-135">educationResource</span></span>](educationresource.md)|<span data-ttu-id="652b4-136">与此工作分配关联的 Resource 对象。</span><span class="sxs-lookup"><span data-stu-id="652b4-136">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="652b4-137">关系</span><span class="sxs-lookup"><span data-stu-id="652b4-137">Relationships</span></span>
<span data-ttu-id="652b4-138">无。</span><span class="sxs-lookup"><span data-stu-id="652b4-138">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="652b4-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="652b4-139">JSON representation</span></span>

<span data-ttu-id="652b4-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="652b4-140">The following is a JSON representation of the resource.</span></span>

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


