---
title: securityBaselineDeviceState 资源类型
description: 设备安全基准的安全基准合规性状态摘要。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b9fb2195a2cdf68c85e05988b1d2063d21a97228
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983440"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="fe1e7-103">securityBaselineDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="fe1e7-103">securityBaselineDeviceState resource type</span></span>

> <span data-ttu-id="fe1e7-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fe1e7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fe1e7-106">设备安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-106">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="fe1e7-107">方法</span><span class="sxs-lookup"><span data-stu-id="fe1e7-107">Methods</span></span>
|<span data-ttu-id="fe1e7-108">方法</span><span class="sxs-lookup"><span data-stu-id="fe1e7-108">Method</span></span>|<span data-ttu-id="fe1e7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fe1e7-109">Return Type</span></span>|<span data-ttu-id="fe1e7-110">说明</span><span class="sxs-lookup"><span data-stu-id="fe1e7-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="fe1e7-111">列出 securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="fe1e7-111">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="fe1e7-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="fe1e7-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="fe1e7-113">列出[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-113">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="fe1e7-114">获取 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="fe1e7-114">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="fe1e7-115">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="fe1e7-115">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="fe1e7-116">读取[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-116">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="fe1e7-117">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="fe1e7-117">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="fe1e7-118">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="fe1e7-118">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="fe1e7-119">创建新的[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-119">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="fe1e7-120">删除 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="fe1e7-120">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="fe1e7-121">无</span><span class="sxs-lookup"><span data-stu-id="fe1e7-121">None</span></span>|<span data-ttu-id="fe1e7-122">删除[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-122">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="fe1e7-123">更新 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="fe1e7-123">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="fe1e7-124">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="fe1e7-124">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="fe1e7-125">更新[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-125">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe1e7-126">属性</span><span class="sxs-lookup"><span data-stu-id="fe1e7-126">Properties</span></span>
|<span data-ttu-id="fe1e7-127">属性</span><span class="sxs-lookup"><span data-stu-id="fe1e7-127">Property</span></span>|<span data-ttu-id="fe1e7-128">类型</span><span class="sxs-lookup"><span data-stu-id="fe1e7-128">Type</span></span>|<span data-ttu-id="fe1e7-129">说明</span><span class="sxs-lookup"><span data-stu-id="fe1e7-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fe1e7-130">id</span><span class="sxs-lookup"><span data-stu-id="fe1e7-130">id</span></span>|<span data-ttu-id="fe1e7-131">String</span><span class="sxs-lookup"><span data-stu-id="fe1e7-131">String</span></span>|<span data-ttu-id="fe1e7-132">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="fe1e7-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="fe1e7-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="fe1e7-133">managedDeviceId</span></span>|<span data-ttu-id="fe1e7-134">String</span><span class="sxs-lookup"><span data-stu-id="fe1e7-134">String</span></span>|<span data-ttu-id="fe1e7-135">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="fe1e7-135">Intune device id</span></span>|
|<span data-ttu-id="fe1e7-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="fe1e7-136">deviceDisplayName</span></span>|<span data-ttu-id="fe1e7-137">String</span><span class="sxs-lookup"><span data-stu-id="fe1e7-137">String</span></span>|<span data-ttu-id="fe1e7-138">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="fe1e7-138">Display name of the device</span></span>|
|<span data-ttu-id="fe1e7-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fe1e7-139">userPrincipalName</span></span>|<span data-ttu-id="fe1e7-140">String</span><span class="sxs-lookup"><span data-stu-id="fe1e7-140">String</span></span>|<span data-ttu-id="fe1e7-141">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="fe1e7-141">User Principal Name</span></span>|
|<span data-ttu-id="fe1e7-142">state</span><span class="sxs-lookup"><span data-stu-id="fe1e7-142">state</span></span>|[<span data-ttu-id="fe1e7-143">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="fe1e7-143">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="fe1e7-144">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-144">Security baseline compliance state.</span></span> <span data-ttu-id="fe1e7-145">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-145">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="fe1e7-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe1e7-146">lastReportedDateTime</span></span>|<span data-ttu-id="fe1e7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe1e7-147">DateTimeOffset</span></span>|<span data-ttu-id="fe1e7-148">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="fe1e7-148">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe1e7-149">关系</span><span class="sxs-lookup"><span data-stu-id="fe1e7-149">Relationships</span></span>
<span data-ttu-id="fe1e7-150">无</span><span class="sxs-lookup"><span data-stu-id="fe1e7-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe1e7-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe1e7-151">JSON Representation</span></span>
<span data-ttu-id="fe1e7-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe1e7-152">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineDeviceState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
  "id": "String (identifier)",
  "managedDeviceId": "String",
  "deviceDisplayName": "String",
  "userPrincipalName": "String",
  "state": "String",
  "lastReportedDateTime": "String (timestamp)"
}
```





