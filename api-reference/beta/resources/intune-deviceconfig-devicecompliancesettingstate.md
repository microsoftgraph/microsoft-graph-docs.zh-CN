---
title: deviceComplianceSettingState 资源类型
description: 给定设备的设备符合性设置状态。
ms.openlocfilehash: 4fe524f5a737b5e80201f961a48870cb6e0f0928
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046526"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="a55f1-103">deviceComplianceSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="a55f1-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="a55f1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a55f1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a55f1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a55f1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a55f1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a55f1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a55f1-107">给定设备的设备符合性设置状态。</span><span class="sxs-lookup"><span data-stu-id="a55f1-107">Device compliance setting State for a given device.</span></span>
## <a name="methods"></a><span data-ttu-id="a55f1-108">方法</span><span class="sxs-lookup"><span data-stu-id="a55f1-108">Methods</span></span>
|<span data-ttu-id="a55f1-109">方法</span><span class="sxs-lookup"><span data-stu-id="a55f1-109">Method</span></span>|<span data-ttu-id="a55f1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a55f1-110">Return Type</span></span>|<span data-ttu-id="a55f1-111">说明</span><span class="sxs-lookup"><span data-stu-id="a55f1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a55f1-112">列出 deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="a55f1-112">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="a55f1-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a55f1-113">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="a55f1-114">列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a55f1-114">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="a55f1-115">获取 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a55f1-115">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="a55f1-116">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a55f1-116">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a55f1-117">读取 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a55f1-117">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="a55f1-118">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a55f1-118">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="a55f1-119">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a55f1-119">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a55f1-120">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a55f1-120">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="a55f1-121">删除 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a55f1-121">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="a55f1-122">无</span><span class="sxs-lookup"><span data-stu-id="a55f1-122">None</span></span>|<span data-ttu-id="a55f1-123">删除 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="a55f1-123">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="a55f1-124">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a55f1-124">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="a55f1-125">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a55f1-125">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a55f1-126">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a55f1-126">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a55f1-127">属性</span><span class="sxs-lookup"><span data-stu-id="a55f1-127">Properties</span></span>
|<span data-ttu-id="a55f1-128">属性</span><span class="sxs-lookup"><span data-stu-id="a55f1-128">Property</span></span>|<span data-ttu-id="a55f1-129">类型</span><span class="sxs-lookup"><span data-stu-id="a55f1-129">Type</span></span>|<span data-ttu-id="a55f1-130">说明</span><span class="sxs-lookup"><span data-stu-id="a55f1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a55f1-131">id</span><span class="sxs-lookup"><span data-stu-id="a55f1-131">id</span></span>|<span data-ttu-id="a55f1-132">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-132">String</span></span>|<span data-ttu-id="a55f1-133">实体的键</span><span class="sxs-lookup"><span data-stu-id="a55f1-133">Key of the entity</span></span>|
|<span data-ttu-id="a55f1-134">platformType</span><span class="sxs-lookup"><span data-stu-id="a55f1-134">platformType</span></span>|[<span data-ttu-id="a55f1-135">deviceType</span><span class="sxs-lookup"><span data-stu-id="a55f1-135">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="a55f1-136">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="a55f1-136">Device platform type.</span></span> <span data-ttu-id="a55f1-137">可能的值为： `desktop`， `windowsRT`， `winMO6`， `nokia`， `windowsPhone`， `mac`， `winCE`， `winEmbedded`， `iPhone`， `iPad`， `iPod`， `android`， `iSocConsumer`， `unix`， `macMDM`， `holoLens`， `surfaceHub`， `androidForWork`， `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a55f1-137">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="a55f1-138">setting</span><span class="sxs-lookup"><span data-stu-id="a55f1-138">setting</span></span>|<span data-ttu-id="a55f1-139">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-139">String</span></span>|<span data-ttu-id="a55f1-140">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="a55f1-140">The setting class name and property name.</span></span>|
|<span data-ttu-id="a55f1-141">settingName</span><span class="sxs-lookup"><span data-stu-id="a55f1-141">settingName</span></span>|<span data-ttu-id="a55f1-142">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-142">String</span></span>|<span data-ttu-id="a55f1-143">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="a55f1-143">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="a55f1-144">deviceId</span><span class="sxs-lookup"><span data-stu-id="a55f1-144">deviceId</span></span>|<span data-ttu-id="a55f1-145">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-145">String</span></span>|<span data-ttu-id="a55f1-146">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="a55f1-146">The Device Id that is being reported</span></span>|
|<span data-ttu-id="a55f1-147">deviceName</span><span class="sxs-lookup"><span data-stu-id="a55f1-147">deviceName</span></span>|<span data-ttu-id="a55f1-148">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-148">String</span></span>|<span data-ttu-id="a55f1-149">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="a55f1-149">The Device Name that is being reported</span></span>|
|<span data-ttu-id="a55f1-150">userId</span><span class="sxs-lookup"><span data-stu-id="a55f1-150">userId</span></span>|<span data-ttu-id="a55f1-151">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-151">String</span></span>|<span data-ttu-id="a55f1-152">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="a55f1-152">The user Id that is being reported</span></span>|
|<span data-ttu-id="a55f1-153">userEmail</span><span class="sxs-lookup"><span data-stu-id="a55f1-153">userEmail</span></span>|<span data-ttu-id="a55f1-154">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-154">String</span></span>|<span data-ttu-id="a55f1-155">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="a55f1-155">The User email address that is being reported</span></span>|
|<span data-ttu-id="a55f1-156">userName</span><span class="sxs-lookup"><span data-stu-id="a55f1-156">userName</span></span>|<span data-ttu-id="a55f1-157">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-157">String</span></span>|<span data-ttu-id="a55f1-158">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="a55f1-158">The User Name that is being reported</span></span>|
|<span data-ttu-id="a55f1-159">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a55f1-159">userPrincipalName</span></span>|<span data-ttu-id="a55f1-160">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-160">String</span></span>|<span data-ttu-id="a55f1-161">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a55f1-161">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="a55f1-162">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a55f1-162">deviceModel</span></span>|<span data-ttu-id="a55f1-163">String</span><span class="sxs-lookup"><span data-stu-id="a55f1-163">String</span></span>|<span data-ttu-id="a55f1-164">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="a55f1-164">The device model that is being reported</span></span>|
|<span data-ttu-id="a55f1-165">state</span><span class="sxs-lookup"><span data-stu-id="a55f1-165">state</span></span>|[<span data-ttu-id="a55f1-166">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a55f1-166">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a55f1-167">设置合规性状态。</span><span class="sxs-lookup"><span data-stu-id="a55f1-167">The compliance state of the setting.</span></span> <span data-ttu-id="a55f1-168">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="a55f1-168">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a55f1-169">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a55f1-169">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a55f1-170">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a55f1-170">DateTimeOffset</span></span>|<span data-ttu-id="a55f1-171">设备合规性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="a55f1-171">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="a55f1-172">关系</span><span class="sxs-lookup"><span data-stu-id="a55f1-172">Relationships</span></span>
<span data-ttu-id="a55f1-173">无</span><span class="sxs-lookup"><span data-stu-id="a55f1-173">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a55f1-174">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a55f1-174">JSON Representation</span></span>
<span data-ttu-id="a55f1-175">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a55f1-175">Here is a JSON representation of the resource.</span></span>
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





