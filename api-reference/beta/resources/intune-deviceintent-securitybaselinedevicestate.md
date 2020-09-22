---
title: securityBaselineDeviceState 资源类型
description: 设备安全基准的安全基准合规性状态摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae779d85027ff70424d05418c0cd24ae3560e1aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060949"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="74ee6-103">securityBaselineDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="74ee6-103">securityBaselineDeviceState resource type</span></span>

<span data-ttu-id="74ee6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="74ee6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="74ee6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="74ee6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74ee6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="74ee6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74ee6-107">设备安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="74ee6-107">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="74ee6-108">方法</span><span class="sxs-lookup"><span data-stu-id="74ee6-108">Methods</span></span>
|<span data-ttu-id="74ee6-109">方法</span><span class="sxs-lookup"><span data-stu-id="74ee6-109">Method</span></span>|<span data-ttu-id="74ee6-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="74ee6-110">Return Type</span></span>|<span data-ttu-id="74ee6-111">说明</span><span class="sxs-lookup"><span data-stu-id="74ee6-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="74ee6-112">列出 securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="74ee6-112">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="74ee6-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="74ee6-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="74ee6-114">列出 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74ee6-114">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="74ee6-115">获取 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="74ee6-115">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="74ee6-116">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="74ee6-116">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="74ee6-117">读取 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="74ee6-117">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="74ee6-118">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="74ee6-118">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="74ee6-119">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="74ee6-119">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="74ee6-120">创建新的 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="74ee6-120">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="74ee6-121">删除 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="74ee6-121">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="74ee6-122">无</span><span class="sxs-lookup"><span data-stu-id="74ee6-122">None</span></span>|<span data-ttu-id="74ee6-123">删除 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="74ee6-123">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="74ee6-124">更新 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="74ee6-124">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="74ee6-125">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="74ee6-125">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="74ee6-126">更新 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="74ee6-126">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="74ee6-127">属性</span><span class="sxs-lookup"><span data-stu-id="74ee6-127">Properties</span></span>
|<span data-ttu-id="74ee6-128">属性</span><span class="sxs-lookup"><span data-stu-id="74ee6-128">Property</span></span>|<span data-ttu-id="74ee6-129">类型</span><span class="sxs-lookup"><span data-stu-id="74ee6-129">Type</span></span>|<span data-ttu-id="74ee6-130">说明</span><span class="sxs-lookup"><span data-stu-id="74ee6-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74ee6-131">id</span><span class="sxs-lookup"><span data-stu-id="74ee6-131">id</span></span>|<span data-ttu-id="74ee6-132">String</span><span class="sxs-lookup"><span data-stu-id="74ee6-132">String</span></span>|<span data-ttu-id="74ee6-133">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="74ee6-133">Unique identifier of the entity</span></span>|
|<span data-ttu-id="74ee6-134">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="74ee6-134">managedDeviceId</span></span>|<span data-ttu-id="74ee6-135">String</span><span class="sxs-lookup"><span data-stu-id="74ee6-135">String</span></span>|<span data-ttu-id="74ee6-136">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="74ee6-136">Intune device id</span></span>|
|<span data-ttu-id="74ee6-137">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="74ee6-137">deviceDisplayName</span></span>|<span data-ttu-id="74ee6-138">String</span><span class="sxs-lookup"><span data-stu-id="74ee6-138">String</span></span>|<span data-ttu-id="74ee6-139">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="74ee6-139">Display name of the device</span></span>|
|<span data-ttu-id="74ee6-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="74ee6-140">userPrincipalName</span></span>|<span data-ttu-id="74ee6-141">String</span><span class="sxs-lookup"><span data-stu-id="74ee6-141">String</span></span>|<span data-ttu-id="74ee6-142">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="74ee6-142">User Principal Name</span></span>|
|<span data-ttu-id="74ee6-143">state</span><span class="sxs-lookup"><span data-stu-id="74ee6-143">state</span></span>|[<span data-ttu-id="74ee6-144">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="74ee6-144">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="74ee6-145">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="74ee6-145">Security baseline compliance state.</span></span> <span data-ttu-id="74ee6-146">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="74ee6-146">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="74ee6-147">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="74ee6-147">lastReportedDateTime</span></span>|<span data-ttu-id="74ee6-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="74ee6-148">DateTimeOffset</span></span>|<span data-ttu-id="74ee6-149">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="74ee6-149">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="74ee6-150">关系</span><span class="sxs-lookup"><span data-stu-id="74ee6-150">Relationships</span></span>
<span data-ttu-id="74ee6-151">无</span><span class="sxs-lookup"><span data-stu-id="74ee6-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="74ee6-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="74ee6-152">JSON Representation</span></span>
<span data-ttu-id="74ee6-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="74ee6-153">Here is a JSON representation of the resource.</span></span>
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






