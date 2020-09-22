---
title: 更新 androidWorkProfileCustomConfiguration
description: 更新 androidWorkProfileCustomConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8910af93e9431768935ee3a5505f1d62707a854a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48059031"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="b1efa-103">更新 androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="b1efa-103">Update androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="b1efa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1efa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1efa-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1efa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1efa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1efa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1efa-107">更新 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b1efa-107">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b1efa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b1efa-108">Prerequisites</span></span>
<span data-ttu-id="b1efa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1efa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1efa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1efa-111">Permission type</span></span>|<span data-ttu-id="b1efa-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b1efa-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1efa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1efa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b1efa-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1efa-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b1efa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1efa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1efa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1efa-116">Not supported.</span></span>|
|<span data-ttu-id="b1efa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1efa-117">Application</span></span>|<span data-ttu-id="b1efa-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1efa-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b1efa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1efa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b1efa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1efa-120">Request headers</span></span>
|<span data-ttu-id="b1efa-121">标头</span><span class="sxs-lookup"><span data-stu-id="b1efa-121">Header</span></span>|<span data-ttu-id="b1efa-122">值</span><span class="sxs-lookup"><span data-stu-id="b1efa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b1efa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1efa-123">Authorization</span></span>|<span data-ttu-id="b1efa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b1efa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b1efa-125">接受</span><span class="sxs-lookup"><span data-stu-id="b1efa-125">Accept</span></span>|<span data-ttu-id="b1efa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b1efa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1efa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1efa-127">Request body</span></span>
<span data-ttu-id="b1efa-128">在请求正文中，提供 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1efa-128">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="b1efa-129">下表显示创建 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b1efa-129">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="b1efa-130">属性</span><span class="sxs-lookup"><span data-stu-id="b1efa-130">Property</span></span>|<span data-ttu-id="b1efa-131">类型</span><span class="sxs-lookup"><span data-stu-id="b1efa-131">Type</span></span>|<span data-ttu-id="b1efa-132">说明</span><span class="sxs-lookup"><span data-stu-id="b1efa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1efa-133">id</span><span class="sxs-lookup"><span data-stu-id="b1efa-133">id</span></span>|<span data-ttu-id="b1efa-134">String</span><span class="sxs-lookup"><span data-stu-id="b1efa-134">String</span></span>|<span data-ttu-id="b1efa-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b1efa-135">Key of the entity.</span></span> <span data-ttu-id="b1efa-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b1efa-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b1efa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1efa-138">DateTimeOffset</span></span>|<span data-ttu-id="b1efa-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b1efa-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b1efa-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b1efa-141">roleScopeTagIds</span></span>|<span data-ttu-id="b1efa-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b1efa-142">String collection</span></span>|<span data-ttu-id="b1efa-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b1efa-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b1efa-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b1efa-145">supportsScopeTags</span></span>|<span data-ttu-id="b1efa-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b1efa-146">Boolean</span></span>|<span data-ttu-id="b1efa-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b1efa-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b1efa-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b1efa-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b1efa-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b1efa-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b1efa-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b1efa-150">This property is read-only.</span></span> <span data-ttu-id="b1efa-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1efa-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b1efa-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b1efa-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b1efa-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b1efa-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b1efa-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1efa-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b1efa-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b1efa-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b1efa-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b1efa-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b1efa-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1efa-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b1efa-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b1efa-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b1efa-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b1efa-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b1efa-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b1efa-164">createdDateTime</span></span>|<span data-ttu-id="b1efa-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b1efa-165">DateTimeOffset</span></span>|<span data-ttu-id="b1efa-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b1efa-166">DateTime the object was created.</span></span> <span data-ttu-id="b1efa-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-168">说明</span><span class="sxs-lookup"><span data-stu-id="b1efa-168">description</span></span>|<span data-ttu-id="b1efa-169">String</span><span class="sxs-lookup"><span data-stu-id="b1efa-169">String</span></span>|<span data-ttu-id="b1efa-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b1efa-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b1efa-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-172">displayName</span><span class="sxs-lookup"><span data-stu-id="b1efa-172">displayName</span></span>|<span data-ttu-id="b1efa-173">String</span><span class="sxs-lookup"><span data-stu-id="b1efa-173">String</span></span>|<span data-ttu-id="b1efa-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b1efa-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b1efa-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-176">version</span><span class="sxs-lookup"><span data-stu-id="b1efa-176">version</span></span>|<span data-ttu-id="b1efa-177">Int32</span><span class="sxs-lookup"><span data-stu-id="b1efa-177">Int32</span></span>|<span data-ttu-id="b1efa-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b1efa-178">Version of the device configuration.</span></span> <span data-ttu-id="b1efa-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b1efa-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b1efa-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="b1efa-180">omaSettings</span></span>|<span data-ttu-id="b1efa-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1efa-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="b1efa-182">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="b1efa-182">OMA settings.</span></span> <span data-ttu-id="b1efa-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="b1efa-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b1efa-184">响应</span><span class="sxs-lookup"><span data-stu-id="b1efa-184">Response</span></span>
<span data-ttu-id="b1efa-185">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1efa-185">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b1efa-186">示例</span><span class="sxs-lookup"><span data-stu-id="b1efa-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1efa-187">请求</span><span class="sxs-lookup"><span data-stu-id="b1efa-187">Request</span></span>
<span data-ttu-id="b1efa-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b1efa-188">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1252

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="b1efa-189">响应</span><span class="sxs-lookup"><span data-stu-id="b1efa-189">Response</span></span>
<span data-ttu-id="b1efa-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b1efa-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1424

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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






