---
title: printJob 资源类型
description: 代表已对打印机排队的打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 5eff75fba2c9993275c277877fedec7705021c49
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895604"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="a0e2f-103">printJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="a0e2f-103">printJob resource type</span></span>

<span data-ttu-id="a0e2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0e2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0e2f-105">代表已对打印机排队的打印作业。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="a0e2f-106">方法</span><span class="sxs-lookup"><span data-stu-id="a0e2f-106">Methods</span></span>

| <span data-ttu-id="a0e2f-107">方法</span><span class="sxs-lookup"><span data-stu-id="a0e2f-107">Method</span></span>       | <span data-ttu-id="a0e2f-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a0e2f-108">Return Type</span></span> | <span data-ttu-id="a0e2f-109">说明</span><span class="sxs-lookup"><span data-stu-id="a0e2f-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a0e2f-110">Get</span><span class="sxs-lookup"><span data-stu-id="a0e2f-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="a0e2f-111">printJob</span><span class="sxs-lookup"><span data-stu-id="a0e2f-111">printJob</span></span>](printjob.md) | <span data-ttu-id="a0e2f-112">读取 printJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="a0e2f-113">创建</span><span class="sxs-lookup"><span data-stu-id="a0e2f-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="a0e2f-114">printJob</span><span class="sxs-lookup"><span data-stu-id="a0e2f-114">printJob</span></span>](printjob.md) | <span data-ttu-id="a0e2f-115">创建新的打印作业对象。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="a0e2f-116">开始</span><span class="sxs-lookup"><span data-stu-id="a0e2f-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="a0e2f-117">无</span><span class="sxs-lookup"><span data-stu-id="a0e2f-117">None</span></span>|<span data-ttu-id="a0e2f-118">启动打印作业。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-118">Start the print job.</span></span>|
| [<span data-ttu-id="a0e2f-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="a0e2f-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="a0e2f-120">无</span><span class="sxs-lookup"><span data-stu-id="a0e2f-120">None</span></span>|<span data-ttu-id="a0e2f-121">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-121">Cancel the print job.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0e2f-122">属性</span><span class="sxs-lookup"><span data-stu-id="a0e2f-122">Properties</span></span>
| <span data-ttu-id="a0e2f-123">属性</span><span class="sxs-lookup"><span data-stu-id="a0e2f-123">Property</span></span>     | <span data-ttu-id="a0e2f-124">类型</span><span class="sxs-lookup"><span data-stu-id="a0e2f-124">Type</span></span>        | <span data-ttu-id="a0e2f-125">说明</span><span class="sxs-lookup"><span data-stu-id="a0e2f-125">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0e2f-126">id</span><span class="sxs-lookup"><span data-stu-id="a0e2f-126">id</span></span>|<span data-ttu-id="a0e2f-127">String</span><span class="sxs-lookup"><span data-stu-id="a0e2f-127">String</span></span>|<span data-ttu-id="a0e2f-128">打印机的 GUID。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-128">The printer's GUID.</span></span> <span data-ttu-id="a0e2f-129">只读。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-129">Read-only.</span></span>|
|<span data-ttu-id="a0e2f-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0e2f-130">createdDateTime</span></span>|<span data-ttu-id="a0e2f-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0e2f-131">DateTimeOffset</span></span>|<span data-ttu-id="a0e2f-132">创建作业时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-132">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="a0e2f-133">只读。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-133">Read-only.</span></span>|
|<span data-ttu-id="a0e2f-134">状态</span><span class="sxs-lookup"><span data-stu-id="a0e2f-134">status</span></span>|[<span data-ttu-id="a0e2f-135">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="a0e2f-135">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="a0e2f-136">打印作业的状态。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-136">The status of the print job.</span></span> <span data-ttu-id="a0e2f-137">只读。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-137">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0e2f-138">关系</span><span class="sxs-lookup"><span data-stu-id="a0e2f-138">Relationships</span></span>
| <span data-ttu-id="a0e2f-139">关系</span><span class="sxs-lookup"><span data-stu-id="a0e2f-139">Relationship</span></span> | <span data-ttu-id="a0e2f-140">类型</span><span class="sxs-lookup"><span data-stu-id="a0e2f-140">Type</span></span>        | <span data-ttu-id="a0e2f-141">说明</span><span class="sxs-lookup"><span data-stu-id="a0e2f-141">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a0e2f-142">createdBy</span><span class="sxs-lookup"><span data-stu-id="a0e2f-142">createdBy</span></span>|[<span data-ttu-id="a0e2f-143">userIdentity</span><span class="sxs-lookup"><span data-stu-id="a0e2f-143">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="a0e2f-144">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-144">Read-only.</span></span> <span data-ttu-id="a0e2f-145">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-145">Nullable.</span></span>|
|<span data-ttu-id="a0e2f-146">单据</span><span class="sxs-lookup"><span data-stu-id="a0e2f-146">documents</span></span>|<span data-ttu-id="a0e2f-147">[printDocument](printdocument.md)集合</span><span class="sxs-lookup"><span data-stu-id="a0e2f-147">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="a0e2f-148">只读。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-148">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0e2f-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0e2f-149">JSON representation</span></span>

<span data-ttu-id="a0e2f-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0e2f-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.printJob",
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity"
}-->

```json
{
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "documents": [ {"@odata.type": "microsoft.graph.printDocument"} ]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printJob resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->