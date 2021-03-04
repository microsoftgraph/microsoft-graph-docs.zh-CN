---
title: caseExportOperation 资源类型
description: 表示电子数据展示导出的过程。
localization_priority: Normal
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c14f4211706879a6897b5f795202a30058d138bf
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446670"
---
# <a name="caseexportoperation-resource-type"></a><span data-ttu-id="9d8e8-103">caseExportOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9d8e8-103">caseExportOperation resource type</span></span>

<span data-ttu-id="9d8e8-104">命名空间：microsoft.graph.ediscovery</span><span class="sxs-lookup"><span data-stu-id="9d8e8-104">Namespace: microsoft.graph.ediscovery</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9d8e8-105">表示电子数据展示导出的过程。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-105">Represents the process of an eDiscovery export.</span></span> <span data-ttu-id="9d8e8-106">**caseExportOperation** 只能在对审阅集导出的响应中从 `Location` [标头中检索](../api/ediscovery-reviewset-export.md)。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-106">The **caseExportOperation** can only be retrieved from the `Location` header in the response to a [reviewset export](../api/ediscovery-reviewset-export.md).</span></span>

<span data-ttu-id="9d8e8-107">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-107">Inherits from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>

## <a name="methods"></a><span data-ttu-id="9d8e8-108">Methods</span><span class="sxs-lookup"><span data-stu-id="9d8e8-108">Methods</span></span>

|<span data-ttu-id="9d8e8-109">方法</span><span class="sxs-lookup"><span data-stu-id="9d8e8-109">Method</span></span>|<span data-ttu-id="9d8e8-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="9d8e8-110">Return type</span></span>|<span data-ttu-id="9d8e8-111">说明</span><span class="sxs-lookup"><span data-stu-id="9d8e8-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9d8e8-112">getDownloadUrl</span><span class="sxs-lookup"><span data-stu-id="9d8e8-112">getDownloadUrl</span></span>](../api/ediscovery-caseexportoperation-getdownloadurl.md)|<span data-ttu-id="9d8e8-113">String</span><span class="sxs-lookup"><span data-stu-id="9d8e8-113">String</span></span>| <span data-ttu-id="9d8e8-114">返回导出的 URL。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-114">Returns the URL for the export.</span></span>|

## <a name="properties"></a><span data-ttu-id="9d8e8-115">属性</span><span class="sxs-lookup"><span data-stu-id="9d8e8-115">Properties</span></span>

