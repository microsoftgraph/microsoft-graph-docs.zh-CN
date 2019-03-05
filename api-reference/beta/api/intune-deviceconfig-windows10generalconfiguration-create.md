---
title: 创建 windows10GeneralConfiguration
description: 创建新的 windows10GeneralConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 96e51858dbd5b4268a4e663f49ec5dc0c5734f59
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159799"
---
# <a name="create-windows10generalconfiguration"></a><span data-ttu-id="3dfaa-103">创建 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dfaa-103">Create windows10GeneralConfiguration</span></span>

> <span data-ttu-id="3dfaa-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3dfaa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3dfaa-106">创建新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-106">Create a new [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3dfaa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3dfaa-107">Prerequisites</span></span>
<span data-ttu-id="3dfaa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3dfaa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3dfaa-110">Permission type</span></span>|<span data-ttu-id="3dfaa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3dfaa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3dfaa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfaa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3dfaa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3dfaa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3dfaa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3dfaa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3dfaa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-115">Not supported.</span></span>|
|<span data-ttu-id="3dfaa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3dfaa-116">Application</span></span>|<span data-ttu-id="3dfaa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3dfaa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3dfaa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3dfaa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3dfaa-119">Request headers</span></span>
|<span data-ttu-id="3dfaa-120">标头</span><span class="sxs-lookup"><span data-stu-id="3dfaa-120">Header</span></span>|<span data-ttu-id="3dfaa-121">值</span><span class="sxs-lookup"><span data-stu-id="3dfaa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3dfaa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3dfaa-122">Authorization</span></span>|<span data-ttu-id="3dfaa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3dfaa-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3dfaa-124">Accept</span></span>|<span data-ttu-id="3dfaa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3dfaa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3dfaa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3dfaa-126">Request body</span></span>
<span data-ttu-id="3dfaa-127">在请求正文中，提供 windows10GeneralConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-127">In the request body, supply a JSON representation for the windows10GeneralConfiguration object.</span></span>

<span data-ttu-id="3dfaa-128">下表显示了创建 windows10GeneralConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-128">The following table shows the properties that are required when you create the windows10GeneralConfiguration.</span></span>

