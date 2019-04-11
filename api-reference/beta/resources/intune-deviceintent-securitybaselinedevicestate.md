---
title: securityBaselineDeviceState 资源类型
description: 设备安全基准的安全基准合规性状态摘要。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f1fb6bd8ee8e474fdf96bc2c70f4db288571d795
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31779795"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="bb05d-103">securityBaselineDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="bb05d-103">securityBaselineDeviceState resource type</span></span>

> <span data-ttu-id="bb05d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb05d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb05d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb05d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb05d-106">设备安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="bb05d-106">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="bb05d-107">方法</span><span class="sxs-lookup"><span data-stu-id="bb05d-107">Methods</span></span>
|<span data-ttu-id="bb05d-108">方法</span><span class="sxs-lookup"><span data-stu-id="bb05d-108">Method</span></span>|<span data-ttu-id="bb05d-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="bb05d-109">Return Type</span></span>|<span data-ttu-id="bb05d-110">说明</span><span class="sxs-lookup"><span data-stu-id="bb05d-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bb05d-111">列出 securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="bb05d-111">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="bb05d-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="bb05d-112">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="bb05d-113">列出[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb05d-113">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="bb05d-114">获取 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="bb05d-114">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="bb05d-115">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="bb05d-115">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="bb05d-116">读取[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bb05d-116">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="bb05d-117">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="bb05d-117">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="bb05d-118">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="bb05d-118">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="bb05d-119">创建新的[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bb05d-119">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="bb05d-120">删除 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="bb05d-120">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="bb05d-121">无</span><span class="sxs-lookup"><span data-stu-id="bb05d-121">None</span></span>|<span data-ttu-id="bb05d-122">删除[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="bb05d-122">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="bb05d-123">更新 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="bb05d-123">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="bb05d-124">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="bb05d-124">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="bb05d-125">更新[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bb05d-125">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bb05d-126">属性</span><span class="sxs-lookup"><span data-stu-id="bb05d-126">Properties</span></span>
|<span data-ttu-id="bb05d-127">属性</span><span class="sxs-lookup"><span data-stu-id="bb05d-127">Property</span></span>|<span data-ttu-id="bb05d-128">类型</span><span class="sxs-lookup"><span data-stu-id="bb05d-128">Type</span></span>|<span data-ttu-id="bb05d-129">说明</span><span class="sxs-lookup"><span data-stu-id="bb05d-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb05d-130">id</span><span class="sxs-lookup"><span data-stu-id="bb05d-130">id</span></span>|<span data-ttu-id="bb05d-131">String</span><span class="sxs-lookup"><span data-stu-id="bb05d-131">String</span></span>|<span data-ttu-id="bb05d-132">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="bb05d-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="bb05d-133">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="bb05d-133">managedDeviceId</span></span>|<span data-ttu-id="bb05d-134">String</span><span class="sxs-lookup"><span data-stu-id="bb05d-134">String</span></span>|<span data-ttu-id="bb05d-135">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="bb05d-135">Intune device id</span></span>|
|<span data-ttu-id="bb05d-136">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="bb05d-136">deviceDisplayName</span></span>|<span data-ttu-id="bb05d-137">String</span><span class="sxs-lookup"><span data-stu-id="bb05d-137">String</span></span>|<span data-ttu-id="bb05d-138">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="bb05d-138">Display name of the device</span></span>|
|<span data-ttu-id="bb05d-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="bb05d-139">userPrincipalName</span></span>|<span data-ttu-id="bb05d-140">String</span><span class="sxs-lookup"><span data-stu-id="bb05d-140">String</span></span>|<span data-ttu-id="bb05d-141">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="bb05d-141">User Principal Name</span></span>|
|<span data-ttu-id="bb05d-142">state</span><span class="sxs-lookup"><span data-stu-id="bb05d-142">state</span></span>|[<span data-ttu-id="bb05d-143">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="bb05d-143">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="bb05d-144">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="bb05d-144">Security baseline compliance state.</span></span> <span data-ttu-id="bb05d-145">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="bb05d-145">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="bb05d-146">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="bb05d-146">lastReportedDateTime</span></span>|<span data-ttu-id="bb05d-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bb05d-147">DateTimeOffset</span></span>|<span data-ttu-id="bb05d-148">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="bb05d-148">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="bb05d-149">关系</span><span class="sxs-lookup"><span data-stu-id="bb05d-149">Relationships</span></span>
<span data-ttu-id="bb05d-150">无</span><span class="sxs-lookup"><span data-stu-id="bb05d-150">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bb05d-151">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bb05d-151">JSON Representation</span></span>
<span data-ttu-id="bb05d-152">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bb05d-152">Here is a JSON representation of the resource.</span></span>
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





