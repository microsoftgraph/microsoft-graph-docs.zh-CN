---
title: 更新 androidWorkProfileCustomConfiguration
description: 更新 androidWorkProfileCustomConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b7cc14b90daa0b3ea2aa8d220c2859567822bbb3
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178869"
---
# <a name="update-androidworkprofilecustomconfiguration"></a><span data-ttu-id="472e2-103">更新 androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="472e2-103">Update androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="472e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="472e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="472e2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="472e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="472e2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="472e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="472e2-107">更新[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="472e2-107">Update the properties of a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="472e2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="472e2-108">Prerequisites</span></span>
<span data-ttu-id="472e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="472e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="472e2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="472e2-111">Permission type</span></span>|<span data-ttu-id="472e2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="472e2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="472e2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="472e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="472e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="472e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="472e2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="472e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="472e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="472e2-116">Not supported.</span></span>|
|<span data-ttu-id="472e2-117">Application</span><span class="sxs-lookup"><span data-stu-id="472e2-117">Application</span></span>|<span data-ttu-id="472e2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="472e2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="472e2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="472e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="472e2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="472e2-120">Request headers</span></span>
|<span data-ttu-id="472e2-121">标头</span><span class="sxs-lookup"><span data-stu-id="472e2-121">Header</span></span>|<span data-ttu-id="472e2-122">值</span><span class="sxs-lookup"><span data-stu-id="472e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="472e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="472e2-123">Authorization</span></span>|<span data-ttu-id="472e2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="472e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="472e2-125">接受</span><span class="sxs-lookup"><span data-stu-id="472e2-125">Accept</span></span>|<span data-ttu-id="472e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="472e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="472e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="472e2-127">Request body</span></span>
<span data-ttu-id="472e2-128">在请求正文中，提供[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="472e2-128">In the request body, supply a JSON representation for the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

<span data-ttu-id="472e2-129">下表显示创建[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="472e2-129">The following table shows the properties that are required when you create the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md).</span></span>

|<span data-ttu-id="472e2-130">属性</span><span class="sxs-lookup"><span data-stu-id="472e2-130">Property</span></span>|<span data-ttu-id="472e2-131">类型</span><span class="sxs-lookup"><span data-stu-id="472e2-131">Type</span></span>|<span data-ttu-id="472e2-132">说明</span><span class="sxs-lookup"><span data-stu-id="472e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="472e2-133">id</span><span class="sxs-lookup"><span data-stu-id="472e2-133">id</span></span>|<span data-ttu-id="472e2-134">字符串</span><span class="sxs-lookup"><span data-stu-id="472e2-134">String</span></span>|<span data-ttu-id="472e2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="472e2-135">Key of the entity.</span></span> <span data-ttu-id="472e2-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="472e2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="472e2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="472e2-138">DateTimeOffset</span></span>|<span data-ttu-id="472e2-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="472e2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="472e2-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="472e2-141">roleScopeTagIds</span></span>|<span data-ttu-id="472e2-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="472e2-142">String collection</span></span>|<span data-ttu-id="472e2-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="472e2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="472e2-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="472e2-145">supportsScopeTags</span></span>|<span data-ttu-id="472e2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="472e2-146">Boolean</span></span>|<span data-ttu-id="472e2-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="472e2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="472e2-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="472e2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="472e2-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="472e2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="472e2-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="472e2-150">This property is read-only.</span></span> <span data-ttu-id="472e2-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="472e2-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="472e2-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="472e2-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="472e2-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="472e2-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="472e2-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="472e2-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="472e2-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="472e2-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="472e2-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="472e2-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="472e2-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="472e2-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="472e2-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="472e2-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="472e2-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="472e2-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="472e2-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="472e2-164">createdDateTime</span></span>|<span data-ttu-id="472e2-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="472e2-165">DateTimeOffset</span></span>|<span data-ttu-id="472e2-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="472e2-166">DateTime the object was created.</span></span> <span data-ttu-id="472e2-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-168">说明</span><span class="sxs-lookup"><span data-stu-id="472e2-168">description</span></span>|<span data-ttu-id="472e2-169">String</span><span class="sxs-lookup"><span data-stu-id="472e2-169">String</span></span>|<span data-ttu-id="472e2-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="472e2-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="472e2-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-172">displayName</span><span class="sxs-lookup"><span data-stu-id="472e2-172">displayName</span></span>|<span data-ttu-id="472e2-173">String</span><span class="sxs-lookup"><span data-stu-id="472e2-173">String</span></span>|<span data-ttu-id="472e2-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="472e2-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="472e2-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-176">version</span><span class="sxs-lookup"><span data-stu-id="472e2-176">version</span></span>|<span data-ttu-id="472e2-177">Int32</span><span class="sxs-lookup"><span data-stu-id="472e2-177">Int32</span></span>|<span data-ttu-id="472e2-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="472e2-178">Version of the device configuration.</span></span> <span data-ttu-id="472e2-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="472e2-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="472e2-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="472e2-180">omaSettings</span></span>|<span data-ttu-id="472e2-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="472e2-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="472e2-182">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="472e2-182">OMA settings.</span></span> <span data-ttu-id="472e2-183">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="472e2-183">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="472e2-184">响应</span><span class="sxs-lookup"><span data-stu-id="472e2-184">Response</span></span>
<span data-ttu-id="472e2-185">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="472e2-185">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="472e2-186">示例</span><span class="sxs-lookup"><span data-stu-id="472e2-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="472e2-187">请求</span><span class="sxs-lookup"><span data-stu-id="472e2-187">Request</span></span>
<span data-ttu-id="472e2-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="472e2-188">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="472e2-189">响应</span><span class="sxs-lookup"><span data-stu-id="472e2-189">Response</span></span>
<span data-ttu-id="472e2-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="472e2-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



