---
title: deviceComplianceSettingState 资源类型
description: 给定设备的设备符合性设置状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 96ac7526d8392a3c34a719c4a28b30e568bdd213
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530806"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="a77b9-103">deviceComplianceSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="a77b9-103">deviceComplianceSettingState resource type</span></span>

<span data-ttu-id="a77b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a77b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a77b9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a77b9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a77b9-106">给定设备的设备符合性设置状态。</span><span class="sxs-lookup"><span data-stu-id="a77b9-106">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="a77b9-107">Methods</span><span class="sxs-lookup"><span data-stu-id="a77b9-107">Methods</span></span>
|<span data-ttu-id="a77b9-108">方法</span><span class="sxs-lookup"><span data-stu-id="a77b9-108">Method</span></span>|<span data-ttu-id="a77b9-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="a77b9-109">Return Type</span></span>|<span data-ttu-id="a77b9-110">说明</span><span class="sxs-lookup"><span data-stu-id="a77b9-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a77b9-111">列出 deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="a77b9-111">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="a77b9-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a77b9-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="a77b9-113">列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a77b9-113">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="a77b9-114">获取 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a77b9-114">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="a77b9-115">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a77b9-115">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a77b9-116">读取 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a77b9-116">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="a77b9-117">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a77b9-117">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="a77b9-118">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a77b9-118">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a77b9-119">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a77b9-119">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="a77b9-120">删除 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a77b9-120">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="a77b9-121">无</span><span class="sxs-lookup"><span data-stu-id="a77b9-121">None</span></span>|<span data-ttu-id="a77b9-122">删除 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="a77b9-122">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="a77b9-123">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a77b9-123">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="a77b9-124">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="a77b9-124">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="a77b9-125">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a77b9-125">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a77b9-126">属性</span><span class="sxs-lookup"><span data-stu-id="a77b9-126">Properties</span></span>
|<span data-ttu-id="a77b9-127">属性</span><span class="sxs-lookup"><span data-stu-id="a77b9-127">Property</span></span>|<span data-ttu-id="a77b9-128">类型</span><span class="sxs-lookup"><span data-stu-id="a77b9-128">Type</span></span>|<span data-ttu-id="a77b9-129">说明</span><span class="sxs-lookup"><span data-stu-id="a77b9-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a77b9-130">id</span><span class="sxs-lookup"><span data-stu-id="a77b9-130">id</span></span>|<span data-ttu-id="a77b9-131">String</span><span class="sxs-lookup"><span data-stu-id="a77b9-131">String</span></span>|<span data-ttu-id="a77b9-132">实体的键</span><span class="sxs-lookup"><span data-stu-id="a77b9-132">Key of the entity</span></span>|
|<span data-ttu-id="a77b9-133">setting</span><span class="sxs-lookup"><span data-stu-id="a77b9-133">setting</span></span>|<span data-ttu-id="a77b9-134">字符串</span><span class="sxs-lookup"><span data-stu-id="a77b9-134">String</span></span>|<span data-ttu-id="a77b9-135">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="a77b9-135">The setting class name and property name.</span></span>|
|<span data-ttu-id="a77b9-136">settingName</span><span class="sxs-lookup"><span data-stu-id="a77b9-136">settingName</span></span>|<span data-ttu-id="a77b9-137">字符串</span><span class="sxs-lookup"><span data-stu-id="a77b9-137">String</span></span>|<span data-ttu-id="a77b9-138">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="a77b9-138">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="a77b9-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="a77b9-139">deviceId</span></span>|<span data-ttu-id="a77b9-140">字符串</span><span class="sxs-lookup"><span data-stu-id="a77b9-140">String</span></span>|<span data-ttu-id="a77b9-141">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="a77b9-141">The Device Id that is being reported</span></span>|
|<span data-ttu-id="a77b9-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="a77b9-142">deviceName</span></span>|<span data-ttu-id="a77b9-143">字符串</span><span class="sxs-lookup"><span data-stu-id="a77b9-143">String</span></span>|<span data-ttu-id="a77b9-144">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="a77b9-144">The Device Name that is being reported</span></span>|
|<span data-ttu-id="a77b9-145">userId</span><span class="sxs-lookup"><span data-stu-id="a77b9-145">userId</span></span>|<span data-ttu-id="a77b9-146">String</span><span class="sxs-lookup"><span data-stu-id="a77b9-146">String</span></span>|<span data-ttu-id="a77b9-147">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="a77b9-147">The user Id that is being reported</span></span>|
|<span data-ttu-id="a77b9-148">userEmail</span><span class="sxs-lookup"><span data-stu-id="a77b9-148">userEmail</span></span>|<span data-ttu-id="a77b9-149">String</span><span class="sxs-lookup"><span data-stu-id="a77b9-149">String</span></span>|<span data-ttu-id="a77b9-150">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="a77b9-150">The User email address that is being reported</span></span>|
|<span data-ttu-id="a77b9-151">userName</span><span class="sxs-lookup"><span data-stu-id="a77b9-151">userName</span></span>|<span data-ttu-id="a77b9-152">字符串</span><span class="sxs-lookup"><span data-stu-id="a77b9-152">String</span></span>|<span data-ttu-id="a77b9-153">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="a77b9-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="a77b9-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a77b9-154">userPrincipalName</span></span>|<span data-ttu-id="a77b9-155">字符串</span><span class="sxs-lookup"><span data-stu-id="a77b9-155">String</span></span>|<span data-ttu-id="a77b9-156">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="a77b9-156">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="a77b9-157">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a77b9-157">deviceModel</span></span>|<span data-ttu-id="a77b9-158">字符串</span><span class="sxs-lookup"><span data-stu-id="a77b9-158">String</span></span>|<span data-ttu-id="a77b9-159">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="a77b9-159">The device model that is being reported</span></span>|
|<span data-ttu-id="a77b9-160">state</span><span class="sxs-lookup"><span data-stu-id="a77b9-160">state</span></span>|[<span data-ttu-id="a77b9-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a77b9-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a77b9-162">设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="a77b9-162">The compliance state of the setting.</span></span> <span data-ttu-id="a77b9-163">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="a77b9-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a77b9-164">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a77b9-164">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a77b9-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a77b9-165">DateTimeOffset</span></span>|<span data-ttu-id="a77b9-166">设备合规性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="a77b9-166">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="a77b9-167">关系</span><span class="sxs-lookup"><span data-stu-id="a77b9-167">Relationships</span></span>
<span data-ttu-id="a77b9-168">无</span><span class="sxs-lookup"><span data-stu-id="a77b9-168">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a77b9-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a77b9-169">JSON Representation</span></span>
<span data-ttu-id="a77b9-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a77b9-170">Here is a JSON representation of the resource.</span></span>
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




