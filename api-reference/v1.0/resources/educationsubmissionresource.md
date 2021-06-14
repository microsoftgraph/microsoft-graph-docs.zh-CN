---
title: educationSubmissionResource 资源类型
description: 用于提交的资源的包装器。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: d370e930e69e4dff93cbd22efb3104a9511cf880
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912170"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="14579-103">educationSubmissionResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="14579-103">educationSubmissionResource resource type</span></span>

<span data-ttu-id="14579-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14579-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="14579-105">用于提交的资源的包装器。</span><span class="sxs-lookup"><span data-stu-id="14579-105">A wrapper around a resource for use on a submission.</span></span> 

<span data-ttu-id="14579-106">如果从工作分配复制了工作分配资源，包装器会添加一个指向该分配资源的指针。</span><span class="sxs-lookup"><span data-stu-id="14579-106">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="14579-107">方法</span><span class="sxs-lookup"><span data-stu-id="14579-107">Methods</span></span>

| <span data-ttu-id="14579-108">方法</span><span class="sxs-lookup"><span data-stu-id="14579-108">Method</span></span>           | <span data-ttu-id="14579-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="14579-109">Return Type</span></span>    |<span data-ttu-id="14579-110">说明</span><span class="sxs-lookup"><span data-stu-id="14579-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="14579-111">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="14579-111">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="14579-112">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="14579-112">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="14579-113">读取 **educationSubmissionResource 对象的属性和** 关系。</span><span class="sxs-lookup"><span data-stu-id="14579-113">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="14579-114">删除</span><span class="sxs-lookup"><span data-stu-id="14579-114">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="14579-115">无</span><span class="sxs-lookup"><span data-stu-id="14579-115">None</span></span> |<span data-ttu-id="14579-116">删除 **educationSubmissionResource** 对象。</span><span class="sxs-lookup"><span data-stu-id="14579-116">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="14579-117">属性</span><span class="sxs-lookup"><span data-stu-id="14579-117">Properties</span></span>
| <span data-ttu-id="14579-118">属性</span><span class="sxs-lookup"><span data-stu-id="14579-118">Property</span></span>     | <span data-ttu-id="14579-119">类型</span><span class="sxs-lookup"><span data-stu-id="14579-119">Type</span></span>   |<span data-ttu-id="14579-120">说明</span><span class="sxs-lookup"><span data-stu-id="14579-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="14579-121">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="14579-121">assignmentResourceUrl</span></span>|<span data-ttu-id="14579-122">String</span><span class="sxs-lookup"><span data-stu-id="14579-122">String</span></span>|<span data-ttu-id="14579-123">指向从其中复制此资源的分配的指针。</span><span class="sxs-lookup"><span data-stu-id="14579-123">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="14579-124">如果为空，则学生已上传资源。</span><span class="sxs-lookup"><span data-stu-id="14579-124">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="14579-125">id</span><span class="sxs-lookup"><span data-stu-id="14579-125">id</span></span>|<span data-ttu-id="14579-126">String</span><span class="sxs-lookup"><span data-stu-id="14579-126">String</span></span>| <span data-ttu-id="14579-127">只读。</span><span class="sxs-lookup"><span data-stu-id="14579-127">Read-only.</span></span>|
|<span data-ttu-id="14579-128">resource</span><span class="sxs-lookup"><span data-stu-id="14579-128">resource</span></span>|[<span data-ttu-id="14579-129">educationResource</span><span class="sxs-lookup"><span data-stu-id="14579-129">educationResource</span></span>](educationresource.md)|<span data-ttu-id="14579-130">Resource 对象。</span><span class="sxs-lookup"><span data-stu-id="14579-130">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="14579-131">关系</span><span class="sxs-lookup"><span data-stu-id="14579-131">Relationships</span></span>
<span data-ttu-id="14579-132">无</span><span class="sxs-lookup"><span data-stu-id="14579-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="14579-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="14579-133">JSON representation</span></span>

<span data-ttu-id="14579-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14579-134">The following is a JSON representation of the resource.</span></span>

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


