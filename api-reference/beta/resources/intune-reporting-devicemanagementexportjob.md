---
title: deviceManagementExportJob 资源类型
description: 表示导出报告的作业的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c1ee8c07f6083d7e6f5b5b061bd87b3438683912
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538537"
---
# <a name="devicemanagementexportjob-resource-type"></a><span data-ttu-id="a8c72-103">deviceManagementExportJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="a8c72-103">deviceManagementExportJob resource type</span></span>

> <span data-ttu-id="a8c72-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a8c72-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8c72-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8c72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8c72-106">表示导出报告的作业的实体</span><span class="sxs-lookup"><span data-stu-id="a8c72-106">Entity representing a job to export a report</span></span>

## <a name="methods"></a><span data-ttu-id="a8c72-107">方法</span><span class="sxs-lookup"><span data-stu-id="a8c72-107">Methods</span></span>
|<span data-ttu-id="a8c72-108">方法</span><span class="sxs-lookup"><span data-stu-id="a8c72-108">Method</span></span>|<span data-ttu-id="a8c72-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a8c72-109">Return Type</span></span>|<span data-ttu-id="a8c72-110">说明</span><span class="sxs-lookup"><span data-stu-id="a8c72-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a8c72-111">列出 deviceManagementExportJobs</span><span class="sxs-lookup"><span data-stu-id="a8c72-111">List deviceManagementExportJobs</span></span>](../api/intune-reporting-devicemanagementexportjob-list.md)|<span data-ttu-id="a8c72-112">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="a8c72-112">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) collection</span></span>|<span data-ttu-id="a8c72-113">列出[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a8c72-113">List properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) objects.</span></span>|
|[<span data-ttu-id="a8c72-114">获取 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="a8c72-114">Get deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-get.md)|[<span data-ttu-id="a8c72-115">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="a8c72-115">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="a8c72-116">读取[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a8c72-116">Read properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|
|[<span data-ttu-id="a8c72-117">创建 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="a8c72-117">Create deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-create.md)|[<span data-ttu-id="a8c72-118">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="a8c72-118">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="a8c72-119">创建新的[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a8c72-119">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|
|[<span data-ttu-id="a8c72-120">删除 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="a8c72-120">Delete deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-delete.md)|<span data-ttu-id="a8c72-121">无</span><span class="sxs-lookup"><span data-stu-id="a8c72-121">None</span></span>|<span data-ttu-id="a8c72-122">删除[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)。</span><span class="sxs-lookup"><span data-stu-id="a8c72-122">Deletes a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>|
|[<span data-ttu-id="a8c72-123">更新 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="a8c72-123">Update deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-update.md)|[<span data-ttu-id="a8c72-124">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="a8c72-124">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="a8c72-125">更新[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a8c72-125">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8c72-126">属性</span><span class="sxs-lookup"><span data-stu-id="a8c72-126">Properties</span></span>
|<span data-ttu-id="a8c72-127">属性</span><span class="sxs-lookup"><span data-stu-id="a8c72-127">Property</span></span>|<span data-ttu-id="a8c72-128">类型</span><span class="sxs-lookup"><span data-stu-id="a8c72-128">Type</span></span>|<span data-ttu-id="a8c72-129">说明</span><span class="sxs-lookup"><span data-stu-id="a8c72-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8c72-130">id</span><span class="sxs-lookup"><span data-stu-id="a8c72-130">id</span></span>|<span data-ttu-id="a8c72-131">字符串</span><span class="sxs-lookup"><span data-stu-id="a8c72-131">String</span></span>|<span data-ttu-id="a8c72-132">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="a8c72-132">Unique identifier for this entity</span></span>|
|<span data-ttu-id="a8c72-133">reportName</span><span class="sxs-lookup"><span data-stu-id="a8c72-133">reportName</span></span>|<span data-ttu-id="a8c72-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a8c72-134">String</span></span>|<span data-ttu-id="a8c72-135">报告的名称</span><span class="sxs-lookup"><span data-stu-id="a8c72-135">Name of the report</span></span>|
|<span data-ttu-id="a8c72-136">filter</span><span class="sxs-lookup"><span data-stu-id="a8c72-136">filter</span></span>|<span data-ttu-id="a8c72-137">字符串</span><span class="sxs-lookup"><span data-stu-id="a8c72-137">String</span></span>|<span data-ttu-id="a8c72-138">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="a8c72-138">Filters applied on the report</span></span>|
|<span data-ttu-id="a8c72-139">select</span><span class="sxs-lookup"><span data-stu-id="a8c72-139">select</span></span>|<span data-ttu-id="a8c72-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="a8c72-140">String collection</span></span>|<span data-ttu-id="a8c72-141">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="a8c72-141">Columns selected from the report</span></span>|
|<span data-ttu-id="a8c72-142">By</span><span class="sxs-lookup"><span data-stu-id="a8c72-142">orderBy</span></span>|<span data-ttu-id="a8c72-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="a8c72-143">String collection</span></span>|<span data-ttu-id="a8c72-144">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="a8c72-144">Ordering of columns in the report</span></span>|
|<span data-ttu-id="a8c72-145">format</span><span class="sxs-lookup"><span data-stu-id="a8c72-145">format</span></span>|[<span data-ttu-id="a8c72-146">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="a8c72-146">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="a8c72-147">导出的报表的格式。</span><span class="sxs-lookup"><span data-stu-id="a8c72-147">Format of the exported report.</span></span> <span data-ttu-id="a8c72-148">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="a8c72-148">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="a8c72-149">snapshotId</span><span class="sxs-lookup"><span data-stu-id="a8c72-149">snapshotId</span></span>|<span data-ttu-id="a8c72-150">字符串</span><span class="sxs-lookup"><span data-stu-id="a8c72-150">String</span></span>|<span data-ttu-id="a8c72-151">快照是由 ReportName 表示的数据集的可识别子集。</span><span class="sxs-lookup"><span data-stu-id="a8c72-151">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="a8c72-152">可以在此处使用 sessionId 或 CachedReportConfiguration id。</span><span class="sxs-lookup"><span data-stu-id="a8c72-152">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="a8c72-153">如果指定了 sessionId，则筛选器、Select 和 OrderBy 将应用于 sessionId 所代表的数据。</span><span class="sxs-lookup"><span data-stu-id="a8c72-153">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="a8c72-154">Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。</span><span class="sxs-lookup"><span data-stu-id="a8c72-154">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="a8c72-155">status</span><span class="sxs-lookup"><span data-stu-id="a8c72-155">status</span></span>|[<span data-ttu-id="a8c72-156">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="a8c72-156">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="a8c72-157">导出作业的状态。</span><span class="sxs-lookup"><span data-stu-id="a8c72-157">Status of the export job.</span></span> <span data-ttu-id="a8c72-158">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="a8c72-158">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="a8c72-159">url</span><span class="sxs-lookup"><span data-stu-id="a8c72-159">url</span></span>|<span data-ttu-id="a8c72-160">String</span><span class="sxs-lookup"><span data-stu-id="a8c72-160">String</span></span>|<span data-ttu-id="a8c72-161">导出报告的临时位置</span><span class="sxs-lookup"><span data-stu-id="a8c72-161">Temporary location of the exported report</span></span>|
|<span data-ttu-id="a8c72-162">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="a8c72-162">requestDateTime</span></span>|<span data-ttu-id="a8c72-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8c72-163">DateTimeOffset</span></span>|<span data-ttu-id="a8c72-164">请求导出的报告的时间</span><span class="sxs-lookup"><span data-stu-id="a8c72-164">Time that the exported report was requested</span></span>|
|<span data-ttu-id="a8c72-165">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a8c72-165">expirationDateTime</span></span>|<span data-ttu-id="a8c72-166">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8c72-166">DateTimeOffset</span></span>|<span data-ttu-id="a8c72-167">导出的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="a8c72-167">Time that the exported report expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="a8c72-168">关系</span><span class="sxs-lookup"><span data-stu-id="a8c72-168">Relationships</span></span>
<span data-ttu-id="a8c72-169">无</span><span class="sxs-lookup"><span data-stu-id="a8c72-169">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a8c72-170">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a8c72-170">JSON Representation</span></span>
<span data-ttu-id="a8c72-171">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8c72-171">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementExportJob"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementExportJob",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "format": "String",
  "snapshotId": "String",
  "status": "String",
  "url": "String",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