|<span data-ttu-id="3dfaa-129">属性</span><span class="sxs-lookup"><span data-stu-id="3dfaa-129">Property</span></span>|<span data-ttu-id="3dfaa-130">类型</span><span class="sxs-lookup"><span data-stu-id="3dfaa-130">Type</span></span>|<span data-ttu-id="3dfaa-131">说明</span><span class="sxs-lookup"><span data-stu-id="3dfaa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3dfaa-132">id</span><span class="sxs-lookup"><span data-stu-id="3dfaa-132">id</span></span>|<span data-ttu-id="3dfaa-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3dfaa-133">String</span></span>|<span data-ttu-id="3dfaa-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-134">Key of the entity.</span></span> <span data-ttu-id="3dfaa-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dfaa-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dfaa-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3dfaa-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3dfaa-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfaa-137">DateTimeOffset</span></span>|<span data-ttu-id="3dfaa-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3dfaa-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dfaa-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dfaa-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3dfaa-140">roleScopeTagIds</span></span>|<span data-ttu-id="3dfaa-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-141">String collection</span></span>|<span data-ttu-id="3dfaa-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3dfaa-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dfaa-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dfaa-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3dfaa-144">supportsScopeTags</span></span>|<span data-ttu-id="3dfaa-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-145">Boolean</span></span>|<span data-ttu-id="3dfaa-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3dfaa-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3dfaa-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3dfaa-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-149">This property is read-only.</span></span> <span data-ttu-id="3dfaa-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dfaa-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dfaa-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3dfaa-151">createdDateTime</span></span>|<span data-ttu-id="3dfaa-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3dfaa-152">DateTimeOffset</span></span>|<span data-ttu-id="3dfaa-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-153">DateTime the object was created.</span></span> <span data-ttu-id="3dfaa-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dfaa-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dfaa-155">description</span><span class="sxs-lookup"><span data-stu-id="3dfaa-155">description</span></span>|<span data-ttu-id="3dfaa-156">字符串</span><span class="sxs-lookup"><span data-stu-id="3dfaa-156">String</span></span>|<span data-ttu-id="3dfaa-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3dfaa-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dfaa-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dfaa-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3dfaa-159">displayName</span></span>|<span data-ttu-id="3dfaa-160">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-160">String</span></span>|<span data-ttu-id="3dfaa-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3dfaa-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dfaa-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dfaa-163">version</span><span class="sxs-lookup"><span data-stu-id="3dfaa-163">version</span></span>|<span data-ttu-id="3dfaa-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-164">Int32</span></span>|<span data-ttu-id="3dfaa-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-165">Version of the device configuration.</span></span> <span data-ttu-id="3dfaa-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3dfaa-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3dfaa-167">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="3dfaa-167">taskManagerBlockEndTask</span></span>|<span data-ttu-id="3dfaa-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-168">Boolean</span></span>|<span data-ttu-id="3dfaa-169">指定非管理员是否可以使用任务管理器结束任务。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-169">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="3dfaa-170">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="3dfaa-170">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="3dfaa-171">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="3dfaa-171">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="3dfaa-172">应用的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-172">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="3dfaa-173">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="3dfaa-173">enableAutomaticRedeployment</span></span>|<span data-ttu-id="3dfaa-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-174">Boolean</span></span>|<span data-ttu-id="3dfaa-175">允许具有管理权限的用户在设备锁屏的屏幕上使用 CTRL + Win + R 删除所有用户数据和设置, 以便可以自动重新配置设备并将其重新注册到管理中。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-175">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="3dfaa-176">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="3dfaa-176">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="3dfaa-177">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="3dfaa-177">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="3dfaa-178">控制 Microsoft 帐户登录助手 (wlidsvc) NT 服务。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-178">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="3dfaa-179">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-179">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="3dfaa-180">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="3dfaa-180">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="3dfaa-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-181">Boolean</span></span>|<span data-ttu-id="3dfaa-182">允许辅助身份验证设备使用 Windows。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-182">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="3dfaa-183">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="3dfaa-183">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="3dfaa-184">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-184">String</span></span>|<span data-ttu-id="3dfaa-185">指定 Azure AD 租户中可用域之间的首选域。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-185">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="3dfaa-186">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="3dfaa-186">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="3dfaa-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-187">Boolean</span></span>|<span data-ttu-id="3dfaa-188">指定是否允许或禁止联邦信息处理标准 (FIPS) 策略。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-188">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="3dfaa-189">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="3dfaa-189">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="3dfaa-190">String collection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-190">String collection</span></span>|<span data-ttu-id="3dfaa-191">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-191">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="3dfaa-192">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="3dfaa-192">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="3dfaa-193">String collection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-193">String collection</span></span>|<span data-ttu-id="3dfaa-194">启用了 GDI DPI 缩放的旧版应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-194">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="3dfaa-195">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="3dfaa-195">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="3dfaa-196">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-196">String</span></span>|<span data-ttu-id="3dfaa-197">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-197">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="3dfaa-198">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="3dfaa-198">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="3dfaa-199">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-199">String</span></span>|<span data-ttu-id="3dfaa-200">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-200">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="3dfaa-201">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="3dfaa-201">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="3dfaa-202">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-202">String</span></span>|<span data-ttu-id="3dfaa-203">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-203">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="3dfaa-204">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3dfaa-204">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="3dfaa-205">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-205">String</span></span>|<span data-ttu-id="3dfaa-206">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-206">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="3dfaa-207">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="3dfaa-207">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="3dfaa-208">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-208">Int32</span></span>|<span data-ttu-id="3dfaa-209">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-209">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="3dfaa-210">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-210">This is a mobile only setting.</span></span> <span data-ttu-id="3dfaa-211">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="3dfaa-211">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="3dfaa-212">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="3dfaa-212">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="3dfaa-213">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-213">String</span></span>|<span data-ttu-id="3dfaa-214">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-214">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="3dfaa-215">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="3dfaa-215">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="3dfaa-216">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-216">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="3dfaa-217">允许或阻止同步 Microsoft Edge 浏览器设置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-217">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="3dfaa-218">选项可供 IT 管理员阻止跨设备同步, 但允许用户替代。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-218">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="3dfaa-219">可取值为：`notConfigured`、`blockedWithUserOverride`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-219">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="3dfaa-220">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="3dfaa-220">messagingBlockSync</span></span>|<span data-ttu-id="3dfaa-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-221">Boolean</span></span>|<span data-ttu-id="3dfaa-222">指示是否在所有位置阻止短信备份和还原和消息传递。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-222">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="3dfaa-223">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="3dfaa-223">messagingBlockMMS</span></span>|<span data-ttu-id="3dfaa-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-224">Boolean</span></span>|<span data-ttu-id="3dfaa-225">指示是否阻止设备上的 MMS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-225">Indicates whether or not to block the the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="3dfaa-226">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="3dfaa-226">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="3dfaa-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-227">Boolean</span></span>|<span data-ttu-id="3dfaa-228">指示是否阻止设备上的 RCS 发送/接收功能。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-228">Indicates whether or not to block the the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="3dfaa-229">printerNames</span><span class="sxs-lookup"><span data-stu-id="3dfaa-229">printerNames</span></span>|<span data-ttu-id="3dfaa-230">String collection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-230">String collection</span></span>|<span data-ttu-id="3dfaa-231">根据打印机的名称 (网络主机名称) 自动预配打印机。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-231">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="3dfaa-232">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="3dfaa-232">printerDefaultName</span></span>|<span data-ttu-id="3dfaa-233">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-233">String</span></span>|<span data-ttu-id="3dfaa-234">已安装的打印机的名称 (网络主机名称)。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-234">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="3dfaa-235">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="3dfaa-235">printerBlockAddition</span></span>|<span data-ttu-id="3dfaa-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-236">Boolean</span></span>|<span data-ttu-id="3dfaa-237">阻止用户安装来自打印机设置的其他打印机。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-237">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="3dfaa-238">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="3dfaa-238">searchBlockDiacritics</span></span>|<span data-ttu-id="3dfaa-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-239">Boolean</span></span>|<span data-ttu-id="3dfaa-240">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-240">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="3dfaa-241">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-241">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="3dfaa-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-242">Boolean</span></span>|<span data-ttu-id="3dfaa-243">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-243">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="3dfaa-244">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="3dfaa-244">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="3dfaa-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-245">Boolean</span></span>|<span data-ttu-id="3dfaa-246">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-246">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="3dfaa-247">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="3dfaa-247">searchEnableRemoteQueries</span></span>|<span data-ttu-id="3dfaa-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-248">Boolean</span></span>|<span data-ttu-id="3dfaa-249">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-249">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="3dfaa-250">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="3dfaa-250">searchDisableUseLocation</span></span>|<span data-ttu-id="3dfaa-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-251">Boolean</span></span>|<span data-ttu-id="3dfaa-252">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-252">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="3dfaa-253">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="3dfaa-253">searchDisableLocation</span></span>|<span data-ttu-id="3dfaa-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-254">Boolean</span></span>|<span data-ttu-id="3dfaa-255">指定搜索是否可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-255">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="3dfaa-256">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="3dfaa-256">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="3dfaa-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-257">Boolean</span></span>|<span data-ttu-id="3dfaa-258">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-258">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="3dfaa-259">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="3dfaa-259">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="3dfaa-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-260">Boolean</span></span>|<span data-ttu-id="3dfaa-261">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-261">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="3dfaa-262">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="3dfaa-262">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="3dfaa-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-263">Boolean</span></span>|<span data-ttu-id="3dfaa-264">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-264">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="3dfaa-265">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="3dfaa-265">searchBlockWebResults</span></span>|<span data-ttu-id="3dfaa-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-266">Boolean</span></span>|<span data-ttu-id="3dfaa-267">指示是否阻止 web 搜索。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-267">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="3dfaa-268">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="3dfaa-268">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="3dfaa-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-269">Boolean</span></span>|<span data-ttu-id="3dfaa-270">在设备已加入 Azure AD 时, 指定是否允许在 OOBE 期间自动设备加密 (仅限桌面)。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-270">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="3dfaa-271">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="3dfaa-271">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="3dfaa-272">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="3dfaa-272">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="3dfaa-273">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-273">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="3dfaa-274">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-274">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="3dfaa-275">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="3dfaa-275">oneDriveDisableFileSync</span></span>|<span data-ttu-id="3dfaa-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-276">Boolean</span></span>|<span data-ttu-id="3dfaa-277">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-277">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="3dfaa-278">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="3dfaa-278">systemTelemetryProxyServer</span></span>|<span data-ttu-id="3dfaa-279">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-279">String</span></span>|<span data-ttu-id="3dfaa-280">获取或设置代理服务器的完全限定域名 (FQDN) 或 IP 地址, 以转发连接的用户体验和遥测请求。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-280">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="3dfaa-281">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="3dfaa-281">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="3dfaa-282">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="3dfaa-282">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="3dfaa-283">指定将哪种类型的遥测数据 (无、intranet、internet、两者) 发送到 Microsoft 365 Analytics。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-283">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="3dfaa-284">可取值为：`notConfigured`、`intranet`、`internet`、`intranetAndInternet`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-284">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="3dfaa-285">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="3dfaa-285">inkWorkspaceAccess</span></span>|[<span data-ttu-id="3dfaa-286">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-286">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="3dfaa-287">控制用户对墨迹工作区的访问权限, 从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-287">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="3dfaa-288">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-288">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="3dfaa-289">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="3dfaa-289">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="3dfaa-290">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-290">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="3dfaa-291">控制用户对墨迹工作区的访问权限, 从桌面和锁定屏幕上。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-291">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="3dfaa-292">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-292">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="3dfaa-293">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="3dfaa-293">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="3dfaa-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-294">Boolean</span></span>|<span data-ttu-id="3dfaa-295">指定是否在墨迹工作区中显示建议的应用建议。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-295">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="3dfaa-296">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="3dfaa-296">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="3dfaa-297">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-297">Boolean</span></span>|<span data-ttu-id="3dfaa-298">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-298">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="3dfaa-299">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="3dfaa-299">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="3dfaa-300">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-300">String</span></span>|<span data-ttu-id="3dfaa-301">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-301">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="3dfaa-302">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="3dfaa-302">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="3dfaa-303">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-303">String</span></span>|<span data-ttu-id="3dfaa-304">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-304">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="3dfaa-305">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="3dfaa-305">bluetoothAllowedServices</span></span>|<span data-ttu-id="3dfaa-306">String 集合</span><span class="sxs-lookup"><span data-stu-id="3dfaa-306">String collection</span></span>|<span data-ttu-id="3dfaa-307">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-307">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="3dfaa-308">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="3dfaa-308">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="3dfaa-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-309">Boolean</span></span>|<span data-ttu-id="3dfaa-310">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-310">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="3dfaa-311">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="3dfaa-311">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="3dfaa-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-312">Boolean</span></span>|<span data-ttu-id="3dfaa-313">是否阻止用户使用 Swift 对和其他基于邻近的应用场景。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-313">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="3dfaa-314">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="3dfaa-314">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="3dfaa-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-315">Boolean</span></span>|<span data-ttu-id="3dfaa-316">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-316">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="3dfaa-317">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="3dfaa-317">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="3dfaa-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-318">Boolean</span></span>|<span data-ttu-id="3dfaa-319">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-319">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="3dfaa-320">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="3dfaa-320">edgeBlockAutofill</span></span>|<span data-ttu-id="3dfaa-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-321">Boolean</span></span>|<span data-ttu-id="3dfaa-322">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-322">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="3dfaa-323">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-323">edgeBlocked</span></span>|<span data-ttu-id="3dfaa-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-324">Boolean</span></span>|<span data-ttu-id="3dfaa-325">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-325">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="3dfaa-326">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="3dfaa-326">edgeCookiePolicy</span></span>|[<span data-ttu-id="3dfaa-327">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="3dfaa-327">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="3dfaa-328">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-328">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="3dfaa-329">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-329">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="3dfaa-330">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="3dfaa-330">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="3dfaa-331">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-331">Boolean</span></span>|<span data-ttu-id="3dfaa-332">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-332">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="3dfaa-333">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="3dfaa-333">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="3dfaa-334">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-334">Boolean</span></span>|<span data-ttu-id="3dfaa-335">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-335">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="3dfaa-336">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="3dfaa-336">edgeBlockExtensions</span></span>|<span data-ttu-id="3dfaa-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-337">Boolean</span></span>|<span data-ttu-id="3dfaa-338">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-338">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="3dfaa-339">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="3dfaa-339">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="3dfaa-340">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-340">Boolean</span></span>|<span data-ttu-id="3dfaa-341">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-341">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="3dfaa-342">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="3dfaa-342">edgeBlockJavaScript</span></span>|<span data-ttu-id="3dfaa-343">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-343">Boolean</span></span>|<span data-ttu-id="3dfaa-344">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-344">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="3dfaa-345">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="3dfaa-345">edgeBlockPasswordManager</span></span>|<span data-ttu-id="3dfaa-346">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-346">Boolean</span></span>|<span data-ttu-id="3dfaa-347">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-347">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="3dfaa-348">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="3dfaa-348">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="3dfaa-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-349">Boolean</span></span>|<span data-ttu-id="3dfaa-350">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-350">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="3dfaa-351">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-351">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="3dfaa-352">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="3dfaa-352">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="3dfaa-353">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-353">Boolean</span></span>|<span data-ttu-id="3dfaa-354">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-354">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="3dfaa-355">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-355">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="3dfaa-356">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="3dfaa-356">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="3dfaa-357">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-357">Boolean</span></span>|<span data-ttu-id="3dfaa-358">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-358">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="3dfaa-359">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="3dfaa-359">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="3dfaa-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-360">Boolean</span></span>|<span data-ttu-id="3dfaa-361">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-361">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="3dfaa-362">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-362">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="3dfaa-363">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-363">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="3dfaa-364">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-364">Boolean</span></span>|<span data-ttu-id="3dfaa-365">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-365">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="3dfaa-366">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-366">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="3dfaa-367">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-367">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="3dfaa-368">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-368">Boolean</span></span>|<span data-ttu-id="3dfaa-369">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-369">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="3dfaa-370">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="3dfaa-370">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="3dfaa-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-371">Boolean</span></span>|<span data-ttu-id="3dfaa-372">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-372">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="3dfaa-373">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-373">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="3dfaa-374">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="3dfaa-374">edgeFavoritesListLocation</span></span>|<span data-ttu-id="3dfaa-375">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-375">String</span></span>|<span data-ttu-id="3dfaa-376">要设置的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-376">The location of the favorites list to provision.</span></span> <span data-ttu-id="3dfaa-377">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-377">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="3dfaa-378">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="3dfaa-378">edgeBlockEditFavorites</span></span>|<span data-ttu-id="3dfaa-379">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-379">Boolean</span></span>|<span data-ttu-id="3dfaa-380">指示是否阻止用户对收藏夹进行更改。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-380">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="3dfaa-381">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="3dfaa-381">edgeNewTabPageURL</span></span>|<span data-ttu-id="3dfaa-382">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-382">String</span></span>|<span data-ttu-id="3dfaa-383">指定在创建新选项卡时打开的页面。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-383">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="3dfaa-384">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dfaa-384">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="3dfaa-385">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dfaa-385">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="3dfaa-386">使 Home 按钮可以隐藏、加载默认起始页、加载新的选项卡页或自定义 URL</span><span class="sxs-lookup"><span data-stu-id="3dfaa-386">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="3dfaa-387">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="3dfaa-387">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="3dfaa-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-388">Boolean</span></span>|<span data-ttu-id="3dfaa-389">启用 "主页" 按钮配置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-389">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="3dfaa-390">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="3dfaa-390">edgeOpensWith</span></span>|[<span data-ttu-id="3dfaa-391">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="3dfaa-391">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="3dfaa-392">指定在开始时打开的页面类型。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-392">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="3dfaa-393">可取值为：`notConfigured`、`startPage`、`newTabPage`、`previousPages`、`specificPages`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-393">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="3dfaa-394">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="3dfaa-394">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="3dfaa-395">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-395">Boolean</span></span>|<span data-ttu-id="3dfaa-396">指示用户是否可以旁加载扩展。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-396">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="3dfaa-397">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="3dfaa-397">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="3dfaa-398">String collection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-398">String collection</span></span>|<span data-ttu-id="3dfaa-399">指定所需的浏览器扩展的程序包系列名称列表, 用户无法关闭这些扩展。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-399">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="3dfaa-400">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-400">edgeBlockPrinting</span></span>|<span data-ttu-id="3dfaa-401">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-401">Boolean</span></span>|<span data-ttu-id="3dfaa-402">将 Edge 配置为允许或阻止打印。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-402">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="3dfaa-403">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="3dfaa-403">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="3dfaa-404">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-404">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-405">获取或设置一个值, 该值指定是否将收藏夹栏设置为始终在任何页面上都可见或隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-405">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="3dfaa-406">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-406">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-407">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="3dfaa-407">edgeBlockSavingHistory</span></span>|<span data-ttu-id="3dfaa-408">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-408">Boolean</span></span>|<span data-ttu-id="3dfaa-409">将 Edge 配置为允许保存浏览历史记录或从不保存浏览历史记录。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-409">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="3dfaa-410">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="3dfaa-410">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="3dfaa-411">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-411">Boolean</span></span>|<span data-ttu-id="3dfaa-412">允许或阻止边缘进入全屏模式。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-412">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="3dfaa-413">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-413">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="3dfaa-414">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-414">Boolean</span></span>|<span data-ttu-id="3dfaa-415">将配置为在 Edge 中加载空白页面, 而不是默认的新选项卡页面, 并防止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-415">Configure to load a blank page in Edge instead of the default New tab page and prevent users from changing it.</span></span>|
|<span data-ttu-id="3dfaa-416">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="3dfaa-416">edgeBlockTabPreloading</span></span>|<span data-ttu-id="3dfaa-417">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-417">Boolean</span></span>|<span data-ttu-id="3dfaa-418">配置边缘是否在 Windows 启动时预加载新的选项卡页。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-418">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="3dfaa-419">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="3dfaa-419">edgeBlockPrelaunch</span></span>|<span data-ttu-id="3dfaa-420">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-420">Boolean</span></span>|<span data-ttu-id="3dfaa-421">确定 Microsoft Edge 在 Windows 启动时是否为 prelaunched。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-421">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="3dfaa-422">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="3dfaa-422">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="3dfaa-423">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-423">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="3dfaa-424">控制边缘在切换到 Internet Explorer 之前显示的消息。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-424">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="3dfaa-425">可取值为：`notConfigured`、`disabled`、`enabled`、`keepGoing`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-425">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="3dfaa-426">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="3dfaa-426">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="3dfaa-427">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-427">Boolean</span></span>|<span data-ttu-id="3dfaa-428">允许或阻止用户覆盖证书错误。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-428">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="3dfaa-429">edgeKioskModeRestriction</span><span class="sxs-lookup"><span data-stu-id="3dfaa-429">edgeKioskModeRestriction</span></span>|[<span data-ttu-id="3dfaa-430">edgeKioskModeRestrictionType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-430">edgeKioskModeRestrictionType</span></span>](../resources/intune-deviceconfig-edgekioskmoderestrictiontype.md)|<span data-ttu-id="3dfaa-431">根据配置展台模式, 控制 Microsoft Edge 设置的限制方式。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-431">Controls how the Microsoft Edge settings are restricted based on the configure kiosk mode.</span></span> <span data-ttu-id="3dfaa-432">可取值为：`notConfigured`、`digitalSignage`、`normalMode`、`publicBrowsingSingleApp`、`publicBrowsingMultiApp`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-432">Possible values are: `notConfigured`, `digitalSignage`, `normalMode`, `publicBrowsingSingleApp`, `publicBrowsingMultiApp`.</span></span>|
|<span data-ttu-id="3dfaa-433">edgeKioskResetAfterIdleTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="3dfaa-433">edgeKioskResetAfterIdleTimeInMinutes</span></span>|<span data-ttu-id="3dfaa-434">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-434">Int32</span></span>|<span data-ttu-id="3dfaa-435">指定在 Microsoft Edge 展台重置前的上次用户活动的时间 (以分钟为单位)。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-435">Specifies the time in minutes from the last user activity before Microsoft Edge kiosk resets.</span></span>  <span data-ttu-id="3dfaa-436">有效值为0-1440。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-436">Valid values are 0-1440.</span></span> <span data-ttu-id="3dfaa-437">默认值为 5。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-437">The default is 5.</span></span> <span data-ttu-id="3dfaa-438">0表示不重置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-438">0 indicates no reset.</span></span> <span data-ttu-id="3dfaa-439">有效值为0至1440</span><span class="sxs-lookup"><span data-stu-id="3dfaa-439">Valid values 0 to 1440</span></span>|
|<span data-ttu-id="3dfaa-440">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="3dfaa-440">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="3dfaa-441">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-441">Boolean</span></span>|<span data-ttu-id="3dfaa-442">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-442">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="3dfaa-443">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="3dfaa-443">cellularBlockVpn</span></span>|<span data-ttu-id="3dfaa-444">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-444">Boolean</span></span>|<span data-ttu-id="3dfaa-445">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-445">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="3dfaa-446">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="3dfaa-446">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="3dfaa-447">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-447">Boolean</span></span>|<span data-ttu-id="3dfaa-448">是否阻止用户在通过手机网络漫游时使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-448">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="3dfaa-449">cellularData</span><span class="sxs-lookup"><span data-stu-id="3dfaa-449">cellularData</span></span>|[<span data-ttu-id="3dfaa-450">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-450">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="3dfaa-451">是否允许设备上的手机网络数据通道。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-451">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="3dfaa-452">如果未配置, 则允许手机网络数据通道, 用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-452">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="3dfaa-453">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-453">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="3dfaa-454">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="3dfaa-454">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="3dfaa-455">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-455">Boolean</span></span>|<span data-ttu-id="3dfaa-456">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-456">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="3dfaa-457">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="3dfaa-457">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="3dfaa-458">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-458">Int32</span></span>|<span data-ttu-id="3dfaa-459">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-459">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="3dfaa-460">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="3dfaa-460">Valid values 0 to 90</span></span>|
|<span data-ttu-id="3dfaa-461">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="3dfaa-461">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="3dfaa-462">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="3dfaa-462">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="3dfaa-463">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-463">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="3dfaa-464">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="3dfaa-464">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="3dfaa-465">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="3dfaa-465">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="3dfaa-466">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-466">Defender day of the week for the system scan.</span></span> <span data-ttu-id="3dfaa-467">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-467">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="3dfaa-468">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="3dfaa-468">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="3dfaa-469">String collection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-469">String collection</span></span>|<span data-ttu-id="3dfaa-470">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-470">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="3dfaa-471">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="3dfaa-471">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="3dfaa-472">String collection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-472">String collection</span></span>|<span data-ttu-id="3dfaa-473">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-473">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="3dfaa-474">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="3dfaa-474">defenderScanMaxCpu</span></span>|<span data-ttu-id="3dfaa-475">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-475">Int32</span></span>|<span data-ttu-id="3dfaa-476">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-476">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="3dfaa-477">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="3dfaa-477">Valid values 0 to 100</span></span>|
|<span data-ttu-id="3dfaa-478">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="3dfaa-478">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="3dfaa-479">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="3dfaa-479">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="3dfaa-480">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-480">Value for monitoring file activity.</span></span> <span data-ttu-id="3dfaa-481">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-481">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="3dfaa-482">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="3dfaa-482">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="3dfaa-483">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="3dfaa-483">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="3dfaa-484">获取或设置要对可能有害的应用程序 (PUA) 执行的 Defender 操作, 其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时, Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-484">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="3dfaa-485">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-485">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="3dfaa-486">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-486">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="3dfaa-487">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-487">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="3dfaa-488">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-488">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="3dfaa-489">获取或设置要对可能有害的应用程序 (PUA) 执行的 Defender 操作, 其中包括具有广告注入行为的软件、软件捆绑软件绑定、付款或订阅的永久请求等。下载 PUA 或尝试自行安装时, Defender 会通知用户。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-489">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="3dfaa-490">在 Windows 10 中添加的桌面。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-490">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="3dfaa-491">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-491">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="3dfaa-492">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="3dfaa-492">defenderProcessesToExclude</span></span>|<span data-ttu-id="3dfaa-493">String 集合</span><span class="sxs-lookup"><span data-stu-id="3dfaa-493">String collection</span></span>|<span data-ttu-id="3dfaa-494">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-494">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="3dfaa-495">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="3dfaa-495">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="3dfaa-496">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="3dfaa-496">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="3dfaa-497">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-497">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="3dfaa-498">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-498">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="3dfaa-499">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="3dfaa-499">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="3dfaa-500">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-500">Boolean</span></span>|<span data-ttu-id="3dfaa-501">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-501">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="3dfaa-502">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-502">defenderRequireCloudProtection</span></span>|<span data-ttu-id="3dfaa-503">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-503">Boolean</span></span>|<span data-ttu-id="3dfaa-504">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-504">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="3dfaa-505">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="3dfaa-505">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="3dfaa-506">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-506">Boolean</span></span>|<span data-ttu-id="3dfaa-507">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-507">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="3dfaa-508">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="3dfaa-508">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="3dfaa-509">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-509">Boolean</span></span>|<span data-ttu-id="3dfaa-510">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-510">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="3dfaa-511">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="3dfaa-511">defenderScanArchiveFiles</span></span>|<span data-ttu-id="3dfaa-512">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-512">Boolean</span></span>|<span data-ttu-id="3dfaa-513">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-513">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="3dfaa-514">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="3dfaa-514">defenderScanDownloads</span></span>|<span data-ttu-id="3dfaa-515">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-515">Boolean</span></span>|<span data-ttu-id="3dfaa-516">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-516">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="3dfaa-517">defenderScheduleScanEnableLowCpuPriority</span><span class="sxs-lookup"><span data-stu-id="3dfaa-517">defenderScheduleScanEnableLowCpuPriority</span></span>|<span data-ttu-id="3dfaa-518">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-518">Boolean</span></span>|<span data-ttu-id="3dfaa-519">启用后, 在计划扫描期间将使用较低的 CPU 优先级。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-519">When enabled, low CPU priority will be used during scheduled scans.</span></span>|
|<span data-ttu-id="3dfaa-520">defenderDisableCatchupQuickScan</span><span class="sxs-lookup"><span data-stu-id="3dfaa-520">defenderDisableCatchupQuickScan</span></span>|<span data-ttu-id="3dfaa-521">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-521">Boolean</span></span>|<span data-ttu-id="3dfaa-522">当被阻止时, 将关闭计划快速扫描的追赶扫描。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-522">When blocked, catch-up scans for scheduled quick scans will be turned off.</span></span>|
|<span data-ttu-id="3dfaa-523">defenderDisableCatchupFullScan</span><span class="sxs-lookup"><span data-stu-id="3dfaa-523">defenderDisableCatchupFullScan</span></span>|<span data-ttu-id="3dfaa-524">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-524">Boolean</span></span>|<span data-ttu-id="3dfaa-525">当被阻止时, 计划的完全扫描的追赶扫描将被禁用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-525">When blocked, catch-up scans for scheduled full scans will be turned off.</span></span>|
|<span data-ttu-id="3dfaa-526">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="3dfaa-526">defenderScanNetworkFiles</span></span>|<span data-ttu-id="3dfaa-527">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-527">Boolean</span></span>|<span data-ttu-id="3dfaa-528">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-528">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="3dfaa-529">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="3dfaa-529">defenderScanIncomingMail</span></span>|<span data-ttu-id="3dfaa-530">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-530">Boolean</span></span>|<span data-ttu-id="3dfaa-531">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-531">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="3dfaa-532">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="3dfaa-532">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="3dfaa-533">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-533">Boolean</span></span>|<span data-ttu-id="3dfaa-534">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-534">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="3dfaa-535">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="3dfaa-535">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="3dfaa-536">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-536">Boolean</span></span>|<span data-ttu-id="3dfaa-537">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-537">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="3dfaa-538">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="3dfaa-538">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="3dfaa-539">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-539">Boolean</span></span>|<span data-ttu-id="3dfaa-540">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-540">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="3dfaa-541">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="3dfaa-541">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="3dfaa-542">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-542">Int32</span></span>|<span data-ttu-id="3dfaa-543">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-543">The signature update interval in hours.</span></span> <span data-ttu-id="3dfaa-544">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-544">Specify 0 not to check.</span></span> <span data-ttu-id="3dfaa-545">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="3dfaa-545">Valid values 0 to 24</span></span>|
|<span data-ttu-id="3dfaa-546">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-546">defenderScanType</span></span>|[<span data-ttu-id="3dfaa-547">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-547">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="3dfaa-548">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-548">The defender system scan type.</span></span> <span data-ttu-id="3dfaa-549">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-549">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="3dfaa-550">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="3dfaa-550">defenderScheduledScanTime</span></span>|<span data-ttu-id="3dfaa-551">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3dfaa-551">TimeOfDay</span></span>|<span data-ttu-id="3dfaa-552">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-552">The defender time for the system scan.</span></span>|
|<span data-ttu-id="3dfaa-553">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="3dfaa-553">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="3dfaa-554">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="3dfaa-554">TimeOfDay</span></span>|<span data-ttu-id="3dfaa-555">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-555">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="3dfaa-556">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="3dfaa-556">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="3dfaa-557">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-557">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="3dfaa-558">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-558">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="3dfaa-559">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-559">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="3dfaa-560">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="3dfaa-560">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="3dfaa-561">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-561">Int32</span></span>|<span data-ttu-id="3dfaa-562">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-562">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="3dfaa-563">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="3dfaa-563">Valid values 0 to 50</span></span>|
|<span data-ttu-id="3dfaa-564">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="3dfaa-564">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="3dfaa-565">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-565">Int32</span></span>|<span data-ttu-id="3dfaa-566">云文件扫描的超时扩展。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-566">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="3dfaa-567">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="3dfaa-567">Valid values 0 to 50</span></span>|
|<span data-ttu-id="3dfaa-568">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="3dfaa-568">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="3dfaa-569">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-569">Boolean</span></span>|<span data-ttu-id="3dfaa-570">允许或禁止 Windows Defender 访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-570">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="3dfaa-571">defenderScheduleScanDay</span><span class="sxs-lookup"><span data-stu-id="3dfaa-571">defenderScheduleScanDay</span></span>|[<span data-ttu-id="3dfaa-572">defenderScheduleScanDay</span><span class="sxs-lookup"><span data-stu-id="3dfaa-572">defenderScheduleScanDay</span></span>](../resources/intune-deviceconfig-defenderschedulescanday.md)|<span data-ttu-id="3dfaa-573">选择 Windows Defender 扫描应运行的日期。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-573">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="3dfaa-574">可取值为：`everyday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`sunday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-574">Possible values are: `everyday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="3dfaa-575">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-575">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="3dfaa-576">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-576">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="3dfaa-577">检查 Windows Defender 中的用户同意级别以发送数据。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-577">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="3dfaa-578">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-578">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="3dfaa-579">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dfaa-579">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="3dfaa-580">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-580">Boolean</span></span>|<span data-ttu-id="3dfaa-581">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-581">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="3dfaa-582">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-582">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="3dfaa-583">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="3dfaa-583">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="3dfaa-584">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-584">Boolean</span></span>|<span data-ttu-id="3dfaa-585">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-585">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="3dfaa-586">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="3dfaa-586">lockScreenBlockCortana</span></span>|<span data-ttu-id="3dfaa-587">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-587">Boolean</span></span>|<span data-ttu-id="3dfaa-588">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-588">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="3dfaa-589">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="3dfaa-589">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="3dfaa-590">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-590">Boolean</span></span>|<span data-ttu-id="3dfaa-591">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-591">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="3dfaa-592">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="3dfaa-592">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="3dfaa-593">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-593">Int32</span></span>|<span data-ttu-id="3dfaa-594">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-594">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="3dfaa-595">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-595">Supported values are 11-1800.</span></span> <span data-ttu-id="3dfaa-596">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="3dfaa-596">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="3dfaa-597">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3dfaa-597">passwordBlockSimple</span></span>|<span data-ttu-id="3dfaa-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-598">Boolean</span></span>|<span data-ttu-id="3dfaa-599">指定是否允许 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-599">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="3dfaa-600">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-600">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="3dfaa-601">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3dfaa-601">passwordExpirationDays</span></span>|<span data-ttu-id="3dfaa-602">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-602">Int32</span></span>|<span data-ttu-id="3dfaa-603">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-603">The password expiration in days.</span></span> <span data-ttu-id="3dfaa-604">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="3dfaa-604">Valid values 0 to 730</span></span>|
|<span data-ttu-id="3dfaa-605">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3dfaa-605">passwordMinimumLength</span></span>|<span data-ttu-id="3dfaa-606">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-606">Int32</span></span>|<span data-ttu-id="3dfaa-607">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-607">The minimum password length.</span></span> <span data-ttu-id="3dfaa-608">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="3dfaa-608">Valid values 4 to 16</span></span>|
|<span data-ttu-id="3dfaa-609">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="3dfaa-609">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="3dfaa-610">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-610">Int32</span></span>|<span data-ttu-id="3dfaa-611">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-611">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="3dfaa-612">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3dfaa-612">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3dfaa-613">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-613">Int32</span></span>|<span data-ttu-id="3dfaa-614">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-614">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3dfaa-615">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3dfaa-615">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3dfaa-616">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-616">Int32</span></span>|<span data-ttu-id="3dfaa-617">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-617">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="3dfaa-618">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="3dfaa-618">Valid values 0 to 50</span></span>|
|<span data-ttu-id="3dfaa-619">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3dfaa-619">passwordRequired</span></span>|<span data-ttu-id="3dfaa-620">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-620">Boolean</span></span>|<span data-ttu-id="3dfaa-621">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-621">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="3dfaa-622">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="3dfaa-622">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="3dfaa-623">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-623">Boolean</span></span>|<span data-ttu-id="3dfaa-624">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-624">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="3dfaa-625">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-625">passwordRequiredType</span></span>|[<span data-ttu-id="3dfaa-626">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-626">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="3dfaa-627">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-627">The required password type.</span></span> <span data-ttu-id="3dfaa-628">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-628">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="3dfaa-629">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="3dfaa-629">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="3dfaa-630">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-630">Int32</span></span>|<span data-ttu-id="3dfaa-631">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-631">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="3dfaa-632">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="3dfaa-632">Valid values 0 to 999</span></span>|
|<span data-ttu-id="3dfaa-633">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="3dfaa-633">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="3dfaa-634">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-634">Int32</span></span>|<span data-ttu-id="3dfaa-635">此安全设置确定用户可以更改密码之前必须使用该密码的时间 (以天为单位)。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-635">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="3dfaa-636">有效值为0至998</span><span class="sxs-lookup"><span data-stu-id="3dfaa-636">Valid values 0 to 998</span></span>|
|<span data-ttu-id="3dfaa-637">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="3dfaa-637">privacyAdvertisingId</span></span>|[<span data-ttu-id="3dfaa-638">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-638">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="3dfaa-639">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-639">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="3dfaa-640">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-640">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="3dfaa-641">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-641">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="3dfaa-642">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="3dfaa-642">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="3dfaa-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-643">Boolean</span></span>|<span data-ttu-id="3dfaa-644">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-644">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="3dfaa-645">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="3dfaa-645">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="3dfaa-646">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-646">Boolean</span></span>|<span data-ttu-id="3dfaa-647">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-647">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="3dfaa-648">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="3dfaa-648">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="3dfaa-649">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-649">Boolean</span></span>|<span data-ttu-id="3dfaa-650">阻止共享体验和发现任务切换器等中的最近使用的资源。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-650">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="3dfaa-651">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="3dfaa-651">privacyBlockActivityFeed</span></span>|<span data-ttu-id="3dfaa-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-652">Boolean</span></span>|<span data-ttu-id="3dfaa-653">阻止 Cortana、听写或存储应用程序的基于云的语音服务的使用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-653">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="3dfaa-654">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="3dfaa-654">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="3dfaa-655">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-655">Boolean</span></span>|<span data-ttu-id="3dfaa-656">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-656">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="3dfaa-657">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="3dfaa-657">startMenuAppListVisibility</span></span>|[<span data-ttu-id="3dfaa-658">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-658">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="3dfaa-659">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-659">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="3dfaa-660">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-660">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="3dfaa-661">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="3dfaa-661">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="3dfaa-662">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-662">Boolean</span></span>|<span data-ttu-id="3dfaa-663">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-663">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-664">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="3dfaa-664">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="3dfaa-665">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-665">Boolean</span></span>|<span data-ttu-id="3dfaa-666">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-666">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="3dfaa-667">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="3dfaa-667">startMenuHideHibernate</span></span>|<span data-ttu-id="3dfaa-668">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-668">Boolean</span></span>|<span data-ttu-id="3dfaa-669">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-669">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-670">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="3dfaa-670">startMenuHideLock</span></span>|<span data-ttu-id="3dfaa-671">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-671">Boolean</span></span>|<span data-ttu-id="3dfaa-672">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-672">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-673">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="3dfaa-673">startMenuHidePowerButton</span></span>|<span data-ttu-id="3dfaa-674">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-674">Boolean</span></span>|<span data-ttu-id="3dfaa-675">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-675">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-676">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="3dfaa-676">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="3dfaa-677">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-677">Boolean</span></span>|<span data-ttu-id="3dfaa-678">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-678">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="3dfaa-679">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="3dfaa-679">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="3dfaa-680">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-680">Boolean</span></span>|<span data-ttu-id="3dfaa-681">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-681">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="3dfaa-682">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="3dfaa-682">startMenuHideRestartOptions</span></span>|<span data-ttu-id="3dfaa-683">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-683">Boolean</span></span>|<span data-ttu-id="3dfaa-684">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-684">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-685">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="3dfaa-685">startMenuHideShutDown</span></span>|<span data-ttu-id="3dfaa-686">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-686">Boolean</span></span>|<span data-ttu-id="3dfaa-687">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-687">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-688">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="3dfaa-688">startMenuHideSignOut</span></span>|<span data-ttu-id="3dfaa-689">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-689">Boolean</span></span>|<span data-ttu-id="3dfaa-690">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-690">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-691">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="3dfaa-691">startMenuHideSleep</span></span>|<span data-ttu-id="3dfaa-692">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-692">Boolean</span></span>|<span data-ttu-id="3dfaa-693">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-693">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-694">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="3dfaa-694">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="3dfaa-695">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-695">Boolean</span></span>|<span data-ttu-id="3dfaa-696">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-696">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-697">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="3dfaa-697">startMenuHideUserTile</span></span>|<span data-ttu-id="3dfaa-698">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-698">Boolean</span></span>|<span data-ttu-id="3dfaa-699">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-699">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="3dfaa-700">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="3dfaa-700">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="3dfaa-701">Binary</span><span class="sxs-lookup"><span data-stu-id="3dfaa-701">Binary</span></span>|<span data-ttu-id="3dfaa-702">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-702">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="3dfaa-703">开始布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-703">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="3dfaa-704">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-704">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="3dfaa-705">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-705">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="3dfaa-706">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-706">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="3dfaa-707">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="3dfaa-707">startMenuLayoutXml</span></span>|<span data-ttu-id="3dfaa-708">Binary</span><span class="sxs-lookup"><span data-stu-id="3dfaa-708">Binary</span></span>|<span data-ttu-id="3dfaa-709">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-709">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="3dfaa-710">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-710">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="3dfaa-711">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-711">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="3dfaa-712">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="3dfaa-712">startMenuMode</span></span>|[<span data-ttu-id="3dfaa-713">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-713">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="3dfaa-714">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-714">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="3dfaa-715">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-715">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="3dfaa-716">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="3dfaa-716">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="3dfaa-717">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-717">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-718">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-718">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-719">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-719">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-720">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="3dfaa-720">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="3dfaa-721">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-721">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-722">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-722">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-723">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-723">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-724">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="3dfaa-724">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="3dfaa-725">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-725">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-726">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-726">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-727">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-727">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-728">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="3dfaa-728">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="3dfaa-729">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-729">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-730">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-730">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-731">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-731">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-732">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="3dfaa-732">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="3dfaa-733">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-733">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-734">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-734">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-735">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-735">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-736">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="3dfaa-736">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="3dfaa-737">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-737">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-738">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-738">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-739">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-739">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-740">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="3dfaa-740">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="3dfaa-741">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-741">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-742">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-742">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-743">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-743">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-744">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="3dfaa-744">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="3dfaa-745">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-745">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-746">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-746">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-747">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-747">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-748">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="3dfaa-748">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="3dfaa-749">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-749">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-750">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-750">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-751">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-751">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-752">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="3dfaa-752">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="3dfaa-753">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-753">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="3dfaa-754">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-754">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="3dfaa-755">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-755">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="3dfaa-756">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="3dfaa-756">settingsBlockSettingsApp</span></span>|<span data-ttu-id="3dfaa-757">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-757">Boolean</span></span>|<span data-ttu-id="3dfaa-758">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-758">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="3dfaa-759">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-759">settingsBlockSystemPage</span></span>|<span data-ttu-id="3dfaa-760">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-760">Boolean</span></span>|<span data-ttu-id="3dfaa-761">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-761">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-762">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-762">settingsBlockDevicesPage</span></span>|<span data-ttu-id="3dfaa-763">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-763">Boolean</span></span>|<span data-ttu-id="3dfaa-764">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-764">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-765">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-765">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="3dfaa-766">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-766">Boolean</span></span>|<span data-ttu-id="3dfaa-767">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-767">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-768">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-768">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="3dfaa-769">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-769">Boolean</span></span>|<span data-ttu-id="3dfaa-770">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-770">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-771">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-771">settingsBlockAccountsPage</span></span>|<span data-ttu-id="3dfaa-772">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-772">Boolean</span></span>|<span data-ttu-id="3dfaa-773">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-773">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-774">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-774">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="3dfaa-775">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-775">Boolean</span></span>|<span data-ttu-id="3dfaa-776">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-776">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-777">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-777">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="3dfaa-778">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-778">Boolean</span></span>|<span data-ttu-id="3dfaa-779">指示是否阻止在“设置”应用中访问“辅助功能”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-779">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-780">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-780">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="3dfaa-781">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-781">Boolean</span></span>|<span data-ttu-id="3dfaa-782">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-782">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-783">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-783">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="3dfaa-784">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-784">Boolean</span></span>|<span data-ttu-id="3dfaa-785">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-785">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-786">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-786">settingsBlockAppsPage</span></span>|<span data-ttu-id="3dfaa-787">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-787">Boolean</span></span>|<span data-ttu-id="3dfaa-788">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-788">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-789">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-789">settingsBlockGamingPage</span></span>|<span data-ttu-id="3dfaa-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-790">Boolean</span></span>|<span data-ttu-id="3dfaa-791">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-791">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="3dfaa-792">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="3dfaa-792">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="3dfaa-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-793">Boolean</span></span>|<span data-ttu-id="3dfaa-794">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-794">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="3dfaa-795">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-795">windowsSpotlightBlocked</span></span>|<span data-ttu-id="3dfaa-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-796">Boolean</span></span>|<span data-ttu-id="3dfaa-797">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="3dfaa-797">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="3dfaa-798">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="3dfaa-798">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="3dfaa-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-799">Boolean</span></span>|<span data-ttu-id="3dfaa-800">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="3dfaa-800">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="3dfaa-801">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="3dfaa-801">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="3dfaa-802">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-802">Boolean</span></span>|<span data-ttu-id="3dfaa-803">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-803">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="3dfaa-804">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="3dfaa-804">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="3dfaa-805">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-805">Boolean</span></span>|<span data-ttu-id="3dfaa-806">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="3dfaa-806">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="3dfaa-807">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="3dfaa-807">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="3dfaa-808">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-808">Boolean</span></span>|<span data-ttu-id="3dfaa-809">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="3dfaa-809">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="3dfaa-810">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="3dfaa-810">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="3dfaa-811">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-811">Boolean</span></span>|<span data-ttu-id="3dfaa-812">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-812">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="3dfaa-813">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="3dfaa-813">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="3dfaa-814">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="3dfaa-814">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="3dfaa-815">指定聚光灯的类型。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-815">Specifies the type of Spotlight.</span></span> <span data-ttu-id="3dfaa-816">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-816">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="3dfaa-817">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="3dfaa-817">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="3dfaa-818">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-818">Boolean</span></span>|<span data-ttu-id="3dfaa-819">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-819">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="3dfaa-820">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-820">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="3dfaa-821">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="3dfaa-821">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="3dfaa-822">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-822">Boolean</span></span>|<span data-ttu-id="3dfaa-823">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-823">Disable automatic detection of settings.</span></span> <span data-ttu-id="3dfaa-824">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-824">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="3dfaa-825">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="3dfaa-825">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="3dfaa-826">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-826">String</span></span>|<span data-ttu-id="3dfaa-827">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-827">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="3dfaa-828">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="3dfaa-828">networkProxyServer</span></span>|[<span data-ttu-id="3dfaa-829">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="3dfaa-829">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="3dfaa-830">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-830">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="3dfaa-831">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="3dfaa-831">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="3dfaa-832">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-832">Boolean</span></span>|<span data-ttu-id="3dfaa-833">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-833">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="3dfaa-834">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-834">antiTheftModeBlocked</span></span>|<span data-ttu-id="3dfaa-835">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-835">Boolean</span></span>|<span data-ttu-id="3dfaa-836">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-836">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="3dfaa-837">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-837">bluetoothBlocked</span></span>|<span data-ttu-id="3dfaa-838">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-838">Boolean</span></span>|<span data-ttu-id="3dfaa-839">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-839">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="3dfaa-840">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-840">cameraBlocked</span></span>|<span data-ttu-id="3dfaa-841">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-841">Boolean</span></span>|<span data-ttu-id="3dfaa-842">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-842">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="3dfaa-843">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-843">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="3dfaa-844">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-844">Boolean</span></span>|<span data-ttu-id="3dfaa-845">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-845">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="3dfaa-846">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="3dfaa-846">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="3dfaa-847">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-847">Boolean</span></span>|<span data-ttu-id="3dfaa-848">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-848">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="3dfaa-849">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-849">copyPasteBlocked</span></span>|<span data-ttu-id="3dfaa-850">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-850">Boolean</span></span>|<span data-ttu-id="3dfaa-851">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-851">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="3dfaa-852">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-852">cortanaBlocked</span></span>|<span data-ttu-id="3dfaa-853">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-853">Boolean</span></span>|<span data-ttu-id="3dfaa-854">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-854">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="3dfaa-855">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="3dfaa-855">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="3dfaa-856">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-856">Boolean</span></span>|<span data-ttu-id="3dfaa-857">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-857">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="3dfaa-858">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="3dfaa-858">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="3dfaa-859">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-859">Boolean</span></span>|<span data-ttu-id="3dfaa-860">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-860">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="3dfaa-861">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="3dfaa-861">safeSearchFilter</span></span>|[<span data-ttu-id="3dfaa-862">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="3dfaa-862">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="3dfaa-863">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-863">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="3dfaa-864">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-864">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="3dfaa-865">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="3dfaa-865">edgeBlockPopups</span></span>|<span data-ttu-id="3dfaa-866">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-866">Boolean</span></span>|<span data-ttu-id="3dfaa-867">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-867">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="3dfaa-868">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="3dfaa-868">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="3dfaa-869">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-869">Boolean</span></span>|<span data-ttu-id="3dfaa-870">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-870">Indicates whether or not to block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="3dfaa-871">edgeBlockSearchEngineCustomization</span><span class="sxs-lookup"><span data-stu-id="3dfaa-871">edgeBlockSearchEngineCustomization</span></span>|<span data-ttu-id="3dfaa-872">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-872">Boolean</span></span>|<span data-ttu-id="3dfaa-873">指示是否阻止用户添加新的搜索引擎或更改默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-873">Indicates whether or not to block the user from adding new search engine or changing the default search engine.</span></span>|
|<span data-ttu-id="3dfaa-874">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="3dfaa-874">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="3dfaa-875">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-875">Boolean</span></span>|<span data-ttu-id="3dfaa-876">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-876">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="3dfaa-877">注意: 此属性的名称是误导性的;属性已过时, 请改用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-877">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="3dfaa-878">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="3dfaa-878">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="3dfaa-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-879">Boolean</span></span>|<span data-ttu-id="3dfaa-880">指示是否将 intranet 流量从边缘切换到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-880">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="3dfaa-881">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="3dfaa-881">edgeRequireSmartScreen</span></span>|<span data-ttu-id="3dfaa-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-882">Boolean</span></span>|<span data-ttu-id="3dfaa-883">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-883">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="3dfaa-884">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="3dfaa-884">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="3dfaa-885">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-885">String</span></span>|<span data-ttu-id="3dfaa-886">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-886">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="3dfaa-887">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-887">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="3dfaa-888">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="3dfaa-888">edgeFirstRunUrl</span></span>|<span data-ttu-id="3dfaa-889">String</span><span class="sxs-lookup"><span data-stu-id="3dfaa-889">String</span></span>|<span data-ttu-id="3dfaa-890">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-890">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="3dfaa-891">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="3dfaa-891">edgeSearchEngine</span></span>|[<span data-ttu-id="3dfaa-892">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="3dfaa-892">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="3dfaa-893">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-893">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="3dfaa-894">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-894">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="3dfaa-895">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="3dfaa-895">edgeHomepageUrls</span></span>|<span data-ttu-id="3dfaa-896">String 集合</span><span class="sxs-lookup"><span data-stu-id="3dfaa-896">String collection</span></span>|<span data-ttu-id="3dfaa-897">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-897">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="3dfaa-898">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="3dfaa-898">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="3dfaa-899">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-899">Boolean</span></span>|<span data-ttu-id="3dfaa-900">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-900">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="3dfaa-901">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="3dfaa-901">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="3dfaa-902">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-902">Boolean</span></span>|<span data-ttu-id="3dfaa-903">指示用户是否可以覆盖有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-903">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="3dfaa-904">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="3dfaa-904">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="3dfaa-905">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-905">Boolean</span></span>|<span data-ttu-id="3dfaa-906">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="3dfaa-906">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="3dfaa-907">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="3dfaa-907">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="3dfaa-908">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-908">Boolean</span></span>|<span data-ttu-id="3dfaa-909">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="3dfaa-909">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="3dfaa-910">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-910">internetSharingBlocked</span></span>|<span data-ttu-id="3dfaa-911">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-911">Boolean</span></span>|<span data-ttu-id="3dfaa-912">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-912">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="3dfaa-913">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-913">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="3dfaa-914">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-914">Boolean</span></span>|<span data-ttu-id="3dfaa-915">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-915">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="3dfaa-916">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-916">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="3dfaa-917">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-917">Boolean</span></span>|<span data-ttu-id="3dfaa-918">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-918">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="3dfaa-919">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="3dfaa-919">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="3dfaa-920">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-920">Boolean</span></span>|<span data-ttu-id="3dfaa-921">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-921">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="3dfaa-922">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="3dfaa-922">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="3dfaa-923">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-923">Boolean</span></span>|<span data-ttu-id="3dfaa-924">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-924">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="3dfaa-925">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="3dfaa-925">settingsBlockChangeRegion</span></span>|<span data-ttu-id="3dfaa-926">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-926">Boolean</span></span>|<span data-ttu-id="3dfaa-927">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-927">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="3dfaa-928">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-928">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="3dfaa-929">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-929">Boolean</span></span>|<span data-ttu-id="3dfaa-930">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-930">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="3dfaa-931">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="3dfaa-931">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="3dfaa-932">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-932">Boolean</span></span>|<span data-ttu-id="3dfaa-933">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-933">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="3dfaa-934">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-934">locationServicesBlocked</span></span>|<span data-ttu-id="3dfaa-935">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-935">Boolean</span></span>|<span data-ttu-id="3dfaa-936">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-936">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="3dfaa-937">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-937">microsoftAccountBlocked</span></span>|<span data-ttu-id="3dfaa-938">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-938">Boolean</span></span>|<span data-ttu-id="3dfaa-939">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-939">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="3dfaa-940">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="3dfaa-940">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="3dfaa-941">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-941">Boolean</span></span>|<span data-ttu-id="3dfaa-942">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-942">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="3dfaa-943">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-943">nfcBlocked</span></span>|<span data-ttu-id="3dfaa-944">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-944">Boolean</span></span>|<span data-ttu-id="3dfaa-945">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-945">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="3dfaa-946">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-946">resetProtectionModeBlocked</span></span>|<span data-ttu-id="3dfaa-947">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-947">Boolean</span></span>|<span data-ttu-id="3dfaa-948">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-948">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="3dfaa-949">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-949">screenCaptureBlocked</span></span>|<span data-ttu-id="3dfaa-950">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-950">Boolean</span></span>|<span data-ttu-id="3dfaa-951">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-951">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="3dfaa-952">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="3dfaa-952">storageBlockRemovableStorage</span></span>|<span data-ttu-id="3dfaa-953">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-953">Boolean</span></span>|<span data-ttu-id="3dfaa-954">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-954">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="3dfaa-955">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="3dfaa-955">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="3dfaa-956">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-956">Boolean</span></span>|<span data-ttu-id="3dfaa-957">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-957">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="3dfaa-958">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-958">usbBlocked</span></span>|<span data-ttu-id="3dfaa-959">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-959">Boolean</span></span>|<span data-ttu-id="3dfaa-960">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-960">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="3dfaa-961">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-961">voiceRecordingBlocked</span></span>|<span data-ttu-id="3dfaa-962">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-962">Boolean</span></span>|<span data-ttu-id="3dfaa-963">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-963">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="3dfaa-964">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="3dfaa-964">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="3dfaa-965">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-965">Boolean</span></span>|<span data-ttu-id="3dfaa-966">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-966">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="3dfaa-967">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-967">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="3dfaa-968">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-968">wiFiBlocked</span></span>|<span data-ttu-id="3dfaa-969">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-969">Boolean</span></span>|<span data-ttu-id="3dfaa-970">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-970">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="3dfaa-971">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="3dfaa-971">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="3dfaa-972">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-972">Boolean</span></span>|<span data-ttu-id="3dfaa-973">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-973">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="3dfaa-974">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="3dfaa-974">wiFiScanInterval</span></span>|<span data-ttu-id="3dfaa-975">Int32</span><span class="sxs-lookup"><span data-stu-id="3dfaa-975">Int32</span></span>|<span data-ttu-id="3dfaa-976">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-976">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="3dfaa-977">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-977">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="3dfaa-978">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="3dfaa-978">Valid values 1 to 500</span></span>|
|<span data-ttu-id="3dfaa-979">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="3dfaa-979">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="3dfaa-980">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-980">Boolean</span></span>|<span data-ttu-id="3dfaa-981">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-981">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="3dfaa-982">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="3dfaa-982">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="3dfaa-983">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-983">Boolean</span></span>|<span data-ttu-id="3dfaa-984">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-984">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="3dfaa-985">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="3dfaa-985">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="3dfaa-986">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-986">Boolean</span></span>|<span data-ttu-id="3dfaa-987">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-987">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="3dfaa-988">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-988">windowsStoreBlocked</span></span>|<span data-ttu-id="3dfaa-989">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-989">Boolean</span></span>|<span data-ttu-id="3dfaa-990">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-990">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="3dfaa-991">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="3dfaa-991">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="3dfaa-992">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-992">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="3dfaa-993">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-993">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="3dfaa-994">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-994">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="3dfaa-995">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="3dfaa-995">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="3dfaa-996">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-996">Boolean</span></span>|<span data-ttu-id="3dfaa-997">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-997">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="3dfaa-998">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-998">developerUnlockSetting</span></span>|[<span data-ttu-id="3dfaa-999">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="3dfaa-999">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="3dfaa-1000">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1000">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="3dfaa-1001">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1001">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="3dfaa-1002">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1002">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="3dfaa-1003">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1003">Boolean</span></span>|<span data-ttu-id="3dfaa-1004">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1004">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="3dfaa-1005">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1005">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="3dfaa-1006">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1006">Boolean</span></span>|<span data-ttu-id="3dfaa-1007">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1007">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="3dfaa-1008">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1008">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="3dfaa-1009">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1009">Boolean</span></span>|<span data-ttu-id="3dfaa-1010">指示是否启用“仅限私人应用商店”。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1010">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="3dfaa-1011">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1011">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="3dfaa-1012">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1012">Boolean</span></span>|<span data-ttu-id="3dfaa-1013">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1013">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="3dfaa-1014">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1014">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="3dfaa-1015">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1015">Boolean</span></span>|<span data-ttu-id="3dfaa-1016">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1016">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="3dfaa-1017">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1017">gameDvrBlocked</span></span>|<span data-ttu-id="3dfaa-1018">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1018">Boolean</span></span>|<span data-ttu-id="3dfaa-1019">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1019">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="3dfaa-1020">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1020">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="3dfaa-1021">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1021">Boolean</span></span>|<span data-ttu-id="3dfaa-1022">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1022">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="3dfaa-1023">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1023">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="3dfaa-1024">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1024">Boolean</span></span>|<span data-ttu-id="3dfaa-1025">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1025">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="3dfaa-1026">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1026">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="3dfaa-1027">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1027">Boolean</span></span>|<span data-ttu-id="3dfaa-1028">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1028">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="3dfaa-1029">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1029">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="3dfaa-1030">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1030">Boolean</span></span>|<span data-ttu-id="3dfaa-1031">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1031">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="3dfaa-1032">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1032">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="3dfaa-1033">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1033">Boolean</span></span>|<span data-ttu-id="3dfaa-1034">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1034">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="3dfaa-1035">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1035">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="3dfaa-1036">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1036">Boolean</span></span>|<span data-ttu-id="3dfaa-1037">此策略设置允许用户更改通常仅供系统管理员使用的安装选项。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1037">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="3dfaa-1038">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1038">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="3dfaa-1039">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1039">Boolean</span></span>|<span data-ttu-id="3dfaa-1040">此策略设置指示 Windows Installer 在系统上安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1040">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="3dfaa-1041">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1041">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="3dfaa-1042">Boolean</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1042">Boolean</span></span>|<span data-ttu-id="3dfaa-1043">通过此策略设置, 您可以阻止所有热插拔 PCI 下游端口的直接内存访问 (DMA), 直到用户登录 Windows。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1043">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="3dfaa-1044">响应</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1044">Response</span></span>
<span data-ttu-id="3dfaa-1045">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1045">If successful, this method returns a `201 Created` response code and a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3dfaa-1046">示例</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1046">Example</span></span>

### <a name="request"></a><span data-ttu-id="3dfaa-1047">请求</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1047">Request</span></span>
<span data-ttu-id="3dfaa-1048">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1048">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 13338

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
  "defenderScheduleScanDay": "monday",
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
  "dataProtectionBlockDirectMemoryAccess": true
}
```

### <a name="response"></a><span data-ttu-id="3dfaa-1049">响应</span><span class="sxs-lookup"><span data-stu-id="3dfaa-1049">Response</span></span>
<span data-ttu-id="3dfaa-p179">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3dfaa-p179">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 13510

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
  "defenderScheduleScanDay": "monday",
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
  "dataProtectionBlockDirectMemoryAccess": true
}
```




