---
title: securityBaselineDeviceState 资源类型
description: 设备安全基准的安全基准合规性状态摘要。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 412b2f715053abf8ec6ff54cb8be3e75f586209a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419717"
---
# <a name="securitybaselinedevicestate-resource-type"></a><span data-ttu-id="71b35-103">securityBaselineDeviceState 资源类型</span><span class="sxs-lookup"><span data-stu-id="71b35-103">securityBaselineDeviceState resource type</span></span>

<span data-ttu-id="71b35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71b35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="71b35-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="71b35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71b35-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71b35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71b35-107">设备安全基准的安全基准合规性状态摘要。</span><span class="sxs-lookup"><span data-stu-id="71b35-107">The security baseline compliance state summary of the security baseline for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="71b35-108">方法</span><span class="sxs-lookup"><span data-stu-id="71b35-108">Methods</span></span>
|<span data-ttu-id="71b35-109">方法</span><span class="sxs-lookup"><span data-stu-id="71b35-109">Method</span></span>|<span data-ttu-id="71b35-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="71b35-110">Return Type</span></span>|<span data-ttu-id="71b35-111">说明</span><span class="sxs-lookup"><span data-stu-id="71b35-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71b35-112">列出 securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="71b35-112">List securityBaselineDeviceStates</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-list.md)|<span data-ttu-id="71b35-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)集合</span><span class="sxs-lookup"><span data-stu-id="71b35-113">[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) collection</span></span>|<span data-ttu-id="71b35-114">列出[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71b35-114">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>|
|[<span data-ttu-id="71b35-115">获取 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="71b35-115">Get securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-get.md)|[<span data-ttu-id="71b35-116">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="71b35-116">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="71b35-117">读取[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="71b35-117">Read properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="71b35-118">创建 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="71b35-118">Create securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-create.md)|[<span data-ttu-id="71b35-119">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="71b35-119">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="71b35-120">创建新的[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="71b35-120">Create a new [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|
|[<span data-ttu-id="71b35-121">删除 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="71b35-121">Delete securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-delete.md)|<span data-ttu-id="71b35-122">无</span><span class="sxs-lookup"><span data-stu-id="71b35-122">None</span></span>|<span data-ttu-id="71b35-123">删除[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)。</span><span class="sxs-lookup"><span data-stu-id="71b35-123">Deletes a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md).</span></span>|
|[<span data-ttu-id="71b35-124">更新 securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="71b35-124">Update securityBaselineDeviceState</span></span>](../api/intune-deviceintent-securitybaselinedevicestate-update.md)|[<span data-ttu-id="71b35-125">securityBaselineDeviceState</span><span class="sxs-lookup"><span data-stu-id="71b35-125">securityBaselineDeviceState</span></span>](../resources/intune-deviceintent-securitybaselinedevicestate.md)|<span data-ttu-id="71b35-126">更新[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71b35-126">Update the properties of a [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="71b35-127">属性</span><span class="sxs-lookup"><span data-stu-id="71b35-127">Properties</span></span>
|<span data-ttu-id="71b35-128">属性</span><span class="sxs-lookup"><span data-stu-id="71b35-128">Property</span></span>|<span data-ttu-id="71b35-129">类型</span><span class="sxs-lookup"><span data-stu-id="71b35-129">Type</span></span>|<span data-ttu-id="71b35-130">说明</span><span class="sxs-lookup"><span data-stu-id="71b35-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71b35-131">id</span><span class="sxs-lookup"><span data-stu-id="71b35-131">id</span></span>|<span data-ttu-id="71b35-132">String</span><span class="sxs-lookup"><span data-stu-id="71b35-132">String</span></span>|<span data-ttu-id="71b35-133">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="71b35-133">Unique identifier of the entity</span></span>|
|<span data-ttu-id="71b35-134">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="71b35-134">managedDeviceId</span></span>|<span data-ttu-id="71b35-135">String</span><span class="sxs-lookup"><span data-stu-id="71b35-135">String</span></span>|<span data-ttu-id="71b35-136">Intune 设备 id</span><span class="sxs-lookup"><span data-stu-id="71b35-136">Intune device id</span></span>|
|<span data-ttu-id="71b35-137">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="71b35-137">deviceDisplayName</span></span>|<span data-ttu-id="71b35-138">String</span><span class="sxs-lookup"><span data-stu-id="71b35-138">String</span></span>|<span data-ttu-id="71b35-139">设备的显示名称</span><span class="sxs-lookup"><span data-stu-id="71b35-139">Display name of the device</span></span>|
|<span data-ttu-id="71b35-140">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="71b35-140">userPrincipalName</span></span>|<span data-ttu-id="71b35-141">String</span><span class="sxs-lookup"><span data-stu-id="71b35-141">String</span></span>|<span data-ttu-id="71b35-142">用户主体名称</span><span class="sxs-lookup"><span data-stu-id="71b35-142">User Principal Name</span></span>|
|<span data-ttu-id="71b35-143">state</span><span class="sxs-lookup"><span data-stu-id="71b35-143">state</span></span>|[<span data-ttu-id="71b35-144">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="71b35-144">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="71b35-145">安全基准合规性状态。</span><span class="sxs-lookup"><span data-stu-id="71b35-145">Security baseline compliance state.</span></span> <span data-ttu-id="71b35-146">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="71b35-146">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="71b35-147">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="71b35-147">lastReportedDateTime</span></span>|<span data-ttu-id="71b35-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71b35-148">DateTimeOffset</span></span>|<span data-ttu-id="71b35-149">策略报告的上次修改日期时间</span><span class="sxs-lookup"><span data-stu-id="71b35-149">Last modified date time of the policy report</span></span>|

## <a name="relationships"></a><span data-ttu-id="71b35-150">关系</span><span class="sxs-lookup"><span data-stu-id="71b35-150">Relationships</span></span>
<span data-ttu-id="71b35-151">无</span><span class="sxs-lookup"><span data-stu-id="71b35-151">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="71b35-152">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="71b35-152">JSON Representation</span></span>
<span data-ttu-id="71b35-153">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71b35-153">Here is a JSON representation of the resource.</span></span>
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



