---
title: deviceManagementCachedReportConfiguration 资源类型
description: 表示缓存报告配置的实体
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 01a13b6f8b2b11743469770826bdacf9db4eb2ed
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793617"
---
# <a name="devicemanagementcachedreportconfiguration-resource-type"></a><span data-ttu-id="84a24-103">deviceManagementCachedReportConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="84a24-103">deviceManagementCachedReportConfiguration resource type</span></span>

<span data-ttu-id="84a24-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84a24-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84a24-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84a24-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84a24-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84a24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84a24-107">表示缓存报告配置的实体</span><span class="sxs-lookup"><span data-stu-id="84a24-107">Entity representing the configuration of a cached report</span></span>

## <a name="methods"></a><span data-ttu-id="84a24-108">Methods</span><span class="sxs-lookup"><span data-stu-id="84a24-108">Methods</span></span>
|<span data-ttu-id="84a24-109">方法</span><span class="sxs-lookup"><span data-stu-id="84a24-109">Method</span></span>|<span data-ttu-id="84a24-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="84a24-110">Return Type</span></span>|<span data-ttu-id="84a24-111">说明</span><span class="sxs-lookup"><span data-stu-id="84a24-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="84a24-112">列出 deviceManagementCachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="84a24-112">List deviceManagementCachedReportConfigurations</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-list.md)|<span data-ttu-id="84a24-113">[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="84a24-113">[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) collection</span></span>|<span data-ttu-id="84a24-114">列出[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84a24-114">List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="84a24-115">获取 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a24-115">Get deviceManagementCachedReportConfiguration</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-get.md)|[<span data-ttu-id="84a24-116">deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a24-116">deviceManagementCachedReportConfiguration</span></span>](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|<span data-ttu-id="84a24-117">读取[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84a24-117">Read properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>|
|[<span data-ttu-id="84a24-118">创建 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a24-118">Create deviceManagementCachedReportConfiguration</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-create.md)|[<span data-ttu-id="84a24-119">deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a24-119">deviceManagementCachedReportConfiguration</span></span>](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|<span data-ttu-id="84a24-120">创建新的[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84a24-120">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>|
|[<span data-ttu-id="84a24-121">删除 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a24-121">Delete deviceManagementCachedReportConfiguration</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-delete.md)|<span data-ttu-id="84a24-122">无</span><span class="sxs-lookup"><span data-stu-id="84a24-122">None</span></span>|<span data-ttu-id="84a24-123">删除[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="84a24-123">Deletes a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>|
|[<span data-ttu-id="84a24-124">更新 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a24-124">Update deviceManagementCachedReportConfiguration</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-update.md)|[<span data-ttu-id="84a24-125">deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="84a24-125">deviceManagementCachedReportConfiguration</span></span>](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|<span data-ttu-id="84a24-126">更新[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84a24-126">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="84a24-127">属性</span><span class="sxs-lookup"><span data-stu-id="84a24-127">Properties</span></span>
|<span data-ttu-id="84a24-128">属性</span><span class="sxs-lookup"><span data-stu-id="84a24-128">Property</span></span>|<span data-ttu-id="84a24-129">类型</span><span class="sxs-lookup"><span data-stu-id="84a24-129">Type</span></span>|<span data-ttu-id="84a24-130">说明</span><span class="sxs-lookup"><span data-stu-id="84a24-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84a24-131">id</span><span class="sxs-lookup"><span data-stu-id="84a24-131">id</span></span>|<span data-ttu-id="84a24-132">String</span><span class="sxs-lookup"><span data-stu-id="84a24-132">String</span></span>|<span data-ttu-id="84a24-133">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="84a24-133">Unique identifier for this entity</span></span>|
|<span data-ttu-id="84a24-134">reportName</span><span class="sxs-lookup"><span data-stu-id="84a24-134">reportName</span></span>|<span data-ttu-id="84a24-135">String</span><span class="sxs-lookup"><span data-stu-id="84a24-135">String</span></span>|<span data-ttu-id="84a24-136">报告的名称</span><span class="sxs-lookup"><span data-stu-id="84a24-136">Name of the report</span></span>|
|<span data-ttu-id="84a24-137">filter</span><span class="sxs-lookup"><span data-stu-id="84a24-137">filter</span></span>|<span data-ttu-id="84a24-138">String</span><span class="sxs-lookup"><span data-stu-id="84a24-138">String</span></span>|<span data-ttu-id="84a24-139">在创建报表时应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="84a24-139">Filters applied on report creation.</span></span>|
|<span data-ttu-id="84a24-140">select</span><span class="sxs-lookup"><span data-stu-id="84a24-140">select</span></span>|<span data-ttu-id="84a24-141">String collection</span><span class="sxs-lookup"><span data-stu-id="84a24-141">String collection</span></span>|<span data-ttu-id="84a24-142">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="84a24-142">Columns selected from the report</span></span>|
|<span data-ttu-id="84a24-143">By</span><span class="sxs-lookup"><span data-stu-id="84a24-143">orderBy</span></span>|<span data-ttu-id="84a24-144">String collection</span><span class="sxs-lookup"><span data-stu-id="84a24-144">String collection</span></span>|<span data-ttu-id="84a24-145">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="84a24-145">Ordering of columns in the report</span></span>|
|<span data-ttu-id="84a24-146">metadata</span><span class="sxs-lookup"><span data-stu-id="84a24-146">metadata</span></span>|<span data-ttu-id="84a24-147">String</span><span class="sxs-lookup"><span data-stu-id="84a24-147">String</span></span>|<span data-ttu-id="84a24-148">与报告关联的调用方托管元数据</span><span class="sxs-lookup"><span data-stu-id="84a24-148">Caller-managed metadata associated with the report</span></span>|
|<span data-ttu-id="84a24-149">status</span><span class="sxs-lookup"><span data-stu-id="84a24-149">status</span></span>|[<span data-ttu-id="84a24-150">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="84a24-150">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="84a24-151">缓存报告的状态。</span><span class="sxs-lookup"><span data-stu-id="84a24-151">Status of the cached report.</span></span> <span data-ttu-id="84a24-152">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="84a24-152">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="84a24-153">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="84a24-153">lastRefreshDateTime</span></span>|<span data-ttu-id="84a24-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84a24-154">DateTimeOffset</span></span>|<span data-ttu-id="84a24-155">上次刷新缓存的报告的时间</span><span class="sxs-lookup"><span data-stu-id="84a24-155">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="84a24-156">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="84a24-156">expirationDateTime</span></span>|<span data-ttu-id="84a24-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="84a24-157">DateTimeOffset</span></span>|<span data-ttu-id="84a24-158">缓存的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="84a24-158">Time that the cached report expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="84a24-159">关系</span><span class="sxs-lookup"><span data-stu-id="84a24-159">Relationships</span></span>
<span data-ttu-id="84a24-160">无</span><span class="sxs-lookup"><span data-stu-id="84a24-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="84a24-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84a24-161">JSON Representation</span></span>
<span data-ttu-id="84a24-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84a24-162">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementCachedReportConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
  "id": "String (identifier)",
  "reportName": "String",
  "filter": "String",
  "select": [
    "String"
  ],
  "orderBy": [
    "String"
  ],
  "metadata": "String",
  "status": "String",
  "lastRefreshDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



