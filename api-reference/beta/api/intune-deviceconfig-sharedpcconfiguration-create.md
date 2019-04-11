---
title: 创建 sharedPCConfiguration
description: 创建新的 sharedPCConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf3dcd240a807012ffc476b7acf364cb51318bf8
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771591"
---
# <a name="create-sharedpcconfiguration"></a><span data-ttu-id="f9f9e-103">创建 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="f9f9e-103">Create sharedPCConfiguration</span></span>

> <span data-ttu-id="f9f9e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9f9e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9f9e-106">创建新的 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-106">Create a new [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9f9e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9f9e-107">Prerequisites</span></span>
<span data-ttu-id="f9f9e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9f9e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9f9e-110">Permission type</span></span>|<span data-ttu-id="f9f9e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9f9e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9f9e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9f9e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9f9e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9f9e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f9f9e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9f9e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9f9e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-115">Not supported.</span></span>|
|<span data-ttu-id="f9f9e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9f9e-116">Application</span></span>|<span data-ttu-id="f9f9e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9f9e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9f9e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f9f9e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9f9e-119">Request headers</span></span>
|<span data-ttu-id="f9f9e-120">标头</span><span class="sxs-lookup"><span data-stu-id="f9f9e-120">Header</span></span>|<span data-ttu-id="f9f9e-121">值</span><span class="sxs-lookup"><span data-stu-id="f9f9e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9f9e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9f9e-122">Authorization</span></span>|<span data-ttu-id="f9f9e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9f9e-124">接受</span><span class="sxs-lookup"><span data-stu-id="f9f9e-124">Accept</span></span>|<span data-ttu-id="f9f9e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9f9e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9f9e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9f9e-126">Request body</span></span>
<span data-ttu-id="f9f9e-127">在请求正文中，提供 sharedPCConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-127">In the request body, supply a JSON representation for the sharedPCConfiguration object.</span></span>

<span data-ttu-id="f9f9e-128">下表显示创建 sharedPCConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-128">The following table shows the properties that are required when you create the sharedPCConfiguration.</span></span>

