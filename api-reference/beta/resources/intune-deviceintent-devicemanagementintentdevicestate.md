---
title: deviceManagementIntentDeviceState 资源类型
description: 表示设备状态的意向的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 03951ac855e699856684e32e9baf36c40ce8e2f2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943317"
---
# <a name="devicemanagementintentdevicestate-resource-type"></a><span data-ttu-id="e6519-103">deviceManagementIntentDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6519-103">deviceManagementIntentDeviceState resource type</span></span>

> <span data-ttu-id="e6519-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e6519-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e6519-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6519-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6519-106">表示设备状态的意向的实体</span><span class="sxs-lookup"><span data-stu-id="e6519-106">Entity that represents device state for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="e6519-107">方法</span><span class="sxs-lookup"><span data-stu-id="e6519-107">Methods</span></span>
|<span data-ttu-id="e6519-108">方法</span><span class="sxs-lookup"><span data-stu-id="e6519-108">Method</span></span>|<span data-ttu-id="e6519-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="e6519-109">Return Type</span></span>|<span data-ttu-id="e6519-110">说明</span><span class="sxs-lookup"><span data-stu-id="e6519-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e6519-111">列出 deviceManagementIntentDeviceStates</span><span class="sxs-lookup"><span data-stu-id="e6519-111">List deviceManagementIntentDeviceStates</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-list.md)|<span data-ttu-id="e6519-112">[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="e6519-112">[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) collection</span></span>|<span data-ttu-id="e6519-113">列出[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e6519-113">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="e6519-114">获取 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="e6519-114">Get deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-get.md)|[<span data-ttu-id="e6519-115">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="e6519-115">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="e6519-116">读取[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e6519-116">Read properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|
|[<span data-ttu-id="e6519-117">创建 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="e6519-117">Create deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-create.md)|[<span data-ttu-id="e6519-118">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="e6519-118">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="e6519-119">创建新的[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e6519-119">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|
|[<span data-ttu-id="e6519-120">删除 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="e6519-120">Delete deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-delete.md)|<span data-ttu-id="e6519-121">无</span><span class="sxs-lookup"><span data-stu-id="e6519-121">None</span></span>|<span data-ttu-id="e6519-122">删除[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="e6519-122">Deletes a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>|
|[<span data-ttu-id="e6519-123">更新 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="e6519-123">Update deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-update.md)|[<span data-ttu-id="e6519-124">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="e6519-124">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="e6519-125">更新[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e6519-125">Update the properties of a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e6519-126">属性</span><span class="sxs-lookup"><span data-stu-id="e6519-126">Properties</span></span>
|<span data-ttu-id="e6519-127">属性</span><span class="sxs-lookup"><span data-stu-id="e6519-127">Property</span></span>|<span data-ttu-id="e6519-128">类型</span><span class="sxs-lookup"><span data-stu-id="e6519-128">Type</span></span>|<span data-ttu-id="e6519-129">说明</span><span class="sxs-lookup"><span data-stu-id="e6519-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6519-130">id</span><span class="sxs-lookup"><span data-stu-id="e6519-130">id</span></span>|<span data-ttu-id="e6519-131">String</span><span class="sxs-lookup"><span data-stu-id="e6519-131">String</span></span>|<span data-ttu-id="e6519-132">ID</span><span class="sxs-lookup"><span data-stu-id="e6519-132">The ID</span></span>|
|<span data-ttu-id="e6519-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6519-133">userPrincipalName</span></span>|<span data-ttu-id="e6519-134">String</span><span class="sxs-lookup"><span data-stu-id="e6519-134">String</span></span>|<span data-ttu-id="e6519-135">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="e6519-135">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="e6519-136">userName</span><span class="sxs-lookup"><span data-stu-id="e6519-136">userName</span></span>|<span data-ttu-id="e6519-137">String</span><span class="sxs-lookup"><span data-stu-id="e6519-137">String</span></span>|<span data-ttu-id="e6519-138">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="e6519-138">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="e6519-139">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6519-139">deviceDisplayName</span></span>|<span data-ttu-id="e6519-140">String</span><span class="sxs-lookup"><span data-stu-id="e6519-140">String</span></span>|<span data-ttu-id="e6519-141">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="e6519-141">Device name that is being reported</span></span>|
|<span data-ttu-id="e6519-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6519-142">lastReportedDateTime</span></span>|<span data-ttu-id="e6519-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6519-143">DateTimeOffset</span></span>|<span data-ttu-id="e6519-144">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="e6519-144">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="e6519-145">state</span><span class="sxs-lookup"><span data-stu-id="e6519-145">state</span></span>|[<span data-ttu-id="e6519-146">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e6519-146">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="e6519-147">意图的设备状态。</span><span class="sxs-lookup"><span data-stu-id="e6519-147">Device state for an intent.</span></span> <span data-ttu-id="e6519-148">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="e6519-148">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e6519-149">deviceId</span><span class="sxs-lookup"><span data-stu-id="e6519-149">deviceId</span></span>|<span data-ttu-id="e6519-150">String</span><span class="sxs-lookup"><span data-stu-id="e6519-150">String</span></span>|<span data-ttu-id="e6519-151">报告的设备 id</span><span class="sxs-lookup"><span data-stu-id="e6519-151">Device id that is being reported</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6519-152">关系</span><span class="sxs-lookup"><span data-stu-id="e6519-152">Relationships</span></span>
<span data-ttu-id="e6519-153">无</span><span class="sxs-lookup"><span data-stu-id="e6519-153">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6519-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6519-154">JSON Representation</span></span>
<span data-ttu-id="e6519-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6519-155">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentDeviceState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceDisplayName": "String",
  "lastReportedDateTime": "String (timestamp)",
  "state": "String",
  "deviceId": "String"
}
```




