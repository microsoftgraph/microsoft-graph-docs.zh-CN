---
title: 更新 sharedPCConfiguration
description: 更新 sharedPCConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ef2807f2c1becdc9f39e5fff1ac70c2a90c01855
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879742"
---
# <a name="update-sharedpcconfiguration"></a><span data-ttu-id="295c3-103">更新 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="295c3-103">Update sharedPCConfiguration</span></span>

> <span data-ttu-id="295c3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="295c3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="295c3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="295c3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="295c3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="295c3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="295c3-107">更新 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="295c3-107">Update the properties of a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="295c3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="295c3-108">Prerequisites</span></span>
<span data-ttu-id="295c3-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="295c3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="295c3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="295c3-111">Permission type</span></span>|<span data-ttu-id="295c3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="295c3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="295c3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="295c3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="295c3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="295c3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="295c3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="295c3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="295c3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="295c3-116">Not supported.</span></span>|
|<span data-ttu-id="295c3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="295c3-117">Application</span></span>|<span data-ttu-id="295c3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="295c3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="295c3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="295c3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="295c3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="295c3-120">Request headers</span></span>
|<span data-ttu-id="295c3-121">标头</span><span class="sxs-lookup"><span data-stu-id="295c3-121">Header</span></span>|<span data-ttu-id="295c3-122">值</span><span class="sxs-lookup"><span data-stu-id="295c3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="295c3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="295c3-123">Authorization</span></span>|<span data-ttu-id="295c3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="295c3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="295c3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="295c3-125">Accept</span></span>|<span data-ttu-id="295c3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="295c3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="295c3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="295c3-127">Request body</span></span>
<span data-ttu-id="295c3-128">在请求正文中，提供 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="295c3-128">In the request body, supply a JSON representation for the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

