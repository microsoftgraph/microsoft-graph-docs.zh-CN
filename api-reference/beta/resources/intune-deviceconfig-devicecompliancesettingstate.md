---
title: deviceComplianceSettingState 资源类型
description: 给定设备的设备符合性设置状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 96fa7bf9b93e64051b0f6271d04c1e08897c748e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333112"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="03739-103">deviceComplianceSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="03739-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="03739-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03739-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03739-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03739-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03739-106">给定设备的设备符合性设置状态。</span><span class="sxs-lookup"><span data-stu-id="03739-106">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="03739-107">方法</span><span class="sxs-lookup"><span data-stu-id="03739-107">Methods</span></span>
|<span data-ttu-id="03739-108">方法</span><span class="sxs-lookup"><span data-stu-id="03739-108">Method</span></span>|<span data-ttu-id="03739-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="03739-109">Return Type</span></span>|<span data-ttu-id="03739-110">说明</span><span class="sxs-lookup"><span data-stu-id="03739-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03739-111">列出 deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="03739-111">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="03739-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="03739-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="03739-113">列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="03739-113">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="03739-114">获取 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="03739-114">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="03739-115">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="03739-115">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="03739-116">读取 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="03739-116">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="03739-117">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="03739-117">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="03739-118">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="03739-118">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="03739-119">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03739-119">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="03739-120">删除 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="03739-120">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="03739-121">无</span><span class="sxs-lookup"><span data-stu-id="03739-121">None</span></span>|<span data-ttu-id="03739-122">删除 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="03739-122">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="03739-123">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="03739-123">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="03739-124">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="03739-124">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="03739-125">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03739-125">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="03739-126">属性</span><span class="sxs-lookup"><span data-stu-id="03739-126">Properties</span></span>
|<span data-ttu-id="03739-127">属性</span><span class="sxs-lookup"><span data-stu-id="03739-127">Property</span></span>|<span data-ttu-id="03739-128">类型</span><span class="sxs-lookup"><span data-stu-id="03739-128">Type</span></span>|<span data-ttu-id="03739-129">说明</span><span class="sxs-lookup"><span data-stu-id="03739-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03739-130">id</span><span class="sxs-lookup"><span data-stu-id="03739-130">id</span></span>|<span data-ttu-id="03739-131">String</span><span class="sxs-lookup"><span data-stu-id="03739-131">String</span></span>|<span data-ttu-id="03739-132">实体的键</span><span class="sxs-lookup"><span data-stu-id="03739-132">Key of the entity</span></span>|
|<span data-ttu-id="03739-133">platformType</span><span class="sxs-lookup"><span data-stu-id="03739-133">platformType</span></span>|[<span data-ttu-id="03739-134">deviceType</span><span class="sxs-lookup"><span data-stu-id="03739-134">deviceType</span></span>](../resources/intune-shared-devicetype.md)|<span data-ttu-id="03739-135">设备平台类型。</span><span class="sxs-lookup"><span data-stu-id="03739-135">Device platform type.</span></span> <span data-ttu-id="03739-136">可能的值为`desktop`: `windowsRT`、 `winMO6`、 `nokia` `windowsPhone` `mac` `winCE` `winEmbedded` `iPhone` `iPad` `iPod` `android` `iSocConsumer`、、、、、、、、、、、、、、、、 `unix` `macMDM` `holoLens` `surfaceHub` `androidForWork` `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="03739-136">Possible values are: `desktop`, `windowsRT`, `winMO6`, `nokia`, `windowsPhone`, `mac`, `winCE`, `winEmbedded`, `iPhone`, `iPad`, `iPod`, `android`, `iSocConsumer`, `unix`, `macMDM`, `holoLens`, `surfaceHub`, `androidForWork`, `androidEnterprise`, `blackberry`, `palm`, `unknown`.</span></span>|
|<span data-ttu-id="03739-137">setting</span><span class="sxs-lookup"><span data-stu-id="03739-137">setting</span></span>|<span data-ttu-id="03739-138">String</span><span class="sxs-lookup"><span data-stu-id="03739-138">String</span></span>|<span data-ttu-id="03739-139">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="03739-139">The setting class name and property name.</span></span>|
|<span data-ttu-id="03739-140">settingName</span><span class="sxs-lookup"><span data-stu-id="03739-140">settingName</span></span>|<span data-ttu-id="03739-141">String</span><span class="sxs-lookup"><span data-stu-id="03739-141">String</span></span>|<span data-ttu-id="03739-142">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="03739-142">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="03739-143">deviceId</span><span class="sxs-lookup"><span data-stu-id="03739-143">deviceId</span></span>|<span data-ttu-id="03739-144">String</span><span class="sxs-lookup"><span data-stu-id="03739-144">String</span></span>|<span data-ttu-id="03739-145">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="03739-145">The Device Id that is being reported</span></span>|
|<span data-ttu-id="03739-146">deviceName</span><span class="sxs-lookup"><span data-stu-id="03739-146">deviceName</span></span>|<span data-ttu-id="03739-147">String</span><span class="sxs-lookup"><span data-stu-id="03739-147">String</span></span>|<span data-ttu-id="03739-148">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="03739-148">The Device Name that is being reported</span></span>|
|<span data-ttu-id="03739-149">userId</span><span class="sxs-lookup"><span data-stu-id="03739-149">userId</span></span>|<span data-ttu-id="03739-150">String</span><span class="sxs-lookup"><span data-stu-id="03739-150">String</span></span>|<span data-ttu-id="03739-151">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="03739-151">The user Id that is being reported</span></span>|
|<span data-ttu-id="03739-152">userEmail</span><span class="sxs-lookup"><span data-stu-id="03739-152">userEmail</span></span>|<span data-ttu-id="03739-153">String</span><span class="sxs-lookup"><span data-stu-id="03739-153">String</span></span>|<span data-ttu-id="03739-154">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="03739-154">The User email address that is being reported</span></span>|
|<span data-ttu-id="03739-155">userName</span><span class="sxs-lookup"><span data-stu-id="03739-155">userName</span></span>|<span data-ttu-id="03739-156">String</span><span class="sxs-lookup"><span data-stu-id="03739-156">String</span></span>|<span data-ttu-id="03739-157">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="03739-157">The User Name that is being reported</span></span>|
|<span data-ttu-id="03739-158">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="03739-158">userPrincipalName</span></span>|<span data-ttu-id="03739-159">字符串</span><span class="sxs-lookup"><span data-stu-id="03739-159">String</span></span>|<span data-ttu-id="03739-160">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="03739-160">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="03739-161">deviceModel</span><span class="sxs-lookup"><span data-stu-id="03739-161">deviceModel</span></span>|<span data-ttu-id="03739-162">String</span><span class="sxs-lookup"><span data-stu-id="03739-162">String</span></span>|<span data-ttu-id="03739-163">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="03739-163">The device model that is being reported</span></span>|
|<span data-ttu-id="03739-164">state</span><span class="sxs-lookup"><span data-stu-id="03739-164">state</span></span>|[<span data-ttu-id="03739-165">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="03739-165">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="03739-166">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="03739-166">The compliance state of the setting.</span></span> <span data-ttu-id="03739-167">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="03739-167">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="03739-168">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="03739-168">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="03739-169">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="03739-169">DateTimeOffset</span></span>|<span data-ttu-id="03739-170">设备合规性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="03739-170">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="03739-171">关系</span><span class="sxs-lookup"><span data-stu-id="03739-171">Relationships</span></span>
<span data-ttu-id="03739-172">无</span><span class="sxs-lookup"><span data-stu-id="03739-172">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="03739-173">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03739-173">JSON Representation</span></span>
<span data-ttu-id="03739-174">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03739-174">Here is a JSON representation of the resource.</span></span>
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