|<span data-ttu-id="f9f9e-129">属性</span><span class="sxs-lookup"><span data-stu-id="f9f9e-129">Property</span></span>|<span data-ttu-id="f9f9e-130">类型</span><span class="sxs-lookup"><span data-stu-id="f9f9e-130">Type</span></span>|<span data-ttu-id="f9f9e-131">说明</span><span class="sxs-lookup"><span data-stu-id="f9f9e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9f9e-132">id</span><span class="sxs-lookup"><span data-stu-id="f9f9e-132">id</span></span>|<span data-ttu-id="f9f9e-133">String</span><span class="sxs-lookup"><span data-stu-id="f9f9e-133">String</span></span>|<span data-ttu-id="f9f9e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-134">Key of the entity.</span></span> <span data-ttu-id="f9f9e-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f9e-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f9e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f9e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f9f9e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f9e-137">DateTimeOffset</span></span>|<span data-ttu-id="f9f9e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f9f9e-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f9e-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f9e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f9f9e-140">roleScopeTagIds</span></span>|<span data-ttu-id="f9f9e-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="f9f9e-141">String collection</span></span>|<span data-ttu-id="f9f9e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f9f9e-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f9e-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f9e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f9f9e-144">supportsScopeTags</span></span>|<span data-ttu-id="f9f9e-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="f9f9e-145">Boolean</span></span>|<span data-ttu-id="f9f9e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f9f9e-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f9f9e-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f9f9e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-149">This property is read-only.</span></span> <span data-ttu-id="f9f9e-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f9e-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f9e-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f9f9e-151">createdDateTime</span></span>|<span data-ttu-id="f9f9e-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9f9e-152">DateTimeOffset</span></span>|<span data-ttu-id="f9f9e-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-153">DateTime the object was created.</span></span> <span data-ttu-id="f9f9e-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f9e-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f9e-155">description</span><span class="sxs-lookup"><span data-stu-id="f9f9e-155">description</span></span>|<span data-ttu-id="f9f9e-156">String</span><span class="sxs-lookup"><span data-stu-id="f9f9e-156">String</span></span>|<span data-ttu-id="f9f9e-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f9f9e-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f9e-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f9e-159">displayName</span><span class="sxs-lookup"><span data-stu-id="f9f9e-159">displayName</span></span>|<span data-ttu-id="f9f9e-160">String</span><span class="sxs-lookup"><span data-stu-id="f9f9e-160">String</span></span>|<span data-ttu-id="f9f9e-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f9f9e-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f9e-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f9e-163">version</span><span class="sxs-lookup"><span data-stu-id="f9f9e-163">version</span></span>|<span data-ttu-id="f9f9e-164">Int32</span><span class="sxs-lookup"><span data-stu-id="f9f9e-164">Int32</span></span>|<span data-ttu-id="f9f9e-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-165">Version of the device configuration.</span></span> <span data-ttu-id="f9f9e-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f9f9e-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f9f9e-167">accountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f9f9e-167">accountManagerPolicy</span></span>|[<span data-ttu-id="f9f9e-168">sharedPCAccountManagerPolicy</span><span class="sxs-lookup"><span data-stu-id="f9f9e-168">sharedPCAccountManagerPolicy</span></span>](../resources/intune-deviceconfig-sharedpcaccountmanagerpolicy.md)|<span data-ttu-id="f9f9e-169">指定在共享电脑上管理帐户的方式。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-169">Specifies how accounts are managed on a shared PC.</span></span> <span data-ttu-id="f9f9e-170">仅当 disableAccountManager 为 false 时适用。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-170">Only applies when disableAccountManager is false.</span></span>|
|<span data-ttu-id="f9f9e-171">allowedAccounts</span><span class="sxs-lookup"><span data-stu-id="f9f9e-171">allowedAccounts</span></span>|[<span data-ttu-id="f9f9e-172">sharedPCAllowedAccountType</span><span class="sxs-lookup"><span data-stu-id="f9f9e-172">sharedPCAllowedAccountType</span></span>](../resources/intune-deviceconfig-sharedpcallowedaccounttype.md)|<span data-ttu-id="f9f9e-173">指示允许在共享电脑上使用哪种类型的帐户。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-173">Indicates which type of accounts are allowed to use on a shared PC.</span></span> <span data-ttu-id="f9f9e-174">可取值为：`notConfigured`、`guest`、`domain`。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-174">Possible values are: `notConfigured`, `guest`, `domain`.</span></span>|
|<span data-ttu-id="f9f9e-175">localStorage</span><span class="sxs-lookup"><span data-stu-id="f9f9e-175">localStorage</span></span>|[<span data-ttu-id="f9f9e-176">启用</span><span class="sxs-lookup"><span data-stu-id="f9f9e-176">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f9f9e-177">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-177">Specifies whether local storage is allowed on a shared PC.</span></span> <span data-ttu-id="f9f9e-178">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-178">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f9f9e-179">allowLocalStorage</span><span class="sxs-lookup"><span data-stu-id="f9f9e-179">allowLocalStorage</span></span>|<span data-ttu-id="f9f9e-180">布尔值</span><span class="sxs-lookup"><span data-stu-id="f9f9e-180">Boolean</span></span>|<span data-ttu-id="f9f9e-181">指定在共享电脑上是否允许本地存储。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-181">Specifies whether local storage is allowed on a shared PC.</span></span>|
|<span data-ttu-id="f9f9e-182">setAccountManager</span><span class="sxs-lookup"><span data-stu-id="f9f9e-182">setAccountManager</span></span>|[<span data-ttu-id="f9f9e-183">启用</span><span class="sxs-lookup"><span data-stu-id="f9f9e-183">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f9f9e-184">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-184">Disables the account manager for shared PC mode.</span></span> <span data-ttu-id="f9f9e-185">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-185">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f9f9e-186">disableAccountManager</span><span class="sxs-lookup"><span data-stu-id="f9f9e-186">disableAccountManager</span></span>|<span data-ttu-id="f9f9e-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="f9f9e-187">Boolean</span></span>|<span data-ttu-id="f9f9e-188">禁用共享电脑模式的帐户管理器。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-188">Disables the account manager for shared PC mode.</span></span>|
|<span data-ttu-id="f9f9e-189">setEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f9f9e-189">setEduPolicies</span></span>|[<span data-ttu-id="f9f9e-190">启用</span><span class="sxs-lookup"><span data-stu-id="f9f9e-190">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f9f9e-191">指定是否应启用/禁用/禁用/禁用默认共享 PC 教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-191">Specifies whether the default shared PC education environment policies should be enabled/disabled/not configured.</span></span> <span data-ttu-id="f9f9e-192">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-192">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span> <span data-ttu-id="f9f9e-193">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-193">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f9f9e-194">disableEduPolicies</span><span class="sxs-lookup"><span data-stu-id="f9f9e-194">disableEduPolicies</span></span>|<span data-ttu-id="f9f9e-195">布尔值</span><span class="sxs-lookup"><span data-stu-id="f9f9e-195">Boolean</span></span>|<span data-ttu-id="f9f9e-196">指定是否应禁用默认的共享电脑教育环境策略。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-196">Specifies whether the default shared PC education environment policies should be disabled.</span></span> <span data-ttu-id="f9f9e-197">对于 Windows 10 RS2 及更高版本，将应用此策略而不将 Enabled 设置为 true。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-197">For Windows 10 RS2 and later, this policy will be applied without setting Enabled to true.</span></span>|
|<span data-ttu-id="f9f9e-198">setPowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f9f9e-198">setPowerPolicies</span></span>|[<span data-ttu-id="f9f9e-199">启用</span><span class="sxs-lookup"><span data-stu-id="f9f9e-199">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f9f9e-200">指定是否应启用/禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-200">Specifies whether the default shared PC power policies should be enabled/disabled.</span></span> <span data-ttu-id="f9f9e-201">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-201">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f9f9e-202">disablePowerPolicies</span><span class="sxs-lookup"><span data-stu-id="f9f9e-202">disablePowerPolicies</span></span>|<span data-ttu-id="f9f9e-203">布尔值</span><span class="sxs-lookup"><span data-stu-id="f9f9e-203">Boolean</span></span>|<span data-ttu-id="f9f9e-204">指定是否应禁用默认的共享电脑电源策略。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-204">Specifies whether the default shared PC power policies should be disabled.</span></span>|
|<span data-ttu-id="f9f9e-205">signInOnResume</span><span class="sxs-lookup"><span data-stu-id="f9f9e-205">signInOnResume</span></span>|[<span data-ttu-id="f9f9e-206">启用</span><span class="sxs-lookup"><span data-stu-id="f9f9e-206">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f9f9e-207">指定当设备从睡眠模式唤醒时登录时的要求。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-207">Specifies the requirement to sign in whenever the device wakes up from sleep mode.</span></span> <span data-ttu-id="f9f9e-208">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-208">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="f9f9e-209">disableSignInOnResume</span><span class="sxs-lookup"><span data-stu-id="f9f9e-209">disableSignInOnResume</span></span>|<span data-ttu-id="f9f9e-210">布尔值</span><span class="sxs-lookup"><span data-stu-id="f9f9e-210">Boolean</span></span>|<span data-ttu-id="f9f9e-211">禁用每当设备从睡眠模式唤醒时需要登录的要求。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-211">Disables the requirement to sign in whenever the device wakes up from sleep mode.</span></span>|
|<span data-ttu-id="f9f9e-212">enabled</span><span class="sxs-lookup"><span data-stu-id="f9f9e-212">enabled</span></span>|<span data-ttu-id="f9f9e-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f9f9e-213">Boolean</span></span>|<span data-ttu-id="f9f9e-214">启用共享的电脑模式并应用共享的电脑策略。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-214">Enables shared PC mode and applies the shared pc policies.</span></span>|
|<span data-ttu-id="f9f9e-215">idleTimeBeforeSleepInSeconds</span><span class="sxs-lookup"><span data-stu-id="f9f9e-215">idleTimeBeforeSleepInSeconds</span></span>|<span data-ttu-id="f9f9e-216">Int32</span><span class="sxs-lookup"><span data-stu-id="f9f9e-216">Int32</span></span>|<span data-ttu-id="f9f9e-217">指定电脑进入睡眠状态之前设备必须保持空闲状态的时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-217">Specifies the time in seconds that a device must sit idle before the PC goes to sleep.</span></span> <span data-ttu-id="f9f9e-218">将此值设置为 0 可防止发生睡眠超时。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-218">Setting this value to 0 prevents the sleep timeout from occurring.</span></span>|
|<span data-ttu-id="f9f9e-219">kioskAppDisplayName</span><span class="sxs-lookup"><span data-stu-id="f9f9e-219">kioskAppDisplayName</span></span>|<span data-ttu-id="f9f9e-220">String</span><span class="sxs-lookup"><span data-stu-id="f9f9e-220">String</span></span>|<span data-ttu-id="f9f9e-221">指定启动由 SetKioskAppUserModelId 指定的应用的登录屏幕上显示的帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-221">Specifies the display text for the account shown on the sign-in screen which launches the app specified by SetKioskAppUserModelId.</span></span> <span data-ttu-id="f9f9e-222">仅在设置 KioskAppUserModelId 后适用。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-222">Only applies when KioskAppUserModelId is set.</span></span>|
|<span data-ttu-id="f9f9e-223">kioskAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f9f9e-223">kioskAppUserModelId</span></span>|<span data-ttu-id="f9f9e-224">String</span><span class="sxs-lookup"><span data-stu-id="f9f9e-224">String</span></span>|<span data-ttu-id="f9f9e-225">指定要与分配的访问权限结合使用的应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-225">Specifies the application user model ID of the app to use with assigned access.</span></span>|
|<span data-ttu-id="f9f9e-226">maintenanceStartTime</span><span class="sxs-lookup"><span data-stu-id="f9f9e-226">maintenanceStartTime</span></span>|<span data-ttu-id="f9f9e-227">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="f9f9e-227">TimeOfDay</span></span>|<span data-ttu-id="f9f9e-228">指定维护小时的每日开始时间。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-228">Specifies the daily start time of maintenance hour.</span></span>|
|<span data-ttu-id="f9f9e-229">fastFirstSignIn</span><span class="sxs-lookup"><span data-stu-id="f9f9e-229">fastFirstSignIn</span></span>|[<span data-ttu-id="f9f9e-230">启用</span><span class="sxs-lookup"><span data-stu-id="f9f9e-230">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="f9f9e-231">指定是否将新的非管理员 Azure AD 帐户自动连接到预配置的候选本地帐户。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-231">Specifies whether to auto connect new non-admin Azure AD accounts to pre-configured candidate local accounts.</span></span> <span data-ttu-id="f9f9e-232">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-232">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|



## <a name="response"></a><span data-ttu-id="f9f9e-233">响应</span><span class="sxs-lookup"><span data-stu-id="f9f9e-233">Response</span></span>
<span data-ttu-id="f9f9e-234">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-234">If successful, this method returns a `201 Created` response code and a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9f9e-235">示例</span><span class="sxs-lookup"><span data-stu-id="f9f9e-235">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9f9e-236">请求</span><span class="sxs-lookup"><span data-stu-id="f9f9e-236">Request</span></span>
<span data-ttu-id="f9f9e-237">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-237">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1147

{
  "@odata.type": "#microsoft.graph.sharedPCConfiguration",
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

### <a name="response"></a><span data-ttu-id="f9f9e-238">响应</span><span class="sxs-lookup"><span data-stu-id="f9f9e-238">Response</span></span>
<span data-ttu-id="f9f9e-p121">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9f9e-p121">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1319

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





