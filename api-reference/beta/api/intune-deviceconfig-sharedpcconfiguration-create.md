---
title: 创建 sharedPCConfiguration
description: 创建新的 sharedPCConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 98e8ba6a548a074c6a682f57a18df693ea9849ff
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36314852"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="a241a-103">创建 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="a241a-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="a241a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a241a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a241a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a241a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a241a-106">创建新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a241a-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a241a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a241a-107">Prerequisites</span></span>
<span data-ttu-id="a241a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a241a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a241a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a241a-110">Permission type</span></span>|<span data-ttu-id="a241a-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a241a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a241a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a241a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a241a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a241a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a241a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a241a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a241a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a241a-115">Not supported.</span></span>|
|<span data-ttu-id="a241a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a241a-116">Application</span></span>|<span data-ttu-id="a241a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a241a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a241a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a241a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a241a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a241a-119">Request headers</span></span>
|<span data-ttu-id="a241a-120">标头</span><span class="sxs-lookup"><span data-stu-id="a241a-120">Header</span></span>|<span data-ttu-id="a241a-121">值</span><span class="sxs-lookup"><span data-stu-id="a241a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a241a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a241a-122">Authorization</span></span>|<span data-ttu-id="a241a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a241a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a241a-124">接受</span><span class="sxs-lookup"><span data-stu-id="a241a-124">Accept</span></span>|<span data-ttu-id="a241a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a241a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a241a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a241a-126">Request body</span></span>
<span data-ttu-id="a241a-127">在请求正文中，提供 sharedPCConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a241a-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="a241a-128">下表显示创建 sharedPCConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a241a-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="a241a-129">属性</span><span class="sxs-lookup"><span data-stu-id="a241a-129">Property</span></span>|<span data-ttu-id="a241a-130">类型</span><span class="sxs-lookup"><span data-stu-id="a241a-130">Type</span></span>|<span data-ttu-id="a241a-131">说明</span><span class="sxs-lookup"><span data-stu-id="a241a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a241a-132">id</span><span class="sxs-lookup"><span data-stu-id="a241a-132">id</span></span>|<span data-ttu-id="a241a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a241a-133">String</span></span>|<span data-ttu-id="a241a-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a241a-134">Key of the entity.</span></span> <span data-ttu-id="a241a-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a241a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a241a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a241a-137">DateTimeOffset</span></span>|<span data-ttu-id="a241a-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a241a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a241a-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a241a-140">roleScopeTagIds</span></span>|<span data-ttu-id="a241a-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a241a-141">String collection</span></span>|<span data-ttu-id="a241a-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a241a-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a241a-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a241a-144">supportsScopeTags</span></span>|<span data-ttu-id="a241a-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="a241a-145">Boolean</span></span>|<span data-ttu-id="a241a-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a241a-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a241a-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a241a-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a241a-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a241a-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a241a-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a241a-149">This property is read-only.</span></span> <span data-ttu-id="a241a-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a241a-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="a241a-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="a241a-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="a241a-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="a241a-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="a241a-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a241a-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="a241a-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="a241a-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="a241a-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a241a-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="a241a-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a241a-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="a241a-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="a241a-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="a241a-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="a241a-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="a241a-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a241a-163">createdDateTime</span></span>|<span data-ttu-id="a241a-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a241a-164">DateTimeOffset</span></span>|<span data-ttu-id="a241a-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a241a-165">DateTime the object was created.</span></span> <span data-ttu-id="a241a-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-167">说明</span><span class="sxs-lookup"><span data-stu-id="a241a-167">description</span></span>|<span data-ttu-id="a241a-168">String</span><span class="sxs-lookup"><span data-stu-id="a241a-168">String</span></span>|<span data-ttu-id="a241a-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a241a-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a241a-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-171">displayName</span><span class="sxs-lookup"><span data-stu-id="a241a-171">displayName</span></span>|<span data-ttu-id="a241a-172">String</span><span class="sxs-lookup"><span data-stu-id="a241a-172">String</span></span>|<span data-ttu-id="a241a-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a241a-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a241a-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-175">version</span><span class="sxs-lookup"><span data-stu-id="a241a-175">version</span></span>|<span data-ttu-id="a241a-176">Int32</span><span class="sxs-lookup"><span data-stu-id="a241a-176">Int32</span></span>|<span data-ttu-id="a241a-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a241a-177">Version of the device configuration.</span></span> <span data-ttu-id="a241a-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a241a-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a241a-179">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a241a-179">accountManagerPolicy</span></span>|[<span data-ttu-id="a241a-180">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="a241a-180">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="a241a-181">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="a241a-181">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="a241a-182">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="a241a-182">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="a241a-183">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="a241a-183">allowedAccounts</span></span>|[<span data-ttu-id="a241a-184">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="a241a-184">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="a241a-185">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="a241a-185">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="a241a-186">可取值为：`notConfigured`、`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="a241a-186">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="a241a-187">localStorage</span><span class="sxs-lookup"><span data-stu-id="a241a-187">localStorage</span></span>|[<span data-ttu-id="a241a-188">启用</span><span class="sxs-lookup"><span data-stu-id="a241a-188">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a241a-189">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="a241a-189">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="a241a-190">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a241a-190">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a241a-191">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="a241a-191">allowLocalStorage</span></span>|<span data-ttu-id="a241a-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="a241a-192">Boolean</span></span>|<span data-ttu-id="a241a-193">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="a241a-193">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="a241a-194">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="a241a-194">setAccountManager</span></span>|[<span data-ttu-id="a241a-195">启用</span><span class="sxs-lookup"><span data-stu-id="a241a-195">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a241a-196">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="a241a-196">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="a241a-197">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a241a-197">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a241a-198">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="a241a-198">disableAccountManager</span></span>|<span data-ttu-id="a241a-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="a241a-199">Boolean</span></span>|<span data-ttu-id="a241a-200">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="a241a-200">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="a241a-201">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="a241a-201">setEduPolicies</span></span>|[<span data-ttu-id="a241a-202">启用</span><span class="sxs-lookup"><span data-stu-id="a241a-202">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a241a-203">指定是否应启用/禁用/禁用/禁用默认共享 PC 教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="a241a-203">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="a241a-204">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="a241a-204">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="a241a-205">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a241a-205">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a241a-206">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="a241a-206">disableEduPolicies</span></span>|<span data-ttu-id="a241a-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="a241a-207">Boolean</span></span>|<span data-ttu-id="a241a-208">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="a241a-208">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="a241a-209">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="a241a-209">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="a241a-210">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="a241a-210">setPowerPolicies</span></span>|[<span data-ttu-id="a241a-211">启用</span><span class="sxs-lookup"><span data-stu-id="a241a-211">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a241a-212">指定是否应启用/禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="a241a-212">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="a241a-213">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a241a-213">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a241a-214">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="a241a-214">disablePowerPolicies</span></span>|<span data-ttu-id="a241a-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="a241a-215">Boolean</span></span>|<span data-ttu-id="a241a-216">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="a241a-216">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="a241a-217">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="a241a-217">signInOnResume</span></span>|[<span data-ttu-id="a241a-218">启用</span><span class="sxs-lookup"><span data-stu-id="a241a-218">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a241a-219">指定当设备从睡眠模式唤醒时登录时的要求。</span><span class="sxs-lookup"><span data-stu-id="a241a-219">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="a241a-220">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a241a-220">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="a241a-221">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="a241a-221">disableSignInOnResume</span></span>|<span data-ttu-id="a241a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="a241a-222">Boolean</span></span>|<span data-ttu-id="a241a-223">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="a241a-223">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="a241a-224">enabled</span><span class="sxs-lookup"><span data-stu-id="a241a-224">enabled</span></span>|<span data-ttu-id="a241a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="a241a-225">Boolean</span></span>|<span data-ttu-id="a241a-226">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="a241a-226">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="a241a-227">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="a241a-227">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="a241a-228">Int32</span><span class="sxs-lookup"><span data-stu-id="a241a-228">Int32</span></span>|<span data-ttu-id="a241a-229">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="a241a-229">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="a241a-230">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="a241a-230">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="a241a-231">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="a241a-231">kioskAppDisplayName</span></span>|<span data-ttu-id="a241a-232">String</span><span class="sxs-lookup"><span data-stu-id="a241a-232">String</span></span>|<span data-ttu-id="a241a-233">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="a241a-233">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="a241a-234">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="a241a-234">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="a241a-235">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="a241a-235">kioskAppUserModelId</span></span>|<span data-ttu-id="a241a-236">String</span><span class="sxs-lookup"><span data-stu-id="a241a-236">String</span></span>|<span data-ttu-id="a241a-237">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="a241a-237">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="a241a-238">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="a241a-238">maintenanceStartTime</span></span>|<span data-ttu-id="a241a-239">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a241a-239">TimeOfDay</span></span>|<span data-ttu-id="a241a-240">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="a241a-240">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="a241a-241">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="a241a-241">fastFirstSignIn</span></span>|[<span data-ttu-id="a241a-242">启用</span><span class="sxs-lookup"><span data-stu-id="a241a-242">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="a241a-243">指定是否将新的非管理员 Azure AD 帐户自动连接到预配置的候选本地帐户。</span><span class="sxs-lookup"><span data-stu-id="a241a-243">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="a241a-244">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="a241a-244">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="a241a-245">响应</span><span class="sxs-lookup"><span data-stu-id="a241a-245">Response</span></span>
<span data-ttu-id="a241a-246">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a241a-246">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a241a-247">示例</span><span class="sxs-lookup"><span data-stu-id="a241a-247">Example</span></span>

### <a name="request"></a><span data-ttu-id="a241a-248">请求</span><span class="sxs-lookup"><span data-stu-id="a241a-248">Request</span></span>
<span data-ttu-id="a241a-249">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a241a-249">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="a241a-250">响应</span><span class="sxs-lookup"><span data-stu-id="a241a-250">Response</span></span>
<span data-ttu-id="a241a-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a241a-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






