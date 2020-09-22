---
title: 创建 sharedPCConfiguration
description: 创建新的 sharedPCConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 15fc74514587190f2ead79bd2b5af6546ac2047e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48028033"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="897ae-103">创建 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="897ae-103">Create sharedPCConfiguration</span></span>

<span data-ttu-id="897ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="897ae-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="897ae-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="897ae-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="897ae-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="897ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="897ae-107">创建新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="897ae-107">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="897ae-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="897ae-108">Prerequisites</span></span>
<span data-ttu-id="897ae-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="897ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="897ae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="897ae-111">Permission type</span></span>|<span data-ttu-id="897ae-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="897ae-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="897ae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="897ae-113">Delegated (work or school account)</span></span>|<span data-ttu-id="897ae-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="897ae-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="897ae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="897ae-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="897ae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="897ae-116">Not supported.</span></span>|
|<span data-ttu-id="897ae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="897ae-117">Application</span></span>|<span data-ttu-id="897ae-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="897ae-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="897ae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="897ae-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="897ae-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="897ae-120">Request headers</span></span>
|<span data-ttu-id="897ae-121">标头</span><span class="sxs-lookup"><span data-stu-id="897ae-121">Header</span></span>|<span data-ttu-id="897ae-122">值</span><span class="sxs-lookup"><span data-stu-id="897ae-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="897ae-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="897ae-123">Authorization</span></span>|<span data-ttu-id="897ae-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="897ae-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="897ae-125">接受</span><span class="sxs-lookup"><span data-stu-id="897ae-125">Accept</span></span>|<span data-ttu-id="897ae-126">application/json</span><span class="sxs-lookup"><span data-stu-id="897ae-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="897ae-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="897ae-127">Request body</span></span>
<span data-ttu-id="897ae-128">在请求正文中，提供 sharedPCConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="897ae-128">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="897ae-129">下表显示创建 sharedPCConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="897ae-129">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="897ae-130">属性</span><span class="sxs-lookup"><span data-stu-id="897ae-130">Property</span></span>|<span data-ttu-id="897ae-131">类型</span><span class="sxs-lookup"><span data-stu-id="897ae-131">Type</span></span>|<span data-ttu-id="897ae-132">说明</span><span class="sxs-lookup"><span data-stu-id="897ae-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="897ae-133">id</span><span class="sxs-lookup"><span data-stu-id="897ae-133">id</span></span>|<span data-ttu-id="897ae-134">String</span><span class="sxs-lookup"><span data-stu-id="897ae-134">String</span></span>|<span data-ttu-id="897ae-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="897ae-135">Key of the entity.</span></span> <span data-ttu-id="897ae-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="897ae-137">lastModifiedDateTime</span></span>|<span data-ttu-id="897ae-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="897ae-138">DateTimeOffset</span></span>|<span data-ttu-id="897ae-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="897ae-139">DateTime the object was last modified.</span></span> <span data-ttu-id="897ae-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="897ae-141">roleScopeTagIds</span></span>|<span data-ttu-id="897ae-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="897ae-142">String collection</span></span>|<span data-ttu-id="897ae-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="897ae-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="897ae-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="897ae-145">supportsScopeTags</span></span>|<span data-ttu-id="897ae-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="897ae-146">Boolean</span></span>|<span data-ttu-id="897ae-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="897ae-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="897ae-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="897ae-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="897ae-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="897ae-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="897ae-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="897ae-150">This property is read-only.</span></span> <span data-ttu-id="897ae-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="897ae-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="897ae-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="897ae-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="897ae-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="897ae-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="897ae-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="897ae-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="897ae-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="897ae-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="897ae-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="897ae-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="897ae-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="897ae-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="897ae-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="897ae-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="897ae-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="897ae-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="897ae-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="897ae-164">createdDateTime</span></span>|<span data-ttu-id="897ae-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="897ae-165">DateTimeOffset</span></span>|<span data-ttu-id="897ae-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="897ae-166">DateTime the object was created.</span></span> <span data-ttu-id="897ae-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-168">description</span><span class="sxs-lookup"><span data-stu-id="897ae-168">description</span></span>|<span data-ttu-id="897ae-169">String</span><span class="sxs-lookup"><span data-stu-id="897ae-169">String</span></span>|<span data-ttu-id="897ae-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="897ae-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="897ae-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-172">displayName</span><span class="sxs-lookup"><span data-stu-id="897ae-172">displayName</span></span>|<span data-ttu-id="897ae-173">String</span><span class="sxs-lookup"><span data-stu-id="897ae-173">String</span></span>|<span data-ttu-id="897ae-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="897ae-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="897ae-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-176">version</span><span class="sxs-lookup"><span data-stu-id="897ae-176">version</span></span>|<span data-ttu-id="897ae-177">Int32</span><span class="sxs-lookup"><span data-stu-id="897ae-177">Int32</span></span>|<span data-ttu-id="897ae-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="897ae-178">Version of the device configuration.</span></span> <span data-ttu-id="897ae-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="897ae-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="897ae-180">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="897ae-180">accountManagerPolicy</span></span>|[<span data-ttu-id="897ae-181">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="897ae-181">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="897ae-182">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="897ae-182">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="897ae-183">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="897ae-183">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="897ae-184">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="897ae-184">allowedAccounts</span></span>|[<span data-ttu-id="897ae-185">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="897ae-185">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="897ae-186">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="897ae-186">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="897ae-187">可取值为：`notConfigured`、`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="897ae-187">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="897ae-188">localStorage</span><span class="sxs-lookup"><span data-stu-id="897ae-188">localStorage</span></span>|[<span data-ttu-id="897ae-189">启用</span><span class="sxs-lookup"><span data-stu-id="897ae-189">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="897ae-190">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="897ae-190">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="897ae-191">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="897ae-191">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="897ae-192">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="897ae-192">allowLocalStorage</span></span>|<span data-ttu-id="897ae-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="897ae-193">Boolean</span></span>|<span data-ttu-id="897ae-194">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="897ae-194">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="897ae-195">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="897ae-195">setAccountManager</span></span>|[<span data-ttu-id="897ae-196">启用</span><span class="sxs-lookup"><span data-stu-id="897ae-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="897ae-197">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="897ae-197">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="897ae-198">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="897ae-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="897ae-199">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="897ae-199">disableAccountManager</span></span>|<span data-ttu-id="897ae-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="897ae-200">Boolean</span></span>|<span data-ttu-id="897ae-201">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="897ae-201">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="897ae-202">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="897ae-202">setEduPolicies</span></span>|[<span data-ttu-id="897ae-203">启用</span><span class="sxs-lookup"><span data-stu-id="897ae-203">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="897ae-204">指定是否应启用/禁用/禁用/禁用默认共享 PC 教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="897ae-204">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="897ae-205">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="897ae-205">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="897ae-206">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="897ae-206">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="897ae-207">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="897ae-207">disableEduPolicies</span></span>|<span data-ttu-id="897ae-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="897ae-208">Boolean</span></span>|<span data-ttu-id="897ae-209">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="897ae-209">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="897ae-210">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="897ae-210">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="897ae-211">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="897ae-211">setPowerPolicies</span></span>|[<span data-ttu-id="897ae-212">启用</span><span class="sxs-lookup"><span data-stu-id="897ae-212">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="897ae-213">指定是否应启用/禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="897ae-213">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="897ae-214">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="897ae-214">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="897ae-215">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="897ae-215">disablePowerPolicies</span></span>|<span data-ttu-id="897ae-216">Boolean</span><span class="sxs-lookup"><span data-stu-id="897ae-216">Boolean</span></span>|<span data-ttu-id="897ae-217">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="897ae-217">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="897ae-218">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="897ae-218">signInOnResume</span></span>|[<span data-ttu-id="897ae-219">启用</span><span class="sxs-lookup"><span data-stu-id="897ae-219">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="897ae-220">指定当设备从睡眠模式唤醒时登录时的要求。</span><span class="sxs-lookup"><span data-stu-id="897ae-220">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="897ae-221">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="897ae-221">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="897ae-222">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="897ae-222">disableSignInOnResume</span></span>|<span data-ttu-id="897ae-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="897ae-223">Boolean</span></span>|<span data-ttu-id="897ae-224">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="897ae-224">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="897ae-225">enabled</span><span class="sxs-lookup"><span data-stu-id="897ae-225">enabled</span></span>|<span data-ttu-id="897ae-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="897ae-226">Boolean</span></span>|<span data-ttu-id="897ae-227">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="897ae-227">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="897ae-228">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="897ae-228">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="897ae-229">Int32</span><span class="sxs-lookup"><span data-stu-id="897ae-229">Int32</span></span>|<span data-ttu-id="897ae-230">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="897ae-230">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="897ae-231">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="897ae-231">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="897ae-232">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="897ae-232">kioskAppDisplayName</span></span>|<span data-ttu-id="897ae-233">String</span><span class="sxs-lookup"><span data-stu-id="897ae-233">String</span></span>|<span data-ttu-id="897ae-234">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="897ae-234">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="897ae-235">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="897ae-235">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="897ae-236">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="897ae-236">kioskAppUserModelId</span></span>|<span data-ttu-id="897ae-237">String</span><span class="sxs-lookup"><span data-stu-id="897ae-237">String</span></span>|<span data-ttu-id="897ae-238">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="897ae-238">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="897ae-239">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="897ae-239">maintenanceStartTime</span></span>|<span data-ttu-id="897ae-240">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="897ae-240">TimeOfDay</span></span>|<span data-ttu-id="897ae-241">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="897ae-241">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="897ae-242">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="897ae-242">fastFirstSignIn</span></span>|[<span data-ttu-id="897ae-243">启用</span><span class="sxs-lookup"><span data-stu-id="897ae-243">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="897ae-244">指定是否将新的非管理员 Azure AD 帐户自动连接到预配置的候选本地帐户。</span><span class="sxs-lookup"><span data-stu-id="897ae-244">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="897ae-245">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="897ae-245">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="897ae-246">响应</span><span class="sxs-lookup"><span data-stu-id="897ae-246">Response</span></span>
<span data-ttu-id="897ae-247">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="897ae-247">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="897ae-248">示例</span><span class="sxs-lookup"><span data-stu-id="897ae-248">Example</span></span>

### <a name="request"></a><span data-ttu-id="897ae-249">请求</span><span class="sxs-lookup"><span data-stu-id="897ae-249">Request</span></span>
<span data-ttu-id="897ae-250">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="897ae-250">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="897ae-251">响应</span><span class="sxs-lookup"><span data-stu-id="897ae-251">Response</span></span>
<span data-ttu-id="897ae-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="897ae-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






