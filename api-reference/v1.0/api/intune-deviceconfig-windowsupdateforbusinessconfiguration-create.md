---
title: 创建 windowsUpdateForBusinessConfiguration
description: 创建新的 windowsUpdateForBusinessConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e47aa6db924d18e1c6f84bedf877722ec4e6521
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52753788"
---
# <a name="create-windowsupdateforbusinessconfiguration"></a><span data-ttu-id="3cac9-103">创建 windowsUpdateForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="3cac9-103">Create windowsUpdateForBusinessConfiguration</span></span>

<span data-ttu-id="3cac9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3cac9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3cac9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3cac9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cac9-106">创建新的 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3cac9-106">Create a new [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3cac9-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3cac9-107">Prerequisites</span></span>
<span data-ttu-id="3cac9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3cac9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3cac9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3cac9-110">Permission type</span></span>|<span data-ttu-id="3cac9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3cac9-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3cac9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3cac9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3cac9-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cac9-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3cac9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3cac9-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3cac9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3cac9-115">Not supported.</span></span>|
|<span data-ttu-id="3cac9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3cac9-116">Application</span></span>|<span data-ttu-id="3cac9-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3cac9-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3cac9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3cac9-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3cac9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3cac9-119">Request headers</span></span>
|<span data-ttu-id="3cac9-120">标头</span><span class="sxs-lookup"><span data-stu-id="3cac9-120">Header</span></span>|<span data-ttu-id="3cac9-121">值</span><span class="sxs-lookup"><span data-stu-id="3cac9-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3cac9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3cac9-122">Authorization</span></span>|<span data-ttu-id="3cac9-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3cac9-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3cac9-124">接受</span><span class="sxs-lookup"><span data-stu-id="3cac9-124">Accept</span></span>|<span data-ttu-id="3cac9-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3cac9-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3cac9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3cac9-126">Request body</span></span>
<span data-ttu-id="3cac9-127">在请求正文中，提供 windowsUpdateForBusinessConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3cac9-127">In the request body, supply a JSON representation for the windowsUpdateForBusinessConfiguration object.</span></span>

<span data-ttu-id="3cac9-128">下表显示创建 windowsUpdateForBusinessConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3cac9-128">The following table shows the properties that are required when you create the windowsUpdateForBusinessConfiguration.</span></span>

