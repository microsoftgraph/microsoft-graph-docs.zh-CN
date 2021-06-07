---
title: deviceComplianceSettingState 资源类型
description: 给定设备的设备符合性设置状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7691614bbad8ecc24b4122848e75c4b4a1bb1409
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758874"
---
# <a name="devicecompliancesettingstate-resource-type"></a><span data-ttu-id="786b3-103">deviceComplianceSettingState 资源类型</span><span class="sxs-lookup"><span data-stu-id="786b3-103">deviceComplianceSettingState resource type</span></span>

<span data-ttu-id="786b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="786b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="786b3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="786b3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="786b3-106">给定设备的设备符合性设置状态。</span><span class="sxs-lookup"><span data-stu-id="786b3-106">Device compliance setting State for a given device.</span></span>

## <a name="methods"></a><span data-ttu-id="786b3-107">方法</span><span class="sxs-lookup"><span data-stu-id="786b3-107">Methods</span></span>
|<span data-ttu-id="786b3-108">方法</span><span class="sxs-lookup"><span data-stu-id="786b3-108">Method</span></span>|<span data-ttu-id="786b3-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="786b3-109">Return Type</span></span>|<span data-ttu-id="786b3-110">说明</span><span class="sxs-lookup"><span data-stu-id="786b3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="786b3-111">列出 deviceComplianceSettingStates</span><span class="sxs-lookup"><span data-stu-id="786b3-111">List deviceComplianceSettingStates</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-list.md)|<span data-ttu-id="786b3-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 集合</span><span class="sxs-lookup"><span data-stu-id="786b3-112">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) collection</span></span>|<span data-ttu-id="786b3-113">列出 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="786b3-113">List properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="786b3-114">获取 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="786b3-114">Get deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-get.md)|[<span data-ttu-id="786b3-115">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="786b3-115">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="786b3-116">读取 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="786b3-116">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="786b3-117">创建 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="786b3-117">Create deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-create.md)|[<span data-ttu-id="786b3-118">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="786b3-118">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="786b3-119">创建新的 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="786b3-119">Create a new [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|
|[<span data-ttu-id="786b3-120">删除 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="786b3-120">Delete deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-delete.md)|<span data-ttu-id="786b3-121">无</span><span class="sxs-lookup"><span data-stu-id="786b3-121">None</span></span>|<span data-ttu-id="786b3-122">删除 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md)。</span><span class="sxs-lookup"><span data-stu-id="786b3-122">Deletes a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md).</span></span>|
|[<span data-ttu-id="786b3-123">更新 deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="786b3-123">Update deviceComplianceSettingState</span></span>](../api/intune-deviceconfig-devicecompliancesettingstate-update.md)|[<span data-ttu-id="786b3-124">deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="786b3-124">deviceComplianceSettingState</span></span>](../resources/intune-deviceconfig-devicecompliancesettingstate.md)|<span data-ttu-id="786b3-125">更新 [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="786b3-125">Update the properties of a [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="786b3-126">属性</span><span class="sxs-lookup"><span data-stu-id="786b3-126">Properties</span></span>
|<span data-ttu-id="786b3-127">属性</span><span class="sxs-lookup"><span data-stu-id="786b3-127">Property</span></span>|<span data-ttu-id="786b3-128">类型</span><span class="sxs-lookup"><span data-stu-id="786b3-128">Type</span></span>|<span data-ttu-id="786b3-129">说明</span><span class="sxs-lookup"><span data-stu-id="786b3-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="786b3-130">id</span><span class="sxs-lookup"><span data-stu-id="786b3-130">id</span></span>|<span data-ttu-id="786b3-131">String</span><span class="sxs-lookup"><span data-stu-id="786b3-131">String</span></span>|<span data-ttu-id="786b3-132">实体的键</span><span class="sxs-lookup"><span data-stu-id="786b3-132">Key of the entity</span></span>|
|<span data-ttu-id="786b3-133">setting</span><span class="sxs-lookup"><span data-stu-id="786b3-133">setting</span></span>|<span data-ttu-id="786b3-134">String</span><span class="sxs-lookup"><span data-stu-id="786b3-134">String</span></span>|<span data-ttu-id="786b3-135">设置类名和属性名。</span><span class="sxs-lookup"><span data-stu-id="786b3-135">The setting class name and property name.</span></span>|
|<span data-ttu-id="786b3-136">settingName</span><span class="sxs-lookup"><span data-stu-id="786b3-136">settingName</span></span>|<span data-ttu-id="786b3-137">String</span><span class="sxs-lookup"><span data-stu-id="786b3-137">String</span></span>|<span data-ttu-id="786b3-138">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="786b3-138">The Setting Name that is being reported</span></span>|
|<span data-ttu-id="786b3-139">deviceId</span><span class="sxs-lookup"><span data-stu-id="786b3-139">deviceId</span></span>|<span data-ttu-id="786b3-140">String</span><span class="sxs-lookup"><span data-stu-id="786b3-140">String</span></span>|<span data-ttu-id="786b3-141">报告的设备 ID</span><span class="sxs-lookup"><span data-stu-id="786b3-141">The Device Id that is being reported</span></span>|
|<span data-ttu-id="786b3-142">deviceName</span><span class="sxs-lookup"><span data-stu-id="786b3-142">deviceName</span></span>|<span data-ttu-id="786b3-143">String</span><span class="sxs-lookup"><span data-stu-id="786b3-143">String</span></span>|<span data-ttu-id="786b3-144">报告的设备名称</span><span class="sxs-lookup"><span data-stu-id="786b3-144">The Device Name that is being reported</span></span>|
|<span data-ttu-id="786b3-145">userId</span><span class="sxs-lookup"><span data-stu-id="786b3-145">userId</span></span>|<span data-ttu-id="786b3-146">String</span><span class="sxs-lookup"><span data-stu-id="786b3-146">String</span></span>|<span data-ttu-id="786b3-147">报告的用户 ID</span><span class="sxs-lookup"><span data-stu-id="786b3-147">The user Id that is being reported</span></span>|
|<span data-ttu-id="786b3-148">userEmail</span><span class="sxs-lookup"><span data-stu-id="786b3-148">userEmail</span></span>|<span data-ttu-id="786b3-149">String</span><span class="sxs-lookup"><span data-stu-id="786b3-149">String</span></span>|<span data-ttu-id="786b3-150">报告的用户电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="786b3-150">The User email address that is being reported</span></span>|
|<span data-ttu-id="786b3-151">userName</span><span class="sxs-lookup"><span data-stu-id="786b3-151">userName</span></span>|<span data-ttu-id="786b3-152">String</span><span class="sxs-lookup"><span data-stu-id="786b3-152">String</span></span>|<span data-ttu-id="786b3-153">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="786b3-153">The User Name that is being reported</span></span>|
|<span data-ttu-id="786b3-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="786b3-154">userPrincipalName</span></span>|<span data-ttu-id="786b3-155">String</span><span class="sxs-lookup"><span data-stu-id="786b3-155">String</span></span>|<span data-ttu-id="786b3-156">报告的用户主体名称</span><span class="sxs-lookup"><span data-stu-id="786b3-156">The User PrincipalName that is being reported</span></span>|
|<span data-ttu-id="786b3-157">deviceModel</span><span class="sxs-lookup"><span data-stu-id="786b3-157">deviceModel</span></span>|<span data-ttu-id="786b3-158">String</span><span class="sxs-lookup"><span data-stu-id="786b3-158">String</span></span>|<span data-ttu-id="786b3-159">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="786b3-159">The device model that is being reported</span></span>|
|<span data-ttu-id="786b3-160">state</span><span class="sxs-lookup"><span data-stu-id="786b3-160">state</span></span>|[<span data-ttu-id="786b3-161">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="786b3-161">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="786b3-162">设置的合规性状态。</span><span class="sxs-lookup"><span data-stu-id="786b3-162">The compliance state of the setting.</span></span> <span data-ttu-id="786b3-163">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="786b3-163">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="786b3-164">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="786b3-164">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="786b3-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="786b3-165">DateTimeOffset</span></span>|<span data-ttu-id="786b3-166">设备合规性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="786b3-166">The DateTime when device compliance grace period expires</span></span>|

## <a name="relationships"></a><span data-ttu-id="786b3-167">关系</span><span class="sxs-lookup"><span data-stu-id="786b3-167">Relationships</span></span>
<span data-ttu-id="786b3-168">无</span><span class="sxs-lookup"><span data-stu-id="786b3-168">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="786b3-169">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="786b3-169">JSON Representation</span></span>
<span data-ttu-id="786b3-170">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="786b3-170">Here is a JSON representation of the resource.</span></span>
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




