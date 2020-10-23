---
title: securityBaselineDeviceState 资源类型
description: 设备安全基准的安全基准合规性状态摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 33d3b6614957426c48d2f8b9ee9b4ac8b5941ed1
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696081"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="78383-103">securityBaselineDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="78383-103">securityBaselineDeviceState resource type</span></span>

<span data-ttu-id="78383-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="78383-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="78383-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="78383-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78383-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="78383-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78383-107">设备安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="78383-107">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="78383-108">Methods</span><span class="sxs-lookup"><span data-stu-id="78383-108">Methods</span></span>
|<span data-ttu-id="78383-109">方法</span><span class="sxs-lookup"><span data-stu-id="78383-109">Method</span></span>|<span data-ttu-id="78383-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="78383-110">Return Type</span></span>|<span data-ttu-id="78383-111">说明</span><span class="sxs-lookup"><span data-stu-id="78383-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78383-112">列出 securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="78383-112">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="78383-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="78383-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="78383-114">列出 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="78383-114">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="78383-115">获取 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="78383-115">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="78383-116">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="78383-116">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="78383-117">读取 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="78383-117">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="78383-118">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="78383-118">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="78383-119">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="78383-119">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="78383-120">创建新的 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="78383-120">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="78383-121">删除 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="78383-121">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="78383-122">无</span><span class="sxs-lookup"><span data-stu-id="78383-122">None</span></span>|<span data-ttu-id="78383-123">删除 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="78383-123">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="78383-124">更新 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="78383-124">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="78383-125">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="78383-125">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="78383-126">更新 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="78383-126">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="78383-127">属性</span><span class="sxs-lookup"><span data-stu-id="78383-127">Properties</span></span>
|<span data-ttu-id="78383-128">属性</span><span class="sxs-lookup"><span data-stu-id="78383-128">Property</span></span>|<span data-ttu-id="78383-129">类型</span><span class="sxs-lookup"><span data-stu-id="78383-129">Type</span></span>|<span data-ttu-id="78383-130">说明</span><span class="sxs-lookup"><span data-stu-id="78383-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78383-131">id</span><span class="sxs-lookup"><span data-stu-id="78383-131">id</span></span>|<span data-ttu-id="78383-132">String</span><span class="sxs-lookup"><span data-stu-id="78383-132">String</span></span>|<span data-ttu-id="78383-133">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="78383-133">Unique identifier of the entity</span></span>|
|<span data-ttu-id="78383-134">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="78383-134">managedDeviceId</span></span>|<span data-ttu-id="78383-135">String</span><span class="sxs-lookup"><span data-stu-id="78383-135">String</span></span>|<span data-ttu-id="78383-136">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="78383-136">Intune device id</span></span>|
|<span data-ttu-id="78383-137">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="78383-137">deviceDisplayName</span></span>|<span data-ttu-id="78383-138">String</span><span class="sxs-lookup"><span data-stu-id="78383-138">String</span></span>|<span data-ttu-id="78383-139">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="78383-139">Display name of the device</span></span>|
|<span data-ttu-id="78383-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="78383-140">userPrincipalName</span></span>|<span data-ttu-id="78383-141">String</span><span class="sxs-lookup"><span data-stu-id="78383-141">String</span></span>|<span data-ttu-id="78383-142">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="78383-142">User Principal Name</span></span>|
|<span data-ttu-id="78383-143">state</span><span class="sxs-lookup"><span data-stu-id="78383-143">state</span></span>|[<span data-ttu-id="78383-144">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="78383-144">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="78383-145">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="78383-145">Security baseline compliance state.</span></span> <span data-ttu-id="78383-146">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="78383-146">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="78383-147">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="78383-147">lastReportedDateTime</span></span>|<span data-ttu-id="78383-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78383-148">DateTimeOffset</span></span>|<span data-ttu-id="78383-149">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="78383-149">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="78383-150">关系</span><span class="sxs-lookup"><span data-stu-id="78383-150">Relationships</span></span>
<span data-ttu-id="78383-151">无</span><span class="sxs-lookup"><span data-stu-id="78383-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="78383-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="78383-152">JSON Representation</span></span>
<span data-ttu-id="78383-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="78383-153">Here is a JSON representation of the resource.</span></span>
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





