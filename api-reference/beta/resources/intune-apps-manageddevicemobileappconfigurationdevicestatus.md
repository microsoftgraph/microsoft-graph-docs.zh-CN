---
title: managedDeviceMobileAppConfigurationDeviceStatus 资源类型
description: 包含设备的 MDM 移动应用配置状态的属性、继承属性和操作。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d20a910a2ed2a409c7dc3853da4fc5a507b76384
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42492472"
---
# <a name="manageddevicemobileappconfigurationdevicestatus-resource-type"></a><span data-ttu-id="a70a7-103">managedDeviceMobileAppConfigurationDeviceStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="a70a7-103">managedDeviceMobileAppConfigurationDeviceStatus resource type</span></span>

<span data-ttu-id="a70a7-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a70a7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a70a7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a70a7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a70a7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a70a7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a70a7-107">包含设备的 MDM 移动应用配置状态的属性、继承属性和操作。</span><span class="sxs-lookup"><span data-stu-id="a70a7-107">Contains properties, inherited properties and actions for an MDM mobile app configuration status for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="a70a7-108">方法</span><span class="sxs-lookup"><span data-stu-id="a70a7-108">Methods</span></span>
|<span data-ttu-id="a70a7-109">方法</span><span class="sxs-lookup"><span data-stu-id="a70a7-109">Method</span></span>|<span data-ttu-id="a70a7-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="a70a7-110">Return Type</span></span>|<span data-ttu-id="a70a7-111">说明</span><span class="sxs-lookup"><span data-stu-id="a70a7-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a70a7-112">列出 managedDeviceMobileAppConfigurationDeviceStatuses</span><span class="sxs-lookup"><span data-stu-id="a70a7-112">List managedDeviceMobileAppConfigurationDeviceStatuses</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-list.md)|<span data-ttu-id="a70a7-113">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)集合</span><span class="sxs-lookup"><span data-stu-id="a70a7-113">[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) collection</span></span>|<span data-ttu-id="a70a7-114">列出[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a70a7-114">List properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) objects.</span></span>|
|[<span data-ttu-id="a70a7-115">获取 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a70a7-115">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-get.md)|[<span data-ttu-id="a70a7-116">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a70a7-116">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="a70a7-117">读取[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a70a7-117">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="a70a7-118">创建 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a70a7-118">Create managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-create.md)|[<span data-ttu-id="a70a7-119">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a70a7-119">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="a70a7-120">创建新的[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a70a7-120">Create a new [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|
|[<span data-ttu-id="a70a7-121">删除 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a70a7-121">Delete managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-delete.md)|<span data-ttu-id="a70a7-122">无</span><span class="sxs-lookup"><span data-stu-id="a70a7-122">None</span></span>|<span data-ttu-id="a70a7-123">删除[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)。</span><span class="sxs-lookup"><span data-stu-id="a70a7-123">Deletes a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md).</span></span>|
|[<span data-ttu-id="a70a7-124">更新 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a70a7-124">Update managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../api/intune-apps-manageddevicemobileappconfigurationdevicestatus-update.md)|[<span data-ttu-id="a70a7-125">managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="a70a7-125">managedDeviceMobileAppConfigurationDeviceStatus</span></span>](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)|<span data-ttu-id="a70a7-126">更新[managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a70a7-126">Update the properties of a [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a70a7-127">属性</span><span class="sxs-lookup"><span data-stu-id="a70a7-127">Properties</span></span>
|<span data-ttu-id="a70a7-128">属性</span><span class="sxs-lookup"><span data-stu-id="a70a7-128">Property</span></span>|<span data-ttu-id="a70a7-129">类型</span><span class="sxs-lookup"><span data-stu-id="a70a7-129">Type</span></span>|<span data-ttu-id="a70a7-130">说明</span><span class="sxs-lookup"><span data-stu-id="a70a7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a70a7-131">id</span><span class="sxs-lookup"><span data-stu-id="a70a7-131">id</span></span>|<span data-ttu-id="a70a7-132">String</span><span class="sxs-lookup"><span data-stu-id="a70a7-132">String</span></span>|<span data-ttu-id="a70a7-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a70a7-133">Key of the entity.</span></span>|
|<span data-ttu-id="a70a7-134">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="a70a7-134">deviceDisplayName</span></span>|<span data-ttu-id="a70a7-135">String</span><span class="sxs-lookup"><span data-stu-id="a70a7-135">String</span></span>|<span data-ttu-id="a70a7-136">DevicePolicyStatus 的设备名。</span><span class="sxs-lookup"><span data-stu-id="a70a7-136">Device name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="a70a7-137">userName</span><span class="sxs-lookup"><span data-stu-id="a70a7-137">userName</span></span>|<span data-ttu-id="a70a7-138">String</span><span class="sxs-lookup"><span data-stu-id="a70a7-138">String</span></span>|<span data-ttu-id="a70a7-139">报告的用户名</span><span class="sxs-lookup"><span data-stu-id="a70a7-139">The User Name that is being reported</span></span>|
|<span data-ttu-id="a70a7-140">deviceModel</span><span class="sxs-lookup"><span data-stu-id="a70a7-140">deviceModel</span></span>|<span data-ttu-id="a70a7-141">String</span><span class="sxs-lookup"><span data-stu-id="a70a7-141">String</span></span>|<span data-ttu-id="a70a7-142">报告的设备模型</span><span class="sxs-lookup"><span data-stu-id="a70a7-142">The device model that is being reported</span></span>|
|<span data-ttu-id="a70a7-143">platform</span><span class="sxs-lookup"><span data-stu-id="a70a7-143">platform</span></span>|<span data-ttu-id="a70a7-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a70a7-144">Int32</span></span>|<span data-ttu-id="a70a7-145">报告的设备的平台</span><span class="sxs-lookup"><span data-stu-id="a70a7-145">Platform of the device that is being reported</span></span>|
|<span data-ttu-id="a70a7-146">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a70a7-146">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="a70a7-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70a7-147">DateTimeOffset</span></span>|<span data-ttu-id="a70a7-148">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="a70a7-148">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="a70a7-149">status</span><span class="sxs-lookup"><span data-stu-id="a70a7-149">status</span></span>|[<span data-ttu-id="a70a7-150">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="a70a7-150">complianceStatus</span></span>](../resources/intune-shared-compliancestatus.md)|<span data-ttu-id="a70a7-151">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="a70a7-151">Compliance status of the policy report.</span></span> <span data-ttu-id="a70a7-152">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="a70a7-152">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="a70a7-153">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="a70a7-153">lastReportedDateTime</span></span>|<span data-ttu-id="a70a7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a70a7-154">DateTimeOffset</span></span>|<span data-ttu-id="a70a7-155">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="a70a7-155">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="a70a7-156">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a70a7-156">userPrincipalName</span></span>|<span data-ttu-id="a70a7-157">String</span><span class="sxs-lookup"><span data-stu-id="a70a7-157">String</span></span>|<span data-ttu-id="a70a7-158">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="a70a7-158">UserPrincipalName.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a70a7-159">关系</span><span class="sxs-lookup"><span data-stu-id="a70a7-159">Relationships</span></span>
<span data-ttu-id="a70a7-160">无</span><span class="sxs-lookup"><span data-stu-id="a70a7-160">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a70a7-161">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a70a7-161">JSON Representation</span></span>
<span data-ttu-id="a70a7-162">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a70a7-162">Here is a JSON representation of the resource.</span></span>
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



