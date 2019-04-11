---
title: managedDeviceMobileAppConfigurationDeviceStatus 资源类型
description: 包含设备的 MDM 移动应用配置状态的属性、继承属性和操作。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7933404f3e40117dfb04318c93df3fc48df6e594
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31802994"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a><span data-ttu-id="b6b7a-103">managedDeviceMobileAppConfigurationDeviceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6b7a-103">managedDeviceMobileAppConfigurationDeviceStatus resource type</span></span>

> <span data-ttu-id="b6b7a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6b7a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6b7a-106">包含设备的 MDM 移动应用配置状态的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-106">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="b6b7a-107">方法</span><span class="sxs-lookup"><span data-stu-id="b6b7a-107">Methods</span></span>
|<span data-ttu-id="b6b7a-108">方法</span><span class="sxs-lookup"><span data-stu-id="b6b7a-108">Method</span></span>|<span data-ttu-id="b6b7a-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="b6b7a-109">Return Type</span></span>|<span data-ttu-id="b6b7a-110">说明</span><span class="sxs-lookup"><span data-stu-id="b6b7a-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b6b7a-111">列出 managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="b6b7a-111">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|<span data-ttu-id="b6b7a-112">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6b7a-112">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="b6b7a-113">列出[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-113">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>|
|[<span data-ttu-id="b6b7a-114">获取 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b6b7a-114">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[<span data-ttu-id="b6b7a-115">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b6b7a-115">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="b6b7a-116">读取[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-116">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="b6b7a-117">创建 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b6b7a-117">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[<span data-ttu-id="b6b7a-118">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b6b7a-118">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="b6b7a-119">创建新的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-119">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="b6b7a-120">删除 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b6b7a-120">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|<span data-ttu-id="b6b7a-121">无</span><span class="sxs-lookup"><span data-stu-id="b6b7a-121">None</span></span>|<span data-ttu-id="b6b7a-122">删除[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-122">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>|
|[<span data-ttu-id="b6b7a-123">更新 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b6b7a-123">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[<span data-ttu-id="b6b7a-124">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="b6b7a-124">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="b6b7a-125">更新[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-125">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6b7a-126">属性</span><span class="sxs-lookup"><span data-stu-id="b6b7a-126">Properties</span></span>
|<span data-ttu-id="b6b7a-127">属性</span><span class="sxs-lookup"><span data-stu-id="b6b7a-127">Property</span></span>|<span data-ttu-id="b6b7a-128">类型</span><span class="sxs-lookup"><span data-stu-id="b6b7a-128">Type</span></span>|<span data-ttu-id="b6b7a-129">说明</span><span class="sxs-lookup"><span data-stu-id="b6b7a-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6b7a-130">id</span><span class="sxs-lookup"><span data-stu-id="b6b7a-130">id</span></span>|<span data-ttu-id="b6b7a-131">String</span><span class="sxs-lookup"><span data-stu-id="b6b7a-131">String</span></span>|<span data-ttu-id="b6b7a-132">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-132">Key of the entity.</span></span>|
|<span data-ttu-id="b6b7a-133">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="b6b7a-133">deviceDisplayName</span></span>|<span data-ttu-id="b6b7a-134">String</span><span class="sxs-lookup"><span data-stu-id="b6b7a-134">String</span></span>|<span data-ttu-id="b6b7a-135">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-135">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="b6b7a-136">userName</span><span class="sxs-lookup"><span data-stu-id="b6b7a-136">userName</span></span>|<span data-ttu-id="b6b7a-137">String</span><span class="sxs-lookup"><span data-stu-id="b6b7a-137">String</span></span>|<span data-ttu-id="b6b7a-138">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="b6b7a-138">The User Name that is being reported</span></span>|
|<span data-ttu-id="b6b7a-139">deviceModel</span><span class="sxs-lookup"><span data-stu-id="b6b7a-139">deviceModel</span></span>|<span data-ttu-id="b6b7a-140">String</span><span class="sxs-lookup"><span data-stu-id="b6b7a-140">String</span></span>|<span data-ttu-id="b6b7a-141">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="b6b7a-141">The device model that is being reported</span></span>|
|<span data-ttu-id="b6b7a-142">platform</span><span class="sxs-lookup"><span data-stu-id="b6b7a-142">platform</span></span>|<span data-ttu-id="b6b7a-143">Int32</span><span class="sxs-lookup"><span data-stu-id="b6b7a-143">Int32</span></span>|<span data-ttu-id="b6b7a-144">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="b6b7a-144">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="b6b7a-145">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="b6b7a-145">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="b6b7a-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6b7a-146">DateTimeOffset</span></span>|<span data-ttu-id="b6b7a-147">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="b6b7a-147">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="b6b7a-148">status</span><span class="sxs-lookup"><span data-stu-id="b6b7a-148">status</span></span>|[<span data-ttu-id="b6b7a-149">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="b6b7a-149">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="b6b7a-150">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-150">Compliance status of the policy report.</span></span> <span data-ttu-id="b6b7a-151">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-151">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="b6b7a-152">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6b7a-152">lastReportedDateTime</span></span>|<span data-ttu-id="b6b7a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6b7a-153">DateTimeOffset</span></span>|<span data-ttu-id="b6b7a-154">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-154">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="b6b7a-155">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6b7a-155">userPrincipalName</span></span>|<span data-ttu-id="b6b7a-156">String</span><span class="sxs-lookup"><span data-stu-id="b6b7a-156">String</span></span>|<span data-ttu-id="b6b7a-157">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-157">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6b7a-158">关系</span><span class="sxs-lookup"><span data-stu-id="b6b7a-158">Relationships</span></span>
<span data-ttu-id="b6b7a-159">无</span><span class="sxs-lookup"><span data-stu-id="b6b7a-159">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6b7a-160">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6b7a-160">JSON Representation</span></span>
<span data-ttu-id="b6b7a-161">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6b7a-161">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
  "id": "String (identifier)",
  "deviceDisplayName": "String",
  "userName": "String",
  "deviceModel": "String",
  "platform": 1024,
  "complianceGracePeriodExpirationDateTime": "String (timestamp)",
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```





