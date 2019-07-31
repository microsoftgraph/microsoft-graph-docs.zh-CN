---
title: 创建 windows10GeneralConfiguration
description: 创建新的 windows10GeneralConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1fb21e9bf0a426ea9119ec7a277bf87cd8026d9a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35975485"
---
# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="b530c-103">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b530c-103">Create windows10GeneralConfiguration</span></span>

> <span data-ttu-id="b530c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b530c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b530c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b530c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b530c-106">创建新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b530c-106">Create a new [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b530c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b530c-107">Prerequisites</span></span>
<span data-ttu-id="b530c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b530c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b530c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b530c-110">Permission type</span></span>|<span data-ttu-id="b530c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b530c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b530c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b530c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b530c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b530c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b530c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b530c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b530c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b530c-115">Not supported.</span></span>|
|<span data-ttu-id="b530c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b530c-116">Application</span></span>|<span data-ttu-id="b530c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b530c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b530c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b530c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b530c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b530c-119">Request headers</span></span>
|<span data-ttu-id="b530c-120">标头</span><span class="sxs-lookup"><span data-stu-id="b530c-120">Header</span></span>|<span data-ttu-id="b530c-121">值</span><span class="sxs-lookup"><span data-stu-id="b530c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b530c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b530c-122">Authorization</span></span>|<span data-ttu-id="b530c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b530c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b530c-124">接受</span><span class="sxs-lookup"><span data-stu-id="b530c-124">Accept</span></span>|<span data-ttu-id="b530c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b530c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b530c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b530c-126">Request body</span></span>
<span data-ttu-id="b530c-127">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b530c-127">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="b530c-128">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b530c-128">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="b530c-129">属性</span><span class="sxs-lookup"><span data-stu-id="b530c-129">Property</span></span>|<span data-ttu-id="b530c-130">类型</span><span class="sxs-lookup"><span data-stu-id="b530c-130">Type</span></span>|<span data-ttu-id="b530c-131">说明</span><span class="sxs-lookup"><span data-stu-id="b530c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b530c-132">id</span><span class="sxs-lookup"><span data-stu-id="b530c-132">id</span></span>|<span data-ttu-id="b530c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b530c-133">String</span></span>|<span data-ttu-id="b530c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b530c-134">Key of the entity.</span></span> <span data-ttu-id="b530c-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b530c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b530c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b530c-137">DateTimeOffset</span></span>|<span data-ttu-id="b530c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b530c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b530c-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b530c-140">roleScopeTagIds</span></span>|<span data-ttu-id="b530c-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b530c-141">String collection</span></span>|<span data-ttu-id="b530c-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b530c-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b530c-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b530c-144">supportsScopeTags</span></span>|<span data-ttu-id="b530c-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-145">Boolean</span></span>|<span data-ttu-id="b530c-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b530c-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b530c-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b530c-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b530c-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b530c-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b530c-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b530c-149">This property is read-only.</span></span> <span data-ttu-id="b530c-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b530c-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="b530c-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="b530c-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="b530c-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="b530c-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="b530c-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b530c-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="b530c-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="b530c-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="b530c-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b530c-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="b530c-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b530c-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="b530c-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="b530c-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="b530c-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="b530c-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="b530c-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b530c-163">createdDateTime</span></span>|<span data-ttu-id="b530c-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b530c-164">DateTimeOffset</span></span>|<span data-ttu-id="b530c-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b530c-165">DateTime the object was created.</span></span> <span data-ttu-id="b530c-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-167">说明</span><span class="sxs-lookup"><span data-stu-id="b530c-167">description</span></span>|<span data-ttu-id="b530c-168">String</span><span class="sxs-lookup"><span data-stu-id="b530c-168">String</span></span>|<span data-ttu-id="b530c-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b530c-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b530c-170">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-170">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-171">displayName</span><span class="sxs-lookup"><span data-stu-id="b530c-171">displayName</span></span>|<span data-ttu-id="b530c-172">字符串</span><span class="sxs-lookup"><span data-stu-id="b530c-172">String</span></span>|<span data-ttu-id="b530c-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b530c-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b530c-174">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-174">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-175">version</span><span class="sxs-lookup"><span data-stu-id="b530c-175">version</span></span>|<span data-ttu-id="b530c-176">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-176">Int32</span></span>|<span data-ttu-id="b530c-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b530c-177">Version of the device configuration.</span></span> <span data-ttu-id="b530c-178">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b530c-178">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b530c-179">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="b530c-179">taskManagerBlockEndTask</span></span>|<span data-ttu-id="b530c-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-180">Boolean</span></span>|<span data-ttu-id="b530c-181">指定非管理员是否可以使用任务管理器结束任务。</span><span class="sxs-lookup"><span data-stu-id="b530c-181">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="b530c-182">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="b530c-182">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="b530c-183">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="b530c-183">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="b530c-184">应用的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="b530c-184">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="b530c-185">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="b530c-185">enableAutomaticRedeployment</span></span>|<span data-ttu-id="b530c-186">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-186">Boolean</span></span>|<span data-ttu-id="b530c-187">允许具有管理权限的用户在设备锁屏的屏幕上使用 CTRL + Win + R 删除所有用户数据和设置, 以便可以自动重新配置设备并将其重新注册到管理中。</span><span class="sxs-lookup"><span data-stu-id="b530c-187">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="b530c-188">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="b530c-188">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="b530c-189">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="b530c-189">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="b530c-190">控制 Microsoft 帐户登录助手 (wlidsvc) NT 服务。</span><span class="sxs-lookup"><span data-stu-id="b530c-190">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="b530c-191">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b530c-191">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="b530c-192">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="b530c-192">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="b530c-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-193">Boolean</span></span>|<span data-ttu-id="b530c-194">允许辅助身份验证设备使用 Windows。</span><span class="sxs-lookup"><span data-stu-id="b530c-194">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="b530c-195">authenticationWebSignIn</span><span class="sxs-lookup"><span data-stu-id="b530c-195">authenticationWebSignIn</span></span>|[<span data-ttu-id="b530c-196">启用</span><span class="sxs-lookup"><span data-stu-id="b530c-196">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b530c-197">指示是否将启用 Web 凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="b530c-197">Indicates whether or not Web Credential Provider will be enabled.</span></span> <span data-ttu-id="b530c-198">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b530c-198">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b530c-199">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="b530c-199">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="b530c-200">String</span><span class="sxs-lookup"><span data-stu-id="b530c-200">String</span></span>|<span data-ttu-id="b530c-201">指定 Azure AD 租户中可用域之间的首选域。</span><span class="sxs-lookup"><span data-stu-id="b530c-201">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="b530c-202">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="b530c-202">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="b530c-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-203">Boolean</span></span>|<span data-ttu-id="b530c-204">指定是否允许或禁止联邦信息处理标准 (FIPS) 策略。</span><span class="sxs-lookup"><span data-stu-id="b530c-204">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="b530c-205">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="b530c-205">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="b530c-206">String collection</span><span class="sxs-lookup"><span data-stu-id="b530c-206">String collection</span></span>|<span data-ttu-id="b530c-207">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="b530c-207">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="b530c-208">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="b530c-208">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="b530c-209">String collection</span><span class="sxs-lookup"><span data-stu-id="b530c-209">String collection</span></span>|<span data-ttu-id="b530c-210">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="b530c-210">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="b530c-211">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="b530c-211">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="b530c-212">String</span><span class="sxs-lookup"><span data-stu-id="b530c-212">String</span></span>|<span data-ttu-id="b530c-213">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="b530c-213">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="b530c-214">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="b530c-214">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="b530c-215">String</span><span class="sxs-lookup"><span data-stu-id="b530c-215">String</span></span>|<span data-ttu-id="b530c-216">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="b530c-216">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="b530c-217">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="b530c-217">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="b530c-218">String</span><span class="sxs-lookup"><span data-stu-id="b530c-218">String</span></span>|<span data-ttu-id="b530c-219">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="b530c-219">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="b530c-220">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b530c-220">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="b530c-221">String</span><span class="sxs-lookup"><span data-stu-id="b530c-221">String</span></span>|<span data-ttu-id="b530c-222">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="b530c-222">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="b530c-223">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="b530c-223">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="b530c-224">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-224">Int32</span></span>|<span data-ttu-id="b530c-225">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="b530c-225">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="b530c-226">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="b530c-226">This is a mobile only setting.</span></span> <span data-ttu-id="b530c-227">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="b530c-227">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b530c-228">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b530c-228">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="b530c-229">String</span><span class="sxs-lookup"><span data-stu-id="b530c-229">String</span></span>|<span data-ttu-id="b530c-230">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="b530c-230">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="b530c-231">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="b530c-231">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="b530c-232">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-232">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="b530c-233">允许或阻止同步 Microsoft Edge 浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="b530c-233">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="b530c-234">选项可供 IT 管理员阻止跨设备同步, 但允许用户替代。</span><span class="sxs-lookup"><span data-stu-id="b530c-234">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="b530c-235">可取值为：`notConfigured`、`blockedWithUserOverride`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="b530c-235">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="b530c-236">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="b530c-236">messagingBlockSync</span></span>|<span data-ttu-id="b530c-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-237">Boolean</span></span>|<span data-ttu-id="b530c-238">指示是否在所有位置阻止短信备份和还原和消息传递。</span><span class="sxs-lookup"><span data-stu-id="b530c-238">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="b530c-239">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="b530c-239">messagingBlockMMS</span></span>|<span data-ttu-id="b530c-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-240">Boolean</span></span>|<span data-ttu-id="b530c-241">指示是否阻止设备上的 MMS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="b530c-241">Indicates whether or not to block the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="b530c-242">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="b530c-242">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="b530c-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-243">Boolean</span></span>|<span data-ttu-id="b530c-244">指示是否阻止设备上的 RCS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="b530c-244">Indicates whether or not to block the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="b530c-245">printerNames</span><span class="sxs-lookup"><span data-stu-id="b530c-245">printerNames</span></span>|<span data-ttu-id="b530c-246">String collection</span><span class="sxs-lookup"><span data-stu-id="b530c-246">String collection</span></span>|<span data-ttu-id="b530c-247">根据打印机的名称 (网络主机名称) 自动预配打印机。</span><span class="sxs-lookup"><span data-stu-id="b530c-247">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="b530c-248">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="b530c-248">printerDefaultName</span></span>|<span data-ttu-id="b530c-249">String</span><span class="sxs-lookup"><span data-stu-id="b530c-249">String</span></span>|<span data-ttu-id="b530c-250">已安装的打印机的名称 (网络主机名称)。</span><span class="sxs-lookup"><span data-stu-id="b530c-250">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="b530c-251">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="b530c-251">printerBlockAddition</span></span>|<span data-ttu-id="b530c-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-252">Boolean</span></span>|<span data-ttu-id="b530c-253">阻止用户安装来自打印机设置的其他打印机。</span><span class="sxs-lookup"><span data-stu-id="b530c-253">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="b530c-254">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="b530c-254">searchBlockDiacritics</span></span>|<span data-ttu-id="b530c-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-255">Boolean</span></span>|<span data-ttu-id="b530c-256">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="b530c-256">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="b530c-257">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="b530c-257">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="b530c-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-258">Boolean</span></span>|<span data-ttu-id="b530c-259">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="b530c-259">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="b530c-260">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="b530c-260">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="b530c-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-261">Boolean</span></span>|<span data-ttu-id="b530c-262">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="b530c-262">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="b530c-263">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="b530c-263">searchEnableRemoteQueries</span></span>|<span data-ttu-id="b530c-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-264">Boolean</span></span>|<span data-ttu-id="b530c-265">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="b530c-265">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="b530c-266">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="b530c-266">searchDisableUseLocation</span></span>|<span data-ttu-id="b530c-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-267">Boolean</span></span>|<span data-ttu-id="b530c-268">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="b530c-268">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="b530c-269">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="b530c-269">searchDisableLocation</span></span>|<span data-ttu-id="b530c-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-270">Boolean</span></span>|<span data-ttu-id="b530c-271">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="b530c-271">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="b530c-272">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="b530c-272">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="b530c-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-273">Boolean</span></span>|<span data-ttu-id="b530c-274">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="b530c-274">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="b530c-275">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="b530c-275">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="b530c-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-276">Boolean</span></span>|<span data-ttu-id="b530c-277">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="b530c-277">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="b530c-278">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="b530c-278">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="b530c-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-279">Boolean</span></span>|<span data-ttu-id="b530c-280">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="b530c-280">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="b530c-281">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="b530c-281">searchBlockWebResults</span></span>|<span data-ttu-id="b530c-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-282">Boolean</span></span>|<span data-ttu-id="b530c-283">指示是否阻止 web 搜索。</span><span class="sxs-lookup"><span data-stu-id="b530c-283">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="b530c-284">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="b530c-284">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="b530c-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-285">Boolean</span></span>|<span data-ttu-id="b530c-286">在设备已加入 Azure AD 时, 指定是否允许在 OOBE 期间自动设备加密 (仅限桌面)。</span><span class="sxs-lookup"><span data-stu-id="b530c-286">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="b530c-287">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="b530c-287">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="b530c-288">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="b530c-288">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="b530c-289">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="b530c-289">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="b530c-290">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="b530c-290">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="b530c-291">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="b530c-291">oneDriveDisableFileSync</span></span>|<span data-ttu-id="b530c-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-292">Boolean</span></span>|<span data-ttu-id="b530c-293">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="b530c-293">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="b530c-294">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="b530c-294">systemTelemetryProxyServer</span></span>|<span data-ttu-id="b530c-295">String</span><span class="sxs-lookup"><span data-stu-id="b530c-295">String</span></span>|<span data-ttu-id="b530c-296">获取或设置代理服务器的完全限定域名 (FQDN) 或 IP 地址, 以转发连接的用户体验和遥测请求。</span><span class="sxs-lookup"><span data-stu-id="b530c-296">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="b530c-297">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="b530c-297">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="b530c-298">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="b530c-298">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="b530c-299">指定将哪种类型的遥测数据 (无、intranet、internet、两者) 发送到 Microsoft 365 Analytics。</span><span class="sxs-lookup"><span data-stu-id="b530c-299">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="b530c-300">可取值为：`notConfigured`、`intranet`、`internet`、`intranetAndInternet`。</span><span class="sxs-lookup"><span data-stu-id="b530c-300">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="b530c-301">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="b530c-301">inkWorkspaceAccess</span></span>|[<span data-ttu-id="b530c-302">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-302">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="b530c-303">控制用户对墨迹工作区的访问权限, 从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="b530c-303">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="b530c-304">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b530c-304">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b530c-305">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="b530c-305">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="b530c-306">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-306">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b530c-307">控制用户对墨迹工作区的访问权限, 从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="b530c-307">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="b530c-308">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b530c-308">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b530c-309">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="b530c-309">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="b530c-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-310">Boolean</span></span>|<span data-ttu-id="b530c-311">指定是否在墨迹工作区中显示建议的应用建议。</span><span class="sxs-lookup"><span data-stu-id="b530c-311">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="b530c-312">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="b530c-312">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="b530c-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-313">Boolean</span></span>|<span data-ttu-id="b530c-314">此属性将在7月2019中弃用, 并将替换为属性 SmartScreenAppInstallControl。</span><span class="sxs-lookup"><span data-stu-id="b530c-314">This property will be deprecated in July 2019 and will be replaced by property SmartScreenAppInstallControl.</span></span> <span data-ttu-id="b530c-315">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="b530c-315">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="b530c-316">smartScreenAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="b530c-316">smartScreenAppInstallControl</span></span>|[<span data-ttu-id="b530c-317">appInstallControlType</span><span class="sxs-lookup"><span data-stu-id="b530c-317">appInstallControlType</span></span>](../resources/intune-deviceconfig-appinstallcontroltype.md)|<span data-ttu-id="b530c-318">在 Windows 10 版本1703中添加。</span><span class="sxs-lookup"><span data-stu-id="b530c-318">Added in Windows 10, version 1703.</span></span> <span data-ttu-id="b530c-319">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="b530c-319">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span> <span data-ttu-id="b530c-320">可取值为：`notConfigured`、`anywhere`、`storeOnly`、`recommendations`、`preferStore`。</span><span class="sxs-lookup"><span data-stu-id="b530c-320">Possible values are: `notConfigured`, `anywhere`, `storeOnly`, `recommendations`, `preferStore`.</span></span>|
|<span data-ttu-id="b530c-321">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="b530c-321">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="b530c-322">String</span><span class="sxs-lookup"><span data-stu-id="b530c-322">String</span></span>|<span data-ttu-id="b530c-323">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="b530c-323">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="b530c-324">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="b530c-324">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="b530c-325">String</span><span class="sxs-lookup"><span data-stu-id="b530c-325">String</span></span>|<span data-ttu-id="b530c-326">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="b530c-326">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="b530c-327">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="b530c-327">bluetoothAllowedServices</span></span>|<span data-ttu-id="b530c-328">String 集合</span><span class="sxs-lookup"><span data-stu-id="b530c-328">String collection</span></span>|<span data-ttu-id="b530c-329">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="b530c-329">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="b530c-330">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="b530c-330">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="b530c-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-331">Boolean</span></span>|<span data-ttu-id="b530c-332">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="b530c-332">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="b530c-333">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="b530c-333">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="b530c-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-334">Boolean</span></span>|<span data-ttu-id="b530c-335">是否阻止用户使用 Swift 对和其他基于邻近的应用场景。</span><span class="sxs-lookup"><span data-stu-id="b530c-335">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="b530c-336">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="b530c-336">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="b530c-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-337">Boolean</span></span>|<span data-ttu-id="b530c-338">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="b530c-338">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="b530c-339">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="b530c-339">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="b530c-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-340">Boolean</span></span>|<span data-ttu-id="b530c-341">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="b530c-341">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="b530c-342">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b530c-342">edgeBlockAutofill</span></span>|<span data-ttu-id="b530c-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-343">Boolean</span></span>|<span data-ttu-id="b530c-344">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="b530c-344">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="b530c-345">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-345">edgeBlocked</span></span>|<span data-ttu-id="b530c-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-346">Boolean</span></span>|<span data-ttu-id="b530c-347">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="b530c-347">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="b530c-348">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="b530c-348">edgeCookiePolicy</span></span>|[<span data-ttu-id="b530c-349">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="b530c-349">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="b530c-350">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="b530c-350">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="b530c-351">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="b530c-351">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="b530c-352">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="b530c-352">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="b530c-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-353">Boolean</span></span>|<span data-ttu-id="b530c-354">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="b530c-354">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="b530c-355">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="b530c-355">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="b530c-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-356">Boolean</span></span>|<span data-ttu-id="b530c-357">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="b530c-357">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="b530c-358">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="b530c-358">edgeBlockExtensions</span></span>|<span data-ttu-id="b530c-359">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-359">Boolean</span></span>|<span data-ttu-id="b530c-360">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="b530c-360">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="b530c-361">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="b530c-361">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="b530c-362">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-362">Boolean</span></span>|<span data-ttu-id="b530c-363">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="b530c-363">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="b530c-364">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b530c-364">edgeBlockJavaScript</span></span>|<span data-ttu-id="b530c-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-365">Boolean</span></span>|<span data-ttu-id="b530c-366">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="b530c-366">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="b530c-367">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="b530c-367">edgeBlockPasswordManager</span></span>|<span data-ttu-id="b530c-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-368">Boolean</span></span>|<span data-ttu-id="b530c-369">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="b530c-369">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="b530c-370">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="b530c-370">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="b530c-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-371">Boolean</span></span>|<span data-ttu-id="b530c-372">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="b530c-372">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="b530c-373">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="b530c-373">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="b530c-374">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="b530c-374">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="b530c-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-375">Boolean</span></span>|<span data-ttu-id="b530c-376">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="b530c-376">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="b530c-377">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="b530c-377">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="b530c-378">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="b530c-378">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="b530c-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-379">Boolean</span></span>|<span data-ttu-id="b530c-380">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="b530c-380">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="b530c-381">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="b530c-381">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="b530c-382">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-382">Boolean</span></span>|<span data-ttu-id="b530c-383">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="b530c-383">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="b530c-384">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="b530c-384">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="b530c-385">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="b530c-385">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="b530c-386">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-386">Boolean</span></span>|<span data-ttu-id="b530c-387">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="b530c-387">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="b530c-388">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="b530c-388">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="b530c-389">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="b530c-389">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="b530c-390">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-390">Boolean</span></span>|<span data-ttu-id="b530c-391">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="b530c-391">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="b530c-392">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b530c-392">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="b530c-393">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-393">Boolean</span></span>|<span data-ttu-id="b530c-394">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="b530c-394">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="b530c-395">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="b530c-395">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="b530c-396">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="b530c-396">edgeFavoritesListLocation</span></span>|<span data-ttu-id="b530c-397">String</span><span class="sxs-lookup"><span data-stu-id="b530c-397">String</span></span>|<span data-ttu-id="b530c-398">要设置的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="b530c-398">The location of the favorites list to provision.</span></span> <span data-ttu-id="b530c-399">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="b530c-399">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b530c-400">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="b530c-400">edgeBlockEditFavorites</span></span>|<span data-ttu-id="b530c-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-401">Boolean</span></span>|<span data-ttu-id="b530c-402">指示是否阻止用户对收藏夹进行更改。</span><span class="sxs-lookup"><span data-stu-id="b530c-402">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="b530c-403">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="b530c-403">edgeNewTabPageURL</span></span>|<span data-ttu-id="b530c-404">String</span><span class="sxs-lookup"><span data-stu-id="b530c-404">String</span></span>|<span data-ttu-id="b530c-405">指定在创建新选项卡时打开的页面。</span><span class="sxs-lookup"><span data-stu-id="b530c-405">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="b530c-406">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="b530c-406">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="b530c-407">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="b530c-407">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="b530c-408">使 Home 按钮可以隐藏、加载默认起始页、加载新的选项卡页或自定义 URL</span><span class="sxs-lookup"><span data-stu-id="b530c-408">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="b530c-409">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="b530c-409">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="b530c-410">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-410">Boolean</span></span>|<span data-ttu-id="b530c-411">启用 "主页" 按钮配置。</span><span class="sxs-lookup"><span data-stu-id="b530c-411">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="b530c-412">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="b530c-412">edgeOpensWith</span></span>|[<span data-ttu-id="b530c-413">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="b530c-413">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="b530c-414">指定在开始时打开的页面类型。</span><span class="sxs-lookup"><span data-stu-id="b530c-414">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="b530c-415">可取值为：`notConfigured`、`startPage`、`newTabPage`、`previousPages`、`specificPages`。</span><span class="sxs-lookup"><span data-stu-id="b530c-415">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="b530c-416">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="b530c-416">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="b530c-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-417">Boolean</span></span>|<span data-ttu-id="b530c-418">指示用户是否可以旁加载扩展。</span><span class="sxs-lookup"><span data-stu-id="b530c-418">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="b530c-419">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="b530c-419">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="b530c-420">String collection</span><span class="sxs-lookup"><span data-stu-id="b530c-420">String collection</span></span>|<span data-ttu-id="b530c-421">指定所需的浏览器扩展的程序包系列名称列表, 用户无法关闭这些扩展。</span><span class="sxs-lookup"><span data-stu-id="b530c-421">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="b530c-422">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="b530c-422">edgeBlockPrinting</span></span>|<span data-ttu-id="b530c-423">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-423">Boolean</span></span>|<span data-ttu-id="b530c-424">将 Edge 配置为允许或阻止打印。</span><span class="sxs-lookup"><span data-stu-id="b530c-424">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="b530c-425">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="b530c-425">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="b530c-426">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-426">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-427">获取或设置一个值, 该值指定是否将收藏夹栏设置为始终在任何页面上都可见或隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-427">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="b530c-428">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-428">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-429">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="b530c-429">edgeBlockSavingHistory</span></span>|<span data-ttu-id="b530c-430">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-430">Boolean</span></span>|<span data-ttu-id="b530c-431">将 Edge 配置为允许保存浏览历史记录或从不保存浏览历史记录。</span><span class="sxs-lookup"><span data-stu-id="b530c-431">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="b530c-432">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="b530c-432">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="b530c-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-433">Boolean</span></span>|<span data-ttu-id="b530c-434">允许或阻止边缘进入全屏模式。</span><span class="sxs-lookup"><span data-stu-id="b530c-434">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="b530c-435">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="b530c-435">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="b530c-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-436">Boolean</span></span>|<span data-ttu-id="b530c-437">将配置为在 Edge 中加载空白页面, 而不是默认的新选项卡页面, 并防止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="b530c-437">Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.</span></span>|
|<span data-ttu-id="b530c-438">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="b530c-438">edgeBlockTabPreloading</span></span>|<span data-ttu-id="b530c-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-439">Boolean</span></span>|<span data-ttu-id="b530c-440">配置边缘是否在 Windows 启动时预加载新的选项卡页。</span><span class="sxs-lookup"><span data-stu-id="b530c-440">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="b530c-441">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="b530c-441">edgeBlockPrelaunch</span></span>|<span data-ttu-id="b530c-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-442">Boolean</span></span>|<span data-ttu-id="b530c-443">确定 Microsoft Edge 在 Windows 启动时是否为 prelaunched。</span><span class="sxs-lookup"><span data-stu-id="b530c-443">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="b530c-444">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="b530c-444">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="b530c-445">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-445">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="b530c-446">控制边缘在切换到 Internet Explorer 之前显示的消息。</span><span class="sxs-lookup"><span data-stu-id="b530c-446">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="b530c-447">可取值为：`notConfigured`、`disabled`、`enabled`、`keepGoing`。</span><span class="sxs-lookup"><span data-stu-id="b530c-447">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="b530c-448">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="b530c-448">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="b530c-449">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-449">Boolean</span></span>|<span data-ttu-id="b530c-450">允许或阻止用户覆盖证书错误。</span><span class="sxs-lookup"><span data-stu-id="b530c-450">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="b530c-451">edgeKioskModeRestriction</span><span class="sxs-lookup"><span data-stu-id="b530c-451">edgeKioskModeRestriction</span></span>|[<span data-ttu-id="b530c-452">edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="b530c-452">edgeKioskModeRestrictionType</span></span>](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|<span data-ttu-id="b530c-453">根据配置展台模式, 控制 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="b530c-453">Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode.</span></span> <span data-ttu-id="b530c-454">可取值为：`notConfigured`、`digitalSignage`、`normalMode`、`publicBrowsingSingleApp`、`publicBrowsingMultiApp`。</span><span class="sxs-lookup"><span data-stu-id="b530c-454">Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.</span></span>|
|<span data-ttu-id="b530c-455">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="b530c-455">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="b530c-456">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-456">Int32</span></span>|<span data-ttu-id="b530c-457">指定在 Microsoft Edge 展台重置前的上次用户活动的时间 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="b530c-457">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="b530c-458">有效值为0-1440。</span><span class="sxs-lookup"><span data-stu-id="b530c-458">Valid values are 0-1440.</span></span> <span data-ttu-id="b530c-459">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="b530c-459">The default is 5.</span></span> <span data-ttu-id="b530c-460">0表示不重置。</span><span class="sxs-lookup"><span data-stu-id="b530c-460">0 indicates no reset.</span></span> <span data-ttu-id="b530c-461">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="b530c-461">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="b530c-462">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="b530c-462">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="b530c-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-463">Boolean</span></span>|<span data-ttu-id="b530c-464">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="b530c-464">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="b530c-465">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="b530c-465">cellularBlockVpn</span></span>|<span data-ttu-id="b530c-466">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-466">Boolean</span></span>|<span data-ttu-id="b530c-467">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="b530c-467">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="b530c-468">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="b530c-468">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="b530c-469">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-469">Boolean</span></span>|<span data-ttu-id="b530c-470">通过手机网络漫游时是否阻止用户使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="b530c-470">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="b530c-471">cellularData</span><span class="sxs-lookup"><span data-stu-id="b530c-471">cellularData</span></span>|[<span data-ttu-id="b530c-472">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="b530c-472">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="b530c-473">是否允许设备上的手机网络数据通道。</span><span class="sxs-lookup"><span data-stu-id="b530c-473">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="b530c-474">如果未配置, 则允许手机网络数据通道, 用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="b530c-474">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="b530c-475">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b530c-475">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="b530c-476">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="b530c-476">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="b530c-477">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-477">Boolean</span></span>|<span data-ttu-id="b530c-478">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="b530c-478">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="b530c-479">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="b530c-479">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="b530c-480">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-480">Int32</span></span>|<span data-ttu-id="b530c-481">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="b530c-481">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="b530c-482">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="b530c-482">Valid values 0 to 90</span></span>|
|<span data-ttu-id="b530c-483">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="b530c-483">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="b530c-484">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="b530c-484">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="b530c-485">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="b530c-485">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="b530c-486">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="b530c-486">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="b530c-487">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="b530c-487">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="b530c-488">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="b530c-488">Defender day of the week for the system scan.</span></span> <span data-ttu-id="b530c-489">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="b530c-489">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="b530c-490">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="b530c-490">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="b530c-491">String collection</span><span class="sxs-lookup"><span data-stu-id="b530c-491">String collection</span></span>|<span data-ttu-id="b530c-492">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="b530c-492">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b530c-493">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="b530c-493">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="b530c-494">String collection</span><span class="sxs-lookup"><span data-stu-id="b530c-494">String collection</span></span>|<span data-ttu-id="b530c-495">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="b530c-495">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b530c-496">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="b530c-496">defenderScanMaxCpu</span></span>|<span data-ttu-id="b530c-497">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-497">Int32</span></span>|<span data-ttu-id="b530c-498">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="b530c-498">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="b530c-499">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="b530c-499">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b530c-500">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="b530c-500">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="b530c-501">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="b530c-501">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="b530c-502">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="b530c-502">Value for monitoring file activity.</span></span> <span data-ttu-id="b530c-503">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="b530c-503">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="b530c-504">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="b530c-504">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="b530c-505">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="b530c-505">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="b530c-506">获取或设置要对可能有害的应用程序 (PUA) 执行的 Defender 操作, 其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时, Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="b530c-506">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="b530c-507">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="b530c-507">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="b530c-508">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="b530c-508">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="b530c-509">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-509">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="b530c-510">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b530c-510">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b530c-511">获取或设置要对可能有害的应用程序 (PUA) 执行的 Defender 操作, 其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时, Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="b530c-511">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="b530c-512">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="b530c-512">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="b530c-513">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b530c-513">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b530c-514">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="b530c-514">defenderProcessesToExclude</span></span>|<span data-ttu-id="b530c-515">String 集合</span><span class="sxs-lookup"><span data-stu-id="b530c-515">String collection</span></span>|<span data-ttu-id="b530c-516">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="b530c-516">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b530c-517">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="b530c-517">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="b530c-518">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="b530c-518">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="b530c-519">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="b530c-519">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="b530c-520">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="b530c-520">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="b530c-521">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="b530c-521">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="b530c-522">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-522">Boolean</span></span>|<span data-ttu-id="b530c-523">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="b530c-523">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="b530c-524">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="b530c-524">defenderRequireCloudProtection</span></span>|<span data-ttu-id="b530c-525">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-525">Boolean</span></span>|<span data-ttu-id="b530c-526">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="b530c-526">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="b530c-527">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="b530c-527">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="b530c-528">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-528">Boolean</span></span>|<span data-ttu-id="b530c-529">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="b530c-529">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="b530c-530">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="b530c-530">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="b530c-531">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-531">Boolean</span></span>|<span data-ttu-id="b530c-532">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="b530c-532">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="b530c-533">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="b530c-533">defenderScanArchiveFiles</span></span>|<span data-ttu-id="b530c-534">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-534">Boolean</span></span>|<span data-ttu-id="b530c-535">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="b530c-535">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="b530c-536">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="b530c-536">defenderScanDownloads</span></span>|<span data-ttu-id="b530c-537">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-537">Boolean</span></span>|<span data-ttu-id="b530c-538">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="b530c-538">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="b530c-539">defenderScheduleScanEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="b530c-539">defenderScheduleScanEnableLowCpuPriority</span></span>|<span data-ttu-id="b530c-540">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-540">Boolean</span></span>|<span data-ttu-id="b530c-541">启用后, 在计划扫描期间将使用较低的 CPU 优先级。</span><span class="sxs-lookup"><span data-stu-id="b530c-541">When enabled, low CPU priority will be used during scheduled scans.</span></span>|
|<span data-ttu-id="b530c-542">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="b530c-542">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="b530c-543">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-543">Boolean</span></span>|<span data-ttu-id="b530c-544">当被阻止时, 将关闭计划快速扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="b530c-544">When blocked, catch-up scans for scheduled quick scans will be turned off.</span></span>|
|<span data-ttu-id="b530c-545">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="b530c-545">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="b530c-546">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-546">Boolean</span></span>|<span data-ttu-id="b530c-547">当被阻止时, 计划的完全扫描的追赶扫描将被禁用。</span><span class="sxs-lookup"><span data-stu-id="b530c-547">When blocked, catch-up scans for scheduled full scans will be turned off.</span></span>|
|<span data-ttu-id="b530c-548">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="b530c-548">defenderScanNetworkFiles</span></span>|<span data-ttu-id="b530c-549">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-549">Boolean</span></span>|<span data-ttu-id="b530c-550">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="b530c-550">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="b530c-551">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="b530c-551">defenderScanIncomingMail</span></span>|<span data-ttu-id="b530c-552">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-552">Boolean</span></span>|<span data-ttu-id="b530c-553">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="b530c-553">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="b530c-554">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="b530c-554">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="b530c-555">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-555">Boolean</span></span>|<span data-ttu-id="b530c-556">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="b530c-556">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="b530c-557">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="b530c-557">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="b530c-558">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-558">Boolean</span></span>|<span data-ttu-id="b530c-559">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="b530c-559">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="b530c-560">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b530c-560">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="b530c-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-561">Boolean</span></span>|<span data-ttu-id="b530c-562">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="b530c-562">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="b530c-563">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="b530c-563">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="b530c-564">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-564">Int32</span></span>|<span data-ttu-id="b530c-565">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="b530c-565">The signature update interval in hours.</span></span> <span data-ttu-id="b530c-566">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="b530c-566">Specify 0 not to check.</span></span> <span data-ttu-id="b530c-567">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="b530c-567">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b530c-568">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="b530c-568">defenderScanType</span></span>|[<span data-ttu-id="b530c-569">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="b530c-569">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="b530c-570">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="b530c-570">The defender system scan type.</span></span> <span data-ttu-id="b530c-571">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="b530c-571">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="b530c-572">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="b530c-572">defenderScheduledScanTime</span></span>|<span data-ttu-id="b530c-573">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b530c-573">TimeOfDay</span></span>|<span data-ttu-id="b530c-574">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="b530c-574">The defender time for the system scan.</span></span>|
|<span data-ttu-id="b530c-575">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="b530c-575">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="b530c-576">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b530c-576">TimeOfDay</span></span>|<span data-ttu-id="b530c-577">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="b530c-577">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="b530c-578">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="b530c-578">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="b530c-579">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="b530c-579">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="b530c-580">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="b530c-580">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="b530c-581">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="b530c-581">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="b530c-582">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="b530c-582">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="b530c-583">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-583">Int32</span></span>|<span data-ttu-id="b530c-584">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="b530c-584">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="b530c-585">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b530c-585">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b530c-586">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b530c-586">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="b530c-587">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-587">Int32</span></span>|<span data-ttu-id="b530c-588">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="b530c-588">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="b530c-589">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b530c-589">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b530c-590">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="b530c-590">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="b530c-591">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-591">Boolean</span></span>|<span data-ttu-id="b530c-592">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="b530c-592">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="b530c-593">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="b530c-593">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="b530c-594">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="b530c-594">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="b530c-595">检查 Windows Defender 中的用户同意级别以发送数据。</span><span class="sxs-lookup"><span data-stu-id="b530c-595">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="b530c-596">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="b530c-596">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="b530c-597">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="b530c-597">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="b530c-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-598">Boolean</span></span>|<span data-ttu-id="b530c-599">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="b530c-599">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="b530c-600">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="b530c-600">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="b530c-601">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="b530c-601">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="b530c-602">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-602">Boolean</span></span>|<span data-ttu-id="b530c-603">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="b530c-603">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="b530c-604">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="b530c-604">lockScreenBlockCortana</span></span>|<span data-ttu-id="b530c-605">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-605">Boolean</span></span>|<span data-ttu-id="b530c-606">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="b530c-606">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="b530c-607">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="b530c-607">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="b530c-608">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-608">Boolean</span></span>|<span data-ttu-id="b530c-609">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="b530c-609">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="b530c-610">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b530c-610">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="b530c-611">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-611">Int32</span></span>|<span data-ttu-id="b530c-612">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="b530c-612">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="b530c-613">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="b530c-613">Supported values are 11-1800.</span></span> <span data-ttu-id="b530c-614">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="b530c-614">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="b530c-615">lockScreenActivateAppsWithVoice</span><span class="sxs-lookup"><span data-stu-id="b530c-615">lockScreenActivateAppsWithVoice</span></span>|[<span data-ttu-id="b530c-616">启用</span><span class="sxs-lookup"><span data-stu-id="b530c-616">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b530c-617">此策略设置指定在系统处于锁定状态时, Windows 应用是否可以通过语音激活。</span><span class="sxs-lookup"><span data-stu-id="b530c-617">This policy setting specifies whether Windows apps can be activated by voice while the system is locked.</span></span> <span data-ttu-id="b530c-618">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b530c-618">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b530c-619">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b530c-619">passwordBlockSimple</span></span>|<span data-ttu-id="b530c-620">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-620">Boolean</span></span>|<span data-ttu-id="b530c-621">指定是否允许使用 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="b530c-621">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="b530c-622">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="b530c-622">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="b530c-623">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b530c-623">passwordExpirationDays</span></span>|<span data-ttu-id="b530c-624">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-624">Int32</span></span>|<span data-ttu-id="b530c-625">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="b530c-625">The password expiration in days.</span></span> <span data-ttu-id="b530c-626">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="b530c-626">Valid values 0 to 730</span></span>|
|<span data-ttu-id="b530c-627">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b530c-627">passwordMinimumLength</span></span>|<span data-ttu-id="b530c-628">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-628">Int32</span></span>|<span data-ttu-id="b530c-629">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="b530c-629">The minimum password length.</span></span> <span data-ttu-id="b530c-630">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="b530c-630">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b530c-631">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b530c-631">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b530c-632">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-632">Int32</span></span>|<span data-ttu-id="b530c-633">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="b530c-633">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b530c-634">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b530c-634">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b530c-635">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-635">Int32</span></span>|<span data-ttu-id="b530c-636">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="b530c-636">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b530c-637">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b530c-637">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b530c-638">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-638">Int32</span></span>|<span data-ttu-id="b530c-639">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b530c-639">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="b530c-640">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b530c-640">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b530c-641">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b530c-641">passwordRequired</span></span>|<span data-ttu-id="b530c-642">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-642">Boolean</span></span>|<span data-ttu-id="b530c-643">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="b530c-643">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="b530c-644">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="b530c-644">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="b530c-645">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-645">Boolean</span></span>|<span data-ttu-id="b530c-646">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="b530c-646">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="b530c-647">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b530c-647">passwordRequiredType</span></span>|[<span data-ttu-id="b530c-648">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b530c-648">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b530c-649">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b530c-649">The required password type.</span></span> <span data-ttu-id="b530c-650">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="b530c-650">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b530c-651">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b530c-651">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b530c-652">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-652">Int32</span></span>|<span data-ttu-id="b530c-653">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="b530c-653">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="b530c-654">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="b530c-654">Valid values 0 to 999</span></span>|
|<span data-ttu-id="b530c-655">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="b530c-655">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="b530c-656">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-656">Int32</span></span>|<span data-ttu-id="b530c-657">此安全设置确定用户可以更改密码之前必须使用该密码的时间 (以天为单位)。</span><span class="sxs-lookup"><span data-stu-id="b530c-657">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="b530c-658">有效值为0至998</span><span class="sxs-lookup"><span data-stu-id="b530c-658">Valid values 0 to 998</span></span>|
|<span data-ttu-id="b530c-659">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="b530c-659">privacyAdvertisingId</span></span>|[<span data-ttu-id="b530c-660">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-660">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b530c-661">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="b530c-661">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="b530c-662">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="b530c-662">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="b530c-663">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b530c-663">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b530c-664">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="b530c-664">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="b530c-665">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-665">Boolean</span></span>|<span data-ttu-id="b530c-666">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="b530c-666">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="b530c-667">privacyDisableLaunchExperience</span><span class="sxs-lookup"><span data-stu-id="b530c-667">privacyDisableLaunchExperience</span></span>|<span data-ttu-id="b530c-668">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-668">Boolean</span></span>|<span data-ttu-id="b530c-669">此策略可防止在用户登录时为新的和已升级的用户启动隐私体验。</span><span class="sxs-lookup"><span data-stu-id="b530c-669">This policy prevents the privacy experience from launching during user logon for new and upgraded users.</span></span>|
|<span data-ttu-id="b530c-670">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="b530c-670">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="b530c-671">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-671">Boolean</span></span>|<span data-ttu-id="b530c-672">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="b530c-672">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="b530c-673">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="b530c-673">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="b530c-674">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-674">Boolean</span></span>|<span data-ttu-id="b530c-675">阻止共享体验和发现任务切换器等中的最近使用的资源。</span><span class="sxs-lookup"><span data-stu-id="b530c-675">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="b530c-676">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="b530c-676">privacyBlockActivityFeed</span></span>|<span data-ttu-id="b530c-677">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-677">Boolean</span></span>|<span data-ttu-id="b530c-678">阻止 Cortana、听写或存储应用程序的基于云的语音服务的使用。</span><span class="sxs-lookup"><span data-stu-id="b530c-678">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="b530c-679">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="b530c-679">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="b530c-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-680">Boolean</span></span>|<span data-ttu-id="b530c-681">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="b530c-681">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="b530c-682">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="b530c-682">startMenuAppListVisibility</span></span>|[<span data-ttu-id="b530c-683">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="b530c-683">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="b530c-684">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="b530c-684">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="b530c-685">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="b530c-685">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="b530c-686">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="b530c-686">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="b530c-687">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-687">Boolean</span></span>|<span data-ttu-id="b530c-688">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-688">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b530c-689">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="b530c-689">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="b530c-690">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-690">Boolean</span></span>|<span data-ttu-id="b530c-691">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b530c-691">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b530c-692">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="b530c-692">startMenuHideHibernate</span></span>|<span data-ttu-id="b530c-693">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-693">Boolean</span></span>|<span data-ttu-id="b530c-694">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-694">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b530c-695">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="b530c-695">startMenuHideLock</span></span>|<span data-ttu-id="b530c-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-696">Boolean</span></span>|<span data-ttu-id="b530c-697">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-697">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b530c-698">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="b530c-698">startMenuHidePowerButton</span></span>|<span data-ttu-id="b530c-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-699">Boolean</span></span>|<span data-ttu-id="b530c-700">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-700">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="b530c-701">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="b530c-701">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="b530c-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-702">Boolean</span></span>|<span data-ttu-id="b530c-703">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b530c-703">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b530c-704">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="b530c-704">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="b530c-705">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-705">Boolean</span></span>|<span data-ttu-id="b530c-706">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b530c-706">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b530c-707">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="b530c-707">startMenuHideRestartOptions</span></span>|<span data-ttu-id="b530c-708">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-708">Boolean</span></span>|<span data-ttu-id="b530c-709">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-709">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b530c-710">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="b530c-710">startMenuHideShutDown</span></span>|<span data-ttu-id="b530c-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-711">Boolean</span></span>|<span data-ttu-id="b530c-712">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-712">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b530c-713">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="b530c-713">startMenuHideSignOut</span></span>|<span data-ttu-id="b530c-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-714">Boolean</span></span>|<span data-ttu-id="b530c-715">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-715">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b530c-716">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="b530c-716">startMenuHideSleep</span></span>|<span data-ttu-id="b530c-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-717">Boolean</span></span>|<span data-ttu-id="b530c-718">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-718">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b530c-719">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="b530c-719">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="b530c-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-720">Boolean</span></span>|<span data-ttu-id="b530c-721">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-721">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b530c-722">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="b530c-722">startMenuHideUserTile</span></span>|<span data-ttu-id="b530c-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-723">Boolean</span></span>|<span data-ttu-id="b530c-724">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b530c-724">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="b530c-725">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="b530c-725">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="b530c-726">Binary</span><span class="sxs-lookup"><span data-stu-id="b530c-726">Binary</span></span>|<span data-ttu-id="b530c-727">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="b530c-727">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="b530c-728">“开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="b530c-728">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="b530c-729">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="b530c-729">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="b530c-730">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="b530c-730">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="b530c-731">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="b530c-731">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="b530c-732">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="b530c-732">startMenuLayoutXml</span></span>|<span data-ttu-id="b530c-733">Binary</span><span class="sxs-lookup"><span data-stu-id="b530c-733">Binary</span></span>|<span data-ttu-id="b530c-734">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="b530c-734">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="b530c-735">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="b530c-735">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="b530c-736">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="b530c-736">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="b530c-737">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="b530c-737">startMenuMode</span></span>|[<span data-ttu-id="b530c-738">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="b530c-738">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="b530c-739">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="b530c-739">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="b530c-740">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="b530c-740">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="b530c-741">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="b530c-741">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="b530c-742">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-742">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-743">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-743">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-744">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-744">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-745">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="b530c-745">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="b530c-746">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-746">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-747">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-747">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-748">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-748">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-749">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="b530c-749">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="b530c-750">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-750">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-751">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-751">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-752">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-752">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-753">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="b530c-753">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="b530c-754">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-754">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-755">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-755">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-756">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-756">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-757">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="b530c-757">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="b530c-758">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-758">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-759">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-759">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-760">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-760">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-761">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="b530c-761">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="b530c-762">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-762">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-763">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-763">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-764">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-764">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-765">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="b530c-765">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="b530c-766">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-766">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-767">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-767">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-768">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-768">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-769">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="b530c-769">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="b530c-770">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-770">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-771">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-771">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-772">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-772">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-773">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="b530c-773">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="b530c-774">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-774">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-775">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-775">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-776">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-776">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-777">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="b530c-777">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="b530c-778">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b530c-778">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b530c-779">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b530c-779">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="b530c-780">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b530c-780">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b530c-781">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="b530c-781">settingsBlockSettingsApp</span></span>|<span data-ttu-id="b530c-782">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-782">Boolean</span></span>|<span data-ttu-id="b530c-783">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="b530c-783">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="b530c-784">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="b530c-784">settingsBlockSystemPage</span></span>|<span data-ttu-id="b530c-785">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-785">Boolean</span></span>|<span data-ttu-id="b530c-786">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="b530c-786">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="b530c-787">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="b530c-787">settingsBlockDevicesPage</span></span>|<span data-ttu-id="b530c-788">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-788">Boolean</span></span>|<span data-ttu-id="b530c-789">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="b530c-789">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="b530c-790">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="b530c-790">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="b530c-791">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-791">Boolean</span></span>|<span data-ttu-id="b530c-792">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="b530c-792">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="b530c-793">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="b530c-793">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="b530c-794">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-794">Boolean</span></span>|<span data-ttu-id="b530c-795">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="b530c-795">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="b530c-796">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="b530c-796">settingsBlockAccountsPage</span></span>|<span data-ttu-id="b530c-797">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-797">Boolean</span></span>|<span data-ttu-id="b530c-798">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="b530c-798">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="b530c-799">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="b530c-799">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="b530c-800">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-800">Boolean</span></span>|<span data-ttu-id="b530c-801">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="b530c-801">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="b530c-802">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="b530c-802">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="b530c-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-803">Boolean</span></span>|<span data-ttu-id="b530c-804">指示是否阻止在“设置”应用中访问“轻松使用”。</span><span class="sxs-lookup"><span data-stu-id="b530c-804">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="b530c-805">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="b530c-805">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="b530c-806">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-806">Boolean</span></span>|<span data-ttu-id="b530c-807">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="b530c-807">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="b530c-808">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="b530c-808">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="b530c-809">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-809">Boolean</span></span>|<span data-ttu-id="b530c-810">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="b530c-810">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="b530c-811">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="b530c-811">settingsBlockAppsPage</span></span>|<span data-ttu-id="b530c-812">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-812">Boolean</span></span>|<span data-ttu-id="b530c-813">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="b530c-813">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="b530c-814">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="b530c-814">settingsBlockGamingPage</span></span>|<span data-ttu-id="b530c-815">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-815">Boolean</span></span>|<span data-ttu-id="b530c-816">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="b530c-816">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="b530c-817">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="b530c-817">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="b530c-818">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-818">Boolean</span></span>|<span data-ttu-id="b530c-819">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="b530c-819">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="b530c-820">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-820">windowsSpotlightBlocked</span></span>|<span data-ttu-id="b530c-821">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-821">Boolean</span></span>|<span data-ttu-id="b530c-822">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="b530c-822">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="b530c-823">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="b530c-823">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="b530c-824">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-824">Boolean</span></span>|<span data-ttu-id="b530c-825">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="b530c-825">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="b530c-826">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="b530c-826">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="b530c-827">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-827">Boolean</span></span>|<span data-ttu-id="b530c-828">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="b530c-828">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="b530c-829">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="b530c-829">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="b530c-830">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-830">Boolean</span></span>|<span data-ttu-id="b530c-831">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="b530c-831">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="b530c-832">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="b530c-832">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="b530c-833">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-833">Boolean</span></span>|<span data-ttu-id="b530c-834">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="b530c-834">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="b530c-835">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="b530c-835">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="b530c-836">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-836">Boolean</span></span>|<span data-ttu-id="b530c-837">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b530c-837">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="b530c-838">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b530c-838">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="b530c-839">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="b530c-839">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="b530c-840">指定聚光灯的类型。</span><span class="sxs-lookup"><span data-stu-id="b530c-840">Specifies the type of Spotlight.</span></span> <span data-ttu-id="b530c-841">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="b530c-841">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="b530c-842">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="b530c-842">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="b530c-843">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-843">Boolean</span></span>|<span data-ttu-id="b530c-844">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="b530c-844">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="b530c-845">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="b530c-845">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="b530c-846">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="b530c-846">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="b530c-847">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-847">Boolean</span></span>|<span data-ttu-id="b530c-848">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="b530c-848">Disable automatic detection of settings.</span></span> <span data-ttu-id="b530c-849">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="b530c-849">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="b530c-850">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b530c-850">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b530c-851">String</span><span class="sxs-lookup"><span data-stu-id="b530c-851">String</span></span>|<span data-ttu-id="b530c-852">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="b530c-852">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="b530c-853">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="b530c-853">networkProxyServer</span></span>|[<span data-ttu-id="b530c-854">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="b530c-854">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="b530c-855">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="b530c-855">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="b530c-856">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b530c-856">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="b530c-857">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-857">Boolean</span></span>|<span data-ttu-id="b530c-858">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="b530c-858">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="b530c-859">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-859">antiTheftModeBlocked</span></span>|<span data-ttu-id="b530c-860">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-860">Boolean</span></span>|<span data-ttu-id="b530c-861">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="b530c-861">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="b530c-862">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-862">bluetoothBlocked</span></span>|<span data-ttu-id="b530c-863">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-863">Boolean</span></span>|<span data-ttu-id="b530c-864">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="b530c-864">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="b530c-865">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-865">cameraBlocked</span></span>|<span data-ttu-id="b530c-866">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-866">Boolean</span></span>|<span data-ttu-id="b530c-867">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="b530c-867">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b530c-868">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-868">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="b530c-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-869">Boolean</span></span>|<span data-ttu-id="b530c-870">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="b530c-870">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="b530c-871">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="b530c-871">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="b530c-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-872">Boolean</span></span>|<span data-ttu-id="b530c-873">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="b530c-873">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="b530c-874">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-874">copyPasteBlocked</span></span>|<span data-ttu-id="b530c-875">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-875">Boolean</span></span>|<span data-ttu-id="b530c-876">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="b530c-876">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="b530c-877">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-877">cortanaBlocked</span></span>|<span data-ttu-id="b530c-878">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-878">Boolean</span></span>|<span data-ttu-id="b530c-879">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="b530c-879">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="b530c-880">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="b530c-880">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="b530c-881">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-881">Boolean</span></span>|<span data-ttu-id="b530c-882">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="b530c-882">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="b530c-883">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="b530c-883">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="b530c-884">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-884">Boolean</span></span>|<span data-ttu-id="b530c-885">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="b530c-885">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="b530c-886">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="b530c-886">safeSearchFilter</span></span>|[<span data-ttu-id="b530c-887">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="b530c-887">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="b530c-888">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="b530c-888">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="b530c-889">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="b530c-889">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="b530c-890">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b530c-890">edgeBlockPopups</span></span>|<span data-ttu-id="b530c-891">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-891">Boolean</span></span>|<span data-ttu-id="b530c-892">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b530c-892">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="b530c-893">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="b530c-893">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="b530c-894">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-894">Boolean</span></span>|<span data-ttu-id="b530c-895">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="b530c-895">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="b530c-896">edgeBlockSearchEngineCustomization</span><span class="sxs-lookup"><span data-stu-id="b530c-896">edgeBlockSearchEngineCustomization</span></span>|<span data-ttu-id="b530c-897">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-897">Boolean</span></span>|<span data-ttu-id="b530c-898">指示是否阻止用户添加新的搜索引擎或更改默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b530c-898">Indicates whether or not to block the user from adding new search engine or changing the default search engine.</span></span>|
|<span data-ttu-id="b530c-899">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b530c-899">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="b530c-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-900">Boolean</span></span>|<span data-ttu-id="b530c-901">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="b530c-901">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="b530c-902">注意: 此属性的名称是误导性的;属性已过时, 请改用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="b530c-902">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="b530c-903">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b530c-903">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="b530c-904">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-904">Boolean</span></span>|<span data-ttu-id="b530c-905">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="b530c-905">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="b530c-906">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="b530c-906">edgeRequireSmartScreen</span></span>|<span data-ttu-id="b530c-907">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-907">Boolean</span></span>|<span data-ttu-id="b530c-908">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="b530c-908">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="b530c-909">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="b530c-909">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="b530c-910">String</span><span class="sxs-lookup"><span data-stu-id="b530c-910">String</span></span>|<span data-ttu-id="b530c-911">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="b530c-911">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="b530c-912">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="b530c-912">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b530c-913">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="b530c-913">edgeFirstRunUrl</span></span>|<span data-ttu-id="b530c-914">String</span><span class="sxs-lookup"><span data-stu-id="b530c-914">String</span></span>|<span data-ttu-id="b530c-915">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="b530c-915">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="b530c-916">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="b530c-916">edgeSearchEngine</span></span>|[<span data-ttu-id="b530c-917">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="b530c-917">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="b530c-918">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b530c-918">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="b530c-919">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b530c-919">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="b530c-920">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="b530c-920">edgeHomepageUrls</span></span>|<span data-ttu-id="b530c-921">String 集合</span><span class="sxs-lookup"><span data-stu-id="b530c-921">String collection</span></span>|<span data-ttu-id="b530c-922">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="b530c-922">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="b530c-923">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="b530c-923">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="b530c-924">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-924">Boolean</span></span>|<span data-ttu-id="b530c-925">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="b530c-925">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="b530c-926">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="b530c-926">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="b530c-927">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-927">Boolean</span></span>|<span data-ttu-id="b530c-928">指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="b530c-928">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="b530c-929">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="b530c-929">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="b530c-930">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-930">Boolean</span></span>|<span data-ttu-id="b530c-931">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="b530c-931">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="b530c-932">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="b530c-932">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="b530c-933">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-933">Boolean</span></span>|<span data-ttu-id="b530c-934">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="b530c-934">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="b530c-935">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-935">internetSharingBlocked</span></span>|<span data-ttu-id="b530c-936">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-936">Boolean</span></span>|<span data-ttu-id="b530c-937">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="b530c-937">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="b530c-938">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="b530c-938">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="b530c-939">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-939">Boolean</span></span>|<span data-ttu-id="b530c-940">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="b530c-940">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="b530c-941">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="b530c-941">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="b530c-942">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-942">Boolean</span></span>|<span data-ttu-id="b530c-943">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="b530c-943">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="b530c-944">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="b530c-944">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="b530c-945">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-945">Boolean</span></span>|<span data-ttu-id="b530c-946">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="b530c-946">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="b530c-947">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="b530c-947">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="b530c-948">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-948">Boolean</span></span>|<span data-ttu-id="b530c-949">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="b530c-949">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="b530c-950">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="b530c-950">settingsBlockChangeRegion</span></span>|<span data-ttu-id="b530c-951">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-951">Boolean</span></span>|<span data-ttu-id="b530c-952">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="b530c-952">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="b530c-953">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="b530c-953">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="b530c-954">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-954">Boolean</span></span>|<span data-ttu-id="b530c-955">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="b530c-955">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="b530c-956">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="b530c-956">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="b530c-957">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-957">Boolean</span></span>|<span data-ttu-id="b530c-958">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="b530c-958">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="b530c-959">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-959">locationServicesBlocked</span></span>|<span data-ttu-id="b530c-960">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-960">Boolean</span></span>|<span data-ttu-id="b530c-961">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="b530c-961">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="b530c-962">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-962">microsoftAccountBlocked</span></span>|<span data-ttu-id="b530c-963">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-963">Boolean</span></span>|<span data-ttu-id="b530c-964">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="b530c-964">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="b530c-965">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="b530c-965">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="b530c-966">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-966">Boolean</span></span>|<span data-ttu-id="b530c-967">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="b530c-967">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="b530c-968">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-968">nfcBlocked</span></span>|<span data-ttu-id="b530c-969">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-969">Boolean</span></span>|<span data-ttu-id="b530c-970">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="b530c-970">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="b530c-971">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-971">resetProtectionModeBlocked</span></span>|<span data-ttu-id="b530c-972">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-972">Boolean</span></span>|<span data-ttu-id="b530c-973">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="b530c-973">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="b530c-974">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-974">screenCaptureBlocked</span></span>|<span data-ttu-id="b530c-975">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-975">Boolean</span></span>|<span data-ttu-id="b530c-976">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="b530c-976">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b530c-977">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="b530c-977">storageBlockRemovableStorage</span></span>|<span data-ttu-id="b530c-978">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-978">Boolean</span></span>|<span data-ttu-id="b530c-979">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="b530c-979">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="b530c-980">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="b530c-980">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="b530c-981">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-981">Boolean</span></span>|<span data-ttu-id="b530c-982">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="b530c-982">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="b530c-983">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-983">usbBlocked</span></span>|<span data-ttu-id="b530c-984">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-984">Boolean</span></span>|<span data-ttu-id="b530c-985">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="b530c-985">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="b530c-986">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-986">voiceRecordingBlocked</span></span>|<span data-ttu-id="b530c-987">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-987">Boolean</span></span>|<span data-ttu-id="b530c-988">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="b530c-988">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="b530c-989">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="b530c-989">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="b530c-990">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-990">Boolean</span></span>|<span data-ttu-id="b530c-991">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="b530c-991">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="b530c-992">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="b530c-992">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b530c-993">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-993">wiFiBlocked</span></span>|<span data-ttu-id="b530c-994">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-994">Boolean</span></span>|<span data-ttu-id="b530c-995">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="b530c-995">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="b530c-996">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="b530c-996">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="b530c-997">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-997">Boolean</span></span>|<span data-ttu-id="b530c-998">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="b530c-998">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="b530c-999">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="b530c-999">wiFiScanInterval</span></span>|<span data-ttu-id="b530c-1000">Int32</span><span class="sxs-lookup"><span data-stu-id="b530c-1000">Int32</span></span>|<span data-ttu-id="b530c-1001">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="b530c-1001">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="b530c-1002">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="b530c-1002">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="b530c-1003">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="b530c-1003">Valid values 1 to 500</span></span>|
|<span data-ttu-id="b530c-1004">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="b530c-1004">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="b530c-1005">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1005">Boolean</span></span>|<span data-ttu-id="b530c-1006">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="b530c-1006">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="b530c-1007">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="b530c-1007">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="b530c-1008">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1008">Boolean</span></span>|<span data-ttu-id="b530c-1009">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="b530c-1009">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="b530c-1010">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="b530c-1010">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="b530c-1011">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1011">Boolean</span></span>|<span data-ttu-id="b530c-1012">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="b530c-1012">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="b530c-1013">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-1013">windowsStoreBlocked</span></span>|<span data-ttu-id="b530c-1014">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1014">Boolean</span></span>|<span data-ttu-id="b530c-1015">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="b530c-1015">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="b530c-1016">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="b530c-1016">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="b530c-1017">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-1017">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b530c-1018">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="b530c-1018">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="b530c-1019">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b530c-1019">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b530c-1020">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="b530c-1020">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="b530c-1021">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1021">Boolean</span></span>|<span data-ttu-id="b530c-1022">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="b530c-1022">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="b530c-1023">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-1023">developerUnlockSetting</span></span>|[<span data-ttu-id="b530c-1024">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b530c-1024">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b530c-1025">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="b530c-1025">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="b530c-1026">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b530c-1026">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b530c-1027">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="b530c-1027">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="b530c-1028">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1028">Boolean</span></span>|<span data-ttu-id="b530c-1029">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="b530c-1029">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="b530c-1030">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="b530c-1030">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="b530c-1031">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1031">Boolean</span></span>|<span data-ttu-id="b530c-1032">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="b530c-1032">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="b530c-1033">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="b530c-1033">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="b530c-1034">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1034">Boolean</span></span>|<span data-ttu-id="b530c-1035">指示是否启用“仅限专用应用商店”。</span><span class="sxs-lookup"><span data-stu-id="b530c-1035">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="b530c-1036">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="b530c-1036">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="b530c-1037">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1037">Boolean</span></span>|<span data-ttu-id="b530c-1038">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="b530c-1038">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="b530c-1039">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="b530c-1039">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="b530c-1040">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1040">Boolean</span></span>|<span data-ttu-id="b530c-1041">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="b530c-1041">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="b530c-1042">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="b530c-1042">gameDvrBlocked</span></span>|<span data-ttu-id="b530c-1043">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1043">Boolean</span></span>|<span data-ttu-id="b530c-1044">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="b530c-1044">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="b530c-1045">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="b530c-1045">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="b530c-1046">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1046">Boolean</span></span>|<span data-ttu-id="b530c-1047">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="b530c-1047">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="b530c-1048">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="b530c-1048">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="b530c-1049">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1049">Boolean</span></span>|<span data-ttu-id="b530c-1050">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="b530c-1050">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="b530c-1051">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="b530c-1051">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="b530c-1052">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1052">Boolean</span></span>|<span data-ttu-id="b530c-1053">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="b530c-1053">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="b530c-1054">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="b530c-1054">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="b530c-1055">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1055">Boolean</span></span>|<span data-ttu-id="b530c-1056">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="b530c-1056">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="b530c-1057">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="b530c-1057">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="b530c-1058">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1058">Boolean</span></span>|<span data-ttu-id="b530c-1059">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="b530c-1059">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="b530c-1060">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="b530c-1060">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="b530c-1061">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1061">Boolean</span></span>|<span data-ttu-id="b530c-1062">此策略设置允许用户更改通常仅供系统管理员使用的安装选项。</span><span class="sxs-lookup"><span data-stu-id="b530c-1062">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="b530c-1063">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="b530c-1063">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="b530c-1064">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1064">Boolean</span></span>|<span data-ttu-id="b530c-1065">此策略设置指示 Windows Installer 在系统上安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="b530c-1065">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="b530c-1066">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="b530c-1066">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="b530c-1067">Boolean</span><span class="sxs-lookup"><span data-stu-id="b530c-1067">Boolean</span></span>|<span data-ttu-id="b530c-1068">通过此策略设置, 您可以阻止所有热插拔 PCI 下游端口的直接内存访问 (DMA), 直到用户登录 Windows。</span><span class="sxs-lookup"><span data-stu-id="b530c-1068">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|
|<span data-ttu-id="b530c-1069">appManagementPackageFamilyNamesToLaunchAfterLogOn</span><span class="sxs-lookup"><span data-stu-id="b530c-1069">appManagementPackageFamilyNamesToLaunchAfterLogOn</span></span>|<span data-ttu-id="b530c-1070">String collection</span><span class="sxs-lookup"><span data-stu-id="b530c-1070">String collection</span></span>|<span data-ttu-id="b530c-1071">Windows 应用的以分号分隔的程序包系列名称的列表。</span><span class="sxs-lookup"><span data-stu-id="b530c-1071">List of semi-colon delimited Package Family Names of Windows apps.</span></span> <span data-ttu-id="b530c-1072">登录后将启动列出的 Windows 应用。</span><span class="sxs-lookup"><span data-stu-id="b530c-1072">Listed Windows apps are to be launched after logon.</span></span>|



## <a name="response"></a><span data-ttu-id="b530c-1073">响应</span><span class="sxs-lookup"><span data-stu-id="b530c-1073">Response</span></span>
<span data-ttu-id="b530c-1074">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b530c-1074">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b530c-1075">示例</span><span class="sxs-lookup"><span data-stu-id="b530c-1075">Example</span></span>

### <a name="request"></a><span data-ttu-id="b530c-1076">请求</span><span class="sxs-lookup"><span data-stu-id="b530c-1076">Request</span></span>
<span data-ttu-id="b530c-1077">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b530c-1077">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 14387

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
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
  "taskManagerBlockEndTask": true,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "anywhere",
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "lockScreenActivateAppsWithVoice": "enabled",
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="b530c-1078">响应</span><span class="sxs-lookup"><span data-stu-id="b530c-1078">Response</span></span>
<span data-ttu-id="b530c-p186">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b530c-p186">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 14559

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
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
  "taskManagerBlockEndTask": true,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationWebSignIn": "enabled",
  "authenticationPreferredAzureADTenantDomainName": "Authentication Preferred Azure ADTenant Domain Name value",
  "cryptographyAllowFipsAlgorithmPolicy": true,
  "displayAppListWithGdiDPIScalingTurnedOn": [
    "Display App List With Gdi DPIScaling Turned On value"
  ],
  "displayAppListWithGdiDPIScalingTurnedOff": [
    "Display App List With Gdi DPIScaling Turned Off value"
  ],
  "enterpriseCloudPrintDiscoveryEndPoint": "Enterprise Cloud Print Discovery End Point value",
  "enterpriseCloudPrintOAuthAuthority": "Enterprise Cloud Print OAuth Authority value",
  "enterpriseCloudPrintOAuthClientIdentifier": "Enterprise Cloud Print OAuth Client Identifier value",
  "enterpriseCloudPrintResourceIdentifier": "Enterprise Cloud Print Resource Identifier value",
  "enterpriseCloudPrintDiscoveryMaxLimit": 5,
  "enterpriseCloudPrintMopriaDiscoveryResourceIdentifier": "Enterprise Cloud Print Mopria Discovery Resource Identifier value",
  "experienceDoNotSyncBrowserSettings": "blockedWithUserOverride",
  "messagingBlockSync": true,
  "messagingBlockMMS": true,
  "messagingBlockRichCommunicationServices": true,
  "printerNames": [
    "Printer Names value"
  ],
  "printerDefaultName": "Printer Default Name value",
  "printerBlockAddition": true,
  "searchBlockDiacritics": true,
  "searchDisableAutoLanguageDetection": true,
  "searchDisableIndexingEncryptedItems": true,
  "searchEnableRemoteQueries": true,
  "searchDisableUseLocation": true,
  "searchDisableLocation": true,
  "searchDisableIndexerBackoff": true,
  "searchDisableIndexingRemovableDrive": true,
  "searchEnableAutomaticIndexSizeManangement": true,
  "searchBlockWebResults": true,
  "securityBlockAzureADJoinedDevicesAutoEncryption": true,
  "diagnosticsDataSubmissionMode": "none",
  "oneDriveDisableFileSync": true,
  "systemTelemetryProxyServer": "System Telemetry Proxy Server value",
  "edgeTelemetryForMicrosoft365Analytics": "intranet",
  "inkWorkspaceAccess": "enabled",
  "inkWorkspaceAccessState": "blocked",
  "inkWorkspaceBlockSuggestedApps": true,
  "smartScreenEnableAppInstallControl": true,
  "smartScreenAppInstallControl": "anywhere",
  "personalizationDesktopImageUrl": "https://example.com/personalizationDesktopImageUrl/",
  "personalizationLockScreenImageUrl": "https://example.com/personalizationLockScreenImageUrl/",
  "bluetoothAllowedServices": [
    "Bluetooth Allowed Services value"
  ],
  "bluetoothBlockAdvertising": true,
  "bluetoothBlockPromptedProximalConnections": true,
  "bluetoothBlockDiscoverableMode": true,
  "bluetoothBlockPrePairing": true,
  "edgeBlockAutofill": true,
  "edgeBlocked": true,
  "edgeCookiePolicy": "allow",
  "edgeBlockDeveloperTools": true,
  "edgeBlockSendingDoNotTrackHeader": true,
  "edgeBlockExtensions": true,
  "edgeBlockInPrivateBrowsing": true,
  "edgeBlockJavaScript": true,
  "edgeBlockPasswordManager": true,
  "edgeBlockAddressBarDropdown": true,
  "edgeBlockCompatibilityList": true,
  "edgeClearBrowsingDataOnExit": true,
  "edgeAllowStartPagesModification": true,
  "edgeDisableFirstRunPage": true,
  "edgeBlockLiveTileDataCollection": true,
  "edgeSyncFavoritesWithInternetExplorer": true,
  "edgeFavoritesListLocation": "Edge Favorites List Location value",
  "edgeBlockEditFavorites": true,
  "edgeNewTabPageURL": "Edge New Tab Page URL value",
  "edgeHomeButtonConfiguration": {
    "@odata.type": "microsoft.graph.edgeHomeButtonConfiguration"
  },
  "edgeHomeButtonConfigurationEnabled": true,
  "edgeOpensWith": "startPage",
  "edgeBlockSideloadingExtensions": true,
  "edgeRequiredExtensionPackageFamilyNames": [
    "Edge Required Extension Package Family Names value"
  ],
  "edgeBlockPrinting": true,
  "edgeFavoritesBarVisibility": "hide",
  "edgeBlockSavingHistory": true,
  "edgeBlockFullScreenMode": true,
  "edgeBlockWebContentOnNewTabPage": true,
  "edgeBlockTabPreloading": true,
  "edgeBlockPrelaunch": true,
  "edgeShowMessageWhenOpeningInternetExplorerSites": "disabled",
  "edgePreventCertificateErrorOverride": true,
  "edgeKioskModeRestriction": "digitalSignage",
  "edgeKioskResetAfterIdleTimeInMinutes": 4,
  "cellularBlockDataWhenRoaming": true,
  "cellularBlockVpn": true,
  "cellularBlockVpnWhenRoaming": true,
  "cellularData": "required",
  "defenderBlockEndUserAccess": true,
  "defenderDaysBeforeDeletingQuarantinedMalware": 12,
  "defenderDetectedMalwareActions": {
    "@odata.type": "microsoft.graph.defenderDetectedMalwareActions",
    "lowSeverity": "clean",
    "moderateSeverity": "clean",
    "highSeverity": "clean",
    "severeSeverity": "clean"
  },
  "defenderSystemScanSchedule": "everyday",
  "defenderFilesAndFoldersToExclude": [
    "Defender Files And Folders To Exclude value"
  ],
  "defenderFileExtensionsToExclude": [
    "Defender File Extensions To Exclude value"
  ],
  "defenderScanMaxCpu": 2,
  "defenderMonitorFileActivity": "disable",
  "defenderPotentiallyUnwantedAppAction": "block",
  "defenderPotentiallyUnwantedAppActionSetting": "enable",
  "defenderProcessesToExclude": [
    "Defender Processes To Exclude value"
  ],
  "defenderPromptForSampleSubmission": "alwaysPrompt",
  "defenderRequireBehaviorMonitoring": true,
  "defenderRequireCloudProtection": true,
  "defenderRequireNetworkInspectionSystem": true,
  "defenderRequireRealTimeMonitoring": true,
  "defenderScanArchiveFiles": true,
  "defenderScanDownloads": true,
  "defenderScheduleScanEnableLowCpuPriority": true,
  "defenderDisableCatchupQuickScan": true,
  "defenderDisableCatchupFullScan": true,
  "defenderScanNetworkFiles": true,
  "defenderScanIncomingMail": true,
  "defenderScanMappedNetworkDrivesDuringFullScan": true,
  "defenderScanRemovableDrivesDuringFullScan": true,
  "defenderScanScriptsLoadedInInternetExplorer": true,
  "defenderSignatureUpdateIntervalInHours": 6,
  "defenderScanType": "disabled",
  "defenderScheduledScanTime": "11:59:10.9990000",
  "defenderScheduledQuickScanTime": "11:58:49.3840000",
  "defenderCloudBlockLevel": "high",
  "defenderCloudExtendedTimeout": 12,
  "defenderCloudExtendedTimeoutInSeconds": 5,
  "defenderBlockOnAccessProtection": true,
  "defenderSubmitSamplesConsentType": "alwaysPrompt",
  "lockScreenAllowTimeoutConfiguration": true,
  "lockScreenBlockActionCenterNotifications": true,
  "lockScreenBlockCortana": true,
  "lockScreenBlockToastNotifications": true,
  "lockScreenTimeoutInSeconds": 10,
  "lockScreenActivateAppsWithVoice": "enabled",
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordMinimumCharacterSetCount": 0,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequired": true,
  "passwordRequireWhenResumeFromIdleState": true,
  "passwordRequiredType": "alphanumeric",
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordMinimumAgeInDays": 8,
  "privacyAdvertisingId": "blocked",
  "privacyAutoAcceptPairingAndConsentPrompts": true,
  "privacyDisableLaunchExperience": true,
  "privacyBlockInputPersonalization": true,
  "privacyBlockPublishUserActivities": true,
  "privacyBlockActivityFeed": true,
  "startBlockUnpinningAppsFromTaskbar": true,
  "startMenuAppListVisibility": "collapse",
  "startMenuHideChangeAccountSettings": true,
  "startMenuHideFrequentlyUsedApps": true,
  "startMenuHideHibernate": true,
  "startMenuHideLock": true,
  "startMenuHidePowerButton": true,
  "startMenuHideRecentJumpLists": true,
  "startMenuHideRecentlyAddedApps": true,
  "startMenuHideRestartOptions": true,
  "startMenuHideShutDown": true,
  "startMenuHideSignOut": true,
  "startMenuHideSleep": true,
  "startMenuHideSwitchAccount": true,
  "startMenuHideUserTile": true,
  "startMenuLayoutEdgeAssetsXml": "c3RhcnRNZW51TGF5b3V0RWRnZUFzc2V0c1htbA==",
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s",
  "startMenuMode": "fullScreen",
  "startMenuPinnedFolderDocuments": "hide",
  "startMenuPinnedFolderDownloads": "hide",
  "startMenuPinnedFolderFileExplorer": "hide",
  "startMenuPinnedFolderHomeGroup": "hide",
  "startMenuPinnedFolderMusic": "hide",
  "startMenuPinnedFolderNetwork": "hide",
  "startMenuPinnedFolderPersonalFolder": "hide",
  "startMenuPinnedFolderPictures": "hide",
  "startMenuPinnedFolderSettings": "hide",
  "startMenuPinnedFolderVideos": "hide",
  "settingsBlockSettingsApp": true,
  "settingsBlockSystemPage": true,
  "settingsBlockDevicesPage": true,
  "settingsBlockNetworkInternetPage": true,
  "settingsBlockPersonalizationPage": true,
  "settingsBlockAccountsPage": true,
  "settingsBlockTimeLanguagePage": true,
  "settingsBlockEaseOfAccessPage": true,
  "settingsBlockPrivacyPage": true,
  "settingsBlockUpdateSecurityPage": true,
  "settingsBlockAppsPage": true,
  "settingsBlockGamingPage": true,
  "windowsSpotlightBlockConsumerSpecificFeatures": true,
  "windowsSpotlightBlocked": true,
  "windowsSpotlightBlockOnActionCenter": true,
  "windowsSpotlightBlockTailoredExperiences": true,
  "windowsSpotlightBlockThirdPartyNotifications": true,
  "windowsSpotlightBlockWelcomeExperience": true,
  "windowsSpotlightBlockWindowsTips": true,
  "windowsSpotlightConfigureOnLockScreen": "disabled",
  "networkProxyApplySettingsDeviceWide": true,
  "networkProxyDisableAutoDetect": true,
  "networkProxyAutomaticConfigurationUrl": "https://example.com/networkProxyAutomaticConfigurationUrl/",
  "networkProxyServer": {
    "@odata.type": "microsoft.graph.windows10NetworkProxyServer",
    "address": "Address value",
    "exceptions": [
      "Exceptions value"
    ],
    "useForLocalAddresses": true
  },
  "accountsBlockAddingNonMicrosoftAccountEmail": true,
  "antiTheftModeBlocked": true,
  "bluetoothBlocked": true,
  "cameraBlocked": true,
  "connectedDevicesServiceBlocked": true,
  "certificatesBlockManualRootCertificateInstallation": true,
  "copyPasteBlocked": true,
  "cortanaBlocked": true,
  "deviceManagementBlockFactoryResetOnMobile": true,
  "deviceManagementBlockManualUnenroll": true,
  "safeSearchFilter": "strict",
  "edgeBlockPopups": true,
  "edgeBlockSearchSuggestions": true,
  "edgeBlockSearchEngineCustomization": true,
  "edgeBlockSendingIntranetTrafficToInternetExplorer": true,
  "edgeSendIntranetTrafficToInternetExplorer": true,
  "edgeRequireSmartScreen": true,
  "edgeEnterpriseModeSiteListLocation": "Edge Enterprise Mode Site List Location value",
  "edgeFirstRunUrl": "https://example.com/edgeFirstRunUrl/",
  "edgeSearchEngine": {
    "@odata.type": "microsoft.graph.edgeSearchEngineBase"
  },
  "edgeHomepageUrls": [
    "Edge Homepage Urls value"
  ],
  "edgeBlockAccessToAboutFlags": true,
  "smartScreenBlockPromptOverride": true,
  "smartScreenBlockPromptOverrideForFiles": true,
  "webRtcBlockLocalhostIpAddress": true,
  "internetSharingBlocked": true,
  "settingsBlockAddProvisioningPackage": true,
  "settingsBlockRemoveProvisioningPackage": true,
  "settingsBlockChangeSystemTime": true,
  "settingsBlockEditDeviceName": true,
  "settingsBlockChangeRegion": true,
  "settingsBlockChangeLanguage": true,
  "settingsBlockChangePowerSleep": true,
  "locationServicesBlocked": true,
  "microsoftAccountBlocked": true,
  "microsoftAccountBlockSettingsSync": true,
  "nfcBlocked": true,
  "resetProtectionModeBlocked": true,
  "screenCaptureBlocked": true,
  "storageBlockRemovableStorage": true,
  "storageRequireMobileDeviceEncryption": true,
  "usbBlocked": true,
  "voiceRecordingBlocked": true,
  "wiFiBlockAutomaticConnectHotspots": true,
  "wiFiBlocked": true,
  "wiFiBlockManualConfiguration": true,
  "wiFiScanInterval": 0,
  "wirelessDisplayBlockProjectionToThisDevice": true,
  "wirelessDisplayBlockUserInputFromReceiver": true,
  "wirelessDisplayRequirePinForPairing": true,
  "windowsStoreBlocked": true,
  "appsAllowTrustedAppsSideloading": "blocked",
  "windowsStoreBlockAutoUpdate": true,
  "developerUnlockSetting": "blocked",
  "sharedUserAppDataAllowed": true,
  "appsBlockWindowsStoreOriginatedApps": true,
  "windowsStoreEnablePrivateStoreOnly": true,
  "storageRestrictAppDataToSystemVolume": true,
  "storageRestrictAppInstallToSystemVolume": true,
  "gameDvrBlocked": true,
  "experienceBlockDeviceDiscovery": true,
  "experienceBlockErrorDialogWhenNoSIM": true,
  "experienceBlockTaskSwitcher": true,
  "logonBlockFastUserSwitching": true,
  "tenantLockdownRequireNetworkDuringOutOfBoxExperience": true,
  "appManagementMSIAllowUserControlOverInstall": true,
  "appManagementMSIAlwaysInstallWithElevatedPrivileges": true,
  "dataProtectionBlockDirectMemoryAccess": true,
  "appManagementPackageFamilyNamesToLaunchAfterLogOn": [
    "App Management Package Family Names To Launch After Log On value"
  ]
}
```





