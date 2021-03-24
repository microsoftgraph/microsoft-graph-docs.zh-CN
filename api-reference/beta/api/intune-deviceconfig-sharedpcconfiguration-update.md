---
title: 更新 sharedPCConfiguration
description: 更新 sharedPCConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0ed8402d459a750f120754a5e33a087656de958b
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51137082"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="88e84-103">更新 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="88e84-103">Update sharedPCConfiguration</span></span>

<span data-ttu-id="88e84-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88e84-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="88e84-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="88e84-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="88e84-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88e84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88e84-107">更新 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88e84-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88e84-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88e84-108">Prerequisites</span></span>
<span data-ttu-id="88e84-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88e84-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88e84-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88e84-111">Permission type</span></span>|<span data-ttu-id="88e84-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88e84-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88e84-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88e84-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88e84-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e84-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="88e84-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88e84-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88e84-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88e84-116">Not supported.</span></span>|
|<span data-ttu-id="88e84-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88e84-117">Application</span></span>|<span data-ttu-id="88e84-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="88e84-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="88e84-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88e84-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="88e84-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88e84-120">Request headers</span></span>
|<span data-ttu-id="88e84-121">标头</span><span class="sxs-lookup"><span data-stu-id="88e84-121">Header</span></span>|<span data-ttu-id="88e84-122">值</span><span class="sxs-lookup"><span data-stu-id="88e84-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88e84-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="88e84-123">Authorization</span></span>|<span data-ttu-id="88e84-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88e84-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88e84-125">接受</span><span class="sxs-lookup"><span data-stu-id="88e84-125">Accept</span></span>|<span data-ttu-id="88e84-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88e84-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88e84-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88e84-127">Request body</span></span>
<span data-ttu-id="88e84-128">在请求正文中，提供 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88e84-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="88e84-129">下表显示创建 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88e84-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="88e84-130">属性</span><span class="sxs-lookup"><span data-stu-id="88e84-130">Property</span></span>|<span data-ttu-id="88e84-131">类型</span><span class="sxs-lookup"><span data-stu-id="88e84-131">Type</span></span>|<span data-ttu-id="88e84-132">说明</span><span class="sxs-lookup"><span data-stu-id="88e84-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88e84-133">id</span><span class="sxs-lookup"><span data-stu-id="88e84-133">id</span></span>|<span data-ttu-id="88e84-134">String</span><span class="sxs-lookup"><span data-stu-id="88e84-134">String</span></span>|<span data-ttu-id="88e84-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="88e84-135">Key of the entity.</span></span> <span data-ttu-id="88e84-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="88e84-137">lastModifiedDateTime</span></span>|<span data-ttu-id="88e84-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88e84-138">DateTimeOffset</span></span>|<span data-ttu-id="88e84-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88e84-139">DateTime the object was last modified.</span></span> <span data-ttu-id="88e84-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="88e84-141">roleScopeTagIds</span></span>|<span data-ttu-id="88e84-142">String collection</span><span class="sxs-lookup"><span data-stu-id="88e84-142">String collection</span></span>|<span data-ttu-id="88e84-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="88e84-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="88e84-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="88e84-145">supportsScopeTags</span></span>|<span data-ttu-id="88e84-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="88e84-146">Boolean</span></span>|<span data-ttu-id="88e84-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="88e84-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="88e84-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="88e84-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="88e84-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="88e84-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="88e84-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="88e84-150">This property is read-only.</span></span> <span data-ttu-id="88e84-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88e84-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="88e84-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="88e84-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="88e84-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="88e84-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="88e84-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88e84-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="88e84-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="88e84-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="88e84-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="88e84-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="88e84-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88e84-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="88e84-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="88e84-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="88e84-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="88e84-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="88e84-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="88e84-164">createdDateTime</span></span>|<span data-ttu-id="88e84-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="88e84-165">DateTimeOffset</span></span>|<span data-ttu-id="88e84-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="88e84-166">DateTime the object was created.</span></span> <span data-ttu-id="88e84-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-168">说明</span><span class="sxs-lookup"><span data-stu-id="88e84-168">description</span></span>|<span data-ttu-id="88e84-169">String</span><span class="sxs-lookup"><span data-stu-id="88e84-169">String</span></span>|<span data-ttu-id="88e84-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="88e84-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="88e84-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-172">displayName</span><span class="sxs-lookup"><span data-stu-id="88e84-172">displayName</span></span>|<span data-ttu-id="88e84-173">String</span><span class="sxs-lookup"><span data-stu-id="88e84-173">String</span></span>|<span data-ttu-id="88e84-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="88e84-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="88e84-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-176">version</span><span class="sxs-lookup"><span data-stu-id="88e84-176">version</span></span>|<span data-ttu-id="88e84-177">Int32</span><span class="sxs-lookup"><span data-stu-id="88e84-177">Int32</span></span>|<span data-ttu-id="88e84-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="88e84-178">Version of the device configuration.</span></span> <span data-ttu-id="88e84-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="88e84-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="88e84-180">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="88e84-180">accountManagerPolicy</span></span>|[<span data-ttu-id="88e84-181">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="88e84-181">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="88e84-182">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="88e84-182">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="88e84-183">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="88e84-183">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="88e84-184">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="88e84-184">allowedAccounts</span></span>|[<span data-ttu-id="88e84-185">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="88e84-185">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="88e84-186">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="88e84-186">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="88e84-187">可取值为：`notConfigured`、`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="88e84-187">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="88e84-188">localStorage</span><span class="sxs-lookup"><span data-stu-id="88e84-188">localStorage</span></span>|[<span data-ttu-id="88e84-189">enablement</span><span class="sxs-lookup"><span data-stu-id="88e84-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="88e84-190">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="88e84-190">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="88e84-191">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="88e84-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="88e84-192">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="88e84-192">allowLocalStorage</span></span>|<span data-ttu-id="88e84-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="88e84-193">Boolean</span></span>|<span data-ttu-id="88e84-194">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="88e84-194">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="88e84-195">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="88e84-195">setAccountManager</span></span>|[<span data-ttu-id="88e84-196">enablement</span><span class="sxs-lookup"><span data-stu-id="88e84-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="88e84-197">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="88e84-197">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="88e84-198">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="88e84-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="88e84-199">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="88e84-199">disableAccountManager</span></span>|<span data-ttu-id="88e84-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="88e84-200">Boolean</span></span>|<span data-ttu-id="88e84-201">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="88e84-201">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="88e84-202">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="88e84-202">setEduPolicies</span></span>|[<span data-ttu-id="88e84-203">enablement</span><span class="sxs-lookup"><span data-stu-id="88e84-203">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="88e84-204">指定是否应该启用/禁用/不配置默认共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="88e84-204">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="88e84-205">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="88e84-205">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="88e84-206">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="88e84-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="88e84-207">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="88e84-207">disableEduPolicies</span></span>|<span data-ttu-id="88e84-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="88e84-208">Boolean</span></span>|<span data-ttu-id="88e84-209">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="88e84-209">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="88e84-210">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="88e84-210">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="88e84-211">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="88e84-211">setPowerPolicies</span></span>|[<span data-ttu-id="88e84-212">enablement</span><span class="sxs-lookup"><span data-stu-id="88e84-212">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="88e84-213">指定是否应该启用/禁用默认共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="88e84-213">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="88e84-214">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="88e84-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="88e84-215">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="88e84-215">disablePowerPolicies</span></span>|<span data-ttu-id="88e84-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="88e84-216">Boolean</span></span>|<span data-ttu-id="88e84-217">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="88e84-217">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="88e84-218">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="88e84-218">signInOnResume</span></span>|[<span data-ttu-id="88e84-219">enablement</span><span class="sxs-lookup"><span data-stu-id="88e84-219">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="88e84-220">指定设备从睡眠模式唤醒时登录的要求。</span><span class="sxs-lookup"><span data-stu-id="88e84-220">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="88e84-221">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="88e84-221">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="88e84-222">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="88e84-222">disableSignInOnResume</span></span>|<span data-ttu-id="88e84-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="88e84-223">Boolean</span></span>|<span data-ttu-id="88e84-224">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="88e84-224">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="88e84-225">enabled</span><span class="sxs-lookup"><span data-stu-id="88e84-225">enabled</span></span>|<span data-ttu-id="88e84-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="88e84-226">Boolean</span></span>|<span data-ttu-id="88e84-227">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="88e84-227">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="88e84-228">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="88e84-228">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="88e84-229">Int32</span><span class="sxs-lookup"><span data-stu-id="88e84-229">Int32</span></span>|<span data-ttu-id="88e84-230">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="88e84-230">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="88e84-231">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="88e84-231">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="88e84-232">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="88e84-232">kioskAppDisplayName</span></span>|<span data-ttu-id="88e84-233">String</span><span class="sxs-lookup"><span data-stu-id="88e84-233">String</span></span>|<span data-ttu-id="88e84-234">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="88e84-234">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="88e84-235">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="88e84-235">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="88e84-236">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="88e84-236">kioskAppUserModelId</span></span>|<span data-ttu-id="88e84-237">String</span><span class="sxs-lookup"><span data-stu-id="88e84-237">String</span></span>|<span data-ttu-id="88e84-238">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="88e84-238">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="88e84-239">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="88e84-239">maintenanceStartTime</span></span>|<span data-ttu-id="88e84-240">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="88e84-240">TimeOfDay</span></span>|<span data-ttu-id="88e84-241">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="88e84-241">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="88e84-242">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="88e84-242">fastFirstSignIn</span></span>|[<span data-ttu-id="88e84-243">enablement</span><span class="sxs-lookup"><span data-stu-id="88e84-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="88e84-244">指定是否自动将新的非管理员 Azure AD 帐户连接到预配置的候选本地帐户。</span><span class="sxs-lookup"><span data-stu-id="88e84-244">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="88e84-245">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="88e84-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="88e84-246">响应</span><span class="sxs-lookup"><span data-stu-id="88e84-246">Response</span></span>
<span data-ttu-id="88e84-247">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="88e84-247">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88e84-248">示例</span><span class="sxs-lookup"><span data-stu-id="88e84-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="88e84-249">请求</span><span class="sxs-lookup"><span data-stu-id="88e84-249">Request</span></span>
<span data-ttu-id="88e84-250">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88e84-250">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1920

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
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
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "guest",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```

### <a name="response"></a><span data-ttu-id="88e84-251">响应</span><span class="sxs-lookup"><span data-stu-id="88e84-251">Response</span></span>
<span data-ttu-id="88e84-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88e84-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2092

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
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
  "accountManagerPolicy": {
    "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy",
    "accountDeletionPolicy": "diskSpaceThreshold",
    "cacheAccountsAboveDiskFreePercentage": 4,
    "inactiveThresholdDays": 5,
    "removeAccountsBelowDiskFreePercentage": 5
  },
  "allowedAccounts": "guest",
  "localStorage": "enabled",
  "allowLocalStorage": true,
  "setAccountManager": "enabled",
  "disableAccountManager": true,
  "setEduPolicies": "enabled",
  "disableEduPolicies": true,
  "setPowerPolicies": "enabled",
  "disablePowerPolicies": true,
  "signInOnResume": "enabled",
  "disableSignInOnResume": true,
  "enabled": true,
  "idleTimeBeforeSleepInSeconds": 12,
  "kioskAppDisplayName": "Kiosk App Display Name value",
  "kioskAppUserModelId": "Kiosk App User Model Id value",
  "maintenanceStartTime": "11:59:24.7240000",
  "fastFirstSignIn": "enabled"
}
```




