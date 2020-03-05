---
title: deviceManagementIntentDeviceState 资源类型
description: 表示设备状态的意向的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 83b114fb4d3168cdafb09b89441ef7aa63833ef1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525297"
---
# <a name="devicemanagementintentdevicestate-resource-type"></a><span data-ttu-id="11f1a-103">deviceManagementIntentDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="11f1a-103">deviceManagementIntentDeviceState resource type</span></span>

<span data-ttu-id="11f1a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="11f1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11f1a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11f1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11f1a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11f1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11f1a-107">表示设备状态的意向的实体</span><span class="sxs-lookup"><span data-stu-id="11f1a-107">Entity that represents device state for an intent</span></span>

## <a name="methods"></a><span data-ttu-id="11f1a-108">方法</span><span class="sxs-lookup"><span data-stu-id="11f1a-108">Methods</span></span>
|<span data-ttu-id="11f1a-109">方法</span><span class="sxs-lookup"><span data-stu-id="11f1a-109">Method</span></span>|<span data-ttu-id="11f1a-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="11f1a-110">Return Type</span></span>|<span data-ttu-id="11f1a-111">说明</span><span class="sxs-lookup"><span data-stu-id="11f1a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="11f1a-112">列出 deviceManagementIntentDeviceStates</span><span class="sxs-lookup"><span data-stu-id="11f1a-112">List deviceManagementIntentDeviceStates</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-list.md)|<span data-ttu-id="11f1a-113">[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="11f1a-113">[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) collection</span></span>|<span data-ttu-id="11f1a-114">列出[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11f1a-114">List properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) objects.</span></span>|
|[<span data-ttu-id="11f1a-115">获取 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="11f1a-115">Get deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-get.md)|[<span data-ttu-id="11f1a-116">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="11f1a-116">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="11f1a-117">读取[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="11f1a-117">Read properties and relationships of the [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|
|[<span data-ttu-id="11f1a-118">创建 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="11f1a-118">Create deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-create.md)|[<span data-ttu-id="11f1a-119">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="11f1a-119">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="11f1a-120">创建新的[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="11f1a-120">Create a new [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|
|[<span data-ttu-id="11f1a-121">删除 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="11f1a-121">Delete deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-delete.md)|<span data-ttu-id="11f1a-122">无</span><span class="sxs-lookup"><span data-stu-id="11f1a-122">None</span></span>|<span data-ttu-id="11f1a-123">删除[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="11f1a-123">Deletes a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md).</span></span>|
|[<span data-ttu-id="11f1a-124">更新 deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="11f1a-124">Update deviceManagementIntentDeviceState</span></span>](../api/intune-deviceintent-devicemanagementintentdevicestate-update.md)|[<span data-ttu-id="11f1a-125">deviceManagementIntentDeviceState</span><span class="sxs-lookup"><span data-stu-id="11f1a-125">deviceManagementIntentDeviceState</span></span>](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)|<span data-ttu-id="11f1a-126">更新[deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="11f1a-126">Update the properties of a [deviceManagementIntentDeviceState](../resources/intune-deviceintent-devicemanagementintentdevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="11f1a-127">属性</span><span class="sxs-lookup"><span data-stu-id="11f1a-127">Properties</span></span>
|<span data-ttu-id="11f1a-128">属性</span><span class="sxs-lookup"><span data-stu-id="11f1a-128">Property</span></span>|<span data-ttu-id="11f1a-129">类型</span><span class="sxs-lookup"><span data-stu-id="11f1a-129">Type</span></span>|<span data-ttu-id="11f1a-130">说明</span><span class="sxs-lookup"><span data-stu-id="11f1a-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11f1a-131">id</span><span class="sxs-lookup"><span data-stu-id="11f1a-131">id</span></span>|<span data-ttu-id="11f1a-132">String</span><span class="sxs-lookup"><span data-stu-id="11f1a-132">String</span></span>|<span data-ttu-id="11f1a-133">ID</span><span class="sxs-lookup"><span data-stu-id="11f1a-133">The ID</span></span>|
|<span data-ttu-id="11f1a-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="11f1a-134">userPrincipalName</span></span>|<span data-ttu-id="11f1a-135">String</span><span class="sxs-lookup"><span data-stu-id="11f1a-135">String</span></span>|<span data-ttu-id="11f1a-136">在设备上报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="11f1a-136">The user principal name that is being reported on a device</span></span>|
|<span data-ttu-id="11f1a-137">userName</span><span class="sxs-lookup"><span data-stu-id="11f1a-137">userName</span></span>|<span data-ttu-id="11f1a-138">String</span><span class="sxs-lookup"><span data-stu-id="11f1a-138">String</span></span>|<span data-ttu-id="11f1a-139">在设备上报告的用户名</span><span class="sxs-lookup"><span data-stu-id="11f1a-139">The user name that is being reported on a device</span></span>|
|<span data-ttu-id="11f1a-140">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="11f1a-140">deviceDisplayName</span></span>|<span data-ttu-id="11f1a-141">String</span><span class="sxs-lookup"><span data-stu-id="11f1a-141">String</span></span>|<span data-ttu-id="11f1a-142">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="11f1a-142">Device name that is being reported</span></span>|
|<span data-ttu-id="11f1a-143">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="11f1a-143">lastReportedDateTime</span></span>|<span data-ttu-id="11f1a-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="11f1a-144">DateTimeOffset</span></span>|<span data-ttu-id="11f1a-145">意向报表的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="11f1a-145">Last modified date time of an intent report</span></span>|
|<span data-ttu-id="11f1a-146">state</span><span class="sxs-lookup"><span data-stu-id="11f1a-146">state</span></span>|[<span data-ttu-id="11f1a-147">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="11f1a-147">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="11f1a-148">意图的设备状态。</span><span class="sxs-lookup"><span data-stu-id="11f1a-148">Device state for an intent.</span></span> <span data-ttu-id="11f1a-149">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="11f1a-149">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="11f1a-150">deviceId</span><span class="sxs-lookup"><span data-stu-id="11f1a-150">deviceId</span></span>|<span data-ttu-id="11f1a-151">String</span><span class="sxs-lookup"><span data-stu-id="11f1a-151">String</span></span>|<span data-ttu-id="11f1a-152">报告的设备 id</span><span class="sxs-lookup"><span data-stu-id="11f1a-152">Device id that is being reported</span></span>|

## <a name="relationships"></a><span data-ttu-id="11f1a-153">关系</span><span class="sxs-lookup"><span data-stu-id="11f1a-153">Relationships</span></span>
<span data-ttu-id="11f1a-154">无</span><span class="sxs-lookup"><span data-stu-id="11f1a-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="11f1a-155">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11f1a-155">JSON Representation</span></span>
<span data-ttu-id="11f1a-156">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11f1a-156">Here is a JSON representation of the resource.</span></span>
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



