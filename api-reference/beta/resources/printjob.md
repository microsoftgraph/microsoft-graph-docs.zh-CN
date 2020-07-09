---
title: printJob 资源类型
description: 代表已对打印机排队的打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 0d46263e5f393362cec155a9be3e2e5a54c3dfec
ms.sourcegitcommit: 8a74c06be9c41390331ca1717efedc5b5a244db5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/09/2020
ms.locfileid: "45091520"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="f9acc-103">printJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9acc-103">printJob resource type</span></span>

<span data-ttu-id="f9acc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9acc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9acc-105">代表已对打印机排队的打印作业。</span><span class="sxs-lookup"><span data-stu-id="f9acc-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="f9acc-106">方法</span><span class="sxs-lookup"><span data-stu-id="f9acc-106">Methods</span></span>

| <span data-ttu-id="f9acc-107">方法</span><span class="sxs-lookup"><span data-stu-id="f9acc-107">Method</span></span>       | <span data-ttu-id="f9acc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f9acc-108">Return Type</span></span> | <span data-ttu-id="f9acc-109">说明</span><span class="sxs-lookup"><span data-stu-id="f9acc-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f9acc-110">获取</span><span class="sxs-lookup"><span data-stu-id="f9acc-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="f9acc-111">printJob</span><span class="sxs-lookup"><span data-stu-id="f9acc-111">printJob</span></span>](printjob.md) | <span data-ttu-id="f9acc-112">读取 printJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9acc-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="f9acc-113">创建</span><span class="sxs-lookup"><span data-stu-id="f9acc-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="f9acc-114">printJob</span><span class="sxs-lookup"><span data-stu-id="f9acc-114">printJob</span></span>](printjob.md) | <span data-ttu-id="f9acc-115">创建新的打印作业对象。</span><span class="sxs-lookup"><span data-stu-id="f9acc-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="f9acc-116">开始</span><span class="sxs-lookup"><span data-stu-id="f9acc-116">Start</span></span>](../api/printjob-startprintjob.md)|<span data-ttu-id="f9acc-117">无</span><span class="sxs-lookup"><span data-stu-id="f9acc-117">None</span></span>|<span data-ttu-id="f9acc-118">启动打印作业。</span><span class="sxs-lookup"><span data-stu-id="f9acc-118">Start the print job.</span></span>|
| [<span data-ttu-id="f9acc-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="f9acc-119">Cancel</span></span>](../api/printjob-cancelprintjob.md)|<span data-ttu-id="f9acc-120">无</span><span class="sxs-lookup"><span data-stu-id="f9acc-120">None</span></span>|<span data-ttu-id="f9acc-121">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="f9acc-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="f9acc-122">将 (重定向到另一台打印机) </span><span class="sxs-lookup"><span data-stu-id="f9acc-122">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="f9acc-123">printJob</span><span class="sxs-lookup"><span data-stu-id="f9acc-123">printJob</span></span>](printjob.md) | <span data-ttu-id="f9acc-124">排队等候目标打印机的打印作业。</span><span class="sxs-lookup"><span data-stu-id="f9acc-124">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="f9acc-125">属性</span><span class="sxs-lookup"><span data-stu-id="f9acc-125">Properties</span></span>
| <span data-ttu-id="f9acc-126">属性</span><span class="sxs-lookup"><span data-stu-id="f9acc-126">Property</span></span>     | <span data-ttu-id="f9acc-127">类型</span><span class="sxs-lookup"><span data-stu-id="f9acc-127">Type</span></span>        | <span data-ttu-id="f9acc-128">说明</span><span class="sxs-lookup"><span data-stu-id="f9acc-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f9acc-129">id</span><span class="sxs-lookup"><span data-stu-id="f9acc-129">id</span></span>|<span data-ttu-id="f9acc-130">String</span><span class="sxs-lookup"><span data-stu-id="f9acc-130">String</span></span>|<span data-ttu-id="f9acc-131">打印机的 GUID。</span><span class="sxs-lookup"><span data-stu-id="f9acc-131">The printer's GUID.</span></span> <span data-ttu-id="f9acc-132">只读。</span><span class="sxs-lookup"><span data-stu-id="f9acc-132">Read-only.</span></span>|
|<span data-ttu-id="f9acc-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9acc-133">createdDateTime</span></span>|<span data-ttu-id="f9acc-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9acc-134">DateTimeOffset</span></span>|<span data-ttu-id="f9acc-135">创建作业时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="f9acc-135">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="f9acc-136">只读。</span><span class="sxs-lookup"><span data-stu-id="f9acc-136">Read-only.</span></span>|
|<span data-ttu-id="f9acc-137">status</span><span class="sxs-lookup"><span data-stu-id="f9acc-137">status</span></span>|[<span data-ttu-id="f9acc-138">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="f9acc-138">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="f9acc-139">打印作业的状态。</span><span class="sxs-lookup"><span data-stu-id="f9acc-139">The status of the print job.</span></span> <span data-ttu-id="f9acc-140">只读。</span><span class="sxs-lookup"><span data-stu-id="f9acc-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f9acc-141">关系</span><span class="sxs-lookup"><span data-stu-id="f9acc-141">Relationships</span></span>
| <span data-ttu-id="f9acc-142">关系</span><span class="sxs-lookup"><span data-stu-id="f9acc-142">Relationship</span></span> | <span data-ttu-id="f9acc-143">类型</span><span class="sxs-lookup"><span data-stu-id="f9acc-143">Type</span></span>        | <span data-ttu-id="f9acc-144">说明</span><span class="sxs-lookup"><span data-stu-id="f9acc-144">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f9acc-145">createdBy</span><span class="sxs-lookup"><span data-stu-id="f9acc-145">createdBy</span></span>|[<span data-ttu-id="f9acc-146">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f9acc-146">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="f9acc-147">此为只读属性。</span><span class="sxs-lookup"><span data-stu-id="f9acc-147">Read-only.</span></span> <span data-ttu-id="f9acc-148">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="f9acc-148">Nullable.</span></span>|
|<span data-ttu-id="f9acc-149">单据</span><span class="sxs-lookup"><span data-stu-id="f9acc-149">documents</span></span>|<span data-ttu-id="f9acc-150">[printDocument](printdocument.md)集合</span><span class="sxs-lookup"><span data-stu-id="f9acc-150">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="f9acc-151">只读。</span><span class="sxs-lookup"><span data-stu-id="f9acc-151">Read-only.</span></span>|
|<span data-ttu-id="f9acc-152">tasks</span><span class="sxs-lookup"><span data-stu-id="f9acc-152">tasks</span></span>|<span data-ttu-id="f9acc-153">[printTask](printtask.md)集合</span><span class="sxs-lookup"><span data-stu-id="f9acc-153">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="f9acc-154">此打印作业触发的[printTasks](printtask.md)的列表。</span><span class="sxs-lookup"><span data-stu-id="f9acc-154">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9acc-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9acc-155">JSON representation</span></span>

<span data-ttu-id="f9acc-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9acc-156">The following is a JSON representation of the resource.</span></span>

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