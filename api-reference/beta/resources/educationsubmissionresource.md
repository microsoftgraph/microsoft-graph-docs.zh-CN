---
title: educationSubmissionResource 资源类型
description: '资源周围的包装，用于提交。 如果从分配中复制了该包装，则包装将添加指向该工作分配资源的指针。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 876a490c3dfcf69eb993d1ba18868e2fc5a62fa8
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42500637"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="e4fa5-104">educationSubmissionResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="e4fa5-104">educationSubmissionResource resource type</span></span>

<span data-ttu-id="e4fa5-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e4fa5-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e4fa5-106">资源周围的包装，用于提交。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-106">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="e4fa5-107">如果从分配中复制了该包装，则包装将添加指向该工作分配资源的指针。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-107">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="e4fa5-108">方法</span><span class="sxs-lookup"><span data-stu-id="e4fa5-108">Methods</span></span>

| <span data-ttu-id="e4fa5-109">方法</span><span class="sxs-lookup"><span data-stu-id="e4fa5-109">Method</span></span>           | <span data-ttu-id="e4fa5-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="e4fa5-110">Return Type</span></span>    |<span data-ttu-id="e4fa5-111">说明</span><span class="sxs-lookup"><span data-stu-id="e4fa5-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e4fa5-112">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="e4fa5-112">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="e4fa5-113">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="e4fa5-113">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="e4fa5-114">读取**educationSubmissionResource**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-114">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="e4fa5-115">删除</span><span class="sxs-lookup"><span data-stu-id="e4fa5-115">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="e4fa5-116">无</span><span class="sxs-lookup"><span data-stu-id="e4fa5-116">None</span></span> |<span data-ttu-id="e4fa5-117">删除**educationSubmissionResource**对象。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-117">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="e4fa5-118">属性</span><span class="sxs-lookup"><span data-stu-id="e4fa5-118">Properties</span></span>
| <span data-ttu-id="e4fa5-119">属性</span><span class="sxs-lookup"><span data-stu-id="e4fa5-119">Property</span></span>     | <span data-ttu-id="e4fa5-120">类型</span><span class="sxs-lookup"><span data-stu-id="e4fa5-120">Type</span></span>   |<span data-ttu-id="e4fa5-121">说明</span><span class="sxs-lookup"><span data-stu-id="e4fa5-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e4fa5-122">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="e4fa5-122">assignmentResourceUrl</span></span>|<span data-ttu-id="e4fa5-123">String</span><span class="sxs-lookup"><span data-stu-id="e4fa5-123">String</span></span>|<span data-ttu-id="e4fa5-124">指向从其复制此资源的工作分配的指针。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-124">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="e4fa5-125">如果为 null，则学生上传了资源。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-125">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="e4fa5-126">id</span><span class="sxs-lookup"><span data-stu-id="e4fa5-126">id</span></span>|<span data-ttu-id="e4fa5-127">String</span><span class="sxs-lookup"><span data-stu-id="e4fa5-127">String</span></span>| <span data-ttu-id="e4fa5-128">只读。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-128">Read-only.</span></span>|
|<span data-ttu-id="e4fa5-129">resource</span><span class="sxs-lookup"><span data-stu-id="e4fa5-129">resource</span></span>|[<span data-ttu-id="e4fa5-130">educationResource</span><span class="sxs-lookup"><span data-stu-id="e4fa5-130">educationResource</span></span>](educationresource.md)|<span data-ttu-id="e4fa5-131">Resource 对象。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-131">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4fa5-132">关系</span><span class="sxs-lookup"><span data-stu-id="e4fa5-132">Relationships</span></span>
<span data-ttu-id="e4fa5-133">无</span><span class="sxs-lookup"><span data-stu-id="e4fa5-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e4fa5-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e4fa5-134">JSON representation</span></span>

<span data-ttu-id="e4fa5-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4fa5-135">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
