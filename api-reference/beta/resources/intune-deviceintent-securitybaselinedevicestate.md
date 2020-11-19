---
title: securityBaselineDeviceState 资源类型
description: 设备安全基准的安全基准合规性状态摘要。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9188446a5c270b7dc25e21b9880ecec479dfa90f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49209330"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="4b38b-103">securityBaselineDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="4b38b-103">securityBaselineDeviceState resource type</span></span>

<span data-ttu-id="4b38b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b38b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b38b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4b38b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4b38b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b38b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b38b-107">设备安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="4b38b-107">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="4b38b-108">方法</span><span class="sxs-lookup"><span data-stu-id="4b38b-108">Methods</span></span>
|<span data-ttu-id="4b38b-109">方法</span><span class="sxs-lookup"><span data-stu-id="4b38b-109">Method</span></span>|<span data-ttu-id="4b38b-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="4b38b-110">Return Type</span></span>|<span data-ttu-id="4b38b-111">说明</span><span class="sxs-lookup"><span data-stu-id="4b38b-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b38b-112">列出 securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="4b38b-112">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="4b38b-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b38b-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="4b38b-114">列出 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b38b-114">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="4b38b-115">获取 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="4b38b-115">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="4b38b-116">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="4b38b-116">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="4b38b-117">读取 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4b38b-117">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="4b38b-118">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="4b38b-118">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="4b38b-119">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="4b38b-119">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="4b38b-120">创建新的 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b38b-120">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="4b38b-121">删除 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="4b38b-121">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="4b38b-122">无</span><span class="sxs-lookup"><span data-stu-id="4b38b-122">None</span></span>|<span data-ttu-id="4b38b-123">删除 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="4b38b-123">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="4b38b-124">更新 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="4b38b-124">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="4b38b-125">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="4b38b-125">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="4b38b-126">更新 [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4b38b-126">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="4b38b-127">属性</span><span class="sxs-lookup"><span data-stu-id="4b38b-127">Properties</span></span>
|<span data-ttu-id="4b38b-128">属性</span><span class="sxs-lookup"><span data-stu-id="4b38b-128">Property</span></span>|<span data-ttu-id="4b38b-129">类型</span><span class="sxs-lookup"><span data-stu-id="4b38b-129">Type</span></span>|<span data-ttu-id="4b38b-130">说明</span><span class="sxs-lookup"><span data-stu-id="4b38b-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b38b-131">id</span><span class="sxs-lookup"><span data-stu-id="4b38b-131">id</span></span>|<span data-ttu-id="4b38b-132">String</span><span class="sxs-lookup"><span data-stu-id="4b38b-132">String</span></span>|<span data-ttu-id="4b38b-133">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="4b38b-133">Unique identifier of the entity</span></span>|
|<span data-ttu-id="4b38b-134">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="4b38b-134">managedDeviceId</span></span>|<span data-ttu-id="4b38b-135">String</span><span class="sxs-lookup"><span data-stu-id="4b38b-135">String</span></span>|<span data-ttu-id="4b38b-136">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="4b38b-136">Intune device id</span></span>|
|<span data-ttu-id="4b38b-137">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="4b38b-137">deviceDisplayName</span></span>|<span data-ttu-id="4b38b-138">String</span><span class="sxs-lookup"><span data-stu-id="4b38b-138">String</span></span>|<span data-ttu-id="4b38b-139">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="4b38b-139">Display name of the device</span></span>|
|<span data-ttu-id="4b38b-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4b38b-140">userPrincipalName</span></span>|<span data-ttu-id="4b38b-141">String</span><span class="sxs-lookup"><span data-stu-id="4b38b-141">String</span></span>|<span data-ttu-id="4b38b-142">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="4b38b-142">User Principal Name</span></span>|
|<span data-ttu-id="4b38b-143">state</span><span class="sxs-lookup"><span data-stu-id="4b38b-143">state</span></span>|[<span data-ttu-id="4b38b-144">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="4b38b-144">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="4b38b-145">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="4b38b-145">Security baseline compliance state.</span></span> <span data-ttu-id="4b38b-146">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="4b38b-146">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="4b38b-147">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b38b-147">lastReportedDateTime</span></span>|<span data-ttu-id="4b38b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b38b-148">DateTimeOffset</span></span>|<span data-ttu-id="4b38b-149">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="4b38b-149">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b38b-150">关系</span><span class="sxs-lookup"><span data-stu-id="4b38b-150">Relationships</span></span>
<span data-ttu-id="4b38b-151">无</span><span class="sxs-lookup"><span data-stu-id="4b38b-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4b38b-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4b38b-152">JSON Representation</span></span>
<span data-ttu-id="4b38b-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b38b-153">Here is a JSON representation of the resource.</span></span>
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




