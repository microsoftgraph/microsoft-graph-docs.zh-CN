---
title: deviceComplianceSettingState 资源类型
description: 给定设备的设备符合性设置状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 9ad64ca5d89700fc5cb90ec7b548a396a9648035
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031722"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="1b6e3-103">deviceComplianceSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="1b6e3-103">deviceComplianceSettingState resource type</span></span>

> <span data-ttu-id="1b6e3-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b6e3-105">给定设备的设备符合性设置状态。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-105">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="1b6e3-106">方法</span><span class="sxs-lookup"><span data-stu-id="1b6e3-106">Methods</span></span>
|<span data-ttu-id="1b6e3-107">方法</span><span class="sxs-lookup"><span data-stu-id="1b6e3-107">Method</span></span>|<span data-ttu-id="1b6e3-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="1b6e3-108">Return Type</span></span>|<span data-ttu-id="1b6e3-109">说明</span><span class="sxs-lookup"><span data-stu-id="1b6e3-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1b6e3-110">列出 deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="1b6e3-110">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="1b6e3-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1b6e3-111">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="1b6e3-112">列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-112">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="1b6e3-113">获取 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1b6e3-113">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="1b6e3-114">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1b6e3-114">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="1b6e3-115">读取 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-115">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="1b6e3-116">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1b6e3-116">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="1b6e3-117">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1b6e3-117">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="1b6e3-118">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-118">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="1b6e3-119">删除 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1b6e3-119">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="1b6e3-120">无</span><span class="sxs-lookup"><span data-stu-id="1b6e3-120">None</span></span>|<span data-ttu-id="1b6e3-121">删除 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-121">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="1b6e3-122">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1b6e3-122">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="1b6e3-123">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="1b6e3-123">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="1b6e3-124">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-124">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1b6e3-125">属性</span><span class="sxs-lookup"><span data-stu-id="1b6e3-125">Properties</span></span>
|<span data-ttu-id="1b6e3-126">属性</span><span class="sxs-lookup"><span data-stu-id="1b6e3-126">Property</span></span>|<span data-ttu-id="1b6e3-127">类型</span><span class="sxs-lookup"><span data-stu-id="1b6e3-127">Type</span></span>|<span data-ttu-id="1b6e3-128">说明</span><span class="sxs-lookup"><span data-stu-id="1b6e3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b6e3-129">id</span><span class="sxs-lookup"><span data-stu-id="1b6e3-129">id</span></span>|<span data-ttu-id="1b6e3-130">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-130">String</span></span>|<span data-ttu-id="1b6e3-131">实体的键</span><span class="sxs-lookup"><span data-stu-id="1b6e3-131">Key of the entity</span></span>|
|<span data-ttu-id="1b6e3-132">setting</span><span class="sxs-lookup"><span data-stu-id="1b6e3-132">setting</span></span>|<span data-ttu-id="1b6e3-133">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-133">String</span></span>|<span data-ttu-id="1b6e3-134">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-134">The setting class name and property name.</span></span>|
|<span data-ttu-id="1b6e3-135">settingName</span><span class="sxs-lookup"><span data-stu-id="1b6e3-135">settingName</span></span>|<span data-ttu-id="1b6e3-136">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-136">String</span></span>|<span data-ttu-id="1b6e3-137">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="1b6e3-137">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="1b6e3-138">deviceId</span><span class="sxs-lookup"><span data-stu-id="1b6e3-138">deviceId</span></span>|<span data-ttu-id="1b6e3-139">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-139">String</span></span>|<span data-ttu-id="1b6e3-140">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="1b6e3-140">The Device Id that is being reported</span></span>|
|<span data-ttu-id="1b6e3-141">deviceName</span><span class="sxs-lookup"><span data-stu-id="1b6e3-141">deviceName</span></span>|<span data-ttu-id="1b6e3-142">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-142">String</span></span>|<span data-ttu-id="1b6e3-143">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="1b6e3-143">The Device Name that is being reported</span></span>|
|<span data-ttu-id="1b6e3-144">userId</span><span class="sxs-lookup"><span data-stu-id="1b6e3-144">userId</span></span>|<span data-ttu-id="1b6e3-145">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-145">String</span></span>|<span data-ttu-id="1b6e3-146">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="1b6e3-146">The user Id that is being reported</span></span>|
|<span data-ttu-id="1b6e3-147">userEmail</span><span class="sxs-lookup"><span data-stu-id="1b6e3-147">userEmail</span></span>|<span data-ttu-id="1b6e3-148">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-148">String</span></span>|<span data-ttu-id="1b6e3-149">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="1b6e3-149">The User email address that is being reported</span></span>|
|<span data-ttu-id="1b6e3-150">userName</span><span class="sxs-lookup"><span data-stu-id="1b6e3-150">userName</span></span>|<span data-ttu-id="1b6e3-151">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-151">String</span></span>|<span data-ttu-id="1b6e3-152">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="1b6e3-152">The User Name that is being reported</span></span>|
|<span data-ttu-id="1b6e3-153">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1b6e3-153">userPrincipalName</span></span>|<span data-ttu-id="1b6e3-154">字符串</span><span class="sxs-lookup"><span data-stu-id="1b6e3-154">String</span></span>|<span data-ttu-id="1b6e3-155">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="1b6e3-155">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="1b6e3-156">deviceModel</span><span class="sxs-lookup"><span data-stu-id="1b6e3-156">deviceModel</span></span>|<span data-ttu-id="1b6e3-157">String</span><span class="sxs-lookup"><span data-stu-id="1b6e3-157">String</span></span>|<span data-ttu-id="1b6e3-158">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="1b6e3-158">The device model that is being reported</span></span>|
|<span data-ttu-id="1b6e3-159">state</span><span class="sxs-lookup"><span data-stu-id="1b6e3-159">state</span></span>|[<span data-ttu-id="1b6e3-160">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="1b6e3-160">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="1b6e3-161">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-161">The compliance state of the setting.</span></span> <span data-ttu-id="1b6e3-162">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-162">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="1b6e3-163">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1b6e3-163">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="1b6e3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1b6e3-164">DateTimeOffset</span></span>|<span data-ttu-id="1b6e3-165">设备合规性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="1b6e3-165">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="1b6e3-166">关系</span><span class="sxs-lookup"><span data-stu-id="1b6e3-166">Relationships</span></span>
<span data-ttu-id="1b6e3-167">无</span><span class="sxs-lookup"><span data-stu-id="1b6e3-167">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1b6e3-168">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1b6e3-168">JSON Representation</span></span>
<span data-ttu-id="1b6e3-169">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1b6e3-169">Here is a JSON representation of the resource.</span></span>
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



