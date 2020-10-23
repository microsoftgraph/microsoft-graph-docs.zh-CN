---
title: printJob 资源类型
description: 代表已对打印机排队的打印作业。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: resourcePageType
ms.openlocfilehash: 7810c8cd864020c42de4482deea67620950f6cf0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48726290"
---
# <a name="printjob-resource-type"></a><span data-ttu-id="f2dd9-103">printJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="f2dd9-103">printJob resource type</span></span>

<span data-ttu-id="f2dd9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2dd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2dd9-105">代表已对打印机排队的打印作业。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-105">Represents a print job that has been queued for a printer.</span></span>

## <a name="methods"></a><span data-ttu-id="f2dd9-106">Methods</span><span class="sxs-lookup"><span data-stu-id="f2dd9-106">Methods</span></span>

| <span data-ttu-id="f2dd9-107">方法</span><span class="sxs-lookup"><span data-stu-id="f2dd9-107">Method</span></span>       | <span data-ttu-id="f2dd9-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="f2dd9-108">Return Type</span></span> | <span data-ttu-id="f2dd9-109">说明</span><span class="sxs-lookup"><span data-stu-id="f2dd9-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="f2dd9-110">获取</span><span class="sxs-lookup"><span data-stu-id="f2dd9-110">Get</span></span>](../api/printjob-get.md) | [<span data-ttu-id="f2dd9-111">printJob</span><span class="sxs-lookup"><span data-stu-id="f2dd9-111">printJob</span></span>](printjob.md) | <span data-ttu-id="f2dd9-112">读取 printJob 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-112">Read properties and relationships of printJob object.</span></span> |
| [<span data-ttu-id="f2dd9-113">创建</span><span class="sxs-lookup"><span data-stu-id="f2dd9-113">Create</span></span>](../api/printer-post-jobs.md) | [<span data-ttu-id="f2dd9-114">printJob</span><span class="sxs-lookup"><span data-stu-id="f2dd9-114">printJob</span></span>](printjob.md) | <span data-ttu-id="f2dd9-115">创建新的打印作业对象。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-115">Create a new print job object.</span></span> |
| [<span data-ttu-id="f2dd9-116">开始</span><span class="sxs-lookup"><span data-stu-id="f2dd9-116">Start</span></span>](../api/printjob-start.md)|<span data-ttu-id="f2dd9-117">无</span><span class="sxs-lookup"><span data-stu-id="f2dd9-117">None</span></span>|<span data-ttu-id="f2dd9-118">启动打印作业。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-118">Start the print job.</span></span>|
| [<span data-ttu-id="f2dd9-119">Cancel</span><span class="sxs-lookup"><span data-stu-id="f2dd9-119">Cancel</span></span>](../api/printjob-cancel.md)|<span data-ttu-id="f2dd9-120">无</span><span class="sxs-lookup"><span data-stu-id="f2dd9-120">None</span></span>|<span data-ttu-id="f2dd9-121">取消打印作业。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-121">Cancel the print job.</span></span>|
| [<span data-ttu-id="f2dd9-122">将 (重定向到另一台打印机) </span><span class="sxs-lookup"><span data-stu-id="f2dd9-122">Redirect (to another printer)</span></span>](../api/printjob-redirect.md) | [<span data-ttu-id="f2dd9-123">printJob</span><span class="sxs-lookup"><span data-stu-id="f2dd9-123">printJob</span></span>](printjob.md) | <span data-ttu-id="f2dd9-124">排队等候目标打印机的打印作业。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-124">A print job that is queued for the destination printer.</span></span> |

