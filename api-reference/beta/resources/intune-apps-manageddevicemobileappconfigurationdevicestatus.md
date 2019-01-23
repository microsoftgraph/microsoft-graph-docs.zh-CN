---
title: managedDeviceMobileAppConfigurationDeviceStatus 资源类型
description: 包含的属性、 继承的属性和设备 MDM 移动应用程序配置状态的操作。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d987cc379e72c06a1c766e3110988a0bcd4db746
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419560"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a><span data-ttu-id="24622-103">managedDeviceMobileAppConfigurationDeviceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="24622-103">managedDeviceMobileAppConfigurationDeviceStatus resource type</span></span>

> <span data-ttu-id="24622-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="24622-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="24622-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="24622-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="24622-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24622-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24622-107">包含的属性、 继承的属性和设备 MDM 移动应用程序配置状态的操作。</span><span class="sxs-lookup"><span data-stu-id="24622-107">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="24622-108">方法</span><span class="sxs-lookup"><span data-stu-id="24622-108">Methods</span></span>
|<span data-ttu-id="24622-109">方法</span><span class="sxs-lookup"><span data-stu-id="24622-109">Method</span></span>|<span data-ttu-id="24622-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="24622-110">Return Type</span></span>|<span data-ttu-id="24622-111">说明</span><span class="sxs-lookup"><span data-stu-id="24622-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="24622-112">列表 managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="24622-112">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|<span data-ttu-id="24622-113">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="24622-113">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="24622-114">列出属性和[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="24622-114">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>|
|[<span data-ttu-id="24622-115">获取 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="24622-115">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[<span data-ttu-id="24622-116">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="24622-116">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="24622-117">读取属性和[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="24622-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="24622-118">创建 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="24622-118">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[<span data-ttu-id="24622-119">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="24622-119">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="24622-120">创建新的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="24622-120">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="24622-121">删除 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="24622-121">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|<span data-ttu-id="24622-122">无</span><span class="sxs-lookup"><span data-stu-id="24622-122">None</span></span>|<span data-ttu-id="24622-123">删除[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="24622-123">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>|
|[<span data-ttu-id="24622-124">更新 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="24622-124">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[<span data-ttu-id="24622-125">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="24622-125">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="24622-126">更新[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="24622-126">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="24622-127">属性</span><span class="sxs-lookup"><span data-stu-id="24622-127">Properties</span></span>
|<span data-ttu-id="24622-128">属性</span><span class="sxs-lookup"><span data-stu-id="24622-128">Property</span></span>|<span data-ttu-id="24622-129">类型</span><span class="sxs-lookup"><span data-stu-id="24622-129">Type</span></span>|<span data-ttu-id="24622-130">说明</span><span class="sxs-lookup"><span data-stu-id="24622-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24622-131">id</span><span class="sxs-lookup"><span data-stu-id="24622-131">id</span></span>|<span data-ttu-id="24622-132">String</span><span class="sxs-lookup"><span data-stu-id="24622-132">String</span></span>|<span data-ttu-id="24622-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="24622-133">Key of the entity.</span></span>|
|<span data-ttu-id="24622-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="24622-134">deviceDisplayName</span></span>|<span data-ttu-id="24622-135">String</span><span class="sxs-lookup"><span data-stu-id="24622-135">String</span></span>|<span data-ttu-id="24622-136">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="24622-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="24622-137">userName</span><span class="sxs-lookup"><span data-stu-id="24622-137">userName</span></span>|<span data-ttu-id="24622-138">String</span><span class="sxs-lookup"><span data-stu-id="24622-138">String</span></span>|<span data-ttu-id="24622-139">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="24622-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="24622-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="24622-140">deviceModel</span></span>|<span data-ttu-id="24622-141">String</span><span class="sxs-lookup"><span data-stu-id="24622-141">String</span></span>|<span data-ttu-id="24622-142">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="24622-142">The device model that is being reported</span></span>|
|<span data-ttu-id="24622-143">platform</span><span class="sxs-lookup"><span data-stu-id="24622-143">platform</span></span>|<span data-ttu-id="24622-144">Int32</span><span class="sxs-lookup"><span data-stu-id="24622-144">Int32</span></span>|<span data-ttu-id="24622-145">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="24622-145">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="24622-146">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="24622-146">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="24622-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24622-147">DateTimeOffset</span></span>|<span data-ttu-id="24622-148">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="24622-148">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="24622-149">status</span><span class="sxs-lookup"><span data-stu-id="24622-149">status</span></span>|[<span data-ttu-id="24622-150">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="24622-150">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="24622-151">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="24622-151">Compliance status of the policy report.</span></span> <span data-ttu-id="24622-152">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="24622-152">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="24622-153">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="24622-153">lastReportedDateTime</span></span>|<span data-ttu-id="24622-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24622-154">DateTimeOffset</span></span>|<span data-ttu-id="24622-155">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="24622-155">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="24622-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="24622-156">userPrincipalName</span></span>|<span data-ttu-id="24622-157">String</span><span class="sxs-lookup"><span data-stu-id="24622-157">String</span></span>|<span data-ttu-id="24622-158">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="24622-158">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="24622-159">关系</span><span class="sxs-lookup"><span data-stu-id="24622-159">Relationships</span></span>
<span data-ttu-id="24622-160">无</span><span class="sxs-lookup"><span data-stu-id="24622-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="24622-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="24622-161">JSON Representation</span></span>
<span data-ttu-id="24622-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24622-162">Here is a JSON representation of the resource.</span></span>
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




