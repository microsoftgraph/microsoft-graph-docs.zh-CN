---
title: educationSubmissionResource 资源类型
description: '资源周围的包装, 用于提交。 如果从分配中复制了该包装, 则包装将添加指向该工作分配资源的指针。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 48f4549354603346e39b5e1f6f387b207e2f14ef
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972479"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="1e609-104">educationSubmissionResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e609-104">educationSubmissionResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e609-105">资源周围的包装, 用于提交。</span><span class="sxs-lookup"><span data-stu-id="1e609-105">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="1e609-106">如果从分配中复制了该包装, 则包装将添加指向该工作分配资源的指针。</span><span class="sxs-lookup"><span data-stu-id="1e609-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="1e609-107">方法</span><span class="sxs-lookup"><span data-stu-id="1e609-107">Methods</span></span>

| <span data-ttu-id="1e609-108">方法</span><span class="sxs-lookup"><span data-stu-id="1e609-108">Method</span></span>           | <span data-ttu-id="1e609-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="1e609-109">Return Type</span></span>    |<span data-ttu-id="1e609-110">说明</span><span class="sxs-lookup"><span data-stu-id="1e609-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1e609-111">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="1e609-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="1e609-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="1e609-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="1e609-113">读取**educationSubmissionResource**对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1e609-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="1e609-114">删除</span><span class="sxs-lookup"><span data-stu-id="1e609-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="1e609-115">无</span><span class="sxs-lookup"><span data-stu-id="1e609-115">None</span></span> |<span data-ttu-id="1e609-116">删除**educationSubmissionResource**对象。</span><span class="sxs-lookup"><span data-stu-id="1e609-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="1e609-117">属性</span><span class="sxs-lookup"><span data-stu-id="1e609-117">Properties</span></span>
| <span data-ttu-id="1e609-118">属性</span><span class="sxs-lookup"><span data-stu-id="1e609-118">Property</span></span>     | <span data-ttu-id="1e609-119">类型</span><span class="sxs-lookup"><span data-stu-id="1e609-119">Type</span></span>   |<span data-ttu-id="1e609-120">说明</span><span class="sxs-lookup"><span data-stu-id="1e609-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e609-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="1e609-121">assignmentResourceUrl</span></span>|<span data-ttu-id="1e609-122">String</span><span class="sxs-lookup"><span data-stu-id="1e609-122">String</span></span>|<span data-ttu-id="1e609-123">指向从其复制此资源的工作分配的指针。</span><span class="sxs-lookup"><span data-stu-id="1e609-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="1e609-124">如果为 null, 则学生上传了资源。</span><span class="sxs-lookup"><span data-stu-id="1e609-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="1e609-125">id</span><span class="sxs-lookup"><span data-stu-id="1e609-125">id</span></span>|<span data-ttu-id="1e609-126">String</span><span class="sxs-lookup"><span data-stu-id="1e609-126">String</span></span>| <span data-ttu-id="1e609-127">只读。</span><span class="sxs-lookup"><span data-stu-id="1e609-127">Read-only.</span></span>|
|<span data-ttu-id="1e609-128">resource</span><span class="sxs-lookup"><span data-stu-id="1e609-128">resource</span></span>|[<span data-ttu-id="1e609-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="1e609-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="1e609-130">Resource 对象。</span><span class="sxs-lookup"><span data-stu-id="1e609-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e609-131">关系</span><span class="sxs-lookup"><span data-stu-id="1e609-131">Relationships</span></span>
<span data-ttu-id="1e609-132">无</span><span class="sxs-lookup"><span data-stu-id="1e609-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1e609-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e609-133">JSON representation</span></span>

<span data-ttu-id="1e609-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e609-134">The following is a JSON representation of the resource.</span></span>

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
