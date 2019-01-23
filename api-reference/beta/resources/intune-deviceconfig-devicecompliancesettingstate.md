---
title: deviceComplianceSettingState 资源类型
description: 给定设备的设备符合性设置状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d618356d115f437bccccee57f6c259a1cdbd14a8
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403033"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="7bb24-103">deviceComplianceSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="7bb24-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="7bb24-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7bb24-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7bb24-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7bb24-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7bb24-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7bb24-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bb24-107">给定设备的设备符合性设置状态。</span><span class="sxs-lookup"><span data-stu-id="7bb24-107">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="7bb24-108">方法</span><span class="sxs-lookup"><span data-stu-id="7bb24-108">Methods</span></span>
|<span data-ttu-id="7bb24-109">方法</span><span class="sxs-lookup"><span data-stu-id="7bb24-109">Method</span></span>|<span data-ttu-id="7bb24-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="7bb24-110">Return Type</span></span>|<span data-ttu-id="7bb24-111">说明</span><span class="sxs-lookup"><span data-stu-id="7bb24-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="7bb24-112">列出 deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="7bb24-112">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="7bb24-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7bb24-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="7bb24-114">列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7bb24-114">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="7bb24-115">获取 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="7bb24-115">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="7bb24-116">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="7bb24-116">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="7bb24-117">读取 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="7bb24-117">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="7bb24-118">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="7bb24-118">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="7bb24-119">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="7bb24-119">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="7bb24-120">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7bb24-120">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="7bb24-121">删除 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="7bb24-121">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="7bb24-122">无</span><span class="sxs-lookup"><span data-stu-id="7bb24-122">None</span></span>|<span data-ttu-id="7bb24-123">删除 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="7bb24-123">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="7bb24-124">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="7bb24-124">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="7bb24-125">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="7bb24-125">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="7bb24-126">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7bb24-126">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="7bb24-127">属性</span><span class="sxs-lookup"><span data-stu-id="7bb24-127">Properties</span></span>
|<span data-ttu-id="7bb24-128">属性</span><span class="sxs-lookup"><span data-stu-id="7bb24-128">Property</span></span>|<span data-ttu-id="7bb24-129">类型</span><span class="sxs-lookup"><span data-stu-id="7bb24-129">Type</span></span>|<span data-ttu-id="7bb24-130">说明</span><span class="sxs-lookup"><span data-stu-id="7bb24-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bb24-131">id</span><span class="sxs-lookup"><span data-stu-id="7bb24-131">id</span></span>|<span data-ttu-id="7bb24-132">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-132">String</span></span>|<span data-ttu-id="7bb24-133">实体的键</span><span class="sxs-lookup"><span data-stu-id="7bb24-133">Key of the entity</span></span>|
|<span data-ttu-id="7bb24-134">platformType</span><span class="sxs-lookup"><span data-stu-id="7bb24-134">platformType</span></span>|[<span data-ttu-id="7bb24-135">deviceType</span><span class="sxs-lookup"><span data-stu-id="7bb24-135">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="7bb24-136">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="7bb24-136">Device platform type.</span></span> <span data-ttu-id="7bb24-137">可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="7bb24-137">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="7bb24-138">setting</span><span class="sxs-lookup"><span data-stu-id="7bb24-138">setting</span></span>|<span data-ttu-id="7bb24-139">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-139">String</span></span>|<span data-ttu-id="7bb24-140">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="7bb24-140">The setting class name and property name.</span></span>|
|<span data-ttu-id="7bb24-141">settingName</span><span class="sxs-lookup"><span data-stu-id="7bb24-141">settingName</span></span>|<span data-ttu-id="7bb24-142">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-142">String</span></span>|<span data-ttu-id="7bb24-143">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="7bb24-143">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="7bb24-144">deviceId</span><span class="sxs-lookup"><span data-stu-id="7bb24-144">deviceId</span></span>|<span data-ttu-id="7bb24-145">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-145">String</span></span>|<span data-ttu-id="7bb24-146">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="7bb24-146">The Device Id that is being reported</span></span>|
|<span data-ttu-id="7bb24-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="7bb24-147">deviceName</span></span>|<span data-ttu-id="7bb24-148">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-148">String</span></span>|<span data-ttu-id="7bb24-149">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="7bb24-149">The Device Name that is being reported</span></span>|
|<span data-ttu-id="7bb24-150">userId</span><span class="sxs-lookup"><span data-stu-id="7bb24-150">userId</span></span>|<span data-ttu-id="7bb24-151">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-151">String</span></span>|<span data-ttu-id="7bb24-152">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="7bb24-152">The user Id that is being reported</span></span>|
|<span data-ttu-id="7bb24-153">userEmail</span><span class="sxs-lookup"><span data-stu-id="7bb24-153">userEmail</span></span>|<span data-ttu-id="7bb24-154">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-154">String</span></span>|<span data-ttu-id="7bb24-155">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="7bb24-155">The User email address that is being reported</span></span>|
|<span data-ttu-id="7bb24-156">userName</span><span class="sxs-lookup"><span data-stu-id="7bb24-156">userName</span></span>|<span data-ttu-id="7bb24-157">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-157">String</span></span>|<span data-ttu-id="7bb24-158">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="7bb24-158">The User Name that is being reported</span></span>|
|<span data-ttu-id="7bb24-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="7bb24-159">userPrincipalName</span></span>|<span data-ttu-id="7bb24-160">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-160">String</span></span>|<span data-ttu-id="7bb24-161">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="7bb24-161">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="7bb24-162">deviceModel</span><span class="sxs-lookup"><span data-stu-id="7bb24-162">deviceModel</span></span>|<span data-ttu-id="7bb24-163">String</span><span class="sxs-lookup"><span data-stu-id="7bb24-163">String</span></span>|<span data-ttu-id="7bb24-164">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="7bb24-164">The device model that is being reported</span></span>|
|<span data-ttu-id="7bb24-165">state</span><span class="sxs-lookup"><span data-stu-id="7bb24-165">state</span></span>|[<span data-ttu-id="7bb24-166">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="7bb24-166">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="7bb24-167">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="7bb24-167">The compliance state of the setting.</span></span> <span data-ttu-id="7bb24-168">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="7bb24-168">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="7bb24-169">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7bb24-169">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="7bb24-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7bb24-170">DateTimeOffset</span></span>|<span data-ttu-id="7bb24-171">设备合规性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="7bb24-171">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="7bb24-172">关系</span><span class="sxs-lookup"><span data-stu-id="7bb24-172">Relationships</span></span>
<span data-ttu-id="7bb24-173">无</span><span class="sxs-lookup"><span data-stu-id="7bb24-173">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bb24-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7bb24-174">JSON Representation</span></span>
<span data-ttu-id="7bb24-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bb24-175">Here is a JSON representation of the resource.</span></span>
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




