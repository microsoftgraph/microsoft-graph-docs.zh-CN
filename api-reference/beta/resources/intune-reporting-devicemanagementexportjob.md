---
title: deviceManagementExportJob 资源类型
description: 表示导出报告的作业的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: e4bbbbd1e579fe8dc5b262cf5e855941227ed940
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38088285"
---
# <a name="devicemanagementexportjob-resource-type"></a><span data-ttu-id="738af-103">deviceManagementExportJob 资源类型</span><span class="sxs-lookup"><span data-stu-id="738af-103">deviceManagementExportJob resource type</span></span>

> <span data-ttu-id="738af-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="738af-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="738af-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="738af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="738af-106">表示导出报告的作业的实体</span><span class="sxs-lookup"><span data-stu-id="738af-106">Entity representing a job to export a report</span></span>

## <a name="methods"></a><span data-ttu-id="738af-107">方法</span><span class="sxs-lookup"><span data-stu-id="738af-107">Methods</span></span>
|<span data-ttu-id="738af-108">方法</span><span class="sxs-lookup"><span data-stu-id="738af-108">Method</span></span>|<span data-ttu-id="738af-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="738af-109">Return Type</span></span>|<span data-ttu-id="738af-110">说明</span><span class="sxs-lookup"><span data-stu-id="738af-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="738af-111">列出 deviceManagementExportJobs</span><span class="sxs-lookup"><span data-stu-id="738af-111">List deviceManagementExportJobs</span></span>](../api/intune-reporting-devicemanagementexportjob-list.md)|<span data-ttu-id="738af-112">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)集合</span><span class="sxs-lookup"><span data-stu-id="738af-112">[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) collection</span></span>|<span data-ttu-id="738af-113">列出[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="738af-113">List properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) objects.</span></span>|
|[<span data-ttu-id="738af-114">获取 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="738af-114">Get deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-get.md)|[<span data-ttu-id="738af-115">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="738af-115">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="738af-116">读取[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="738af-116">Read properties and relationships of the [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|
|[<span data-ttu-id="738af-117">创建 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="738af-117">Create deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-create.md)|[<span data-ttu-id="738af-118">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="738af-118">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="738af-119">创建新的[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象。</span><span class="sxs-lookup"><span data-stu-id="738af-119">Create a new [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|
|[<span data-ttu-id="738af-120">删除 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="738af-120">Delete deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-delete.md)|<span data-ttu-id="738af-121">无</span><span class="sxs-lookup"><span data-stu-id="738af-121">None</span></span>|<span data-ttu-id="738af-122">删除[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)。</span><span class="sxs-lookup"><span data-stu-id="738af-122">Deletes a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md).</span></span>|
|[<span data-ttu-id="738af-123">更新 deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="738af-123">Update deviceManagementExportJob</span></span>](../api/intune-reporting-devicemanagementexportjob-update.md)|[<span data-ttu-id="738af-124">deviceManagementExportJob</span><span class="sxs-lookup"><span data-stu-id="738af-124">deviceManagementExportJob</span></span>](../resources/intune-reporting-devicemanagementexportjob.md)|<span data-ttu-id="738af-125">更新[deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="738af-125">Update the properties of a [deviceManagementExportJob](../resources/intune-reporting-devicemanagementexportjob.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="738af-126">属性</span><span class="sxs-lookup"><span data-stu-id="738af-126">Properties</span></span>
|<span data-ttu-id="738af-127">属性</span><span class="sxs-lookup"><span data-stu-id="738af-127">Property</span></span>|<span data-ttu-id="738af-128">类型</span><span class="sxs-lookup"><span data-stu-id="738af-128">Type</span></span>|<span data-ttu-id="738af-129">说明</span><span class="sxs-lookup"><span data-stu-id="738af-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="738af-130">id</span><span class="sxs-lookup"><span data-stu-id="738af-130">id</span></span>|<span data-ttu-id="738af-131">String</span><span class="sxs-lookup"><span data-stu-id="738af-131">String</span></span>|<span data-ttu-id="738af-132">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="738af-132">Unique identifier for this entity</span></span>|
|<span data-ttu-id="738af-133">reportName</span><span class="sxs-lookup"><span data-stu-id="738af-133">reportName</span></span>|<span data-ttu-id="738af-134">String</span><span class="sxs-lookup"><span data-stu-id="738af-134">String</span></span>|<span data-ttu-id="738af-135">报告的名称</span><span class="sxs-lookup"><span data-stu-id="738af-135">Name of the report</span></span>|
|<span data-ttu-id="738af-136">filter</span><span class="sxs-lookup"><span data-stu-id="738af-136">filter</span></span>|<span data-ttu-id="738af-137">String</span><span class="sxs-lookup"><span data-stu-id="738af-137">String</span></span>|<span data-ttu-id="738af-138">在报表上应用的筛选器</span><span class="sxs-lookup"><span data-stu-id="738af-138">Filters applied on the report</span></span>|
|<span data-ttu-id="738af-139">select</span><span class="sxs-lookup"><span data-stu-id="738af-139">select</span></span>|<span data-ttu-id="738af-140">String collection</span><span class="sxs-lookup"><span data-stu-id="738af-140">String collection</span></span>|<span data-ttu-id="738af-141">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="738af-141">Columns selected from the report</span></span>|
|<span data-ttu-id="738af-142">format</span><span class="sxs-lookup"><span data-stu-id="738af-142">format</span></span>|[<span data-ttu-id="738af-143">deviceManagementReportFileFormat</span><span class="sxs-lookup"><span data-stu-id="738af-143">deviceManagementReportFileFormat</span></span>](../resources/intune-reporting-devicemanagementreportfileformat.md)|<span data-ttu-id="738af-144">导出的报表的格式。</span><span class="sxs-lookup"><span data-stu-id="738af-144">Format of the exported report.</span></span> <span data-ttu-id="738af-145">可取值为：`csv`、`pdf`。</span><span class="sxs-lookup"><span data-stu-id="738af-145">Possible values are: `csv`, `pdf`.</span></span>|
|<span data-ttu-id="738af-146">snapshotId</span><span class="sxs-lookup"><span data-stu-id="738af-146">snapshotId</span></span>|<span data-ttu-id="738af-147">String</span><span class="sxs-lookup"><span data-stu-id="738af-147">String</span></span>|<span data-ttu-id="738af-148">快照是由 ReportName 表示的数据集的可识别子集。</span><span class="sxs-lookup"><span data-stu-id="738af-148">A snapshot is an identifiable subset of the dataset represented by the ReportName.</span></span> <span data-ttu-id="738af-149">可以在此处使用 sessionId 或 CachedReportConfiguration id。</span><span class="sxs-lookup"><span data-stu-id="738af-149">A sessionId or CachedReportConfiguration id can be used here.</span></span> <span data-ttu-id="738af-150">如果指定了 sessionId，则筛选器、Select 和 OrderBy 将应用于 sessionId 所代表的数据。</span><span class="sxs-lookup"><span data-stu-id="738af-150">If a sessionId is specified, Filter, Select, and OrderBy are applied to the data represented by the sessionId.</span></span> <span data-ttu-id="738af-151">Filter、Select 和 OrderBy 不能与 CachedReportConfiguration id 一起指定。</span><span class="sxs-lookup"><span data-stu-id="738af-151">Filter, Select, and OrderBy cannot be specified together with a CachedReportConfiguration id.</span></span>|
|<span data-ttu-id="738af-152">状态</span><span class="sxs-lookup"><span data-stu-id="738af-152">status</span></span>|[<span data-ttu-id="738af-153">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="738af-153">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="738af-154">导出作业的状态。</span><span class="sxs-lookup"><span data-stu-id="738af-154">Status of the export job.</span></span> <span data-ttu-id="738af-155">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="738af-155">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="738af-156">url</span><span class="sxs-lookup"><span data-stu-id="738af-156">url</span></span>|<span data-ttu-id="738af-157">String</span><span class="sxs-lookup"><span data-stu-id="738af-157">String</span></span>|<span data-ttu-id="738af-158">导出报告的临时位置</span><span class="sxs-lookup"><span data-stu-id="738af-158">Temporary location of the exported report</span></span>|
|<span data-ttu-id="738af-159">requestDateTime</span><span class="sxs-lookup"><span data-stu-id="738af-159">requestDateTime</span></span>|<span data-ttu-id="738af-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="738af-160">DateTimeOffset</span></span>|<span data-ttu-id="738af-161">请求导出的报告的时间</span><span class="sxs-lookup"><span data-stu-id="738af-161">Time that the exported report was requested</span></span>|
|<span data-ttu-id="738af-162">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="738af-162">expirationDateTime</span></span>|<span data-ttu-id="738af-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="738af-163">DateTimeOffset</span></span>|<span data-ttu-id="738af-164">导出的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="738af-164">Time that the exported report expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="738af-165">关系</span><span class="sxs-lookup"><span data-stu-id="738af-165">Relationships</span></span>
<span data-ttu-id="738af-166">无</span><span class="sxs-lookup"><span data-stu-id="738af-166">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="738af-167">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="738af-167">JSON Representation</span></span>
<span data-ttu-id="738af-168">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="738af-168">Here is a JSON representation of the resource.</span></span>
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



