---
title: educationAssignmentResource 资源类型
description: 包装对象，用于存储与工作分配关联的资源。 包装添加**distributeForStudentWork**属性，指示该资源将
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: eb0879737d0375bf2463268fe29f2c98f2b6ed51
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991347"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="009e0-104">educationAssignmentResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="009e0-104">educationAssignmentResource resource type</span></span>

> <span data-ttu-id="009e0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="009e0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="009e0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="009e0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="009e0-107">包装对象，用于存储与工作分配关联的资源。</span><span class="sxs-lookup"><span data-stu-id="009e0-107">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="009e0-108">包装添加**distributeForStudentWork**属性，指示该资源将被复制到学生提交。</span><span class="sxs-lookup"><span data-stu-id="009e0-108">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="009e0-109">如果没有复制对象，每个学生工作分配上将显示资源的链接。</span><span class="sxs-lookup"><span data-stu-id="009e0-109">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="009e0-110">学生不能以更新此资源。</span><span class="sxs-lookup"><span data-stu-id="009e0-110">The student will not be able to update this resource.</span></span> <span data-ttu-id="009e0-111">这是与任何打开学生到从教师讲义。</span><span class="sxs-lookup"><span data-stu-id="009e0-111">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="009e0-112">如果资源分布，每个学生将收到其提交的资源列表中的此资源的副本。</span><span class="sxs-lookup"><span data-stu-id="009e0-112">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="009e0-113">每个学生都将能够修改其副本并将其提交的分级。</span><span class="sxs-lookup"><span data-stu-id="009e0-113">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="009e0-114">方法</span><span class="sxs-lookup"><span data-stu-id="009e0-114">Methods</span></span>

| <span data-ttu-id="009e0-115">方法</span><span class="sxs-lookup"><span data-stu-id="009e0-115">Method</span></span>           | <span data-ttu-id="009e0-116">返回类型</span><span class="sxs-lookup"><span data-stu-id="009e0-116">Return Type</span></span>    |<span data-ttu-id="009e0-117">说明</span><span class="sxs-lookup"><span data-stu-id="009e0-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="009e0-118">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="009e0-118">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="009e0-119">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="009e0-119">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="009e0-120">读取属性和**educationAssignmentResource**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="009e0-120">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="009e0-121">更新</span><span class="sxs-lookup"><span data-stu-id="009e0-121">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="009e0-122">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="009e0-122">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="009e0-123">更新**educationAssignmentResource**对象。</span><span class="sxs-lookup"><span data-stu-id="009e0-123">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="009e0-124">删除</span><span class="sxs-lookup"><span data-stu-id="009e0-124">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="009e0-125">无</span><span class="sxs-lookup"><span data-stu-id="009e0-125">None</span></span> |<span data-ttu-id="009e0-126">删除**educationAssignmentResource**对象。</span><span class="sxs-lookup"><span data-stu-id="009e0-126">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="009e0-127">属性</span><span class="sxs-lookup"><span data-stu-id="009e0-127">Properties</span></span>
| <span data-ttu-id="009e0-128">属性</span><span class="sxs-lookup"><span data-stu-id="009e0-128">Property</span></span>     | <span data-ttu-id="009e0-129">类型</span><span class="sxs-lookup"><span data-stu-id="009e0-129">Type</span></span>   |<span data-ttu-id="009e0-130">说明</span><span class="sxs-lookup"><span data-stu-id="009e0-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="009e0-131">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="009e0-131">distributeForStudentWork</span></span>|<span data-ttu-id="009e0-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="009e0-132">Boolean</span></span>|<span data-ttu-id="009e0-133">指示是否应将此资源复制到每个学生提交修改和提交。</span><span class="sxs-lookup"><span data-stu-id="009e0-133">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="009e0-134">id</span><span class="sxs-lookup"><span data-stu-id="009e0-134">id</span></span>|<span data-ttu-id="009e0-135">字符串</span><span class="sxs-lookup"><span data-stu-id="009e0-135">String</span></span>| <span data-ttu-id="009e0-136">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="009e0-136">ID of this resource.</span></span> <span data-ttu-id="009e0-137">只读。</span><span class="sxs-lookup"><span data-stu-id="009e0-137">Read-only.</span></span>|
|<span data-ttu-id="009e0-138">resource</span><span class="sxs-lookup"><span data-stu-id="009e0-138">resource</span></span>|[<span data-ttu-id="009e0-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="009e0-139">educationResource</span></span>](educationresource.md)|<span data-ttu-id="009e0-140">已经与此工作分配的资源对象。</span><span class="sxs-lookup"><span data-stu-id="009e0-140">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="009e0-141">Relationships</span><span class="sxs-lookup"><span data-stu-id="009e0-141">Relationships</span></span>
<span data-ttu-id="009e0-142">无。</span><span class="sxs-lookup"><span data-stu-id="009e0-142">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="009e0-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="009e0-143">JSON representation</span></span>

<span data-ttu-id="009e0-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="009e0-144">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationAssignmentResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