|<span data-ttu-id="3cac9-129">属性</span><span class="sxs-lookup"><span data-stu-id="3cac9-129">Property</span></span>|<span data-ttu-id="3cac9-130">类型</span><span class="sxs-lookup"><span data-stu-id="3cac9-130">Type</span></span>|<span data-ttu-id="3cac9-131">说明</span><span class="sxs-lookup"><span data-stu-id="3cac9-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cac9-132">id</span><span class="sxs-lookup"><span data-stu-id="3cac9-132">id</span></span>|<span data-ttu-id="3cac9-133">String</span><span class="sxs-lookup"><span data-stu-id="3cac9-133">String</span></span>|<span data-ttu-id="3cac9-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3cac9-134">Key of the entity.</span></span> <span data-ttu-id="3cac9-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cac9-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac9-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3cac9-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3cac9-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cac9-137">DateTimeOffset</span></span>|<span data-ttu-id="3cac9-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3cac9-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3cac9-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cac9-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac9-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3cac9-140">createdDateTime</span></span>|<span data-ttu-id="3cac9-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cac9-141">DateTimeOffset</span></span>|<span data-ttu-id="3cac9-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3cac9-142">DateTime the object was created.</span></span> <span data-ttu-id="3cac9-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cac9-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac9-144">说明</span><span class="sxs-lookup"><span data-stu-id="3cac9-144">description</span></span>|<span data-ttu-id="3cac9-145">String</span><span class="sxs-lookup"><span data-stu-id="3cac9-145">String</span></span>|<span data-ttu-id="3cac9-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3cac9-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3cac9-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cac9-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac9-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3cac9-148">displayName</span></span>|<span data-ttu-id="3cac9-149">String</span><span class="sxs-lookup"><span data-stu-id="3cac9-149">String</span></span>|<span data-ttu-id="3cac9-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3cac9-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3cac9-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cac9-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac9-152">version</span><span class="sxs-lookup"><span data-stu-id="3cac9-152">version</span></span>|<span data-ttu-id="3cac9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac9-153">Int32</span></span>|<span data-ttu-id="3cac9-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3cac9-154">Version of the device configuration.</span></span> <span data-ttu-id="3cac9-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3cac9-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3cac9-156">deliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="3cac9-156">deliveryOptimizationMode</span></span>|[<span data-ttu-id="3cac9-157">windowsDeliveryOptimizationMode</span><span class="sxs-lookup"><span data-stu-id="3cac9-157">windowsDeliveryOptimizationMode</span></span>](../resources/intune-deviceconfig-windowsdeliveryoptimizationmode.md)|<span data-ttu-id="3cac9-158">传递优化模式。</span><span class="sxs-lookup"><span data-stu-id="3cac9-158">Delivery Optimization Mode.</span></span> <span data-ttu-id="3cac9-159">可取值为：`userDefined`、`httpOnly`、`httpWithPeeringNat`、`httpWithPeeringPrivateGroup`、`httpWithInternetPeering`、`simpleDownload` 或 `bypassMode`。</span><span class="sxs-lookup"><span data-stu-id="3cac9-159">Possible values are: `userDefined`, `httpOnly`, `httpWithPeeringNat`, `httpWithPeeringPrivateGroup`, `httpWithInternetPeering`, `simpleDownload`, `bypassMode`.</span></span>|
|<span data-ttu-id="3cac9-160">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="3cac9-160">prereleaseFeatures</span></span>|[<span data-ttu-id="3cac9-161">prereleaseFeatures</span><span class="sxs-lookup"><span data-stu-id="3cac9-161">prereleaseFeatures</span></span>](../resources/intune-deviceconfig-prereleasefeatures.md)|<span data-ttu-id="3cac9-162">预发布功能。</span><span class="sxs-lookup"><span data-stu-id="3cac9-162">The pre-release features.</span></span> <span data-ttu-id="3cac9-163">可取值为：`userDefined`、`settingsOnly`、`settingsAndExperimentations`、`notAllowed`。</span><span class="sxs-lookup"><span data-stu-id="3cac9-163">Possible values are: `userDefined`, `settingsOnly`, `settingsAndExperimentations`, `notAllowed`.</span></span>|
|<span data-ttu-id="3cac9-164">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="3cac9-164">automaticUpdateMode</span></span>|[<span data-ttu-id="3cac9-165">automaticUpdateMode</span><span class="sxs-lookup"><span data-stu-id="3cac9-165">automaticUpdateMode</span></span>](../resources/intune-deviceconfig-automaticupdatemode.md)|<span data-ttu-id="3cac9-166">自动更新模式。</span><span class="sxs-lookup"><span data-stu-id="3cac9-166">Automatic update mode.</span></span> <span data-ttu-id="3cac9-167">可取值为：`userDefined`、`notifyDownload`、`autoInstallAtMaintenanceTime`、`autoInstallAndRebootAtMaintenanceTime`、`autoInstallAndRebootAtScheduledTime`、`autoInstallAndRebootWithoutEndUserControl`。</span><span class="sxs-lookup"><span data-stu-id="3cac9-167">Possible values are: `userDefined`, `notifyDownload`, `autoInstallAtMaintenanceTime`, `autoInstallAndRebootAtMaintenanceTime`, `autoInstallAndRebootAtScheduledTime`, `autoInstallAndRebootWithoutEndUserControl`.</span></span>|
|<span data-ttu-id="3cac9-168">microsoftUpdateServiceAllowed</span><span class="sxs-lookup"><span data-stu-id="3cac9-168">microsoftUpdateServiceAllowed</span></span>|<span data-ttu-id="3cac9-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cac9-169">Boolean</span></span>|<span data-ttu-id="3cac9-170">允许 Microsoft 更新服务</span><span class="sxs-lookup"><span data-stu-id="3cac9-170">Allow Microsoft Update Service</span></span>|
|<span data-ttu-id="3cac9-171">driversExcluded</span><span class="sxs-lookup"><span data-stu-id="3cac9-171">driversExcluded</span></span>|<span data-ttu-id="3cac9-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cac9-172">Boolean</span></span>|<span data-ttu-id="3cac9-173">排除 Windows 更新驱动程序</span><span class="sxs-lookup"><span data-stu-id="3cac9-173">Exclude Windows update Drivers</span></span>|
|<span data-ttu-id="3cac9-174">installationSchedule</span><span class="sxs-lookup"><span data-stu-id="3cac9-174">installationSchedule</span></span>|[<span data-ttu-id="3cac9-175">windowsUpdateInstallScheduleType</span><span class="sxs-lookup"><span data-stu-id="3cac9-175">windowsUpdateInstallScheduleType</span></span>](../resources/intune-deviceconfig-windowsupdateinstallscheduletype.md)|<span data-ttu-id="3cac9-176">安装计划</span><span class="sxs-lookup"><span data-stu-id="3cac9-176">Installation schedule</span></span>|
|<span data-ttu-id="3cac9-177">qualityUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="3cac9-177">qualityUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="3cac9-178">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac9-178">Int32</span></span>|<span data-ttu-id="3cac9-179">推迟质量更新的天数</span><span class="sxs-lookup"><span data-stu-id="3cac9-179">Defer Quality Updates by these many days</span></span>|
|<span data-ttu-id="3cac9-180">featureUpdatesDeferralPeriodInDays</span><span class="sxs-lookup"><span data-stu-id="3cac9-180">featureUpdatesDeferralPeriodInDays</span></span>|<span data-ttu-id="3cac9-181">Int32</span><span class="sxs-lookup"><span data-stu-id="3cac9-181">Int32</span></span>|<span data-ttu-id="3cac9-182">推迟功能更新的天数</span><span class="sxs-lookup"><span data-stu-id="3cac9-182">Defer Feature Updates by these many days</span></span>|
|<span data-ttu-id="3cac9-183">qualityUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="3cac9-183">qualityUpdatesPaused</span></span>|<span data-ttu-id="3cac9-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cac9-184">Boolean</span></span>|<span data-ttu-id="3cac9-185">暂停质量更新</span><span class="sxs-lookup"><span data-stu-id="3cac9-185">Pause Quality Updates</span></span>|
|<span data-ttu-id="3cac9-186">featureUpdatesPaused</span><span class="sxs-lookup"><span data-stu-id="3cac9-186">featureUpdatesPaused</span></span>|<span data-ttu-id="3cac9-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3cac9-187">Boolean</span></span>|<span data-ttu-id="3cac9-188">暂停功能更新</span><span class="sxs-lookup"><span data-stu-id="3cac9-188">Pause Feature Updates</span></span>|
|<span data-ttu-id="3cac9-189">qualityUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="3cac9-189">qualityUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="3cac9-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cac9-190">DateTimeOffset</span></span>|<span data-ttu-id="3cac9-191">质量更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="3cac9-191">Quality Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="3cac9-192">featureUpdatesPauseExpiryDateTime</span><span class="sxs-lookup"><span data-stu-id="3cac9-192">featureUpdatesPauseExpiryDateTime</span></span>|<span data-ttu-id="3cac9-193">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3cac9-193">DateTimeOffset</span></span>|<span data-ttu-id="3cac9-194">功能更新暂停到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="3cac9-194">Feature Updates Pause Expiry datetime</span></span>|
|<span data-ttu-id="3cac9-195">businessReadyUpdatesOnly</span><span class="sxs-lookup"><span data-stu-id="3cac9-195">businessReadyUpdatesOnly</span></span>|[<span data-ttu-id="3cac9-196">windowsUpdateType</span><span class="sxs-lookup"><span data-stu-id="3cac9-196">windowsUpdateType</span></span>](../resources/intune-deviceconfig-windowsupdatetype.md)|<span data-ttu-id="3cac9-197">确定接收更新的分支设备。</span><span class="sxs-lookup"><span data-stu-id="3cac9-197">Determines which branch devices will receive their updates from.</span></span> <span data-ttu-id="3cac9-198">可取值为：`userDefined`、`all`、`businessReadyOnly`、`windowsInsiderBuildFast`、`windowsInsiderBuildSlow`、`windowsInsiderBuildRelease`。</span><span class="sxs-lookup"><span data-stu-id="3cac9-198">Possible values are: `userDefined`, `all`, `businessReadyOnly`, `windowsInsiderBuildFast`, `windowsInsiderBuildSlow`, `windowsInsiderBuildRelease`.</span></span>|



