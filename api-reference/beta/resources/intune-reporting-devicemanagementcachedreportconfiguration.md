---
title: deviceManagementCachedReportConfiguration 资源类型
description: 表示缓存报告配置的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8bd2b3ef44c5522011f15f2a1335b325a666f63c
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539041"
---
# <a name="devicemanagementcachedreportconfiguration-resource-type"></a><span data-ttu-id="810b2-103">deviceManagementCachedReportConfiguration 资源类型</span><span class="sxs-lookup"><span data-stu-id="810b2-103">deviceManagementCachedReportConfiguration resource type</span></span>

> <span data-ttu-id="810b2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="810b2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="810b2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="810b2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="810b2-106">表示缓存报告配置的实体</span><span class="sxs-lookup"><span data-stu-id="810b2-106">Entity representing the configuration of a cached report</span></span>

## <a name="methods"></a><span data-ttu-id="810b2-107">方法</span><span class="sxs-lookup"><span data-stu-id="810b2-107">Methods</span></span>
|<span data-ttu-id="810b2-108">方法</span><span class="sxs-lookup"><span data-stu-id="810b2-108">Method</span></span>|<span data-ttu-id="810b2-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="810b2-109">Return Type</span></span>|<span data-ttu-id="810b2-110">说明</span><span class="sxs-lookup"><span data-stu-id="810b2-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="810b2-111">列出 deviceManagementCachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="810b2-111">List deviceManagementCachedReportConfigurations</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-list.md)|<span data-ttu-id="810b2-112">[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)集合</span><span class="sxs-lookup"><span data-stu-id="810b2-112">[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) collection</span></span>|<span data-ttu-id="810b2-113">列出[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="810b2-113">List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="810b2-114">获取 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="810b2-114">Get deviceManagementCachedReportConfiguration</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-get.md)|[<span data-ttu-id="810b2-115">deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="810b2-115">deviceManagementCachedReportConfiguration</span></span>](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|<span data-ttu-id="810b2-116">读取[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="810b2-116">Read properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>|
|[<span data-ttu-id="810b2-117">创建 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="810b2-117">Create deviceManagementCachedReportConfiguration</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-create.md)|[<span data-ttu-id="810b2-118">deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="810b2-118">deviceManagementCachedReportConfiguration</span></span>](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|<span data-ttu-id="810b2-119">创建新的[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="810b2-119">Create a new [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>|
|[<span data-ttu-id="810b2-120">删除 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="810b2-120">Delete deviceManagementCachedReportConfiguration</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-delete.md)|<span data-ttu-id="810b2-121">无</span><span class="sxs-lookup"><span data-stu-id="810b2-121">None</span></span>|<span data-ttu-id="810b2-122">删除[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="810b2-122">Deletes a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md).</span></span>|
|[<span data-ttu-id="810b2-123">更新 deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="810b2-123">Update deviceManagementCachedReportConfiguration</span></span>](../api/intune-reporting-devicemanagementcachedreportconfiguration-update.md)|[<span data-ttu-id="810b2-124">deviceManagementCachedReportConfiguration</span><span class="sxs-lookup"><span data-stu-id="810b2-124">deviceManagementCachedReportConfiguration</span></span>](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)|<span data-ttu-id="810b2-125">更新[deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="810b2-125">Update the properties of a [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="810b2-126">属性</span><span class="sxs-lookup"><span data-stu-id="810b2-126">Properties</span></span>
|<span data-ttu-id="810b2-127">属性</span><span class="sxs-lookup"><span data-stu-id="810b2-127">Property</span></span>|<span data-ttu-id="810b2-128">类型</span><span class="sxs-lookup"><span data-stu-id="810b2-128">Type</span></span>|<span data-ttu-id="810b2-129">说明</span><span class="sxs-lookup"><span data-stu-id="810b2-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="810b2-130">id</span><span class="sxs-lookup"><span data-stu-id="810b2-130">id</span></span>|<span data-ttu-id="810b2-131">字符串</span><span class="sxs-lookup"><span data-stu-id="810b2-131">String</span></span>|<span data-ttu-id="810b2-132">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="810b2-132">Unique identifier for this entity</span></span>|
|<span data-ttu-id="810b2-133">reportName</span><span class="sxs-lookup"><span data-stu-id="810b2-133">reportName</span></span>|<span data-ttu-id="810b2-134">字符串</span><span class="sxs-lookup"><span data-stu-id="810b2-134">String</span></span>|<span data-ttu-id="810b2-135">报告的名称</span><span class="sxs-lookup"><span data-stu-id="810b2-135">Name of the report</span></span>|
|<span data-ttu-id="810b2-136">filter</span><span class="sxs-lookup"><span data-stu-id="810b2-136">filter</span></span>|<span data-ttu-id="810b2-137">字符串</span><span class="sxs-lookup"><span data-stu-id="810b2-137">String</span></span>|<span data-ttu-id="810b2-138">在创建报表时应用的筛选器。</span><span class="sxs-lookup"><span data-stu-id="810b2-138">Filters applied on report creation.</span></span>|
|<span data-ttu-id="810b2-139">select</span><span class="sxs-lookup"><span data-stu-id="810b2-139">select</span></span>|<span data-ttu-id="810b2-140">String 集合</span><span class="sxs-lookup"><span data-stu-id="810b2-140">String collection</span></span>|<span data-ttu-id="810b2-141">从报告中选择的列</span><span class="sxs-lookup"><span data-stu-id="810b2-141">Columns selected from the report</span></span>|
|<span data-ttu-id="810b2-142">By</span><span class="sxs-lookup"><span data-stu-id="810b2-142">orderBy</span></span>|<span data-ttu-id="810b2-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="810b2-143">String collection</span></span>|<span data-ttu-id="810b2-144">报表中的列的排序</span><span class="sxs-lookup"><span data-stu-id="810b2-144">Ordering of columns in the report</span></span>|
|<span data-ttu-id="810b2-145">status</span><span class="sxs-lookup"><span data-stu-id="810b2-145">status</span></span>|[<span data-ttu-id="810b2-146">deviceManagementReportStatus</span><span class="sxs-lookup"><span data-stu-id="810b2-146">deviceManagementReportStatus</span></span>](../resources/intune-reporting-devicemanagementreportstatus.md)|<span data-ttu-id="810b2-147">缓存报告的状态。</span><span class="sxs-lookup"><span data-stu-id="810b2-147">Status of the cached report.</span></span> <span data-ttu-id="810b2-148">可取值为：`unknown`、`notStarted`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="810b2-148">Possible values are: `unknown`, `notStarted`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="810b2-149">lastRefreshDateTime</span><span class="sxs-lookup"><span data-stu-id="810b2-149">lastRefreshDateTime</span></span>|<span data-ttu-id="810b2-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="810b2-150">DateTimeOffset</span></span>|<span data-ttu-id="810b2-151">上次刷新缓存的报告的时间</span><span class="sxs-lookup"><span data-stu-id="810b2-151">Time that the cached report was last refreshed</span></span>|
|<span data-ttu-id="810b2-152">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="810b2-152">expirationDateTime</span></span>|<span data-ttu-id="810b2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="810b2-153">DateTimeOffset</span></span>|<span data-ttu-id="810b2-154">缓存的报表到期的时间</span><span class="sxs-lookup"><span data-stu-id="810b2-154">Time that the cached report expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="810b2-155">关系</span><span class="sxs-lookup"><span data-stu-id="810b2-155">Relationships</span></span>
<span data-ttu-id="810b2-156">无</span><span class="sxs-lookup"><span data-stu-id="810b2-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="810b2-157">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="810b2-157">JSON Representation</span></span>
<span data-ttu-id="810b2-158">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="810b2-158">Here is a JSON representation of the resource.</span></span>
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
  "status": "String",
  "lastRefreshDateTime": "String (timestamp)",
  "expirationDateTime": "String (timestamp)"
}
```



