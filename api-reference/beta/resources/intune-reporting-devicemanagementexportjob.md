---
title: deviceManagementExportJob 资源类型
description: 表示导出报告的作业的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 60977b341516fcd7fb331a49d188a6842a44b0cf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523805"
---
# <a name="devicemanagementexportjob-resource-type"></a><span data-ttu-id="c331e-103">deviceManagementExportJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="c331e-103">deviceManagementExportJob resource type</span></span>

<span data-ttu-id="c331e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c331e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c331e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c331e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c331e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c331e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c331e-107">表示导出报告的作业的实体</span><span class="sxs-lookup"><span data-stu-id="c331e-107">Entity representing a job to export a report</span></span>

## <a name="methods"></a><span data-ttu-id="c331e-108">方法</span><span class="sxs-lookup"><span data-stu-id="c331e-108">Methods</span></span>
|<span data-ttu-id="c331e-109">方法</span><span class="sxs-lookup"><span data-stu-id="c331e-109">Method</span></span>|<span data-ttu-id="c331e-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="c331e-110">Return Type</span></span>|<span data-ttu-id="c331e-111">说明</span><span class="sxs-lookup"><span data-stu-id="c331e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="c331e-112">列出 deviceManagementExportJobs</span><span class="sxs-lookup"><span data-stu-id="c331e-112">List deviceManagementExportJobs</span></span>](../api/intune-reporting-devicemanagementexportjob-list.md)|<span data-ttu-id="c331e-113">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="c331e-113">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) collection</span></span>|<span data-ttu-id="c331e-114">列出[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c331e-114">List properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) objects.</span></span>|
|[<span data-ttu-id="c331e-115">获取 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="c331e-115">Get deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-get.md)|[<span data-ttu-id="c331e-116">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="c331e-116">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="c331e-117">读取[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c331e-117">Read properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|
|[<span data-ttu-id="c331e-118">创建 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="c331e-118">Create deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-create.md)|[<span data-ttu-id="c331e-119">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="c331e-119">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="c331e-120">创建新的[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c331e-120">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|
|[<span data-ttu-id="c331e-121">删除 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="c331e-121">Delete deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-delete.md)|<span data-ttu-id="c331e-122">无</span><span class="sxs-lookup"><span data-stu-id="c331e-122">None</span></span>|<span data-ttu-id="c331e-123">删除[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)。</span><span class="sxs-lookup"><span data-stu-id="c331e-123">Deletes a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>|
|[<span data-ttu-id="c331e-124">更新 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="c331e-124">Update deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-update.md)|[<span data-ttu-id="c331e-125">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="c331e-125">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="c331e-126">更新[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c331e-126">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="c331e-127">属性</span><span class="sxs-lookup"><span data-stu-id="c331e-127">Properties</span></span>
|<span data-ttu-id="c331e-128">属性</span><span class="sxs-lookup"><span data-stu-id="c331e-128">Property</span></span>|<span data-ttu-id="c331e-129">类型</span><span class="sxs-lookup"><span data-stu-id="c331e-129">Type</span></span>|<span data-ttu-id="c331e-130">说明</span><span class="sxs-lookup"><span data-stu-id="c331e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c331e-131">id</span><span class="sxs-lookup"><span data-stu-id="c331e-131">id</span></span>|<span data-ttu-id="c331e-132">String</span><span class="sxs-lookup"><span data-stu-id="c331e-132">String</span></span>|<span data-ttu-id="c331e-133">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="c331e-133">Unique identifier for this entity</span></span>|
|<span data-ttu-id="c331e-134">reportName</span><span class="sxs-lookup"><span data-stu-id="c331e-134">reportName</span></span>|<span data-ttu-id="c331e-135">String</span><span class="sxs-lookup"><span data-stu-id="c331e-135">String</span></span>|<span data-ttu-id="c331e-136">报告的名称</span><span class="sxs-lookup"><span data-stu-id="c331e-136">Name of the report</span></span>|
|<span data-ttu-id="c331e-137">filter</span><span class="sxs-lookup"><span data-stu-id="c331e-137">filter</span></span>|<span data-ttu-id="c331e-138">String</span><span class="sxs-lookup"><span data-stu-id="c331e-138">String</span></span>|<span data-ttu-id="c331e-139">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="c331e-139">Filters applied on the report</span></span>|
|<span data-ttu-id="c331e-140">select</span><span class="sxs-lookup"><span data-stu-id="c331e-140">select</span></span>|<span data-ttu-id="c331e-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="c331e-141">String collection</span></span>|<span data-ttu-id="c331e-142">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="c331e-142">Columns selected from the report</span></span>|
|<span data-ttu-id="c331e-143">format</span><span class="sxs-lookup"><span data-stu-id="c331e-143">format</span></span>|[<span data-ttu-id="c331e-144">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="c331e-144">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="c331e-145">导出的报表的格式。</span><span class="sxs-lookup"><span data-stu-id="c331e-145">Format of the exported report.</span></span> <span data-ttu-id="c331e-146">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="c331e-146">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="c331e-147">snapshotId</span><span class="sxs-lookup"><span data-stu-id="c331e-147">snapshotId</span></span>|<span data-ttu-id="c331e-148">String</span><span class="sxs-lookup"><span data-stu-id="c331e-148">String</span></span>|<span data-ttu-id="c331e-149">快照是由 ReportName 表示的数据集的可识别子集。</span><span class="sxs-lookup"><span data-stu-id="c331e-149">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="c331e-150">可以在此处使用 sessionId 或 CachedReportConfiguration id。</span><span class="sxs-lookup"><span data-stu-id="c331e-150">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="c331e-151">如果指定了 sessionId，则筛选器、Select 和 OrderBy 将应用于 sessionId 所代表的数据。</span><span class="sxs-lookup"><span data-stu-id="c331e-151">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="c331e-152">Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。</span><span class="sxs-lookup"><span data-stu-id="c331e-152">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="c331e-153">status</span><span class="sxs-lookup"><span data-stu-id="c331e-153">status</span></span>|[<span data-ttu-id="c331e-154">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="c331e-154">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="c331e-155">导出作业的状态。</span><span class="sxs-lookup"><span data-stu-id="c331e-155">Status of the export job.</span></span> <span data-ttu-id="c331e-156">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="c331e-156">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="c331e-157">url</span><span class="sxs-lookup"><span data-stu-id="c331e-157">url</span></span>|<span data-ttu-id="c331e-158">String</span><span class="sxs-lookup"><span data-stu-id="c331e-158">String</span></span>|<span data-ttu-id="c331e-159">导出报告的临时位置</span><span class="sxs-lookup"><span data-stu-id="c331e-159">Temporary location of the exported report</span></span>|
|<span data-ttu-id="c331e-160">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="c331e-160">requestDateTime</span></span>|<span data-ttu-id="c331e-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c331e-161">DateTimeOffset</span></span>|<span data-ttu-id="c331e-162">请求导出的报告的时间</span><span class="sxs-lookup"><span data-stu-id="c331e-162">Time that the exported report was requested</span></span>|
|<span data-ttu-id="c331e-163">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c331e-163">expirationDateTime</span></span>|<span data-ttu-id="c331e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c331e-164">DateTimeOffset</span></span>|<span data-ttu-id="c331e-165">导出的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="c331e-165">Time that the exported report expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="c331e-166">关系</span><span class="sxs-lookup"><span data-stu-id="c331e-166">Relationships</span></span>
<span data-ttu-id="c331e-167">无</span><span class="sxs-lookup"><span data-stu-id="c331e-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c331e-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c331e-168">JSON Representation</span></span>
<span data-ttu-id="c331e-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c331e-169">Here is a JSON representation of the resource.</span></span>
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
  "format": "String",
  "snapshotId": "String",
  "status": "String",
  "url": "String",
  "requestDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



