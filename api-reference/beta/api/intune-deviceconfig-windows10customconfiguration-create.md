---
title: 创建 windows10CustomConfiguration
description: 创建新的 windows10CustomConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fa4053c4816ae1e45442024d0879a6ee5c14b9e9
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48692014"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="1dfac-103">创建 windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="1dfac-103">Create windows10CustomConfiguration</span></span>

<span data-ttu-id="1dfac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1dfac-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1dfac-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1dfac-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1dfac-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1dfac-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1dfac-107">创建新的 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dfac-107">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1dfac-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1dfac-108">Prerequisites</span></span>
<span data-ttu-id="1dfac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1dfac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1dfac-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1dfac-111">Permission type</span></span>|<span data-ttu-id="1dfac-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1dfac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1dfac-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1dfac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1dfac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dfac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1dfac-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1dfac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1dfac-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1dfac-116">Not supported.</span></span>|
|<span data-ttu-id="1dfac-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1dfac-117">Application</span></span>|<span data-ttu-id="1dfac-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1dfac-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1dfac-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1dfac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1dfac-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1dfac-120">Request headers</span></span>
|<span data-ttu-id="1dfac-121">标头</span><span class="sxs-lookup"><span data-stu-id="1dfac-121">Header</span></span>|<span data-ttu-id="1dfac-122">值</span><span class="sxs-lookup"><span data-stu-id="1dfac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1dfac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1dfac-123">Authorization</span></span>|<span data-ttu-id="1dfac-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1dfac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1dfac-125">接受</span><span class="sxs-lookup"><span data-stu-id="1dfac-125">Accept</span></span>|<span data-ttu-id="1dfac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1dfac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1dfac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1dfac-127">Request body</span></span>
<span data-ttu-id="1dfac-128">在请求正文中，提供 windows10CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1dfac-128">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="1dfac-129">下表显示了创建 windows10CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1dfac-129">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="1dfac-130">属性</span><span class="sxs-lookup"><span data-stu-id="1dfac-130">Property</span></span>|<span data-ttu-id="1dfac-131">类型</span><span class="sxs-lookup"><span data-stu-id="1dfac-131">Type</span></span>|<span data-ttu-id="1dfac-132">说明</span><span class="sxs-lookup"><span data-stu-id="1dfac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1dfac-133">id</span><span class="sxs-lookup"><span data-stu-id="1dfac-133">id</span></span>|<span data-ttu-id="1dfac-134">String</span><span class="sxs-lookup"><span data-stu-id="1dfac-134">String</span></span>|<span data-ttu-id="1dfac-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1dfac-135">Key of the entity.</span></span> <span data-ttu-id="1dfac-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1dfac-137">lastModifiedDateTime</span></span>|<span data-ttu-id="1dfac-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dfac-138">DateTimeOffset</span></span>|<span data-ttu-id="1dfac-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1dfac-139">DateTime the object was last modified.</span></span> <span data-ttu-id="1dfac-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="1dfac-141">roleScopeTagIds</span></span>|<span data-ttu-id="1dfac-142">String collection</span><span class="sxs-lookup"><span data-stu-id="1dfac-142">String collection</span></span>|<span data-ttu-id="1dfac-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="1dfac-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="1dfac-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="1dfac-145">supportsScopeTags</span></span>|<span data-ttu-id="1dfac-146">布尔</span><span class="sxs-lookup"><span data-stu-id="1dfac-146">Boolean</span></span>|<span data-ttu-id="1dfac-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="1dfac-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="1dfac-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="1dfac-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="1dfac-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="1dfac-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="1dfac-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="1dfac-150">This property is read-only.</span></span> <span data-ttu-id="1dfac-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1dfac-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="1dfac-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="1dfac-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="1dfac-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="1dfac-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="1dfac-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1dfac-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="1dfac-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="1dfac-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="1dfac-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1dfac-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="1dfac-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1dfac-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="1dfac-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="1dfac-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="1dfac-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="1dfac-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="1dfac-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1dfac-164">createdDateTime</span></span>|<span data-ttu-id="1dfac-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1dfac-165">DateTimeOffset</span></span>|<span data-ttu-id="1dfac-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="1dfac-166">DateTime the object was created.</span></span> <span data-ttu-id="1dfac-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-168">说明</span><span class="sxs-lookup"><span data-stu-id="1dfac-168">description</span></span>|<span data-ttu-id="1dfac-169">String</span><span class="sxs-lookup"><span data-stu-id="1dfac-169">String</span></span>|<span data-ttu-id="1dfac-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="1dfac-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1dfac-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-172">displayName</span><span class="sxs-lookup"><span data-stu-id="1dfac-172">displayName</span></span>|<span data-ttu-id="1dfac-173">String</span><span class="sxs-lookup"><span data-stu-id="1dfac-173">String</span></span>|<span data-ttu-id="1dfac-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="1dfac-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1dfac-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-176">version</span><span class="sxs-lookup"><span data-stu-id="1dfac-176">version</span></span>|<span data-ttu-id="1dfac-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1dfac-177">Int32</span></span>|<span data-ttu-id="1dfac-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="1dfac-178">Version of the device configuration.</span></span> <span data-ttu-id="1dfac-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1dfac-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1dfac-180">omaSettings</span><span class="sxs-lookup"><span data-stu-id="1dfac-180">omaSettings</span></span>|<span data-ttu-id="1dfac-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1dfac-181">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="1dfac-182">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="1dfac-182">OMA settings.</span></span> <span data-ttu-id="1dfac-183">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="1dfac-183">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="1dfac-184">响应</span><span class="sxs-lookup"><span data-stu-id="1dfac-184">Response</span></span>
<span data-ttu-id="1dfac-185">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1dfac-185">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1dfac-186">示例</span><span class="sxs-lookup"><span data-stu-id="1dfac-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="1dfac-187">请求</span><span class="sxs-lookup"><span data-stu-id="1dfac-187">Request</span></span>
<span data-ttu-id="1dfac-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1dfac-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1243

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="1dfac-189">响应</span><span class="sxs-lookup"><span data-stu-id="1dfac-189">Response</span></span>
<span data-ttu-id="1dfac-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1dfac-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1415

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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