<span data-ttu-id="295c3-129">下表显示创建 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="295c3-129">The following table shows the properties that are required when you create the [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

|<span data-ttu-id="295c3-130">属性</span><span class="sxs-lookup"><span data-stu-id="295c3-130">Property</span></span>|<span data-ttu-id="295c3-131">类型</span><span class="sxs-lookup"><span data-stu-id="295c3-131">Type</span></span>|<span data-ttu-id="295c3-132">说明</span><span class="sxs-lookup"><span data-stu-id="295c3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="295c3-133">id</span><span class="sxs-lookup"><span data-stu-id="295c3-133">id</span></span>|<span data-ttu-id="295c3-134">String</span><span class="sxs-lookup"><span data-stu-id="295c3-134">String</span></span>|<span data-ttu-id="295c3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="295c3-135">Key of the entity.</span></span> <span data-ttu-id="295c3-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="295c3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="295c3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="295c3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="295c3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="295c3-138">DateTimeOffset</span></span>|<span data-ttu-id="295c3-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="295c3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="295c3-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="295c3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="295c3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="295c3-141">roleScopeTagIds</span></span>|<span data-ttu-id="295c3-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="295c3-142">String collection</span></span>|<span data-ttu-id="295c3-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="295c3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="295c3-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="295c3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="295c3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="295c3-145">supportsScopeTags</span></span>|<span data-ttu-id="295c3-146">布尔</span><span class="sxs-lookup"><span data-stu-id="295c3-146">Boolean</span></span>|<span data-ttu-id="295c3-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="295c3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="295c3-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="295c3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="295c3-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="295c3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="295c3-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="295c3-150">This property is read-only.</span></span> <span data-ttu-id="295c3-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="295c3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="295c3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="295c3-152">createdDateTime</span></span>|<span data-ttu-id="295c3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="295c3-153">DateTimeOffset</span></span>|<span data-ttu-id="295c3-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="295c3-154">DateTime the object was created.</span></span> <span data-ttu-id="295c3-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="295c3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="295c3-156">description</span><span class="sxs-lookup"><span data-stu-id="295c3-156">description</span></span>|<span data-ttu-id="295c3-157">String</span><span class="sxs-lookup"><span data-stu-id="295c3-157">String</span></span>|<span data-ttu-id="295c3-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="295c3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="295c3-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="295c3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="295c3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="295c3-160">displayName</span></span>|<span data-ttu-id="295c3-161">String</span><span class="sxs-lookup"><span data-stu-id="295c3-161">String</span></span>|<span data-ttu-id="295c3-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="295c3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="295c3-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="295c3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="295c3-164">version</span><span class="sxs-lookup"><span data-stu-id="295c3-164">version</span></span>|<span data-ttu-id="295c3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="295c3-165">Int32</span></span>|<span data-ttu-id="295c3-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="295c3-166">Version of the device configuration.</span></span> <span data-ttu-id="295c3-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="295c3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="295c3-168">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="295c3-168">accountManagerPolicy</span></span>|[<span data-ttu-id="295c3-169">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="295c3-169">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="295c3-170">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="295c3-170">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="295c3-171">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="295c3-171">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="295c3-172">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="295c3-172">allowedAccounts</span></span>|[<span data-ttu-id="295c3-173">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="295c3-173">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="295c3-174">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="295c3-174">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="295c3-175">可取值为：`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="295c3-175">Possible values are: `guest`, `domain`.</span></span>|
|<span data-ttu-id="295c3-176">localStorage</span><span class="sxs-lookup"><span data-stu-id="295c3-176">localStorage</span></span>|[<span data-ttu-id="295c3-177">启用</span><span class="sxs-lookup"><span data-stu-id="295c3-177">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="295c3-178">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="295c3-178">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="295c3-179">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="295c3-179">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="295c3-180">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="295c3-180">allowLocalStorage</span></span>|<span data-ttu-id="295c3-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="295c3-181">Boolean</span></span>|<span data-ttu-id="295c3-182">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="295c3-182">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="295c3-183">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="295c3-183">setAccountManager</span></span>|[<span data-ttu-id="295c3-184">启用</span><span class="sxs-lookup"><span data-stu-id="295c3-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="295c3-185">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="295c3-185">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="295c3-186">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="295c3-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="295c3-187">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="295c3-187">disableAccountManager</span></span>|<span data-ttu-id="295c3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="295c3-188">Boolean</span></span>|<span data-ttu-id="295c3-189">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="295c3-189">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="295c3-190">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="295c3-190">setEduPolicies</span></span>|[<span data-ttu-id="295c3-191">启用</span><span class="sxs-lookup"><span data-stu-id="295c3-191">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="295c3-192">指定是否默认共享 PC 教育环境策略应启用/禁用/不配置。</span><span class="sxs-lookup"><span data-stu-id="295c3-192">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="295c3-193">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="295c3-193">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="295c3-194">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="295c3-194">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="295c3-195">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="295c3-195">disableEduPolicies</span></span>|<span data-ttu-id="295c3-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="295c3-196">Boolean</span></span>|<span data-ttu-id="295c3-197">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="295c3-197">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="295c3-198">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="295c3-198">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="295c3-199">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="295c3-199">setPowerPolicies</span></span>|[<span data-ttu-id="295c3-200">启用</span><span class="sxs-lookup"><span data-stu-id="295c3-200">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="295c3-201">指定是否默认共享 PC 电源策略应启用/禁用。</span><span class="sxs-lookup"><span data-stu-id="295c3-201">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="295c3-202">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="295c3-202">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="295c3-203">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="295c3-203">disablePowerPolicies</span></span>|<span data-ttu-id="295c3-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="295c3-204">Boolean</span></span>|<span data-ttu-id="295c3-205">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="295c3-205">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="295c3-206">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="295c3-206">signInOnResume</span></span>|[<span data-ttu-id="295c3-207">启用</span><span class="sxs-lookup"><span data-stu-id="295c3-207">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="295c3-208">指定签名的要求中次设备从唤醒休眠模式。</span><span class="sxs-lookup"><span data-stu-id="295c3-208">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="295c3-209">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="295c3-209">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="295c3-210">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="295c3-210">disableSignInOnResume</span></span>|<span data-ttu-id="295c3-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="295c3-211">Boolean</span></span>|<span data-ttu-id="295c3-212">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="295c3-212">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="295c3-213">enabled</span><span class="sxs-lookup"><span data-stu-id="295c3-213">enabled</span></span>|<span data-ttu-id="295c3-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="295c3-214">Boolean</span></span>|<span data-ttu-id="295c3-215">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="295c3-215">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="295c3-216">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="295c3-216">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="295c3-217">Int32</span><span class="sxs-lookup"><span data-stu-id="295c3-217">Int32</span></span>|<span data-ttu-id="295c3-218">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="295c3-218">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="295c3-219">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="295c3-219">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="295c3-220">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="295c3-220">kioskAppDisplayName</span></span>|<span data-ttu-id="295c3-221">String</span><span class="sxs-lookup"><span data-stu-id="295c3-221">String</span></span>|<span data-ttu-id="295c3-222">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="295c3-222">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="295c3-223">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="295c3-223">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="295c3-224">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="295c3-224">kioskAppUserModelId</span></span>|<span data-ttu-id="295c3-225">String</span><span class="sxs-lookup"><span data-stu-id="295c3-225">String</span></span>|<span data-ttu-id="295c3-226">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="295c3-226">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="295c3-227">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="295c3-227">maintenanceStartTime</span></span>|<span data-ttu-id="295c3-228">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="295c3-228">TimeOfDay</span></span>|<span data-ttu-id="295c3-229">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="295c3-229">Specifies the daily start time of maintenance hour.</span></span>|



## <a name="response"></a><span data-ttu-id="295c3-230">响应</span><span class="sxs-lookup"><span data-stu-id="295c3-230">Response</span></span>
<span data-ttu-id="295c3-231">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="295c3-231">If successful, this method returns a `200 OK` response code and an updated [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="295c3-232">示例</span><span class="sxs-lookup"><span data-stu-id="295c3-232">Example</span></span>
### <a name="request"></a><span data-ttu-id="295c3-233">请求</span><span class="sxs-lookup"><span data-stu-id="295c3-233">Request</span></span>
<span data-ttu-id="295c3-234">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="295c3-234">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1119

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "allowedAccounts": "domain",
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
  "maintenanceStartTime": "11:59:24.7240000"
}
```

### <a name="response"></a><span data-ttu-id="295c3-235">响应</span><span class="sxs-lookup"><span data-stu-id="295c3-235">Response</span></span>
<span data-ttu-id="295c3-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="295c3-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1287

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
  "id": "5206be3b-be3b-5206-3bbe-06523bbe0652",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "allowedAccounts": "domain",
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
  "maintenanceStartTime": "11:59:24.7240000"
}
```





