---
title: 更新 windowsHealthMonitoringConfiguration
description: 更新 windowsHealthMonitoringConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e22db8c85d591c770128dc3db3594fa23826836
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917917"
---
# <a name="update-windowshealthmonitoringconfiguration"></a><span data-ttu-id="aa5b4-103">更新 windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="aa5b4-103">Update windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="aa5b4-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aa5b4-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aa5b4-106">更新[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-106">Update the properties of a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aa5b4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="aa5b4-107">Prerequisites</span></span>
<span data-ttu-id="aa5b4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa5b4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aa5b4-110">Permission type</span></span>|<span data-ttu-id="aa5b4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aa5b4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa5b4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aa5b4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="aa5b4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa5b4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aa5b4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aa5b4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa5b4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-115">Not supported.</span></span>|
|<span data-ttu-id="aa5b4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aa5b4-116">Application</span></span>|<span data-ttu-id="aa5b4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa5b4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aa5b4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aa5b4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aa5b4-119">Request headers</span></span>
|<span data-ttu-id="aa5b4-120">标头</span><span class="sxs-lookup"><span data-stu-id="aa5b4-120">Header</span></span>|<span data-ttu-id="aa5b4-121">值</span><span class="sxs-lookup"><span data-stu-id="aa5b4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa5b4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa5b4-122">Authorization</span></span>|<span data-ttu-id="aa5b4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa5b4-124">接受</span><span class="sxs-lookup"><span data-stu-id="aa5b4-124">Accept</span></span>|<span data-ttu-id="aa5b4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aa5b4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa5b4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aa5b4-126">Request body</span></span>
<span data-ttu-id="aa5b4-127">在请求正文中, 提供[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-127">In the request body, supply a JSON representation for the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

<span data-ttu-id="aa5b4-128">下表显示创建[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-128">The following table shows the properties that are required when you create the [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md).</span></span>

|<span data-ttu-id="aa5b4-129">属性</span><span class="sxs-lookup"><span data-stu-id="aa5b4-129">Property</span></span>|<span data-ttu-id="aa5b4-130">类型</span><span class="sxs-lookup"><span data-stu-id="aa5b4-130">Type</span></span>|<span data-ttu-id="aa5b4-131">说明</span><span class="sxs-lookup"><span data-stu-id="aa5b4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aa5b4-132">id</span><span class="sxs-lookup"><span data-stu-id="aa5b4-132">id</span></span>|<span data-ttu-id="aa5b4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="aa5b4-133">String</span></span>|<span data-ttu-id="aa5b4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-134">Key of the entity.</span></span> <span data-ttu-id="aa5b4-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa5b4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="aa5b4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="aa5b4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa5b4-137">DateTimeOffset</span></span>|<span data-ttu-id="aa5b4-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="aa5b4-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa5b4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="aa5b4-140">roleScopeTagIds</span></span>|<span data-ttu-id="aa5b4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="aa5b4-141">String collection</span></span>|<span data-ttu-id="aa5b4-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="aa5b4-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa5b4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="aa5b4-144">supportsScopeTags</span></span>|<span data-ttu-id="aa5b4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="aa5b4-145">Boolean</span></span>|<span data-ttu-id="aa5b4-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="aa5b4-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="aa5b4-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="aa5b4-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-149">This property is read-only.</span></span> <span data-ttu-id="aa5b4-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa5b4-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="aa5b4-151">createdDateTime</span></span>|<span data-ttu-id="aa5b4-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aa5b4-152">DateTimeOffset</span></span>|<span data-ttu-id="aa5b4-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-153">DateTime the object was created.</span></span> <span data-ttu-id="aa5b4-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa5b4-155">说明</span><span class="sxs-lookup"><span data-stu-id="aa5b4-155">description</span></span>|<span data-ttu-id="aa5b4-156">String</span><span class="sxs-lookup"><span data-stu-id="aa5b4-156">String</span></span>|<span data-ttu-id="aa5b4-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="aa5b4-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa5b4-159">displayName</span><span class="sxs-lookup"><span data-stu-id="aa5b4-159">displayName</span></span>|<span data-ttu-id="aa5b4-160">String</span><span class="sxs-lookup"><span data-stu-id="aa5b4-160">String</span></span>|<span data-ttu-id="aa5b4-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="aa5b4-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa5b4-163">version</span><span class="sxs-lookup"><span data-stu-id="aa5b4-163">version</span></span>|<span data-ttu-id="aa5b4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="aa5b4-164">Int32</span></span>|<span data-ttu-id="aa5b4-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-165">Version of the device configuration.</span></span> <span data-ttu-id="aa5b4-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="aa5b4-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="aa5b4-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="aa5b4-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="aa5b4-168">启用</span><span class="sxs-lookup"><span data-stu-id="aa5b4-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="aa5b4-169">在设备上启用设备运行状况监视。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="aa5b4-170">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="aa5b4-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="aa5b4-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="aa5b4-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="aa5b4-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="aa5b4-173">指定从启用运行状况监视的设备收集的一组事件。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-173">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="aa5b4-174">可取值为：`undefined`、`healthMonitoring`、`bootPerformance`。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|
|<span data-ttu-id="aa5b4-175">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="aa5b4-175">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="aa5b4-176">String</span><span class="sxs-lookup"><span data-stu-id="aa5b4-176">String</span></span>|<span data-ttu-id="aa5b4-177">指定从启用运行状况监视的设备收集的自定义事件集</span><span class="sxs-lookup"><span data-stu-id="aa5b4-177">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="aa5b4-178">响应</span><span class="sxs-lookup"><span data-stu-id="aa5b4-178">Response</span></span>
<span data-ttu-id="aa5b4-179">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-179">If successful, this method returns a `200 OK` response code and an updated [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa5b4-180">示例</span><span class="sxs-lookup"><span data-stu-id="aa5b4-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="aa5b4-181">请求</span><span class="sxs-lookup"><span data-stu-id="aa5b4-181">Request</span></span>
<span data-ttu-id="aa5b4-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-182">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 471

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```

### <a name="response"></a><span data-ttu-id="aa5b4-183">响应</span><span class="sxs-lookup"><span data-stu-id="aa5b4-183">Response</span></span>
<span data-ttu-id="aa5b4-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aa5b4-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 643

{
  "@odata.type": "#microsoft.graph.windowsHealthMonitoringConfiguration",
  "id": "3439bcec-bcec-3439-ecbc-3934ecbc3934",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "allowDeviceHealthMonitoring": "enabled",
  "configDeviceHealthMonitoringScope": "healthMonitoring",
  "configDeviceHealthMonitoringCustomScope": "Config Device Health Monitoring Custom Scope value"
}
```




