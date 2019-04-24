---
title: 更新 windows10GeneralConfiguration
description: 更新 windows10GeneralConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 52ad6af4a58265d2812111a0b1e51ef971d1e4e9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32516586"
---
# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="b7e0d-103">更新 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7e0d-103">Update windows10GeneralConfiguration</span></span>

> <span data-ttu-id="b7e0d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7e0d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7e0d-106">更新 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-106">Update the properties of a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7e0d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b7e0d-107">Prerequisites</span></span>
<span data-ttu-id="b7e0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b7e0d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b7e0d-110">Permission type</span></span>|<span data-ttu-id="b7e0d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b7e0d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7e0d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b7e0d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7e0d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b7e0d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b7e0d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b7e0d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7e0d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-115">Not supported.</span></span>|
|<span data-ttu-id="b7e0d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b7e0d-116">Application</span></span>|<span data-ttu-id="b7e0d-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7e0d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b7e0d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b7e0d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b7e0d-119">Request headers</span></span>
|<span data-ttu-id="b7e0d-120">标头</span><span class="sxs-lookup"><span data-stu-id="b7e0d-120">Header</span></span>|<span data-ttu-id="b7e0d-121">值</span><span class="sxs-lookup"><span data-stu-id="b7e0d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7e0d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7e0d-122">Authorization</span></span>|<span data-ttu-id="b7e0d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7e0d-124">接受</span><span class="sxs-lookup"><span data-stu-id="b7e0d-124">Accept</span></span>|<span data-ttu-id="b7e0d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b7e0d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7e0d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b7e0d-126">Request body</span></span>
<span data-ttu-id="b7e0d-127">在请求正文中，提供 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-127">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="b7e0d-128">下表显示了创建 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-128">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="b7e0d-129">属性</span><span class="sxs-lookup"><span data-stu-id="b7e0d-129">Property</span></span>|<span data-ttu-id="b7e0d-130">类型</span><span class="sxs-lookup"><span data-stu-id="b7e0d-130">Type</span></span>|<span data-ttu-id="b7e0d-131">说明</span><span class="sxs-lookup"><span data-stu-id="b7e0d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7e0d-132">id</span><span class="sxs-lookup"><span data-stu-id="b7e0d-132">id</span></span>|<span data-ttu-id="b7e0d-133">String</span><span class="sxs-lookup"><span data-stu-id="b7e0d-133">String</span></span>|<span data-ttu-id="b7e0d-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-134">Key of the entity.</span></span> <span data-ttu-id="b7e0d-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7e0d-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7e0d-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b7e0d-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b7e0d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7e0d-137">DateTimeOffset</span></span>|<span data-ttu-id="b7e0d-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b7e0d-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7e0d-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7e0d-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b7e0d-140">roleScopeTagIds</span></span>|<span data-ttu-id="b7e0d-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-141">String collection</span></span>|<span data-ttu-id="b7e0d-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b7e0d-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7e0d-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7e0d-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b7e0d-144">supportsScopeTags</span></span>|<span data-ttu-id="b7e0d-145">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-145">Boolean</span></span>|<span data-ttu-id="b7e0d-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b7e0d-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b7e0d-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b7e0d-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-149">This property is read-only.</span></span> <span data-ttu-id="b7e0d-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7e0d-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7e0d-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b7e0d-151">createdDateTime</span></span>|<span data-ttu-id="b7e0d-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b7e0d-152">DateTimeOffset</span></span>|<span data-ttu-id="b7e0d-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-153">DateTime the object was created.</span></span> <span data-ttu-id="b7e0d-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7e0d-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7e0d-155">description</span><span class="sxs-lookup"><span data-stu-id="b7e0d-155">description</span></span>|<span data-ttu-id="b7e0d-156">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-156">String</span></span>|<span data-ttu-id="b7e0d-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b7e0d-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7e0d-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7e0d-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b7e0d-159">displayName</span></span>|<span data-ttu-id="b7e0d-160">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-160">String</span></span>|<span data-ttu-id="b7e0d-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b7e0d-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7e0d-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7e0d-163">version</span><span class="sxs-lookup"><span data-stu-id="b7e0d-163">version</span></span>|<span data-ttu-id="b7e0d-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-164">Int32</span></span>|<span data-ttu-id="b7e0d-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-165">Version of the device configuration.</span></span> <span data-ttu-id="b7e0d-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b7e0d-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b7e0d-167">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="b7e0d-167">taskManagerBlockEndTask</span></span>|<span data-ttu-id="b7e0d-168">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-168">Boolean</span></span>|<span data-ttu-id="b7e0d-169">指定非管理员是否可以使用任务管理器结束任务。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-169">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="b7e0d-170">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="b7e0d-170">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="b7e0d-171">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="b7e0d-171">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="b7e0d-172">应用的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-172">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="b7e0d-173">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="b7e0d-173">enableAutomaticRedeployment</span></span>|<span data-ttu-id="b7e0d-174">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-174">Boolean</span></span>|<span data-ttu-id="b7e0d-175">允许具有管理权限的用户在设备锁屏的屏幕上使用 CTRL + Win + R 删除所有用户数据和设置, 以便可以自动重新配置设备并将其重新注册到管理中。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-175">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="b7e0d-176">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="b7e0d-176">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="b7e0d-177">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="b7e0d-177">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="b7e0d-178">控制 Microsoft 帐户登录助手 (wlidsvc) NT 服务。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-178">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="b7e0d-179">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-179">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="b7e0d-180">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="b7e0d-180">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="b7e0d-181">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-181">Boolean</span></span>|<span data-ttu-id="b7e0d-182">允许辅助身份验证设备使用 Windows。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-182">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="b7e0d-183">authenticationWebSignIn</span><span class="sxs-lookup"><span data-stu-id="b7e0d-183">authenticationWebSignIn</span></span>|[<span data-ttu-id="b7e0d-184">启用</span><span class="sxs-lookup"><span data-stu-id="b7e0d-184">enablement</span></span>](../resources/intune-shared-enablement.md)|<span data-ttu-id="b7e0d-185">指示是否将启用 Web 凭据提供程序。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-185">Indicates whether or not Web Credential Provider will be enabled.</span></span> <span data-ttu-id="b7e0d-186">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-186">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b7e0d-187">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="b7e0d-187">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="b7e0d-188">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-188">String</span></span>|<span data-ttu-id="b7e0d-189">指定 Azure AD 租户中可用域之间的首选域。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-189">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="b7e0d-190">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="b7e0d-190">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="b7e0d-191">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-191">Boolean</span></span>|<span data-ttu-id="b7e0d-192">指定是否允许或禁止联邦信息处理标准 (FIPS) 策略。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-192">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="b7e0d-193">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="b7e0d-193">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="b7e0d-194">String collection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-194">String collection</span></span>|<span data-ttu-id="b7e0d-195">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-195">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="b7e0d-196">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="b7e0d-196">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="b7e0d-197">String collection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-197">String collection</span></span>|<span data-ttu-id="b7e0d-198">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-198">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="b7e0d-199">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="b7e0d-199">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="b7e0d-200">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-200">String</span></span>|<span data-ttu-id="b7e0d-201">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-201">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="b7e0d-202">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="b7e0d-202">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="b7e0d-203">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-203">String</span></span>|<span data-ttu-id="b7e0d-204">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-204">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="b7e0d-205">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="b7e0d-205">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="b7e0d-206">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-206">String</span></span>|<span data-ttu-id="b7e0d-207">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-207">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="b7e0d-208">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b7e0d-208">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="b7e0d-209">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-209">String</span></span>|<span data-ttu-id="b7e0d-210">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-210">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="b7e0d-211">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="b7e0d-211">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="b7e0d-212">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-212">Int32</span></span>|<span data-ttu-id="b7e0d-213">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-213">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="b7e0d-214">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-214">This is a mobile only setting.</span></span> <span data-ttu-id="b7e0d-215">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="b7e0d-215">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b7e0d-216">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b7e0d-216">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="b7e0d-217">String</span><span class="sxs-lookup"><span data-stu-id="b7e0d-217">String</span></span>|<span data-ttu-id="b7e0d-218">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-218">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="b7e0d-219">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="b7e0d-219">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="b7e0d-220">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-220">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="b7e0d-221">允许或阻止同步 Microsoft Edge 浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-221">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="b7e0d-222">选项可供 IT 管理员阻止跨设备同步, 但允许用户替代。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-222">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="b7e0d-223">可取值为：`notConfigured`、`blockedWithUserOverride`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-223">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="b7e0d-224">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="b7e0d-224">messagingBlockSync</span></span>|<span data-ttu-id="b7e0d-225">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-225">Boolean</span></span>|<span data-ttu-id="b7e0d-226">指示是否在所有位置阻止短信备份和还原和消息传递。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-226">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="b7e0d-227">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="b7e0d-227">messagingBlockMMS</span></span>|<span data-ttu-id="b7e0d-228">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-228">Boolean</span></span>|<span data-ttu-id="b7e0d-229">指示是否阻止设备上的 MMS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-229">Indicates whether or not to block the the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="b7e0d-230">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="b7e0d-230">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="b7e0d-231">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-231">Boolean</span></span>|<span data-ttu-id="b7e0d-232">指示是否阻止设备上的 RCS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-232">Indicates whether or not to block the the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="b7e0d-233">printerNames</span><span class="sxs-lookup"><span data-stu-id="b7e0d-233">printerNames</span></span>|<span data-ttu-id="b7e0d-234">String collection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-234">String collection</span></span>|<span data-ttu-id="b7e0d-235">根据打印机的名称 (网络主机名称) 自动预配打印机。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-235">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="b7e0d-236">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="b7e0d-236">printerDefaultName</span></span>|<span data-ttu-id="b7e0d-237">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-237">String</span></span>|<span data-ttu-id="b7e0d-238">已安装的打印机的名称 (网络主机名称)。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-238">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="b7e0d-239">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="b7e0d-239">printerBlockAddition</span></span>|<span data-ttu-id="b7e0d-240">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-240">Boolean</span></span>|<span data-ttu-id="b7e0d-241">阻止用户安装来自打印机设置的其他打印机。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-241">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="b7e0d-242">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="b7e0d-242">searchBlockDiacritics</span></span>|<span data-ttu-id="b7e0d-243">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-243">Boolean</span></span>|<span data-ttu-id="b7e0d-244">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-244">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="b7e0d-245">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-245">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="b7e0d-246">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-246">Boolean</span></span>|<span data-ttu-id="b7e0d-247">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-247">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="b7e0d-248">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="b7e0d-248">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="b7e0d-249">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-249">Boolean</span></span>|<span data-ttu-id="b7e0d-250">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-250">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="b7e0d-251">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="b7e0d-251">searchEnableRemoteQueries</span></span>|<span data-ttu-id="b7e0d-252">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-252">Boolean</span></span>|<span data-ttu-id="b7e0d-253">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-253">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="b7e0d-254">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="b7e0d-254">searchDisableUseLocation</span></span>|<span data-ttu-id="b7e0d-255">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-255">Boolean</span></span>|<span data-ttu-id="b7e0d-256">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-256">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="b7e0d-257">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="b7e0d-257">searchDisableLocation</span></span>|<span data-ttu-id="b7e0d-258">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-258">Boolean</span></span>|<span data-ttu-id="b7e0d-259">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-259">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="b7e0d-260">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="b7e0d-260">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="b7e0d-261">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-261">Boolean</span></span>|<span data-ttu-id="b7e0d-262">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-262">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="b7e0d-263">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="b7e0d-263">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="b7e0d-264">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-264">Boolean</span></span>|<span data-ttu-id="b7e0d-265">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-265">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="b7e0d-266">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="b7e0d-266">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="b7e0d-267">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-267">Boolean</span></span>|<span data-ttu-id="b7e0d-268">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-268">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="b7e0d-269">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="b7e0d-269">searchBlockWebResults</span></span>|<span data-ttu-id="b7e0d-270">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-270">Boolean</span></span>|<span data-ttu-id="b7e0d-271">指示是否阻止 web 搜索。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-271">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="b7e0d-272">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="b7e0d-272">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="b7e0d-273">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-273">Boolean</span></span>|<span data-ttu-id="b7e0d-274">在设备已加入 Azure AD 时, 指定是否允许在 OOBE 期间自动设备加密 (仅限桌面)。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-274">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="b7e0d-275">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="b7e0d-275">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="b7e0d-276">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="b7e0d-276">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="b7e0d-277">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-277">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="b7e0d-278">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-278">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="b7e0d-279">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="b7e0d-279">oneDriveDisableFileSync</span></span>|<span data-ttu-id="b7e0d-280">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-280">Boolean</span></span>|<span data-ttu-id="b7e0d-281">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-281">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="b7e0d-282">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="b7e0d-282">systemTelemetryProxyServer</span></span>|<span data-ttu-id="b7e0d-283">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-283">String</span></span>|<span data-ttu-id="b7e0d-284">获取或设置代理服务器的完全限定域名 (FQDN) 或 IP 地址, 以转发连接的用户体验和遥测请求。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-284">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="b7e0d-285">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="b7e0d-285">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="b7e0d-286">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="b7e0d-286">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="b7e0d-287">指定将哪种类型的遥测数据 (无、intranet、internet、两者) 发送到 Microsoft 365 Analytics。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-287">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="b7e0d-288">可取值为：`notConfigured`、`intranet`、`internet`、`intranetAndInternet`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-288">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="b7e0d-289">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="b7e0d-289">inkWorkspaceAccess</span></span>|[<span data-ttu-id="b7e0d-290">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-290">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="b7e0d-291">控制用户对墨迹工作区的访问权限, 从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-291">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="b7e0d-292">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-292">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b7e0d-293">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="b7e0d-293">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="b7e0d-294">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-294">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b7e0d-295">控制用户对墨迹工作区的访问权限, 从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-295">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="b7e0d-296">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-296">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b7e0d-297">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="b7e0d-297">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="b7e0d-298">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-298">Boolean</span></span>|<span data-ttu-id="b7e0d-299">指定是否在墨迹工作区中显示建议的应用建议。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-299">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="b7e0d-300">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="b7e0d-300">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="b7e0d-301">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-301">Boolean</span></span>|<span data-ttu-id="b7e0d-302">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-302">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="b7e0d-303">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="b7e0d-303">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="b7e0d-304">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-304">String</span></span>|<span data-ttu-id="b7e0d-305">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-305">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="b7e0d-306">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="b7e0d-306">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="b7e0d-307">String</span><span class="sxs-lookup"><span data-stu-id="b7e0d-307">String</span></span>|<span data-ttu-id="b7e0d-308">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-308">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="b7e0d-309">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="b7e0d-309">bluetoothAllowedServices</span></span>|<span data-ttu-id="b7e0d-310">String 集合</span><span class="sxs-lookup"><span data-stu-id="b7e0d-310">String collection</span></span>|<span data-ttu-id="b7e0d-311">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-311">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="b7e0d-312">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="b7e0d-312">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="b7e0d-313">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-313">Boolean</span></span>|<span data-ttu-id="b7e0d-314">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-314">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="b7e0d-315">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="b7e0d-315">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="b7e0d-316">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-316">Boolean</span></span>|<span data-ttu-id="b7e0d-317">是否阻止用户使用 Swift 对和其他基于邻近的应用场景。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-317">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="b7e0d-318">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="b7e0d-318">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="b7e0d-319">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-319">Boolean</span></span>|<span data-ttu-id="b7e0d-320">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-320">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="b7e0d-321">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="b7e0d-321">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="b7e0d-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-322">Boolean</span></span>|<span data-ttu-id="b7e0d-323">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-323">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="b7e0d-324">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b7e0d-324">edgeBlockAutofill</span></span>|<span data-ttu-id="b7e0d-325">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-325">Boolean</span></span>|<span data-ttu-id="b7e0d-326">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-326">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="b7e0d-327">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-327">edgeBlocked</span></span>|<span data-ttu-id="b7e0d-328">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-328">Boolean</span></span>|<span data-ttu-id="b7e0d-329">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-329">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="b7e0d-330">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="b7e0d-330">edgeCookiePolicy</span></span>|[<span data-ttu-id="b7e0d-331">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="b7e0d-331">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="b7e0d-332">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-332">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="b7e0d-333">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-333">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="b7e0d-334">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="b7e0d-334">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="b7e0d-335">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-335">Boolean</span></span>|<span data-ttu-id="b7e0d-336">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-336">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="b7e0d-337">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="b7e0d-337">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="b7e0d-338">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-338">Boolean</span></span>|<span data-ttu-id="b7e0d-339">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-339">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="b7e0d-340">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="b7e0d-340">edgeBlockExtensions</span></span>|<span data-ttu-id="b7e0d-341">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-341">Boolean</span></span>|<span data-ttu-id="b7e0d-342">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-342">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="b7e0d-343">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="b7e0d-343">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="b7e0d-344">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-344">Boolean</span></span>|<span data-ttu-id="b7e0d-345">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-345">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="b7e0d-346">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b7e0d-346">edgeBlockJavaScript</span></span>|<span data-ttu-id="b7e0d-347">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-347">Boolean</span></span>|<span data-ttu-id="b7e0d-348">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-348">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="b7e0d-349">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="b7e0d-349">edgeBlockPasswordManager</span></span>|<span data-ttu-id="b7e0d-350">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-350">Boolean</span></span>|<span data-ttu-id="b7e0d-351">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-351">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="b7e0d-352">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="b7e0d-352">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="b7e0d-353">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-353">Boolean</span></span>|<span data-ttu-id="b7e0d-354">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-354">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="b7e0d-355">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-355">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="b7e0d-356">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="b7e0d-356">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="b7e0d-357">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-357">Boolean</span></span>|<span data-ttu-id="b7e0d-358">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-358">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="b7e0d-359">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-359">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="b7e0d-360">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="b7e0d-360">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="b7e0d-361">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-361">Boolean</span></span>|<span data-ttu-id="b7e0d-362">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-362">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="b7e0d-363">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="b7e0d-363">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="b7e0d-364">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-364">Boolean</span></span>|<span data-ttu-id="b7e0d-365">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-365">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="b7e0d-366">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-366">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="b7e0d-367">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-367">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="b7e0d-368">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-368">Boolean</span></span>|<span data-ttu-id="b7e0d-369">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-369">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="b7e0d-370">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-370">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="b7e0d-371">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-371">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="b7e0d-372">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-372">Boolean</span></span>|<span data-ttu-id="b7e0d-373">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-373">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="b7e0d-374">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b7e0d-374">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="b7e0d-375">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-375">Boolean</span></span>|<span data-ttu-id="b7e0d-376">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-376">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="b7e0d-377">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-377">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="b7e0d-378">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="b7e0d-378">edgeFavoritesListLocation</span></span>|<span data-ttu-id="b7e0d-379">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-379">String</span></span>|<span data-ttu-id="b7e0d-380">要设置的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-380">The location of the favorites list to provision.</span></span> <span data-ttu-id="b7e0d-381">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-381">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b7e0d-382">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="b7e0d-382">edgeBlockEditFavorites</span></span>|<span data-ttu-id="b7e0d-383">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-383">Boolean</span></span>|<span data-ttu-id="b7e0d-384">指示是否阻止用户对收藏夹进行更改。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-384">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="b7e0d-385">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="b7e0d-385">edgeNewTabPageURL</span></span>|<span data-ttu-id="b7e0d-386">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-386">String</span></span>|<span data-ttu-id="b7e0d-387">指定在创建新选项卡时打开的页面。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-387">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="b7e0d-388">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7e0d-388">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="b7e0d-389">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7e0d-389">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="b7e0d-390">使 Home 按钮可以隐藏、加载默认起始页、加载新的选项卡页或自定义 URL</span><span class="sxs-lookup"><span data-stu-id="b7e0d-390">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="b7e0d-391">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="b7e0d-391">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="b7e0d-392">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-392">Boolean</span></span>|<span data-ttu-id="b7e0d-393">启用 "主页" 按钮配置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-393">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="b7e0d-394">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="b7e0d-394">edgeOpensWith</span></span>|[<span data-ttu-id="b7e0d-395">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="b7e0d-395">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="b7e0d-396">指定在开始时打开的页面类型。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-396">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="b7e0d-397">可取值为：`notConfigured`、`startPage`、`newTabPage`、`previousPages` 或 `specificPages`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-397">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="b7e0d-398">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="b7e0d-398">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="b7e0d-399">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-399">Boolean</span></span>|<span data-ttu-id="b7e0d-400">指示用户是否可以旁加载扩展。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-400">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="b7e0d-401">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="b7e0d-401">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="b7e0d-402">String collection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-402">String collection</span></span>|<span data-ttu-id="b7e0d-403">指定所需的浏览器扩展的程序包系列名称列表, 用户无法关闭这些扩展。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-403">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="b7e0d-404">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-404">edgeBlockPrinting</span></span>|<span data-ttu-id="b7e0d-405">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-405">Boolean</span></span>|<span data-ttu-id="b7e0d-406">将 Edge 配置为允许或阻止打印。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-406">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="b7e0d-407">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="b7e0d-407">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="b7e0d-408">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-408">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-409">获取或设置一个值, 该值指定是否将收藏夹栏设置为始终在任何页面上都可见或隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-409">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="b7e0d-410">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-410">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-411">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="b7e0d-411">edgeBlockSavingHistory</span></span>|<span data-ttu-id="b7e0d-412">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-412">Boolean</span></span>|<span data-ttu-id="b7e0d-413">将 Edge 配置为允许保存浏览历史记录或从不保存浏览历史记录。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-413">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="b7e0d-414">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="b7e0d-414">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="b7e0d-415">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-415">Boolean</span></span>|<span data-ttu-id="b7e0d-416">允许或阻止边缘进入全屏模式。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-416">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="b7e0d-417">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-417">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="b7e0d-418">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-418">Boolean</span></span>|<span data-ttu-id="b7e0d-419">将配置为在 Edge 中加载空白页面, 而不是默认的新选项卡页面, 并防止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-419">Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.</span></span>|
|<span data-ttu-id="b7e0d-420">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="b7e0d-420">edgeBlockTabPreloading</span></span>|<span data-ttu-id="b7e0d-421">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-421">Boolean</span></span>|<span data-ttu-id="b7e0d-422">配置边缘是否在 Windows 启动时预加载新的选项卡页。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-422">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="b7e0d-423">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="b7e0d-423">edgeBlockPrelaunch</span></span>|<span data-ttu-id="b7e0d-424">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-424">Boolean</span></span>|<span data-ttu-id="b7e0d-425">确定 Microsoft Edge 在 Windows 启动时是否为 prelaunched。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-425">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="b7e0d-426">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="b7e0d-426">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="b7e0d-427">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-427">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="b7e0d-428">控制边缘在切换到 Internet Explorer 之前显示的消息。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-428">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="b7e0d-429">可取值为：`notConfigured`、`disabled`、`enabled`、`keepGoing`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-429">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="b7e0d-430">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="b7e0d-430">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="b7e0d-431">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-431">Boolean</span></span>|<span data-ttu-id="b7e0d-432">允许或阻止用户覆盖证书错误。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-432">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="b7e0d-433">edgeKioskModeRestriction</span><span class="sxs-lookup"><span data-stu-id="b7e0d-433">edgeKioskModeRestriction</span></span>|[<span data-ttu-id="b7e0d-434">edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-434">edgeKioskModeRestrictionType</span></span>](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|<span data-ttu-id="b7e0d-435">根据配置展台模式, 控制 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-435">Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode.</span></span> <span data-ttu-id="b7e0d-436">可取值为：`notConfigured`、`digitalSignage`、`normalMode`、`publicBrowsingSingleApp` 或 `publicBrowsingMultiApp`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-436">Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.</span></span>|
|<span data-ttu-id="b7e0d-437">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="b7e0d-437">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="b7e0d-438">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-438">Int32</span></span>|<span data-ttu-id="b7e0d-439">指定在 Microsoft Edge 展台重置前的上次用户活动的时间 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-439">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="b7e0d-440">有效值为0-1440。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-440">Valid values are 0-1440.</span></span> <span data-ttu-id="b7e0d-441">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-441">The default is 5.</span></span> <span data-ttu-id="b7e0d-442">0表示不重置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-442">0 indicates no reset.</span></span> <span data-ttu-id="b7e0d-443">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="b7e0d-443">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="b7e0d-444">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="b7e0d-444">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="b7e0d-445">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-445">Boolean</span></span>|<span data-ttu-id="b7e0d-446">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-446">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="b7e0d-447">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="b7e0d-447">cellularBlockVpn</span></span>|<span data-ttu-id="b7e0d-448">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-448">Boolean</span></span>|<span data-ttu-id="b7e0d-449">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-449">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="b7e0d-450">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="b7e0d-450">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="b7e0d-451">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-451">Boolean</span></span>|<span data-ttu-id="b7e0d-452">通过手机网络漫游时是否阻止用户使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-452">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="b7e0d-453">cellularData</span><span class="sxs-lookup"><span data-stu-id="b7e0d-453">cellularData</span></span>|[<span data-ttu-id="b7e0d-454">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-454">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="b7e0d-455">是否允许设备上的手机网络数据通道。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-455">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="b7e0d-456">如果未配置, 则允许手机网络数据通道, 用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-456">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="b7e0d-457">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-457">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="b7e0d-458">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="b7e0d-458">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="b7e0d-459">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-459">Boolean</span></span>|<span data-ttu-id="b7e0d-460">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-460">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="b7e0d-461">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="b7e0d-461">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="b7e0d-462">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-462">Int32</span></span>|<span data-ttu-id="b7e0d-463">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-463">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="b7e0d-464">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="b7e0d-464">Valid values 0 to 90</span></span>|
|<span data-ttu-id="b7e0d-465">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="b7e0d-465">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="b7e0d-466">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="b7e0d-466">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="b7e0d-467">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-467">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="b7e0d-468">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="b7e0d-468">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="b7e0d-469">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="b7e0d-469">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="b7e0d-470">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-470">Defender day of the week for the system scan.</span></span> <span data-ttu-id="b7e0d-471">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-471">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="b7e0d-472">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="b7e0d-472">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="b7e0d-473">String collection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-473">String collection</span></span>|<span data-ttu-id="b7e0d-474">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-474">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b7e0d-475">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="b7e0d-475">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="b7e0d-476">String collection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-476">String collection</span></span>|<span data-ttu-id="b7e0d-477">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-477">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b7e0d-478">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="b7e0d-478">defenderScanMaxCpu</span></span>|<span data-ttu-id="b7e0d-479">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-479">Int32</span></span>|<span data-ttu-id="b7e0d-480">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-480">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="b7e0d-481">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="b7e0d-481">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b7e0d-482">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="b7e0d-482">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="b7e0d-483">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="b7e0d-483">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="b7e0d-484">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-484">Value for monitoring file activity.</span></span> <span data-ttu-id="b7e0d-485">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly` 或 `monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-485">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="b7e0d-486">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="b7e0d-486">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="b7e0d-487">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="b7e0d-487">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="b7e0d-488">获取或设置要对可能有害的应用程序 (PUA) 执行的 Defender 操作, 其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时, Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-488">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="b7e0d-489">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-489">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="b7e0d-490">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-490">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="b7e0d-491">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-491">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="b7e0d-492">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-492">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b7e0d-493">获取或设置要对可能有害的应用程序 (PUA) 执行的 Defender 操作, 其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时, Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-493">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="b7e0d-494">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-494">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="b7e0d-495">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-495">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b7e0d-496">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="b7e0d-496">defenderProcessesToExclude</span></span>|<span data-ttu-id="b7e0d-497">String 集合</span><span class="sxs-lookup"><span data-stu-id="b7e0d-497">String collection</span></span>|<span data-ttu-id="b7e0d-498">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-498">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b7e0d-499">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="b7e0d-499">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="b7e0d-500">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="b7e0d-500">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="b7e0d-501">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-501">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="b7e0d-502">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-502">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="b7e0d-503">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="b7e0d-503">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="b7e0d-504">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-504">Boolean</span></span>|<span data-ttu-id="b7e0d-505">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-505">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="b7e0d-506">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-506">defenderRequireCloudProtection</span></span>|<span data-ttu-id="b7e0d-507">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-507">Boolean</span></span>|<span data-ttu-id="b7e0d-508">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-508">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="b7e0d-509">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="b7e0d-509">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="b7e0d-510">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-510">Boolean</span></span>|<span data-ttu-id="b7e0d-511">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-511">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="b7e0d-512">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="b7e0d-512">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="b7e0d-513">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-513">Boolean</span></span>|<span data-ttu-id="b7e0d-514">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-514">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="b7e0d-515">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="b7e0d-515">defenderScanArchiveFiles</span></span>|<span data-ttu-id="b7e0d-516">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-516">Boolean</span></span>|<span data-ttu-id="b7e0d-517">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-517">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="b7e0d-518">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="b7e0d-518">defenderScanDownloads</span></span>|<span data-ttu-id="b7e0d-519">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-519">Boolean</span></span>|<span data-ttu-id="b7e0d-520">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-520">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="b7e0d-521">defenderScheduleScanEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="b7e0d-521">defenderScheduleScanEnableLowCpuPriority</span></span>|<span data-ttu-id="b7e0d-522">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-522">Boolean</span></span>|<span data-ttu-id="b7e0d-523">启用后, 在计划扫描期间将使用较低的 CPU 优先级。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-523">When enabled, low CPU priority will be used during scheduled scans.</span></span>|
|<span data-ttu-id="b7e0d-524">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="b7e0d-524">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="b7e0d-525">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-525">Boolean</span></span>|<span data-ttu-id="b7e0d-526">当被阻止时, 将关闭计划快速扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-526">When blocked, catch-up scans for scheduled quick scans will be turned off.</span></span>|
|<span data-ttu-id="b7e0d-527">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="b7e0d-527">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="b7e0d-528">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-528">Boolean</span></span>|<span data-ttu-id="b7e0d-529">当被阻止时, 计划的完全扫描的追赶扫描将被禁用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-529">When blocked, catch-up scans for scheduled full scans will be turned off.</span></span>|
|<span data-ttu-id="b7e0d-530">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="b7e0d-530">defenderScanNetworkFiles</span></span>|<span data-ttu-id="b7e0d-531">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-531">Boolean</span></span>|<span data-ttu-id="b7e0d-532">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-532">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="b7e0d-533">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="b7e0d-533">defenderScanIncomingMail</span></span>|<span data-ttu-id="b7e0d-534">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-534">Boolean</span></span>|<span data-ttu-id="b7e0d-535">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-535">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="b7e0d-536">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="b7e0d-536">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="b7e0d-537">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-537">Boolean</span></span>|<span data-ttu-id="b7e0d-538">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-538">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="b7e0d-539">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="b7e0d-539">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="b7e0d-540">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-540">Boolean</span></span>|<span data-ttu-id="b7e0d-541">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-541">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="b7e0d-542">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b7e0d-542">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="b7e0d-543">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-543">Boolean</span></span>|<span data-ttu-id="b7e0d-544">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-544">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="b7e0d-545">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="b7e0d-545">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="b7e0d-546">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-546">Int32</span></span>|<span data-ttu-id="b7e0d-547">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-547">The signature update interval in hours.</span></span> <span data-ttu-id="b7e0d-548">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-548">Specify 0 not to check.</span></span> <span data-ttu-id="b7e0d-549">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="b7e0d-549">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b7e0d-550">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-550">defenderScanType</span></span>|[<span data-ttu-id="b7e0d-551">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-551">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="b7e0d-552">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-552">The defender system scan type.</span></span> <span data-ttu-id="b7e0d-553">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-553">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="b7e0d-554">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="b7e0d-554">defenderScheduledScanTime</span></span>|<span data-ttu-id="b7e0d-555">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b7e0d-555">TimeOfDay</span></span>|<span data-ttu-id="b7e0d-556">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-556">The defender time for the system scan.</span></span>|
|<span data-ttu-id="b7e0d-557">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="b7e0d-557">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="b7e0d-558">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b7e0d-558">TimeOfDay</span></span>|<span data-ttu-id="b7e0d-559">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-559">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="b7e0d-560">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="b7e0d-560">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="b7e0d-561">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-561">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="b7e0d-562">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-562">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="b7e0d-563">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-563">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="b7e0d-564">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="b7e0d-564">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="b7e0d-565">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-565">Int32</span></span>|<span data-ttu-id="b7e0d-566">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-566">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="b7e0d-567">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b7e0d-567">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b7e0d-568">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b7e0d-568">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="b7e0d-569">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-569">Int32</span></span>|<span data-ttu-id="b7e0d-570">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-570">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="b7e0d-571">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b7e0d-571">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b7e0d-572">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-572">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="b7e0d-573">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-573">Boolean</span></span>|<span data-ttu-id="b7e0d-574">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-574">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="b7e0d-575">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-575">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="b7e0d-576">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-576">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="b7e0d-577">检查 Windows Defender 中的用户同意级别以发送数据。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-577">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="b7e0d-578">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-578">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="b7e0d-579">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7e0d-579">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="b7e0d-580">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-580">Boolean</span></span>|<span data-ttu-id="b7e0d-581">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-581">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="b7e0d-582">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-582">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="b7e0d-583">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="b7e0d-583">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="b7e0d-584">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-584">Boolean</span></span>|<span data-ttu-id="b7e0d-585">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-585">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="b7e0d-586">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="b7e0d-586">lockScreenBlockCortana</span></span>|<span data-ttu-id="b7e0d-587">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-587">Boolean</span></span>|<span data-ttu-id="b7e0d-588">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-588">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="b7e0d-589">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="b7e0d-589">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="b7e0d-590">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-590">Boolean</span></span>|<span data-ttu-id="b7e0d-591">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-591">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="b7e0d-592">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b7e0d-592">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="b7e0d-593">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-593">Int32</span></span>|<span data-ttu-id="b7e0d-594">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-594">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="b7e0d-595">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-595">Supported values are 11-1800.</span></span> <span data-ttu-id="b7e0d-596">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="b7e0d-596">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="b7e0d-597">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b7e0d-597">passwordBlockSimple</span></span>|<span data-ttu-id="b7e0d-598">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-598">Boolean</span></span>|<span data-ttu-id="b7e0d-599">指定是否允许使用 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-599">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="b7e0d-600">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-600">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="b7e0d-601">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b7e0d-601">passwordExpirationDays</span></span>|<span data-ttu-id="b7e0d-602">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-602">Int32</span></span>|<span data-ttu-id="b7e0d-603">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-603">The password expiration in days.</span></span> <span data-ttu-id="b7e0d-604">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="b7e0d-604">Valid values 0 to 730</span></span>|
|<span data-ttu-id="b7e0d-605">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b7e0d-605">passwordMinimumLength</span></span>|<span data-ttu-id="b7e0d-606">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-606">Int32</span></span>|<span data-ttu-id="b7e0d-607">密码最短长度。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-607">The minimum password length.</span></span> <span data-ttu-id="b7e0d-608">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="b7e0d-608">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b7e0d-609">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b7e0d-609">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b7e0d-610">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-610">Int32</span></span>|<span data-ttu-id="b7e0d-611">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-611">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b7e0d-612">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b7e0d-612">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b7e0d-613">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-613">Int32</span></span>|<span data-ttu-id="b7e0d-614">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-614">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b7e0d-615">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b7e0d-615">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b7e0d-616">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-616">Int32</span></span>|<span data-ttu-id="b7e0d-617">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-617">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="b7e0d-618">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b7e0d-618">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b7e0d-619">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b7e0d-619">passwordRequired</span></span>|<span data-ttu-id="b7e0d-620">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-620">Boolean</span></span>|<span data-ttu-id="b7e0d-621">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-621">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="b7e0d-622">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="b7e0d-622">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="b7e0d-623">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-623">Boolean</span></span>|<span data-ttu-id="b7e0d-624">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-624">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="b7e0d-625">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-625">passwordRequiredType</span></span>|[<span data-ttu-id="b7e0d-626">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-626">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b7e0d-627">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-627">The required password type.</span></span> <span data-ttu-id="b7e0d-628">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-628">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b7e0d-629">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b7e0d-629">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b7e0d-630">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-630">Int32</span></span>|<span data-ttu-id="b7e0d-631">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-631">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="b7e0d-632">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="b7e0d-632">Valid values 0 to 999</span></span>|
|<span data-ttu-id="b7e0d-633">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="b7e0d-633">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="b7e0d-634">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-634">Int32</span></span>|<span data-ttu-id="b7e0d-635">此安全设置确定用户可以更改密码之前必须使用该密码的时间 (以天为单位)。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-635">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="b7e0d-636">有效值为0至998</span><span class="sxs-lookup"><span data-stu-id="b7e0d-636">Valid values 0 to 998</span></span>|
|<span data-ttu-id="b7e0d-637">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="b7e0d-637">privacyAdvertisingId</span></span>|[<span data-ttu-id="b7e0d-638">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-638">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b7e0d-639">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-639">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="b7e0d-640">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-640">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="b7e0d-641">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-641">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b7e0d-642">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="b7e0d-642">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="b7e0d-643">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-643">Boolean</span></span>|<span data-ttu-id="b7e0d-644">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-644">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="b7e0d-645">privacyDisableLaunchExperience</span><span class="sxs-lookup"><span data-stu-id="b7e0d-645">privacyDisableLaunchExperience</span></span>|<span data-ttu-id="b7e0d-646">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-646">Boolean</span></span>|<span data-ttu-id="b7e0d-647">此策略可防止在用户登录时为新的和已升级的用户启动隐私体验。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-647">This policy prevents the privacy experience from launching during user logon for new and upgraded users.</span></span>|
|<span data-ttu-id="b7e0d-648">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="b7e0d-648">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="b7e0d-649">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-649">Boolean</span></span>|<span data-ttu-id="b7e0d-650">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-650">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="b7e0d-651">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="b7e0d-651">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="b7e0d-652">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-652">Boolean</span></span>|<span data-ttu-id="b7e0d-653">阻止共享体验和发现任务切换器等中的最近使用的资源。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-653">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="b7e0d-654">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="b7e0d-654">privacyBlockActivityFeed</span></span>|<span data-ttu-id="b7e0d-655">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-655">Boolean</span></span>|<span data-ttu-id="b7e0d-656">阻止 Cortana、听写或存储应用程序的基于云的语音服务的使用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-656">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="b7e0d-657">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="b7e0d-657">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="b7e0d-658">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-658">Boolean</span></span>|<span data-ttu-id="b7e0d-659">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-659">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="b7e0d-660">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="b7e0d-660">startMenuAppListVisibility</span></span>|[<span data-ttu-id="b7e0d-661">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-661">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="b7e0d-662">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-662">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="b7e0d-663">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-663">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="b7e0d-664">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="b7e0d-664">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="b7e0d-665">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-665">Boolean</span></span>|<span data-ttu-id="b7e0d-666">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-666">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-667">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="b7e0d-667">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="b7e0d-668">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-668">Boolean</span></span>|<span data-ttu-id="b7e0d-669">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-669">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b7e0d-670">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="b7e0d-670">startMenuHideHibernate</span></span>|<span data-ttu-id="b7e0d-671">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-671">Boolean</span></span>|<span data-ttu-id="b7e0d-672">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-672">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-673">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="b7e0d-673">startMenuHideLock</span></span>|<span data-ttu-id="b7e0d-674">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-674">Boolean</span></span>|<span data-ttu-id="b7e0d-675">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-675">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-676">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="b7e0d-676">startMenuHidePowerButton</span></span>|<span data-ttu-id="b7e0d-677">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-677">Boolean</span></span>|<span data-ttu-id="b7e0d-678">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-678">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-679">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="b7e0d-679">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="b7e0d-680">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-680">Boolean</span></span>|<span data-ttu-id="b7e0d-681">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-681">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b7e0d-682">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="b7e0d-682">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="b7e0d-683">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-683">Boolean</span></span>|<span data-ttu-id="b7e0d-684">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-684">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b7e0d-685">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="b7e0d-685">startMenuHideRestartOptions</span></span>|<span data-ttu-id="b7e0d-686">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-686">Boolean</span></span>|<span data-ttu-id="b7e0d-687">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-687">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-688">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="b7e0d-688">startMenuHideShutDown</span></span>|<span data-ttu-id="b7e0d-689">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-689">Boolean</span></span>|<span data-ttu-id="b7e0d-690">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-690">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-691">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="b7e0d-691">startMenuHideSignOut</span></span>|<span data-ttu-id="b7e0d-692">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-692">Boolean</span></span>|<span data-ttu-id="b7e0d-693">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-693">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-694">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="b7e0d-694">startMenuHideSleep</span></span>|<span data-ttu-id="b7e0d-695">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-695">Boolean</span></span>|<span data-ttu-id="b7e0d-696">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-696">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-697">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="b7e0d-697">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="b7e0d-698">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-698">Boolean</span></span>|<span data-ttu-id="b7e0d-699">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-699">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-700">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="b7e0d-700">startMenuHideUserTile</span></span>|<span data-ttu-id="b7e0d-701">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-701">Boolean</span></span>|<span data-ttu-id="b7e0d-702">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-702">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="b7e0d-703">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="b7e0d-703">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="b7e0d-704">Binary</span><span class="sxs-lookup"><span data-stu-id="b7e0d-704">Binary</span></span>|<span data-ttu-id="b7e0d-705">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-705">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="b7e0d-706">“开始”菜单布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-706">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="b7e0d-707">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-707">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="b7e0d-708">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-708">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="b7e0d-709">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-709">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="b7e0d-710">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="b7e0d-710">startMenuLayoutXml</span></span>|<span data-ttu-id="b7e0d-711">Binary</span><span class="sxs-lookup"><span data-stu-id="b7e0d-711">Binary</span></span>|<span data-ttu-id="b7e0d-712">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-712">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="b7e0d-713">通过基于布局修改架构指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-713">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="b7e0d-714">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-714">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="b7e0d-715">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="b7e0d-715">startMenuMode</span></span>|[<span data-ttu-id="b7e0d-716">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-716">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="b7e0d-717">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-717">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="b7e0d-718">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-718">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="b7e0d-719">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="b7e0d-719">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="b7e0d-720">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-720">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-721">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-721">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-722">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-722">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-723">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="b7e0d-723">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="b7e0d-724">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-724">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-725">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-725">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-726">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-726">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-727">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="b7e0d-727">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="b7e0d-728">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-728">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-729">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-729">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-730">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-730">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-731">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="b7e0d-731">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="b7e0d-732">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-732">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-733">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-733">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-734">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-734">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-735">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="b7e0d-735">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="b7e0d-736">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-736">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-737">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-737">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-738">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-738">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-739">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="b7e0d-739">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="b7e0d-740">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-740">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-741">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-741">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-742">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-742">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-743">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="b7e0d-743">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="b7e0d-744">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-744">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-745">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-745">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-746">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-746">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-747">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="b7e0d-747">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="b7e0d-748">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-748">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-749">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-749">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-750">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-750">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-751">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="b7e0d-751">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="b7e0d-752">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-752">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-753">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-753">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-754">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-754">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-755">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="b7e0d-755">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="b7e0d-756">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-756">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b7e0d-757">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-757">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="b7e0d-758">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-758">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b7e0d-759">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="b7e0d-759">settingsBlockSettingsApp</span></span>|<span data-ttu-id="b7e0d-760">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-760">Boolean</span></span>|<span data-ttu-id="b7e0d-761">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-761">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="b7e0d-762">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-762">settingsBlockSystemPage</span></span>|<span data-ttu-id="b7e0d-763">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-763">Boolean</span></span>|<span data-ttu-id="b7e0d-764">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-764">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-765">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-765">settingsBlockDevicesPage</span></span>|<span data-ttu-id="b7e0d-766">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-766">Boolean</span></span>|<span data-ttu-id="b7e0d-767">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-767">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-768">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-768">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="b7e0d-769">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-769">Boolean</span></span>|<span data-ttu-id="b7e0d-770">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-770">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-771">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-771">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="b7e0d-772">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-772">Boolean</span></span>|<span data-ttu-id="b7e0d-773">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-773">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-774">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-774">settingsBlockAccountsPage</span></span>|<span data-ttu-id="b7e0d-775">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-775">Boolean</span></span>|<span data-ttu-id="b7e0d-776">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-776">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-777">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-777">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="b7e0d-778">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-778">Boolean</span></span>|<span data-ttu-id="b7e0d-779">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-779">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-780">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-780">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="b7e0d-781">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-781">Boolean</span></span>|<span data-ttu-id="b7e0d-782">指示是否阻止在“设置”应用中访问“轻松使用”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-782">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-783">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-783">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="b7e0d-784">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-784">Boolean</span></span>|<span data-ttu-id="b7e0d-785">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-785">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-786">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-786">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="b7e0d-787">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-787">Boolean</span></span>|<span data-ttu-id="b7e0d-788">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-788">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-789">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-789">settingsBlockAppsPage</span></span>|<span data-ttu-id="b7e0d-790">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-790">Boolean</span></span>|<span data-ttu-id="b7e0d-791">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-791">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-792">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-792">settingsBlockGamingPage</span></span>|<span data-ttu-id="b7e0d-793">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-793">Boolean</span></span>|<span data-ttu-id="b7e0d-794">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-794">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="b7e0d-795">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="b7e0d-795">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="b7e0d-796">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-796">Boolean</span></span>|<span data-ttu-id="b7e0d-797">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-797">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="b7e0d-798">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-798">windowsSpotlightBlocked</span></span>|<span data-ttu-id="b7e0d-799">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-799">Boolean</span></span>|<span data-ttu-id="b7e0d-800">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="b7e0d-800">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="b7e0d-801">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="b7e0d-801">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="b7e0d-802">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-802">Boolean</span></span>|<span data-ttu-id="b7e0d-803">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="b7e0d-803">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="b7e0d-804">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="b7e0d-804">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="b7e0d-805">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-805">Boolean</span></span>|<span data-ttu-id="b7e0d-806">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-806">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="b7e0d-807">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="b7e0d-807">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="b7e0d-808">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-808">Boolean</span></span>|<span data-ttu-id="b7e0d-809">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="b7e0d-809">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="b7e0d-810">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="b7e0d-810">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="b7e0d-811">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-811">Boolean</span></span>|<span data-ttu-id="b7e0d-812">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="b7e0d-812">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="b7e0d-813">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="b7e0d-813">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="b7e0d-814">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-814">Boolean</span></span>|<span data-ttu-id="b7e0d-815">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-815">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="b7e0d-816">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b7e0d-816">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="b7e0d-817">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="b7e0d-817">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="b7e0d-818">指定聚光灯的类型。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-818">Specifies the type of Spotlight.</span></span> <span data-ttu-id="b7e0d-819">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-819">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="b7e0d-820">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="b7e0d-820">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="b7e0d-821">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-821">Boolean</span></span>|<span data-ttu-id="b7e0d-822">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-822">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="b7e0d-823">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-823">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="b7e0d-824">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="b7e0d-824">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="b7e0d-825">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-825">Boolean</span></span>|<span data-ttu-id="b7e0d-826">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-826">Disable automatic detection of settings.</span></span> <span data-ttu-id="b7e0d-827">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-827">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="b7e0d-828">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b7e0d-828">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b7e0d-829">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-829">String</span></span>|<span data-ttu-id="b7e0d-830">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-830">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="b7e0d-831">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="b7e0d-831">networkProxyServer</span></span>|[<span data-ttu-id="b7e0d-832">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="b7e0d-832">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="b7e0d-833">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-833">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="b7e0d-834">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b7e0d-834">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="b7e0d-835">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-835">Boolean</span></span>|<span data-ttu-id="b7e0d-836">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-836">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="b7e0d-837">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-837">antiTheftModeBlocked</span></span>|<span data-ttu-id="b7e0d-838">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-838">Boolean</span></span>|<span data-ttu-id="b7e0d-839">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-839">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="b7e0d-840">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-840">bluetoothBlocked</span></span>|<span data-ttu-id="b7e0d-841">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-841">Boolean</span></span>|<span data-ttu-id="b7e0d-842">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-842">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="b7e0d-843">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-843">cameraBlocked</span></span>|<span data-ttu-id="b7e0d-844">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-844">Boolean</span></span>|<span data-ttu-id="b7e0d-845">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-845">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b7e0d-846">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-846">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="b7e0d-847">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-847">Boolean</span></span>|<span data-ttu-id="b7e0d-848">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-848">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="b7e0d-849">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="b7e0d-849">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="b7e0d-850">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-850">Boolean</span></span>|<span data-ttu-id="b7e0d-851">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-851">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="b7e0d-852">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-852">copyPasteBlocked</span></span>|<span data-ttu-id="b7e0d-853">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-853">Boolean</span></span>|<span data-ttu-id="b7e0d-854">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-854">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="b7e0d-855">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-855">cortanaBlocked</span></span>|<span data-ttu-id="b7e0d-856">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-856">Boolean</span></span>|<span data-ttu-id="b7e0d-857">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-857">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="b7e0d-858">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="b7e0d-858">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="b7e0d-859">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-859">Boolean</span></span>|<span data-ttu-id="b7e0d-860">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-860">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="b7e0d-861">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="b7e0d-861">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="b7e0d-862">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-862">Boolean</span></span>|<span data-ttu-id="b7e0d-863">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-863">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="b7e0d-864">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="b7e0d-864">safeSearchFilter</span></span>|[<span data-ttu-id="b7e0d-865">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="b7e0d-865">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="b7e0d-866">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-866">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="b7e0d-867">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-867">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="b7e0d-868">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b7e0d-868">edgeBlockPopups</span></span>|<span data-ttu-id="b7e0d-869">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-869">Boolean</span></span>|<span data-ttu-id="b7e0d-870">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-870">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="b7e0d-871">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="b7e0d-871">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="b7e0d-872">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-872">Boolean</span></span>|<span data-ttu-id="b7e0d-873">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-873">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="b7e0d-874">edgeBlockSearchEngineCustomization</span><span class="sxs-lookup"><span data-stu-id="b7e0d-874">edgeBlockSearchEngineCustomization</span></span>|<span data-ttu-id="b7e0d-875">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-875">Boolean</span></span>|<span data-ttu-id="b7e0d-876">指示是否阻止用户添加新的搜索引擎或更改默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-876">Indicates whether or not to block the user from adding new search engine or changing the default search engine.</span></span>|
|<span data-ttu-id="b7e0d-877">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b7e0d-877">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="b7e0d-878">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-878">Boolean</span></span>|<span data-ttu-id="b7e0d-879">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-879">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="b7e0d-880">注意: 此属性的名称是误导性的;属性已过时, 请改用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-880">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="b7e0d-881">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b7e0d-881">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="b7e0d-882">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-882">Boolean</span></span>|<span data-ttu-id="b7e0d-883">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-883">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="b7e0d-884">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="b7e0d-884">edgeRequireSmartScreen</span></span>|<span data-ttu-id="b7e0d-885">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-885">Boolean</span></span>|<span data-ttu-id="b7e0d-886">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-886">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="b7e0d-887">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="b7e0d-887">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="b7e0d-888">字符串</span><span class="sxs-lookup"><span data-stu-id="b7e0d-888">String</span></span>|<span data-ttu-id="b7e0d-889">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-889">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="b7e0d-890">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-890">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b7e0d-891">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="b7e0d-891">edgeFirstRunUrl</span></span>|<span data-ttu-id="b7e0d-892">String</span><span class="sxs-lookup"><span data-stu-id="b7e0d-892">String</span></span>|<span data-ttu-id="b7e0d-893">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-893">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="b7e0d-894">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="b7e0d-894">edgeSearchEngine</span></span>|[<span data-ttu-id="b7e0d-895">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="b7e0d-895">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="b7e0d-896">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-896">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="b7e0d-897">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-897">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="b7e0d-898">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="b7e0d-898">edgeHomepageUrls</span></span>|<span data-ttu-id="b7e0d-899">String 集合</span><span class="sxs-lookup"><span data-stu-id="b7e0d-899">String collection</span></span>|<span data-ttu-id="b7e0d-900">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-900">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="b7e0d-901">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="b7e0d-901">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="b7e0d-902">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-902">Boolean</span></span>|<span data-ttu-id="b7e0d-903">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-903">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="b7e0d-904">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="b7e0d-904">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="b7e0d-905">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-905">Boolean</span></span>|<span data-ttu-id="b7e0d-906">指示用户是否可以替代有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-906">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="b7e0d-907">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="b7e0d-907">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="b7e0d-908">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-908">Boolean</span></span>|<span data-ttu-id="b7e0d-909">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="b7e0d-909">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="b7e0d-910">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="b7e0d-910">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="b7e0d-911">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-911">Boolean</span></span>|<span data-ttu-id="b7e0d-912">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="b7e0d-912">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="b7e0d-913">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-913">internetSharingBlocked</span></span>|<span data-ttu-id="b7e0d-914">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-914">Boolean</span></span>|<span data-ttu-id="b7e0d-915">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-915">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="b7e0d-916">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-916">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="b7e0d-917">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-917">Boolean</span></span>|<span data-ttu-id="b7e0d-918">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-918">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="b7e0d-919">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-919">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="b7e0d-920">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-920">Boolean</span></span>|<span data-ttu-id="b7e0d-921">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-921">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="b7e0d-922">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="b7e0d-922">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="b7e0d-923">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-923">Boolean</span></span>|<span data-ttu-id="b7e0d-924">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-924">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="b7e0d-925">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="b7e0d-925">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="b7e0d-926">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-926">Boolean</span></span>|<span data-ttu-id="b7e0d-927">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-927">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="b7e0d-928">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="b7e0d-928">settingsBlockChangeRegion</span></span>|<span data-ttu-id="b7e0d-929">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-929">Boolean</span></span>|<span data-ttu-id="b7e0d-930">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-930">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="b7e0d-931">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-931">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="b7e0d-932">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-932">Boolean</span></span>|<span data-ttu-id="b7e0d-933">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-933">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="b7e0d-934">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="b7e0d-934">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="b7e0d-935">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-935">Boolean</span></span>|<span data-ttu-id="b7e0d-936">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-936">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="b7e0d-937">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-937">locationServicesBlocked</span></span>|<span data-ttu-id="b7e0d-938">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-938">Boolean</span></span>|<span data-ttu-id="b7e0d-939">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-939">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="b7e0d-940">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-940">microsoftAccountBlocked</span></span>|<span data-ttu-id="b7e0d-941">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-941">Boolean</span></span>|<span data-ttu-id="b7e0d-942">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-942">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="b7e0d-943">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="b7e0d-943">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="b7e0d-944">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-944">Boolean</span></span>|<span data-ttu-id="b7e0d-945">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-945">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="b7e0d-946">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-946">nfcBlocked</span></span>|<span data-ttu-id="b7e0d-947">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-947">Boolean</span></span>|<span data-ttu-id="b7e0d-948">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-948">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="b7e0d-949">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-949">resetProtectionModeBlocked</span></span>|<span data-ttu-id="b7e0d-950">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-950">Boolean</span></span>|<span data-ttu-id="b7e0d-951">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-951">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="b7e0d-952">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-952">screenCaptureBlocked</span></span>|<span data-ttu-id="b7e0d-953">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-953">Boolean</span></span>|<span data-ttu-id="b7e0d-954">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-954">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b7e0d-955">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="b7e0d-955">storageBlockRemovableStorage</span></span>|<span data-ttu-id="b7e0d-956">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-956">Boolean</span></span>|<span data-ttu-id="b7e0d-957">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-957">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="b7e0d-958">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="b7e0d-958">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="b7e0d-959">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-959">Boolean</span></span>|<span data-ttu-id="b7e0d-960">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-960">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="b7e0d-961">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-961">usbBlocked</span></span>|<span data-ttu-id="b7e0d-962">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-962">Boolean</span></span>|<span data-ttu-id="b7e0d-963">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-963">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="b7e0d-964">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-964">voiceRecordingBlocked</span></span>|<span data-ttu-id="b7e0d-965">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-965">Boolean</span></span>|<span data-ttu-id="b7e0d-966">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-966">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="b7e0d-967">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="b7e0d-967">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="b7e0d-968">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-968">Boolean</span></span>|<span data-ttu-id="b7e0d-969">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-969">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="b7e0d-970">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-970">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b7e0d-971">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-971">wiFiBlocked</span></span>|<span data-ttu-id="b7e0d-972">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-972">Boolean</span></span>|<span data-ttu-id="b7e0d-973">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-973">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="b7e0d-974">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="b7e0d-974">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="b7e0d-975">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-975">Boolean</span></span>|<span data-ttu-id="b7e0d-976">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-976">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="b7e0d-977">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="b7e0d-977">wiFiScanInterval</span></span>|<span data-ttu-id="b7e0d-978">Int32</span><span class="sxs-lookup"><span data-stu-id="b7e0d-978">Int32</span></span>|<span data-ttu-id="b7e0d-979">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-979">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="b7e0d-980">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-980">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="b7e0d-981">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="b7e0d-981">Valid values 1 to 500</span></span>|
|<span data-ttu-id="b7e0d-982">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="b7e0d-982">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="b7e0d-983">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-983">Boolean</span></span>|<span data-ttu-id="b7e0d-984">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-984">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="b7e0d-985">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="b7e0d-985">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="b7e0d-986">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-986">Boolean</span></span>|<span data-ttu-id="b7e0d-987">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-987">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="b7e0d-988">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="b7e0d-988">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="b7e0d-989">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-989">Boolean</span></span>|<span data-ttu-id="b7e0d-990">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-990">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="b7e0d-991">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-991">windowsStoreBlocked</span></span>|<span data-ttu-id="b7e0d-992">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-992">Boolean</span></span>|<span data-ttu-id="b7e0d-993">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-993">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="b7e0d-994">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="b7e0d-994">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="b7e0d-995">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-995">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b7e0d-996">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-996">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="b7e0d-997">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-997">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b7e0d-998">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="b7e0d-998">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="b7e0d-999">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-999">Boolean</span></span>|<span data-ttu-id="b7e0d-1000">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1000">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="b7e0d-1001">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1001">developerUnlockSetting</span></span>|[<span data-ttu-id="b7e0d-1002">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1002">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b7e0d-1003">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1003">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="b7e0d-1004">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1004">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b7e0d-1005">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1005">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="b7e0d-1006">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1006">Boolean</span></span>|<span data-ttu-id="b7e0d-1007">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1007">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="b7e0d-1008">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1008">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="b7e0d-1009">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1009">Boolean</span></span>|<span data-ttu-id="b7e0d-1010">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1010">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="b7e0d-1011">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1011">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="b7e0d-1012">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1012">Boolean</span></span>|<span data-ttu-id="b7e0d-1013">指示是否启用“仅限专用应用商店”。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1013">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="b7e0d-1014">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1014">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="b7e0d-1015">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1015">Boolean</span></span>|<span data-ttu-id="b7e0d-1016">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1016">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="b7e0d-1017">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1017">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="b7e0d-1018">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1018">Boolean</span></span>|<span data-ttu-id="b7e0d-1019">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1019">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="b7e0d-1020">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1020">gameDvrBlocked</span></span>|<span data-ttu-id="b7e0d-1021">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1021">Boolean</span></span>|<span data-ttu-id="b7e0d-1022">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1022">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="b7e0d-1023">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1023">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="b7e0d-1024">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1024">Boolean</span></span>|<span data-ttu-id="b7e0d-1025">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1025">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="b7e0d-1026">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1026">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="b7e0d-1027">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1027">Boolean</span></span>|<span data-ttu-id="b7e0d-1028">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1028">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="b7e0d-1029">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1029">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="b7e0d-1030">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1030">Boolean</span></span>|<span data-ttu-id="b7e0d-1031">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1031">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="b7e0d-1032">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1032">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="b7e0d-1033">Boolean</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1033">Boolean</span></span>|<span data-ttu-id="b7e0d-1034">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1034">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="b7e0d-1035">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1035">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="b7e0d-1036">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1036">Boolean</span></span>|<span data-ttu-id="b7e0d-1037">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1037">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="b7e0d-1038">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1038">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="b7e0d-1039">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1039">Boolean</span></span>|<span data-ttu-id="b7e0d-1040">此策略设置允许用户更改通常仅供系统管理员使用的安装选项。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1040">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="b7e0d-1041">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1041">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="b7e0d-1042">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1042">Boolean</span></span>|<span data-ttu-id="b7e0d-1043">此策略设置指示 Windows Installer 在系统上安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1043">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="b7e0d-1044">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1044">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="b7e0d-1045">布尔</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1045">Boolean</span></span>|<span data-ttu-id="b7e0d-1046">通过此策略设置, 您可以阻止所有热插拔 PCI 下游端口的直接内存访问 (DMA), 直到用户登录 Windows。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1046">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|
|<span data-ttu-id="b7e0d-1047">appManagementPackageFamilyNamesToLaunchAfterLogOn</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1047">appManagementPackageFamilyNamesToLaunchAfterLogOn</span></span>|<span data-ttu-id="b7e0d-1048">String collection</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1048">String collection</span></span>|<span data-ttu-id="b7e0d-1049">Windows 应用的以分号分隔的程序包系列名称的列表。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1049">List of semi-colon delimited Package Family Names of Windows apps.</span></span> <span data-ttu-id="b7e0d-1050">登录后将启动列出的 Windows 应用。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1050">Listed Windows apps are to be launched after logon.</span></span>|



## <a name="response"></a><span data-ttu-id="b7e0d-1051">响应</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1051">Response</span></span>
<span data-ttu-id="b7e0d-1052">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1052">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7e0d-1053">示例</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1053">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7e0d-1054">请求</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1054">Request</span></span>
<span data-ttu-id="b7e0d-1055">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1055">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 13518

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="b7e0d-1056">响应</span><span class="sxs-lookup"><span data-stu-id="b7e0d-1056">Response</span></span>
<span data-ttu-id="b7e0d-p180">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b7e0d-p180">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 13690

{
  "@odata.type": "#microsoft.graph.windows10GeneralConfiguration",
  "id": "a4235d71-5d71-a423-715d-23a4715d23a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





