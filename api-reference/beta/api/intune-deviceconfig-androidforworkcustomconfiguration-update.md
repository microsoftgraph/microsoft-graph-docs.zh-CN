---
title: 更新 androidForWorkCustomConfiguration
description: 更新 androidForWorkCustomConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c71d396887248e0315124ba68782fa1d7ce9aef6
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48708569"
---
# <a name="update-androidforworkcustomconfiguration"></a><span data-ttu-id="185d5-103">更新 androidForWorkCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="185d5-103">Update androidForWorkCustomConfiguration</span></span>

<span data-ttu-id="185d5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="185d5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="185d5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="185d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="185d5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="185d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="185d5-107">更新 [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="185d5-107">Update the properties of a [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="185d5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="185d5-108">Prerequisites</span></span>
<span data-ttu-id="185d5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="185d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="185d5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="185d5-111">Permission type</span></span>|<span data-ttu-id="185d5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="185d5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="185d5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="185d5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="185d5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="185d5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="185d5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="185d5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="185d5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="185d5-116">Not supported.</span></span>|
|<span data-ttu-id="185d5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="185d5-117">Application</span></span>|<span data-ttu-id="185d5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="185d5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="185d5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="185d5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="185d5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="185d5-120">Request headers</span></span>
|<span data-ttu-id="185d5-121">标头</span><span class="sxs-lookup"><span data-stu-id="185d5-121">Header</span></span>|<span data-ttu-id="185d5-122">值</span><span class="sxs-lookup"><span data-stu-id="185d5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="185d5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="185d5-123">Authorization</span></span>|<span data-ttu-id="185d5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="185d5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="185d5-125">接受</span><span class="sxs-lookup"><span data-stu-id="185d5-125">Accept</span></span>|<span data-ttu-id="185d5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="185d5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="185d5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="185d5-127">Request body</span></span>
<span data-ttu-id="185d5-128">在请求正文中，提供 [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="185d5-128">In the request body, supply a JSON representation for the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object.</span></span>

<span data-ttu-id="185d5-129">下表显示创建 [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="185d5-129">The following table shows the properties that are required when you create the [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md).</span></span>

|<span data-ttu-id="185d5-130">属性</span><span class="sxs-lookup"><span data-stu-id="185d5-130">Property</span></span>|<span data-ttu-id="185d5-131">类型</span><span class="sxs-lookup"><span data-stu-id="185d5-131">Type</span></span>|<span data-ttu-id="185d5-132">说明</span><span class="sxs-lookup"><span data-stu-id="185d5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="185d5-133">id</span><span class="sxs-lookup"><span data-stu-id="185d5-133">id</span></span>|<span data-ttu-id="185d5-134">String</span><span class="sxs-lookup"><span data-stu-id="185d5-134">String</span></span>|<span data-ttu-id="185d5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="185d5-135">Key of the entity.</span></span> <span data-ttu-id="185d5-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="185d5-137">lastModifiedDateTime</span></span>|<span data-ttu-id="185d5-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="185d5-138">DateTimeOffset</span></span>|<span data-ttu-id="185d5-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="185d5-139">DateTime the object was last modified.</span></span> <span data-ttu-id="185d5-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="185d5-141">roleScopeTagIds</span></span>|<span data-ttu-id="185d5-142">String collection</span><span class="sxs-lookup"><span data-stu-id="185d5-142">String collection</span></span>|<span data-ttu-id="185d5-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="185d5-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="185d5-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="185d5-145">supportsScopeTags</span></span>|<span data-ttu-id="185d5-146">布尔</span><span class="sxs-lookup"><span data-stu-id="185d5-146">Boolean</span></span>|<span data-ttu-id="185d5-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="185d5-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="185d5-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="185d5-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="185d5-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="185d5-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="185d5-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="185d5-150">This property is read-only.</span></span> <span data-ttu-id="185d5-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="185d5-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="185d5-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="185d5-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="185d5-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="185d5-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="185d5-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="185d5-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="185d5-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="185d5-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="185d5-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="185d5-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="185d5-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="185d5-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="185d5-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="185d5-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="185d5-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="185d5-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="185d5-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="185d5-164">createdDateTime</span></span>|<span data-ttu-id="185d5-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="185d5-165">DateTimeOffset</span></span>|<span data-ttu-id="185d5-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="185d5-166">DateTime the object was created.</span></span> <span data-ttu-id="185d5-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-168">说明</span><span class="sxs-lookup"><span data-stu-id="185d5-168">description</span></span>|<span data-ttu-id="185d5-169">String</span><span class="sxs-lookup"><span data-stu-id="185d5-169">String</span></span>|<span data-ttu-id="185d5-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="185d5-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="185d5-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-172">displayName</span><span class="sxs-lookup"><span data-stu-id="185d5-172">displayName</span></span>|<span data-ttu-id="185d5-173">String</span><span class="sxs-lookup"><span data-stu-id="185d5-173">String</span></span>|<span data-ttu-id="185d5-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="185d5-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="185d5-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-176">version</span><span class="sxs-lookup"><span data-stu-id="185d5-176">version</span></span>|<span data-ttu-id="185d5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="185d5-177">Int32</span></span>|<span data-ttu-id="185d5-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="185d5-178">Version of the device configuration.</span></span> <span data-ttu-id="185d5-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="185d5-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="185d5-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="185d5-180">omaSettings</span></span>|<span data-ttu-id="185d5-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="185d5-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="185d5-182">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="185d5-182">OMA settings.</span></span> <span data-ttu-id="185d5-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="185d5-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="185d5-184">响应</span><span class="sxs-lookup"><span data-stu-id="185d5-184">Response</span></span>
<span data-ttu-id="185d5-185">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="185d5-185">If successful, this method returns a `200 OK` response code and an updated [androidForWorkCustomConfiguration](../resources/intune-deviceconfig-androidforworkcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="185d5-186">示例</span><span class="sxs-lookup"><span data-stu-id="185d5-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="185d5-187">请求</span><span class="sxs-lookup"><span data-stu-id="185d5-187">Request</span></span>
<span data-ttu-id="185d5-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="185d5-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1248

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="185d5-189">响应</span><span class="sxs-lookup"><span data-stu-id="185d5-189">Response</span></span>
<span data-ttu-id="185d5-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="185d5-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1420

{
  "@odata.type": "#microsoft.graph.androidForWorkCustomConfiguration",
  "id": "cca8b2bb-b2bb-cca8-bbb2-a8ccbbb2a8cc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```





