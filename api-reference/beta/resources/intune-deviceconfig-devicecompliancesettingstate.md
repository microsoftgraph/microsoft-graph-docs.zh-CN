---
title: deviceComplianceSettingState 资源类型
description: 给定设备的设备符合性设置状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 30d631857fe33a5eda94698213d2773c5d57a6fc
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44788092"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="779f9-103">deviceComplianceSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="779f9-103">deviceComplianceSettingState resource type</span></span>

<span data-ttu-id="779f9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="779f9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="779f9-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="779f9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="779f9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="779f9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="779f9-107">给定设备的设备符合性设置状态。</span><span class="sxs-lookup"><span data-stu-id="779f9-107">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="779f9-108">Methods</span><span class="sxs-lookup"><span data-stu-id="779f9-108">Methods</span></span>
|<span data-ttu-id="779f9-109">方法</span><span class="sxs-lookup"><span data-stu-id="779f9-109">Method</span></span>|<span data-ttu-id="779f9-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="779f9-110">Return Type</span></span>|<span data-ttu-id="779f9-111">说明</span><span class="sxs-lookup"><span data-stu-id="779f9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="779f9-112">列出 deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="779f9-112">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="779f9-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="779f9-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="779f9-114">列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="779f9-114">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="779f9-115">获取 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="779f9-115">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="779f9-116">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="779f9-116">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="779f9-117">读取 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="779f9-117">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="779f9-118">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="779f9-118">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="779f9-119">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="779f9-119">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="779f9-120">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="779f9-120">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="779f9-121">删除 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="779f9-121">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="779f9-122">无</span><span class="sxs-lookup"><span data-stu-id="779f9-122">None</span></span>|<span data-ttu-id="779f9-123">删除 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="779f9-123">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="779f9-124">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="779f9-124">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="779f9-125">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="779f9-125">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="779f9-126">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="779f9-126">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="779f9-127">属性</span><span class="sxs-lookup"><span data-stu-id="779f9-127">Properties</span></span>
|<span data-ttu-id="779f9-128">属性</span><span class="sxs-lookup"><span data-stu-id="779f9-128">Property</span></span>|<span data-ttu-id="779f9-129">类型</span><span class="sxs-lookup"><span data-stu-id="779f9-129">Type</span></span>|<span data-ttu-id="779f9-130">说明</span><span class="sxs-lookup"><span data-stu-id="779f9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="779f9-131">id</span><span class="sxs-lookup"><span data-stu-id="779f9-131">id</span></span>|<span data-ttu-id="779f9-132">String</span><span class="sxs-lookup"><span data-stu-id="779f9-132">String</span></span>|<span data-ttu-id="779f9-133">实体的键</span><span class="sxs-lookup"><span data-stu-id="779f9-133">Key of the entity</span></span>|
|<span data-ttu-id="779f9-134">platformType</span><span class="sxs-lookup"><span data-stu-id="779f9-134">platformType</span></span>|[<span data-ttu-id="779f9-135">deviceType</span><span class="sxs-lookup"><span data-stu-id="779f9-135">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="779f9-136">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="779f9-136">Device platform type.</span></span> <span data-ttu-id="779f9-137">可能的值为：、、、、、、、、、、、、、、、、、、、、、、、 `desktop` `windowsRT` `winMO6` `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer` `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise` `windows10x` `androidnGMS` `blackberry` `palm` `unknown` 。</span><span class="sxs-lookup"><span data-stu-id="779f9-137">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `windows10x`, `androidnGMS`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="779f9-138">setting</span><span class="sxs-lookup"><span data-stu-id="779f9-138">setting</span></span>|<span data-ttu-id="779f9-139">String</span><span class="sxs-lookup"><span data-stu-id="779f9-139">String</span></span>|<span data-ttu-id="779f9-140">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="779f9-140">The setting class name and property name.</span></span>|
|<span data-ttu-id="779f9-141">settingName</span><span class="sxs-lookup"><span data-stu-id="779f9-141">settingName</span></span>|<span data-ttu-id="779f9-142">String</span><span class="sxs-lookup"><span data-stu-id="779f9-142">String</span></span>|<span data-ttu-id="779f9-143">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="779f9-143">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="779f9-144">deviceId</span><span class="sxs-lookup"><span data-stu-id="779f9-144">deviceId</span></span>|<span data-ttu-id="779f9-145">String</span><span class="sxs-lookup"><span data-stu-id="779f9-145">String</span></span>|<span data-ttu-id="779f9-146">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="779f9-146">The Device Id that is being reported</span></span>|
|<span data-ttu-id="779f9-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="779f9-147">deviceName</span></span>|<span data-ttu-id="779f9-148">String</span><span class="sxs-lookup"><span data-stu-id="779f9-148">String</span></span>|<span data-ttu-id="779f9-149">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="779f9-149">The Device Name that is being reported</span></span>|
|<span data-ttu-id="779f9-150">userId</span><span class="sxs-lookup"><span data-stu-id="779f9-150">userId</span></span>|<span data-ttu-id="779f9-151">String</span><span class="sxs-lookup"><span data-stu-id="779f9-151">String</span></span>|<span data-ttu-id="779f9-152">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="779f9-152">The user Id that is being reported</span></span>|
|<span data-ttu-id="779f9-153">userEmail</span><span class="sxs-lookup"><span data-stu-id="779f9-153">userEmail</span></span>|<span data-ttu-id="779f9-154">String</span><span class="sxs-lookup"><span data-stu-id="779f9-154">String</span></span>|<span data-ttu-id="779f9-155">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="779f9-155">The User email address that is being reported</span></span>|
|<span data-ttu-id="779f9-156">userName</span><span class="sxs-lookup"><span data-stu-id="779f9-156">userName</span></span>|<span data-ttu-id="779f9-157">String</span><span class="sxs-lookup"><span data-stu-id="779f9-157">String</span></span>|<span data-ttu-id="779f9-158">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="779f9-158">The User Name that is being reported</span></span>|
|<span data-ttu-id="779f9-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="779f9-159">userPrincipalName</span></span>|<span data-ttu-id="779f9-160">字符串</span><span class="sxs-lookup"><span data-stu-id="779f9-160">String</span></span>|<span data-ttu-id="779f9-161">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="779f9-161">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="779f9-162">deviceModel</span><span class="sxs-lookup"><span data-stu-id="779f9-162">deviceModel</span></span>|<span data-ttu-id="779f9-163">String</span><span class="sxs-lookup"><span data-stu-id="779f9-163">String</span></span>|<span data-ttu-id="779f9-164">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="779f9-164">The device model that is being reported</span></span>|
|<span data-ttu-id="779f9-165">state</span><span class="sxs-lookup"><span data-stu-id="779f9-165">state</span></span>|[<span data-ttu-id="779f9-166">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="779f9-166">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="779f9-167">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="779f9-167">The compliance state of the setting.</span></span> <span data-ttu-id="779f9-168">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="779f9-168">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="779f9-169">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="779f9-169">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="779f9-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="779f9-170">DateTimeOffset</span></span>|<span data-ttu-id="779f9-171">设备合规性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="779f9-171">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="779f9-172">关系</span><span class="sxs-lookup"><span data-stu-id="779f9-172">Relationships</span></span>
<span data-ttu-id="779f9-173">无</span><span class="sxs-lookup"><span data-stu-id="779f9-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="779f9-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="779f9-174">JSON Representation</span></span>
<span data-ttu-id="779f9-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="779f9-175">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
  "id": "String (identifier)",
  "platformType": "String",
  "setting": "String",
  "settingName": "String",
  "deviceId": "String",
  "deviceName": "String",
  "userId": "String",
  "userEmail": "String",
  "userName": "String",
  "userPrincipalName": "String",
  "deviceModel": "String",
  "state": "String",
  "complianceGracePeriodExpirationDateTime": "String (timestamp)"
}
```