|<span data-ttu-id="9d8e8-116">属性</span><span class="sxs-lookup"><span data-stu-id="9d8e8-116">Property</span></span>|<span data-ttu-id="9d8e8-117">类型</span><span class="sxs-lookup"><span data-stu-id="9d8e8-117">Type</span></span>|<span data-ttu-id="9d8e8-118">说明</span><span class="sxs-lookup"><span data-stu-id="9d8e8-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d8e8-119">action</span><span class="sxs-lookup"><span data-stu-id="9d8e8-119">action</span></span>|[<span data-ttu-id="9d8e8-120">microsoft.graph.ediscovery.caseAction</span><span class="sxs-lookup"><span data-stu-id="9d8e8-120">microsoft.graph.ediscovery.caseAction</span></span>](../resources/ediscovery-caseoperation.md#caseaction-values)| <span data-ttu-id="9d8e8-121">此实体的大小写操作将始终为 `contentExport` 。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-121">The case action for this entity will always be `contentExport`.</span></span> <span data-ttu-id="9d8e8-122">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-122">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d8e8-123">azureBlobContainer</span><span class="sxs-lookup"><span data-stu-id="9d8e8-123">azureBlobContainer</span></span>|<span data-ttu-id="9d8e8-124">String</span><span class="sxs-lookup"><span data-stu-id="9d8e8-124">String</span></span>| <span data-ttu-id="9d8e8-125">将存储导出的 Azure 存储位置的名称。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-125">The name of the Azure storage location where the export will be stored.</span></span> <span data-ttu-id="9d8e8-126">这仅适用于存储在你自己的 Azure 存储位置中的导出。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-126">This only applies to exports stored in your own Azure storage location.</span></span> |
|<span data-ttu-id="9d8e8-127">azureBlobToken</span><span class="sxs-lookup"><span data-stu-id="9d8e8-127">azureBlobToken</span></span>|<span data-ttu-id="9d8e8-128">String</span><span class="sxs-lookup"><span data-stu-id="9d8e8-128">String</span></span>| <span data-ttu-id="9d8e8-129">Azure 存储位置的 SAS 令牌。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-129">The SAS token for the Azure storage location.</span></span>  <span data-ttu-id="9d8e8-130">这仅适用于存储在你自己的 Azure 存储位置中的导出。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-130">This only applies to exports stored in your own Azure storage location.</span></span> |
|<span data-ttu-id="9d8e8-131">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="9d8e8-131">completedDateTime</span></span>|<span data-ttu-id="9d8e8-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d8e8-132">DateTimeOffset</span></span>| <span data-ttu-id="9d8e8-133">导出完成的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-133">The date and time the export was completed.</span></span>  <span data-ttu-id="9d8e8-134">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9d8e8-134">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="9d8e8-135">createdBy</span><span class="sxs-lookup"><span data-stu-id="9d8e8-135">createdBy</span></span>|[<span data-ttu-id="9d8e8-136">identitySet</span><span class="sxs-lookup"><span data-stu-id="9d8e8-136">identitySet</span></span>](../resources/identityset.md)| <span data-ttu-id="9d8e8-137">启动导出操作的用户。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-137">The user who initiated the export operation.</span></span> <span data-ttu-id="9d8e8-138">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9d8e8-138">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="9d8e8-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9d8e8-139">createdDateTime</span></span>|<span data-ttu-id="9d8e8-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d8e8-140">DateTimeOffset</span></span>| <span data-ttu-id="9d8e8-141">创建导出的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-141">The date and time the export was created.</span></span> <span data-ttu-id="9d8e8-142">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9d8e8-142">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="9d8e8-143">说明</span><span class="sxs-lookup"><span data-stu-id="9d8e8-143">description</span></span>|<span data-ttu-id="9d8e8-144">String</span><span class="sxs-lookup"><span data-stu-id="9d8e8-144">String</span></span>| <span data-ttu-id="9d8e8-145">为导出提供的说明。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-145">The description provided for the export.</span></span> |
|<span data-ttu-id="9d8e8-146">exportOptions</span><span class="sxs-lookup"><span data-stu-id="9d8e8-146">exportOptions</span></span>|<span data-ttu-id="9d8e8-147">microsoft.graph.ediscovery.exportOptions</span><span class="sxs-lookup"><span data-stu-id="9d8e8-147">microsoft.graph.ediscovery.exportOptions</span></span>| <span data-ttu-id="9d8e8-148">为导出提供的选项。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-148">The options provided for the export.</span></span> <span data-ttu-id="9d8e8-149">有关详细信息 [，请参阅 reviewSet：](../api/ediscovery-reviewset-export.md) 导出。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-149">See [reviewSet: export](../api/ediscovery-reviewset-export.md) for more details.</span></span> <span data-ttu-id="9d8e8-150">可取值为：`originalFiles`、`text`、`pdfReplacement`、`fileInfo`、`tags`。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-150">Possible values are: `originalFiles`, `text`, `pdfReplacement`, `fileInfo`, `tags`.</span></span>|
|<span data-ttu-id="9d8e8-151">exportStructure</span><span class="sxs-lookup"><span data-stu-id="9d8e8-151">exportStructure</span></span>|<span data-ttu-id="9d8e8-152">microsoft.graph.ediscovery.exportFileStructure</span><span class="sxs-lookup"><span data-stu-id="9d8e8-152">microsoft.graph.ediscovery.exportFileStructure</span></span>|<span data-ttu-id="9d8e8-153">提供的选项指定导出的结构。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-153">The options provided that specify the structure of the export.</span></span> <span data-ttu-id="9d8e8-154">有关详细信息 [，请参阅 reviewSet：](../api/ediscovery-reviewset-export.md) 导出。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-154">See [reviewSet: export](../api/ediscovery-reviewset-export.md) for more details.</span></span> <span data-ttu-id="9d8e8-155">可取值为：`none`、`directory`、`pst`。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-155">Possible values are: `none`, `directory`, `pst`.</span></span>|
|<span data-ttu-id="9d8e8-156">id</span><span class="sxs-lookup"><span data-stu-id="9d8e8-156">id</span></span>|<span data-ttu-id="9d8e8-157">String</span><span class="sxs-lookup"><span data-stu-id="9d8e8-157">String</span></span>| <span data-ttu-id="9d8e8-158">操作 ID。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-158">The ID for the operation.</span></span> <span data-ttu-id="9d8e8-159">只读。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-159">Read-only.</span></span> <span data-ttu-id="9d8e8-160">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-160">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span>|
|<span data-ttu-id="9d8e8-161">outputName</span><span class="sxs-lookup"><span data-stu-id="9d8e8-161">outputName</span></span>|<span data-ttu-id="9d8e8-162">String</span><span class="sxs-lookup"><span data-stu-id="9d8e8-162">String</span></span>| <span data-ttu-id="9d8e8-163">为导出提供的名称。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-163">The name provided for the export.</span></span>|
|<span data-ttu-id="9d8e8-164">percentProgress</span><span class="sxs-lookup"><span data-stu-id="9d8e8-164">percentProgress</span></span>|<span data-ttu-id="9d8e8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="9d8e8-165">Int32</span></span>| <span data-ttu-id="9d8e8-166">操作的进度。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-166">The progress of the operation.</span></span> <span data-ttu-id="9d8e8-167">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9d8e8-167">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="9d8e8-168">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9d8e8-168">resultInfo</span></span>|[<span data-ttu-id="9d8e8-169">resultInfo</span><span class="sxs-lookup"><span data-stu-id="9d8e8-169">resultInfo</span></span>](../resources/resultinfo.md)|<span data-ttu-id="9d8e8-170">包含特定于成功和失败的结果信息。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-170">Contains success and failure-specific result information.</span></span> <span data-ttu-id="9d8e8-171">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)</span><span class="sxs-lookup"><span data-stu-id="9d8e8-171">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md)</span></span>|
|<span data-ttu-id="9d8e8-172">status</span><span class="sxs-lookup"><span data-stu-id="9d8e8-172">status</span></span>|[<span data-ttu-id="9d8e8-173">microsoft.graph.ediscovery.caseOperationStatus</span><span class="sxs-lookup"><span data-stu-id="9d8e8-173">microsoft.graph.ediscovery.caseOperationStatus</span></span>](../resources/ediscovery-caseoperation.md#caseoperationstatus-values)|<span data-ttu-id="9d8e8-174">案例操作的状态。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-174">The status of the case operation.</span></span> <span data-ttu-id="9d8e8-175">继承自 [caseOperation](../resources/ediscovery-caseoperation.md)。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-175">Inherited from [caseOperation](../resources/ediscovery-caseoperation.md).</span></span> <span data-ttu-id="9d8e8-176">可取值为：`notStarted`、`submissionFailed`、`running`、`succeeded`、`partiallySucceeded`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-176">Possible values are: `notStarted`, `submissionFailed`, `running`, `succeeded`, `partiallySucceeded`, `failed`.</span></span>|

### <a name="exportoptions-values"></a><span data-ttu-id="9d8e8-177">exportOptions 值</span><span class="sxs-lookup"><span data-stu-id="9d8e8-177">exportOptions values</span></span>

|<span data-ttu-id="9d8e8-178">成员</span><span class="sxs-lookup"><span data-stu-id="9d8e8-178">Member</span></span>| <span data-ttu-id="9d8e8-179">说明</span><span class="sxs-lookup"><span data-stu-id="9d8e8-179">Description</span></span> |
|:---|:---|
|<span data-ttu-id="9d8e8-180">originalFiles</span><span class="sxs-lookup"><span data-stu-id="9d8e8-180">originalFiles</span></span>| <span data-ttu-id="9d8e8-181">包含原始文件的副本 - 仅在生成报告时排除此选项</span><span class="sxs-lookup"><span data-stu-id="9d8e8-181">Include copies of the original files - exclude this option when generating reports only</span></span> |
|<span data-ttu-id="9d8e8-182">text</span><span class="sxs-lookup"><span data-stu-id="9d8e8-182">text</span></span>| <span data-ttu-id="9d8e8-183">包含每个文档的原始提取文本文件。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-183">Include raw extracted text files for each document.</span></span> |
|<span data-ttu-id="9d8e8-184">pdfReplacement</span><span class="sxs-lookup"><span data-stu-id="9d8e8-184">pdfReplacement</span></span>| <span data-ttu-id="9d8e8-185">如果在审阅期间生成修订的 PDF 文件，则这些文件可供导出。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-185">If redacted PDF files are generated during review, these files are available for export.</span></span> <span data-ttu-id="9d8e8-186">你可以选择通过包括此选项来导出修订的 PDF，而不是原始本机文件。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-186">You can choose to export the redacted PDFs instead of the original native files by including this option.</span></span> |
|<span data-ttu-id="9d8e8-187">fileInfo</span><span class="sxs-lookup"><span data-stu-id="9d8e8-187">fileInfo</span></span>| <span data-ttu-id="9d8e8-188">包括夏时和加载文件 - 应始终包含该文件。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-188">Include the summery and load file - this should always be included.</span></span> |
|<span data-ttu-id="9d8e8-189">tags</span><span class="sxs-lookup"><span data-stu-id="9d8e8-189">tags</span></span>| <span data-ttu-id="9d8e8-190">在加载文件中包括审核期间应用的文档标记。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-190">Include document tags that were applied during review in the load file.</span></span> |

### <a name="exportfilestructure-values"></a><span data-ttu-id="9d8e8-191">exportFileStructure 值</span><span class="sxs-lookup"><span data-stu-id="9d8e8-191">exportFileStructure values</span></span>

|<span data-ttu-id="9d8e8-192">成员</span><span class="sxs-lookup"><span data-stu-id="9d8e8-192">Member</span></span>| <span data-ttu-id="9d8e8-193">说明</span><span class="sxs-lookup"><span data-stu-id="9d8e8-193">Description</span></span> |
|:---|:---|
|<span data-ttu-id="9d8e8-194">目录</span><span class="sxs-lookup"><span data-stu-id="9d8e8-194">directory</span></span>| <span data-ttu-id="9d8e8-195">映射到电子数据展示工具常用的压缩目录结构。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-195">Maps to the condensed directory structure commonly used by eDiscovery tools.</span></span> <span data-ttu-id="9d8e8-196">所有文件都导出到名为 NativeFiles 的根文件。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-196">All files are exported to a root file called NativeFiles.</span></span> |
|<span data-ttu-id="9d8e8-197">pst</span><span class="sxs-lookup"><span data-stu-id="9d8e8-197">pst</span></span>| <span data-ttu-id="9d8e8-198">电子邮件存储在 PTS 中，而网站中的文档存储在表示原始本机文件夹结构的文件夹中。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-198">Emails are stored in PSTs while documents from sites are stored in folders that represent the original native folder structure.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9d8e8-199">关系</span><span class="sxs-lookup"><span data-stu-id="9d8e8-199">Relationships</span></span>

|<span data-ttu-id="9d8e8-200">关系</span><span class="sxs-lookup"><span data-stu-id="9d8e8-200">Relationship</span></span>|<span data-ttu-id="9d8e8-201">类型</span><span class="sxs-lookup"><span data-stu-id="9d8e8-201">Type</span></span>|<span data-ttu-id="9d8e8-202">说明</span><span class="sxs-lookup"><span data-stu-id="9d8e8-202">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d8e8-203">reviewSet</span><span class="sxs-lookup"><span data-stu-id="9d8e8-203">reviewSet</span></span>|[<span data-ttu-id="9d8e8-204">microsoft.graph.ediscovery.reviewSet</span><span class="sxs-lookup"><span data-stu-id="9d8e8-204">microsoft.graph.ediscovery.reviewSet</span></span>](../resources/ediscovery-reviewset.md)| <span data-ttu-id="9d8e8-205">正在导出内容的审阅集。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-205">The review set the content is being exported from.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9d8e8-206">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9d8e8-206">JSON representation</span></span>

<span data-ttu-id="9d8e8-207">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9d8e8-207">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.caseExportOperation",
  "baseType": "microsoft.graph.ediscovery.caseOperation",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.caseExportOperation",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "completedDateTime": "String (timestamp)",
  "percentProgress": "Integer",
  "status": "String",
  "action": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "resultInfo": {
    "@odata.type": "microsoft.graph.resultInfo"
  },
  "outputName": "String",
  "description": "String",
  "outputFolderId": "String",
  "azureBlobContainer": "String",
  "azureBlobToken": "String",
  "exportOptions": "String",
  "exportStructure": "String"
}
```
