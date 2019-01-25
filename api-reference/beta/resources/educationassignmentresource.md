---
title: educationAssignmentResource 资源类型
description: 包装对象，用于存储与工作分配关联的资源。 包装添加**distributeForStudentWork**属性，指示该资源将
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 4d05cf5307e77dc6a7ac438c1bd4f4af4e73784e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529227"
---
# <a name="educationassignmentresource-resource-type"></a><span data-ttu-id="ce4e9-104">educationAssignmentResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="ce4e9-104">educationAssignmentResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce4e9-105">包装对象，用于存储与工作分配关联的资源。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-105">A wrapper object that stores the resources associated with an assignment.</span></span> <span data-ttu-id="ce4e9-106">包装添加**distributeForStudentWork**属性，指示该资源将被复制到学生提交。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-106">The wrapper adds the **distributeForStudentWork** property and indicates that this resource will be copied to the student submission.</span></span>  <span data-ttu-id="ce4e9-107">如果没有复制对象，每个学生工作分配上将显示资源的链接。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-107">If the object is not copied, each student will see a link to the resource on the assignment.</span></span> <span data-ttu-id="ce4e9-108">学生不能以更新此资源。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-108">The student will not be able to update this resource.</span></span> <span data-ttu-id="ce4e9-109">这是与任何打开学生到从教师讲义。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-109">This is a handout from the teacher to the student with nothing to be turned in.</span></span> <span data-ttu-id="ce4e9-110">如果资源分布，每个学生将收到其提交的资源列表中的此资源的副本。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-110">If the resource is distributed, each student will receive a copy of this resource in the resource list of their submission.</span></span> <span data-ttu-id="ce4e9-111">每个学生都将能够修改其副本并将其提交的分级。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-111">Each student will be able to modify their copy and submit it for grading.</span></span>


## <a name="methods"></a><span data-ttu-id="ce4e9-112">方法</span><span class="sxs-lookup"><span data-stu-id="ce4e9-112">Methods</span></span>

| <span data-ttu-id="ce4e9-113">方法</span><span class="sxs-lookup"><span data-stu-id="ce4e9-113">Method</span></span>           | <span data-ttu-id="ce4e9-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="ce4e9-114">Return Type</span></span>    |<span data-ttu-id="ce4e9-115">说明</span><span class="sxs-lookup"><span data-stu-id="ce4e9-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ce4e9-116">获取 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="ce4e9-116">Get educationAssignmentResource</span></span>](../api/educationassignmentresource-get.md) | [<span data-ttu-id="ce4e9-117">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="ce4e9-117">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="ce4e9-118">读取属性和**educationAssignmentResource**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-118">Read properties and relationships of an **educationAssignmentResource** object.</span></span>|
|[<span data-ttu-id="ce4e9-119">Update</span><span class="sxs-lookup"><span data-stu-id="ce4e9-119">Update</span></span>](../api/educationassignmentresource-update.md) | [<span data-ttu-id="ce4e9-120">educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="ce4e9-120">educationAssignmentResource</span></span>](educationassignmentresource.md) |<span data-ttu-id="ce4e9-121">更新**educationAssignmentResource**对象。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-121">Update an **educationAssignmentResource** object.</span></span> |
|[<span data-ttu-id="ce4e9-122">删除</span><span class="sxs-lookup"><span data-stu-id="ce4e9-122">Delete</span></span>](../api/educationassignmentresource-delete.md) | <span data-ttu-id="ce4e9-123">无</span><span class="sxs-lookup"><span data-stu-id="ce4e9-123">None</span></span> |<span data-ttu-id="ce4e9-124">删除**educationAssignmentResource**对象。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-124">Delete an **educationAssignmentResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="ce4e9-125">属性</span><span class="sxs-lookup"><span data-stu-id="ce4e9-125">Properties</span></span>
| <span data-ttu-id="ce4e9-126">属性</span><span class="sxs-lookup"><span data-stu-id="ce4e9-126">Property</span></span>     | <span data-ttu-id="ce4e9-127">类型</span><span class="sxs-lookup"><span data-stu-id="ce4e9-127">Type</span></span>   |<span data-ttu-id="ce4e9-128">说明</span><span class="sxs-lookup"><span data-stu-id="ce4e9-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce4e9-129">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="ce4e9-129">distributeForStudentWork</span></span>|<span data-ttu-id="ce4e9-130">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce4e9-130">Boolean</span></span>|<span data-ttu-id="ce4e9-131">指示是否应将此资源复制到每个学生提交修改和提交。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-131">Indicates whether this resource should be copied to each student submission for modification and submission.</span></span>|
|<span data-ttu-id="ce4e9-132">id</span><span class="sxs-lookup"><span data-stu-id="ce4e9-132">id</span></span>|<span data-ttu-id="ce4e9-133">String</span><span class="sxs-lookup"><span data-stu-id="ce4e9-133">String</span></span>| <span data-ttu-id="ce4e9-134">此资源的 ID。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-134">ID of this resource.</span></span> <span data-ttu-id="ce4e9-135">只读。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-135">Read-only.</span></span>|
|<span data-ttu-id="ce4e9-136">资源</span><span class="sxs-lookup"><span data-stu-id="ce4e9-136">resource</span></span>|[<span data-ttu-id="ce4e9-137">educationResource</span><span class="sxs-lookup"><span data-stu-id="ce4e9-137">educationResource</span></span>](educationresource.md)|<span data-ttu-id="ce4e9-138">已经与此工作分配的资源对象。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-138">Resource object that has been associated with this assignment.</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce4e9-139">关系</span><span class="sxs-lookup"><span data-stu-id="ce4e9-139">Relationships</span></span>
<span data-ttu-id="ce4e9-140">无。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-140">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ce4e9-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ce4e9-141">JSON representation</span></span>

<span data-ttu-id="ce4e9-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ce4e9-142">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
