---
title: educationAssignmentResource 资源类型
description: 一个包装对象，用于存储与工作分配关联的资源。
localization_priority: Normal
author: sharad-sharma-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d301eb8f0d9b9f13197be01b2bcf3ccf4297fa24
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912327"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="b82ef-103">educationAssignmentResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="b82ef-103">educationAssignmentResource resource type</span></span>

<span data-ttu-id="b82ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b82ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b82ef-105">一个包装对象，用于存储与工作分配关联的资源。</span><span class="sxs-lookup"><span data-stu-id="b82ef-105">A wrapper object that stores the resources associated with an assignment.</span></span> 

<span data-ttu-id="b82ef-106">包装器将 **添加 distributeForStudentWork** 属性，并指示此资源将复制到学生提交。</span><span class="sxs-lookup"><span data-stu-id="b82ef-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="b82ef-107">如果未复制对象，则每个学生将在作业中看到指向资源的链接。</span><span class="sxs-lookup"><span data-stu-id="b82ef-107">If the object isn't copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="b82ef-108">学生将无法更新此资源。</span><span class="sxs-lookup"><span data-stu-id="b82ef-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="b82ef-109">这是教师向学生发的讲义，没有要打开的讲义。</span><span class="sxs-lookup"><span data-stu-id="b82ef-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="b82ef-110">如果分配了资源，则每个学生都将在提交的资源列表中收到此资源的副本。</span><span class="sxs-lookup"><span data-stu-id="b82ef-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="b82ef-111">每个学生将能够修改其副本并提交它进行评分。</span><span class="sxs-lookup"><span data-stu-id="b82ef-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="b82ef-112">方法</span><span class="sxs-lookup"><span data-stu-id="b82ef-112">Methods</span></span>

| <span data-ttu-id="b82ef-113">方法</span><span class="sxs-lookup"><span data-stu-id="b82ef-113">Method</span></span>           | <span data-ttu-id="b82ef-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="b82ef-114">Return Type</span></span>    |<span data-ttu-id="b82ef-115">说明</span><span class="sxs-lookup"><span data-stu-id="b82ef-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b82ef-116">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="b82ef-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="b82ef-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="b82ef-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="b82ef-118">读取 **educationAssignmentResource 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="b82ef-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="b82ef-119">删除</span><span class="sxs-lookup"><span data-stu-id="b82ef-119">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="b82ef-120">无</span><span class="sxs-lookup"><span data-stu-id="b82ef-120">None</span></span> |<span data-ttu-id="b82ef-121">删除 **educationAssignmentResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="b82ef-121">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="b82ef-122">属性</span><span class="sxs-lookup"><span data-stu-id="b82ef-122">Properties</span></span>
| <span data-ttu-id="b82ef-123">属性</span><span class="sxs-lookup"><span data-stu-id="b82ef-123">Property</span></span>     | <span data-ttu-id="b82ef-124">类型</span><span class="sxs-lookup"><span data-stu-id="b82ef-124">Type</span></span>   |<span data-ttu-id="b82ef-125">说明</span><span class="sxs-lookup"><span data-stu-id="b82ef-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b82ef-126">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="b82ef-126">distributeForStudentWork</span></span>|<span data-ttu-id="b82ef-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="b82ef-127">Boolean</span></span>|<span data-ttu-id="b82ef-128">指示是否应该将此资源复制到每个学生提交以进行修改和提交。</span><span class="sxs-lookup"><span data-stu-id="b82ef-128">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="b82ef-129">id</span><span class="sxs-lookup"><span data-stu-id="b82ef-129">id</span></span>|<span data-ttu-id="b82ef-130">String</span><span class="sxs-lookup"><span data-stu-id="b82ef-130">String</span></span>| <span data-ttu-id="b82ef-131">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="b82ef-131">ID of this resource.</span></span> <span data-ttu-id="b82ef-132">只读。</span><span class="sxs-lookup"><span data-stu-id="b82ef-132">Read-only.</span></span>|
|<span data-ttu-id="b82ef-133">resource</span><span class="sxs-lookup"><span data-stu-id="b82ef-133">resource</span></span>|[<span data-ttu-id="b82ef-134">educationResource</span><span class="sxs-lookup"><span data-stu-id="b82ef-134">educationResource</span></span>](educationresource.md)|<span data-ttu-id="b82ef-135">与此工作分配关联的 Resource 对象。</span><span class="sxs-lookup"><span data-stu-id="b82ef-135">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b82ef-136">关系</span><span class="sxs-lookup"><span data-stu-id="b82ef-136">Relationships</span></span>
<span data-ttu-id="b82ef-137">无。</span><span class="sxs-lookup"><span data-stu-id="b82ef-137">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b82ef-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b82ef-138">JSON representation</span></span>

<span data-ttu-id="b82ef-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b82ef-139">The following is a JSON representation of the resource.</span></span>

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


