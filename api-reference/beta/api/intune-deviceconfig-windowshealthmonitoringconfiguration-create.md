---
title: 创建 windowsHealthMonitoringConfiguration
description: 创建新的 windowsHealthMonitoringConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a594b406a41eb307b4a3347cfa3f0eb8ecda35e1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33917952"
---
# <a name="create-windowshealthmonitoringconfiguration"></a><span data-ttu-id="c43fb-103">创建 windowsHealthMonitoringConfiguration</span><span class="sxs-lookup"><span data-stu-id="c43fb-103">Create windowsHealthMonitoringConfiguration</span></span>

> <span data-ttu-id="c43fb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c43fb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c43fb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c43fb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c43fb-106">创建新的[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c43fb-106">Create a new [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c43fb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c43fb-107">Prerequisites</span></span>
<span data-ttu-id="c43fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c43fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c43fb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c43fb-110">Permission type</span></span>|<span data-ttu-id="c43fb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c43fb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c43fb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c43fb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c43fb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c43fb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c43fb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c43fb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c43fb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c43fb-115">Not supported.</span></span>|
|<span data-ttu-id="c43fb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c43fb-116">Application</span></span>|<span data-ttu-id="c43fb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c43fb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c43fb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c43fb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="c43fb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c43fb-119">Request headers</span></span>
|<span data-ttu-id="c43fb-120">标头</span><span class="sxs-lookup"><span data-stu-id="c43fb-120">Header</span></span>|<span data-ttu-id="c43fb-121">值</span><span class="sxs-lookup"><span data-stu-id="c43fb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c43fb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c43fb-122">Authorization</span></span>|<span data-ttu-id="c43fb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c43fb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c43fb-124">接受</span><span class="sxs-lookup"><span data-stu-id="c43fb-124">Accept</span></span>|<span data-ttu-id="c43fb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c43fb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c43fb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c43fb-126">Request body</span></span>
<span data-ttu-id="c43fb-127">在请求正文中, 提供 windowsHealthMonitoringConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c43fb-127">In the request body, supply a JSON representation for the windowsHealthMonitoringConfiguration object.</span></span>

<span data-ttu-id="c43fb-128">下表显示创建 windowsHealthMonitoringConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c43fb-128">The following table shows the properties that are required when you create the windowsHealthMonitoringConfiguration.</span></span>

|<span data-ttu-id="c43fb-129">属性</span><span class="sxs-lookup"><span data-stu-id="c43fb-129">Property</span></span>|<span data-ttu-id="c43fb-130">类型</span><span class="sxs-lookup"><span data-stu-id="c43fb-130">Type</span></span>|<span data-ttu-id="c43fb-131">说明</span><span class="sxs-lookup"><span data-stu-id="c43fb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c43fb-132">id</span><span class="sxs-lookup"><span data-stu-id="c43fb-132">id</span></span>|<span data-ttu-id="c43fb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="c43fb-133">String</span></span>|<span data-ttu-id="c43fb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c43fb-134">Key of the entity.</span></span> <span data-ttu-id="c43fb-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c43fb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c43fb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c43fb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="c43fb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c43fb-137">DateTimeOffset</span></span>|<span data-ttu-id="c43fb-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c43fb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="c43fb-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c43fb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c43fb-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c43fb-140">roleScopeTagIds</span></span>|<span data-ttu-id="c43fb-141">String collection</span><span class="sxs-lookup"><span data-stu-id="c43fb-141">String collection</span></span>|<span data-ttu-id="c43fb-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="c43fb-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c43fb-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c43fb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c43fb-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c43fb-144">supportsScopeTags</span></span>|<span data-ttu-id="c43fb-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="c43fb-145">Boolean</span></span>|<span data-ttu-id="c43fb-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="c43fb-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c43fb-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="c43fb-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c43fb-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="c43fb-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c43fb-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="c43fb-149">This property is read-only.</span></span> <span data-ttu-id="c43fb-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c43fb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c43fb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c43fb-151">createdDateTime</span></span>|<span data-ttu-id="c43fb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c43fb-152">DateTimeOffset</span></span>|<span data-ttu-id="c43fb-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c43fb-153">DateTime the object was created.</span></span> <span data-ttu-id="c43fb-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c43fb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c43fb-155">说明</span><span class="sxs-lookup"><span data-stu-id="c43fb-155">description</span></span>|<span data-ttu-id="c43fb-156">String</span><span class="sxs-lookup"><span data-stu-id="c43fb-156">String</span></span>|<span data-ttu-id="c43fb-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="c43fb-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c43fb-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c43fb-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c43fb-159">displayName</span><span class="sxs-lookup"><span data-stu-id="c43fb-159">displayName</span></span>|<span data-ttu-id="c43fb-160">String</span><span class="sxs-lookup"><span data-stu-id="c43fb-160">String</span></span>|<span data-ttu-id="c43fb-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c43fb-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c43fb-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c43fb-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c43fb-163">version</span><span class="sxs-lookup"><span data-stu-id="c43fb-163">version</span></span>|<span data-ttu-id="c43fb-164">Int32</span><span class="sxs-lookup"><span data-stu-id="c43fb-164">Int32</span></span>|<span data-ttu-id="c43fb-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="c43fb-165">Version of the device configuration.</span></span> <span data-ttu-id="c43fb-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c43fb-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c43fb-167">allowDeviceHealthMonitoring</span><span class="sxs-lookup"><span data-stu-id="c43fb-167">allowDeviceHealthMonitoring</span></span>|[<span data-ttu-id="c43fb-168">启用</span><span class="sxs-lookup"><span data-stu-id="c43fb-168">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="c43fb-169">在设备上启用设备运行状况监视。</span><span class="sxs-lookup"><span data-stu-id="c43fb-169">Enables device health monitoring on the device.</span></span> <span data-ttu-id="c43fb-170">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="c43fb-170">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="c43fb-171">configDeviceHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="c43fb-171">configDeviceHealthMonitoringScope</span></span>|[<span data-ttu-id="c43fb-172">windowsHealthMonitoringScope</span><span class="sxs-lookup"><span data-stu-id="c43fb-172">windowsHealthMonitoringScope</span></span>](../resources/intune-deviceconfig-windowshealthmonitoringscope.md)|<span data-ttu-id="c43fb-173">指定从启用运行状况监视的设备收集的一组事件。</span><span class="sxs-lookup"><span data-stu-id="c43fb-173">Specifies set of events collected from the device where health monitoring is enabled.</span></span> <span data-ttu-id="c43fb-174">可取值为：`undefined`、`healthMonitoring`、`bootPerformance`。</span><span class="sxs-lookup"><span data-stu-id="c43fb-174">Possible values are: `undefined`, `healthMonitoring`, `bootPerformance`.</span></span>|
|<span data-ttu-id="c43fb-175">configDeviceHealthMonitoringCustomScope</span><span class="sxs-lookup"><span data-stu-id="c43fb-175">configDeviceHealthMonitoringCustomScope</span></span>|<span data-ttu-id="c43fb-176">String</span><span class="sxs-lookup"><span data-stu-id="c43fb-176">String</span></span>|<span data-ttu-id="c43fb-177">指定从启用运行状况监视的设备收集的自定义事件集</span><span class="sxs-lookup"><span data-stu-id="c43fb-177">Specifies custom set of events collected from the device where health monitoring is enabled</span></span>|



## <a name="response"></a><span data-ttu-id="c43fb-178">响应</span><span class="sxs-lookup"><span data-stu-id="c43fb-178">Response</span></span>
<span data-ttu-id="c43fb-179">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c43fb-179">If successful, this method returns a `201 Created` response code and a [windowsHealthMonitoringConfiguration](../resources/intune-deviceconfig-windowshealthmonitoringconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c43fb-180">示例</span><span class="sxs-lookup"><span data-stu-id="c43fb-180">Example</span></span>

### <a name="request"></a><span data-ttu-id="c43fb-181">请求</span><span class="sxs-lookup"><span data-stu-id="c43fb-181">Request</span></span>
<span data-ttu-id="c43fb-182">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c43fb-182">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="c43fb-183">响应</span><span class="sxs-lookup"><span data-stu-id="c43fb-183">Response</span></span>
<span data-ttu-id="c43fb-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c43fb-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




