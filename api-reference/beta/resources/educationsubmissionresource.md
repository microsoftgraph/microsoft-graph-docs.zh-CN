---
title: educationSubmissionResource 资源类型
description: '用于在提交资源周围的包装。 包装将指针添加到工作分配的资源，如果这从工作分配复制。  '
ms.openlocfilehash: 243d0d8683683df19f7787f7cf6298770950455f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047586"
---
# <a name="educationsubmissionresource-resource-type"></a><span data-ttu-id="52ee2-104">educationSubmissionResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="52ee2-104">educationSubmissionResource resource type</span></span>

> <span data-ttu-id="52ee2-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="52ee2-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52ee2-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="52ee2-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52ee2-107">用于在提交资源周围的包装。</span><span class="sxs-lookup"><span data-stu-id="52ee2-107">A wrapper around a resource for use on a submission.</span></span> <span data-ttu-id="52ee2-108">包装将指针添加到工作分配的资源，如果这从工作分配复制。</span><span class="sxs-lookup"><span data-stu-id="52ee2-108">The wrapper adds a pointer to the assignment resource if this was copied from the assignment.</span></span>  


## <a name="methods"></a><span data-ttu-id="52ee2-109">方法</span><span class="sxs-lookup"><span data-stu-id="52ee2-109">Methods</span></span>

| <span data-ttu-id="52ee2-110">方法</span><span class="sxs-lookup"><span data-stu-id="52ee2-110">Method</span></span>           | <span data-ttu-id="52ee2-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="52ee2-111">Return Type</span></span>    |<span data-ttu-id="52ee2-112">说明</span><span class="sxs-lookup"><span data-stu-id="52ee2-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="52ee2-113">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="52ee2-113">Get educationSubmissionResource</span></span>](../api/educationsubmissionresource-get.md) | [<span data-ttu-id="52ee2-114">educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="52ee2-114">educationSubmissionResource</span></span>](educationsubmissionresource.md) |<span data-ttu-id="52ee2-115">读取属性和**educationSubmissionResource**对象的关系。</span><span class="sxs-lookup"><span data-stu-id="52ee2-115">Read properties and relationships of an **educationSubmissionResource** object.</span></span>|
|[<span data-ttu-id="52ee2-116">删除</span><span class="sxs-lookup"><span data-stu-id="52ee2-116">Delete</span></span>](../api/educationsubmissionresource-delete.md) | <span data-ttu-id="52ee2-117">无</span><span class="sxs-lookup"><span data-stu-id="52ee2-117">None</span></span> |<span data-ttu-id="52ee2-118">删除**educationSubmissionResource**对象。</span><span class="sxs-lookup"><span data-stu-id="52ee2-118">Delete an **educationSubmissionResource** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="52ee2-119">属性</span><span class="sxs-lookup"><span data-stu-id="52ee2-119">Properties</span></span>
| <span data-ttu-id="52ee2-120">属性</span><span class="sxs-lookup"><span data-stu-id="52ee2-120">Property</span></span>     | <span data-ttu-id="52ee2-121">类型</span><span class="sxs-lookup"><span data-stu-id="52ee2-121">Type</span></span>   |<span data-ttu-id="52ee2-122">Description</span><span class="sxs-lookup"><span data-stu-id="52ee2-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="52ee2-123">assignmentResourceUrl</span><span class="sxs-lookup"><span data-stu-id="52ee2-123">assignmentResourceUrl</span></span>|<span data-ttu-id="52ee2-124">字符串</span><span class="sxs-lookup"><span data-stu-id="52ee2-124">String</span></span>|<span data-ttu-id="52ee2-125">到从中复制此资源分配的指针。</span><span class="sxs-lookup"><span data-stu-id="52ee2-125">Pointer to the assignment from which this resource was copied.</span></span> <span data-ttu-id="52ee2-126">如果这是 null，则学生上载资源。</span><span class="sxs-lookup"><span data-stu-id="52ee2-126">If this is null, the student uploaded the resource.</span></span>|
|<span data-ttu-id="52ee2-127">id</span><span class="sxs-lookup"><span data-stu-id="52ee2-127">id</span></span>|<span data-ttu-id="52ee2-128">String</span><span class="sxs-lookup"><span data-stu-id="52ee2-128">String</span></span>| <span data-ttu-id="52ee2-129">只读。</span><span class="sxs-lookup"><span data-stu-id="52ee2-129">Read-only.</span></span>|
|<span data-ttu-id="52ee2-130">resource</span><span class="sxs-lookup"><span data-stu-id="52ee2-130">resource</span></span>|[<span data-ttu-id="52ee2-131">educationResource</span><span class="sxs-lookup"><span data-stu-id="52ee2-131">educationResource</span></span>](educationresource.md)|<span data-ttu-id="52ee2-132">资源对象。</span><span class="sxs-lookup"><span data-stu-id="52ee2-132">Resource object.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52ee2-133">Relationships</span><span class="sxs-lookup"><span data-stu-id="52ee2-133">Relationships</span></span>
<span data-ttu-id="52ee2-134">无</span><span class="sxs-lookup"><span data-stu-id="52ee2-134">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="52ee2-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52ee2-135">JSON representation</span></span>

<span data-ttu-id="52ee2-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52ee2-136">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationSubmissionResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->