## <a name="properties"></a><span data-ttu-id="f2dd9-125">属性</span><span class="sxs-lookup"><span data-stu-id="f2dd9-125">Properties</span></span>
| <span data-ttu-id="f2dd9-126">属性</span><span class="sxs-lookup"><span data-stu-id="f2dd9-126">Property</span></span>     | <span data-ttu-id="f2dd9-127">类型</span><span class="sxs-lookup"><span data-stu-id="f2dd9-127">Type</span></span>        | <span data-ttu-id="f2dd9-128">说明</span><span class="sxs-lookup"><span data-stu-id="f2dd9-128">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2dd9-129">id</span><span class="sxs-lookup"><span data-stu-id="f2dd9-129">id</span></span>|<span data-ttu-id="f2dd9-130">String</span><span class="sxs-lookup"><span data-stu-id="f2dd9-130">String</span></span>|<span data-ttu-id="f2dd9-131">打印机的 GUID。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-131">The printer's GUID.</span></span> <span data-ttu-id="f2dd9-132">只读。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-132">Read-only.</span></span>|
|<span data-ttu-id="f2dd9-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2dd9-133">createdDateTime</span></span>|<span data-ttu-id="f2dd9-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2dd9-134">DateTimeOffset</span></span>|<span data-ttu-id="f2dd9-135">创建作业时的 DateTimeOffset。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-135">The DateTimeOffset when the job was created.</span></span> <span data-ttu-id="f2dd9-136">只读。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-136">Read-only.</span></span>|
|<span data-ttu-id="f2dd9-137">status</span><span class="sxs-lookup"><span data-stu-id="f2dd9-137">status</span></span>|[<span data-ttu-id="f2dd9-138">printJobStatus</span><span class="sxs-lookup"><span data-stu-id="f2dd9-138">printJobStatus</span></span>](printjobstatus.md)|<span data-ttu-id="f2dd9-139">打印作业的状态。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-139">The status of the print job.</span></span> <span data-ttu-id="f2dd9-140">只读。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-140">Read-only.</span></span>|
|<span data-ttu-id="f2dd9-141">configuration</span><span class="sxs-lookup"><span data-stu-id="f2dd9-141">configuration</span></span>|[<span data-ttu-id="f2dd9-142">printJobConfiguration</span><span class="sxs-lookup"><span data-stu-id="f2dd9-142">printJobConfiguration</span></span>](printJobConfiguration.md)|<span data-ttu-id="f2dd9-143">打印机打印作业时应使用的一组设置。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-143">A group of settings that a printer should use to print a job.</span></span>|
|<span data-ttu-id="f2dd9-144">isFetchable</span><span class="sxs-lookup"><span data-stu-id="f2dd9-144">isFetchable</span></span>|<span data-ttu-id="f2dd9-145">Edm.Boolean</span><span class="sxs-lookup"><span data-stu-id="f2dd9-145">Edm.Boolean</span></span>|<span data-ttu-id="f2dd9-146">如果为 true，则打印机可以读取文档。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-146">If true, document can be fetched by printer.</span></span>|
|<span data-ttu-id="f2dd9-147">redirectedFrom</span><span class="sxs-lookup"><span data-stu-id="f2dd9-147">redirectedFrom</span></span>|<span data-ttu-id="f2dd9-148">Edm.String</span><span class="sxs-lookup"><span data-stu-id="f2dd9-148">Edm.String</span></span>|<span data-ttu-id="f2dd9-149">如果作业已从另一台打印机重定向，则包含源作业 URL。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-149">Contains the source job URL, if the job has been redirected from another printer.</span></span>|
|<span data-ttu-id="f2dd9-150">redirectedTo</span><span class="sxs-lookup"><span data-stu-id="f2dd9-150">redirectedTo</span></span>|<span data-ttu-id="f2dd9-151">Edm.String</span><span class="sxs-lookup"><span data-stu-id="f2dd9-151">Edm.String</span></span>|<span data-ttu-id="f2dd9-152">如果作业已重定向到另一台打印机，则包含目标作业 URL。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-152">Contains the destination job URL, if the job has been redirected to another printer.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f2dd9-153">关系</span><span class="sxs-lookup"><span data-stu-id="f2dd9-153">Relationships</span></span>
| <span data-ttu-id="f2dd9-154">关系</span><span class="sxs-lookup"><span data-stu-id="f2dd9-154">Relationship</span></span> | <span data-ttu-id="f2dd9-155">类型</span><span class="sxs-lookup"><span data-stu-id="f2dd9-155">Type</span></span>        | <span data-ttu-id="f2dd9-156">说明</span><span class="sxs-lookup"><span data-stu-id="f2dd9-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f2dd9-157">createdBy</span><span class="sxs-lookup"><span data-stu-id="f2dd9-157">createdBy</span></span>|[<span data-ttu-id="f2dd9-158">userIdentity</span><span class="sxs-lookup"><span data-stu-id="f2dd9-158">userIdentity</span></span>](useridentity.md)| <span data-ttu-id="f2dd9-159">只读。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-159">Read-only.</span></span> <span data-ttu-id="f2dd9-160">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-160">Nullable.</span></span>|
|<span data-ttu-id="f2dd9-161">单据</span><span class="sxs-lookup"><span data-stu-id="f2dd9-161">documents</span></span>|<span data-ttu-id="f2dd9-162">[printDocument](printdocument.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2dd9-162">[printDocument](printdocument.md) collection</span></span>| <span data-ttu-id="f2dd9-163">只读。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-163">Read-only.</span></span>|
|<span data-ttu-id="f2dd9-164">tasks</span><span class="sxs-lookup"><span data-stu-id="f2dd9-164">tasks</span></span>|<span data-ttu-id="f2dd9-165">[printTask](printtask.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f2dd9-165">[printTask](printtask.md) collection</span></span>|<span data-ttu-id="f2dd9-166">此打印作业触发的 [printTasks](printtask.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-166">A list of [printTasks](printtask.md) that were triggered by this print job.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f2dd9-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f2dd9-167">JSON representation</span></span>

<span data-ttu-id="f2dd9-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2dd9-168">The following is a JSON representation of the resource.</span></span>

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
  "isFetchable": "Boolean",
  "redirectedFrom": "String",
  "redirectedTo": "String",
  "status": {"@odata.type": "microsoft.graph.printJobStatus"},
  "createdBy": {"@odata.type": "microsoft.graph.userIdentity"},
  "configuration": {"@odata.type": "microsoft.graph.printJobConfiguration"},
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