## <a name="response"></a><span data-ttu-id="3cac9-199">响应</span><span class="sxs-lookup"><span data-stu-id="3cac9-199">Response</span></span>
<span data-ttu-id="3cac9-200">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3cac9-200">If successful, this method returns a `201 Created` response code and a [windowsUpdateForBusinessConfiguration](../resources/intune-deviceconfig-windowsupdateforbusinessconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3cac9-201">示例</span><span class="sxs-lookup"><span data-stu-id="3cac9-201">Example</span></span>

### <a name="request"></a><span data-ttu-id="3cac9-202">请求</span><span class="sxs-lookup"><span data-stu-id="3cac9-202">Request</span></span>
<span data-ttu-id="3cac9-203">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3cac9-203">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 910

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```

### <a name="response"></a><span data-ttu-id="3cac9-204">响应</span><span class="sxs-lookup"><span data-stu-id="3cac9-204">Response</span></span>
<span data-ttu-id="3cac9-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3cac9-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1082

{
  "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
  "id": "4928dd6a-dd6a-4928-6add-28496add2849",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "deliveryOptimizationMode": "httpOnly",
  "prereleaseFeatures": "settingsOnly",
  "automaticUpdateMode": "notifyDownload",
  "microsoftUpdateServiceAllowed": true,
  "driversExcluded": true,
  "installationSchedule": {
    "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
    "scheduledInstallDay": "everyday",
    "scheduledInstallTime": "11:59:31.3170000"
  },
  "qualityUpdatesDeferralPeriodInDays": 2,
  "featureUpdatesDeferralPeriodInDays": 2,
  "qualityUpdatesPaused": true,
  "featureUpdatesPaused": true,
  "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
  "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
  "businessReadyUpdatesOnly": "all"
}
```




