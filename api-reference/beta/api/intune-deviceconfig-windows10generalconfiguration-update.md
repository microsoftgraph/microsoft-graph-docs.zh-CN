---
title: 更新 windows10GeneralConfiguration
description: 更新 windows10GeneralConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c2ebff0cfce923cf0f208736d30192af72ede00f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423389"
---
# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="b3eb8-103">更新 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3eb8-103">Update windows10GeneralConfiguration</span></span>

> <span data-ttu-id="b3eb8-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b3eb8-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b3eb8-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3eb8-107">更新 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-107">Update the properties of a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3eb8-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3eb8-108">Prerequisites</span></span>
<span data-ttu-id="b3eb8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b3eb8-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3eb8-111">Permission type</span></span>|<span data-ttu-id="b3eb8-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3eb8-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3eb8-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3eb8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3eb8-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3eb8-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b3eb8-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3eb8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3eb8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-116">Not supported.</span></span>|
|<span data-ttu-id="b3eb8-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3eb8-117">Application</span></span>|<span data-ttu-id="b3eb8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3eb8-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3eb8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="b3eb8-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3eb8-120">Request headers</span></span>
|<span data-ttu-id="b3eb8-121">标头</span><span class="sxs-lookup"><span data-stu-id="b3eb8-121">Header</span></span>|<span data-ttu-id="b3eb8-122">值</span><span class="sxs-lookup"><span data-stu-id="b3eb8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3eb8-123">授权</span><span class="sxs-lookup"><span data-stu-id="b3eb8-123">Authorization</span></span>|<span data-ttu-id="b3eb8-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3eb8-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b3eb8-125">Accept</span></span>|<span data-ttu-id="b3eb8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3eb8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3eb8-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3eb8-127">Request body</span></span>
<span data-ttu-id="b3eb8-128">在请求正文中，提供 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-128">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="b3eb8-129">下表显示了创建 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-129">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="b3eb8-130">属性</span><span class="sxs-lookup"><span data-stu-id="b3eb8-130">Property</span></span>|<span data-ttu-id="b3eb8-131">类型</span><span class="sxs-lookup"><span data-stu-id="b3eb8-131">Type</span></span>|<span data-ttu-id="b3eb8-132">说明</span><span class="sxs-lookup"><span data-stu-id="b3eb8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3eb8-133">id</span><span class="sxs-lookup"><span data-stu-id="b3eb8-133">id</span></span>|<span data-ttu-id="b3eb8-134">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-134">String</span></span>|<span data-ttu-id="b3eb8-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-135">Key of the entity.</span></span> <span data-ttu-id="b3eb8-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3eb8-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3eb8-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b3eb8-137">lastModifiedDateTime</span></span>|<span data-ttu-id="b3eb8-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3eb8-138">DateTimeOffset</span></span>|<span data-ttu-id="b3eb8-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-139">DateTime the object was last modified.</span></span> <span data-ttu-id="b3eb8-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3eb8-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3eb8-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b3eb8-141">roleScopeTagIds</span></span>|<span data-ttu-id="b3eb8-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-142">String collection</span></span>|<span data-ttu-id="b3eb8-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b3eb8-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3eb8-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3eb8-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b3eb8-145">supportsScopeTags</span></span>|<span data-ttu-id="b3eb8-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-146">Boolean</span></span>|<span data-ttu-id="b3eb8-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b3eb8-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b3eb8-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b3eb8-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-150">This property is read-only.</span></span> <span data-ttu-id="b3eb8-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3eb8-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3eb8-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b3eb8-152">createdDateTime</span></span>|<span data-ttu-id="b3eb8-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b3eb8-153">DateTimeOffset</span></span>|<span data-ttu-id="b3eb8-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-154">DateTime the object was created.</span></span> <span data-ttu-id="b3eb8-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3eb8-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3eb8-156">description</span><span class="sxs-lookup"><span data-stu-id="b3eb8-156">description</span></span>|<span data-ttu-id="b3eb8-157">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-157">String</span></span>|<span data-ttu-id="b3eb8-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b3eb8-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3eb8-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3eb8-160">displayName</span><span class="sxs-lookup"><span data-stu-id="b3eb8-160">displayName</span></span>|<span data-ttu-id="b3eb8-161">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-161">String</span></span>|<span data-ttu-id="b3eb8-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b3eb8-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3eb8-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3eb8-164">version</span><span class="sxs-lookup"><span data-stu-id="b3eb8-164">version</span></span>|<span data-ttu-id="b3eb8-165">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-165">Int32</span></span>|<span data-ttu-id="b3eb8-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-166">Version of the device configuration.</span></span> <span data-ttu-id="b3eb8-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b3eb8-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b3eb8-168">taskManagerBlockEndTask</span><span class="sxs-lookup"><span data-stu-id="b3eb8-168">taskManagerBlockEndTask</span></span>|<span data-ttu-id="b3eb8-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-169">Boolean</span></span>|<span data-ttu-id="b3eb8-170">指定是否非管理员可以使用结束任务的任务管理器。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-170">Specify whether non-administrators can use Task Manager to end tasks.</span></span>|
|<span data-ttu-id="b3eb8-171">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="b3eb8-171">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="b3eb8-172">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="b3eb8-172">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="b3eb8-173">应用程序的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-173">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="b3eb8-174">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="b3eb8-174">enableAutomaticRedeployment</span></span>|<span data-ttu-id="b3eb8-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-175">Boolean</span></span>|<span data-ttu-id="b3eb8-176">允许用户具有管理权限，以删除所有用户数据和设置在设备锁定屏幕上使用 CTRL + Win + R，以便可以自动重新配置和管理到 re-enrolled 设备。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-176">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="b3eb8-177">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="b3eb8-177">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="b3eb8-178">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="b3eb8-178">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="b3eb8-179">控制 Microsoft 帐户登录助手 (wlidsvc) NT 服务。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-179">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="b3eb8-180">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-180">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="b3eb8-181">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="b3eb8-181">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="b3eb8-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-182">Boolean</span></span>|<span data-ttu-id="b3eb8-183">允许使用 Windows 的辅助身份验证设备。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-183">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="b3eb8-184">authenticationPreferredAzureADTenantDomainName</span><span class="sxs-lookup"><span data-stu-id="b3eb8-184">authenticationPreferredAzureADTenantDomainName</span></span>|<span data-ttu-id="b3eb8-185">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-185">String</span></span>|<span data-ttu-id="b3eb8-186">指定 Azure AD 租户中的可用的域之间的首选的域。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-186">Specifies the preferred domain among available domains in the Azure AD tenant.</span></span>|
|<span data-ttu-id="b3eb8-187">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="b3eb8-187">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="b3eb8-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-188">Boolean</span></span>|<span data-ttu-id="b3eb8-189">指定是否允许或禁止联邦信息处理标准 (FIPS) 策略。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-189">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="b3eb8-190">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="b3eb8-190">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="b3eb8-191">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-191">String collection</span></span>|<span data-ttu-id="b3eb8-192">已打开 GDI DPI 缩放比例的旧应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-192">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="b3eb8-193">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="b3eb8-193">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="b3eb8-194">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-194">String collection</span></span>|<span data-ttu-id="b3eb8-195">已关闭 GDI DPI 缩放比例的旧应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-195">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="b3eb8-196">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="b3eb8-196">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="b3eb8-197">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-197">String</span></span>|<span data-ttu-id="b3eb8-198">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-198">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="b3eb8-199">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="b3eb8-199">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="b3eb8-200">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-200">String</span></span>|<span data-ttu-id="b3eb8-201">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-201">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="b3eb8-202">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="b3eb8-202">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="b3eb8-203">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-203">String</span></span>|<span data-ttu-id="b3eb8-204">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-204">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="b3eb8-205">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b3eb8-205">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="b3eb8-206">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-206">String</span></span>|<span data-ttu-id="b3eb8-207">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-207">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="b3eb8-208">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="b3eb8-208">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="b3eb8-209">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-209">Int32</span></span>|<span data-ttu-id="b3eb8-210">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-210">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="b3eb8-211">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-211">This is a mobile only setting.</span></span> <span data-ttu-id="b3eb8-212">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="b3eb8-212">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="b3eb8-213">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="b3eb8-213">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="b3eb8-214">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-214">String</span></span>|<span data-ttu-id="b3eb8-215">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-215">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="b3eb8-216">experienceDoNotSyncBrowserSettings</span><span class="sxs-lookup"><span data-stu-id="b3eb8-216">experienceDoNotSyncBrowserSettings</span></span>|[<span data-ttu-id="b3eb8-217">browserSyncSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-217">browserSyncSetting</span></span>](../resources/intune-deviceconfig-browsersyncsetting.md)|<span data-ttu-id="b3eb8-218">允许或阻止的 Microsoft 边缘浏览器设置同步。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-218">Allow or prevent the syncing of Microsoft Edge Browser settings.</span></span> <span data-ttu-id="b3eb8-219">对于 IT 管理员，以防止跨设备，同步，但允许用户替代选项。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-219">Option for IT admins to prevent syncing across devices, but allow user override.</span></span> <span data-ttu-id="b3eb8-220">可取值为：`notConfigured`、`blockedWithUserOverride`、`blocked`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-220">Possible values are: `notConfigured`, `blockedWithUserOverride`, `blocked`.</span></span>|
|<span data-ttu-id="b3eb8-221">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="b3eb8-221">messagingBlockSync</span></span>|<span data-ttu-id="b3eb8-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-222">Boolean</span></span>|<span data-ttu-id="b3eb8-223">指示阻止短信备份和还原和消息无处不在。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-223">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="b3eb8-224">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="b3eb8-224">messagingBlockMMS</span></span>|<span data-ttu-id="b3eb8-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-225">Boolean</span></span>|<span data-ttu-id="b3eb8-226">指示是否阻止 MMS 发送/接收的设备上的功能。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-226">Indicates whether or not to block the the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="b3eb8-227">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="b3eb8-227">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="b3eb8-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-228">Boolean</span></span>|<span data-ttu-id="b3eb8-229">指示是否阻止 RC 发送/接收的设备上的功能。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-229">Indicates whether or not to block the the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="b3eb8-230">printerNames</span><span class="sxs-lookup"><span data-stu-id="b3eb8-230">printerNames</span></span>|<span data-ttu-id="b3eb8-231">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-231">String collection</span></span>|<span data-ttu-id="b3eb8-232">自动设置打印机根据其名称 （网络主机名）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-232">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="b3eb8-233">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="b3eb8-233">printerDefaultName</span></span>|<span data-ttu-id="b3eb8-234">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-234">String</span></span>|<span data-ttu-id="b3eb8-235">已安装的打印机的名称 （网络主机名）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-235">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="b3eb8-236">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="b3eb8-236">printerBlockAddition</span></span>|<span data-ttu-id="b3eb8-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-237">Boolean</span></span>|<span data-ttu-id="b3eb8-238">阻止用户安装的打印机设置中的其他打印机。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-238">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="b3eb8-239">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="b3eb8-239">searchBlockDiacritics</span></span>|<span data-ttu-id="b3eb8-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-240">Boolean</span></span>|<span data-ttu-id="b3eb8-241">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-241">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="b3eb8-242">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="b3eb8-242">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="b3eb8-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-243">Boolean</span></span>|<span data-ttu-id="b3eb8-244">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-244">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="b3eb8-245">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="b3eb8-245">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="b3eb8-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-246">Boolean</span></span>|<span data-ttu-id="b3eb8-247">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-247">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="b3eb8-248">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="b3eb8-248">searchEnableRemoteQueries</span></span>|<span data-ttu-id="b3eb8-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-249">Boolean</span></span>|<span data-ttu-id="b3eb8-250">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-250">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="b3eb8-251">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="b3eb8-251">searchDisableUseLocation</span></span>|<span data-ttu-id="b3eb8-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-252">Boolean</span></span>|<span data-ttu-id="b3eb8-253">指定搜索可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-253">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="b3eb8-254">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="b3eb8-254">searchDisableLocation</span></span>|<span data-ttu-id="b3eb8-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-255">Boolean</span></span>|<span data-ttu-id="b3eb8-256">指定搜索可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-256">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="b3eb8-257">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="b3eb8-257">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="b3eb8-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-258">Boolean</span></span>|<span data-ttu-id="b3eb8-259">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-259">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="b3eb8-260">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="b3eb8-260">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="b3eb8-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-261">Boolean</span></span>|<span data-ttu-id="b3eb8-262">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-262">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="b3eb8-263">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="b3eb8-263">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="b3eb8-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-264">Boolean</span></span>|<span data-ttu-id="b3eb8-265">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-265">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="b3eb8-266">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="b3eb8-266">searchBlockWebResults</span></span>|<span data-ttu-id="b3eb8-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-267">Boolean</span></span>|<span data-ttu-id="b3eb8-268">指示阻止 web 搜索。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-268">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="b3eb8-269">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="b3eb8-269">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="b3eb8-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-270">Boolean</span></span>|<span data-ttu-id="b3eb8-271">指定是否允许设备自动加密期间 OOBE 设备时 Azure AD 加入 （仅适用于桌面）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-271">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="b3eb8-272">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="b3eb8-272">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="b3eb8-273">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="b3eb8-273">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="b3eb8-274">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-274">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="b3eb8-275">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-275">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="b3eb8-276">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="b3eb8-276">oneDriveDisableFileSync</span></span>|<span data-ttu-id="b3eb8-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-277">Boolean</span></span>|<span data-ttu-id="b3eb8-278">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-278">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="b3eb8-279">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="b3eb8-279">systemTelemetryProxyServer</span></span>|<span data-ttu-id="b3eb8-280">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-280">String</span></span>|<span data-ttu-id="b3eb8-281">获取或设置的完全限定的域名 (FQDN) 或代理服务器连接的用户体验和遥测请求转发的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-281">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="b3eb8-282">edgeTelemetryForMicrosoft365Analytics</span><span class="sxs-lookup"><span data-stu-id="b3eb8-282">edgeTelemetryForMicrosoft365Analytics</span></span>|[<span data-ttu-id="b3eb8-283">edgeTelemetryMode</span><span class="sxs-lookup"><span data-stu-id="b3eb8-283">edgeTelemetryMode</span></span>](../resources/intune-deviceconfig-edgetelemetrymode.md)|<span data-ttu-id="b3eb8-284">指定的遥测数据的类型 (无、 intranet、 internet，同时) 发送到 Microsoft 365 分析。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-284">Specifies what type of telemetry data (none, intranet, internet, both) is sent to Microsoft 365 Analytics.</span></span> <span data-ttu-id="b3eb8-285">可取值为：`notConfigured`、`intranet`、`internet`、`intranetAndInternet`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-285">Possible values are: `notConfigured`, `intranet`, `internet`, `intranetAndInternet`.</span></span>|
|<span data-ttu-id="b3eb8-286">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="b3eb8-286">inkWorkspaceAccess</span></span>|[<span data-ttu-id="b3eb8-287">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-287">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="b3eb8-288">控制用户访问墨迹工作区中，在桌面上，然后从锁定屏幕上上述。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-288">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="b3eb8-289">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-289">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="b3eb8-290">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="b3eb8-290">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="b3eb8-291">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-291">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b3eb8-292">控制用户访问墨迹工作区中，在桌面上，然后从锁定屏幕上上述。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-292">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="b3eb8-293">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-293">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b3eb8-294">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="b3eb8-294">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="b3eb8-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-295">Boolean</span></span>|<span data-ttu-id="b3eb8-296">指定是否在墨迹工作区中显示建议的应用程序建议。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-296">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="b3eb8-297">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="b3eb8-297">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="b3eb8-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-298">Boolean</span></span>|<span data-ttu-id="b3eb8-299">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-299">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="b3eb8-300">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="b3eb8-300">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="b3eb8-301">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-301">String</span></span>|<span data-ttu-id="b3eb8-302">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-302">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="b3eb8-303">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="b3eb8-303">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="b3eb8-304">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-304">String</span></span>|<span data-ttu-id="b3eb8-305">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-305">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="b3eb8-306">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="b3eb8-306">bluetoothAllowedServices</span></span>|<span data-ttu-id="b3eb8-307">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-307">String collection</span></span>|<span data-ttu-id="b3eb8-308">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-308">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="b3eb8-309">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="b3eb8-309">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="b3eb8-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-310">Boolean</span></span>|<span data-ttu-id="b3eb8-311">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-311">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="b3eb8-312">bluetoothBlockPromptedProximalConnections</span><span class="sxs-lookup"><span data-stu-id="b3eb8-312">bluetoothBlockPromptedProximalConnections</span></span>|<span data-ttu-id="b3eb8-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-313">Boolean</span></span>|<span data-ttu-id="b3eb8-314">阻止用户使用 Swift 对和其他接近度基于方案。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-314">Whether or not to block the users from using Swift Pair and other proximity based scenarios.</span></span>|
|<span data-ttu-id="b3eb8-315">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="b3eb8-315">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="b3eb8-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-316">Boolean</span></span>|<span data-ttu-id="b3eb8-317">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-317">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="b3eb8-318">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="b3eb8-318">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="b3eb8-319">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-319">Boolean</span></span>|<span data-ttu-id="b3eb8-320">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-320">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="b3eb8-321">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="b3eb8-321">edgeBlockAutofill</span></span>|<span data-ttu-id="b3eb8-322">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-322">Boolean</span></span>|<span data-ttu-id="b3eb8-323">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-323">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="b3eb8-324">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-324">edgeBlocked</span></span>|<span data-ttu-id="b3eb8-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-325">Boolean</span></span>|<span data-ttu-id="b3eb8-326">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-326">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="b3eb8-327">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="b3eb8-327">edgeCookiePolicy</span></span>|[<span data-ttu-id="b3eb8-328">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="b3eb8-328">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="b3eb8-329">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-329">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="b3eb8-330">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-330">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="b3eb8-331">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="b3eb8-331">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="b3eb8-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-332">Boolean</span></span>|<span data-ttu-id="b3eb8-333">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-333">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="b3eb8-334">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="b3eb8-334">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="b3eb8-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-335">Boolean</span></span>|<span data-ttu-id="b3eb8-336">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-336">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="b3eb8-337">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="b3eb8-337">edgeBlockExtensions</span></span>|<span data-ttu-id="b3eb8-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-338">Boolean</span></span>|<span data-ttu-id="b3eb8-339">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-339">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="b3eb8-340">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="b3eb8-340">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="b3eb8-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-341">Boolean</span></span>|<span data-ttu-id="b3eb8-342">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-342">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="b3eb8-343">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="b3eb8-343">edgeBlockJavaScript</span></span>|<span data-ttu-id="b3eb8-344">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-344">Boolean</span></span>|<span data-ttu-id="b3eb8-345">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-345">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="b3eb8-346">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="b3eb8-346">edgeBlockPasswordManager</span></span>|<span data-ttu-id="b3eb8-347">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-347">Boolean</span></span>|<span data-ttu-id="b3eb8-348">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-348">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="b3eb8-349">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="b3eb8-349">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="b3eb8-350">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-350">Boolean</span></span>|<span data-ttu-id="b3eb8-351">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-351">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="b3eb8-352">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-352">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="b3eb8-353">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="b3eb8-353">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="b3eb8-354">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-354">Boolean</span></span>|<span data-ttu-id="b3eb8-355">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-355">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="b3eb8-356">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-356">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="b3eb8-357">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="b3eb8-357">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="b3eb8-358">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-358">Boolean</span></span>|<span data-ttu-id="b3eb8-359">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-359">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="b3eb8-360">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="b3eb8-360">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="b3eb8-361">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-361">Boolean</span></span>|<span data-ttu-id="b3eb8-362">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-362">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="b3eb8-363">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-363">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="b3eb8-364">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-364">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="b3eb8-365">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-365">Boolean</span></span>|<span data-ttu-id="b3eb8-366">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-366">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="b3eb8-367">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-367">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="b3eb8-368">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="b3eb8-368">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="b3eb8-369">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-369">Boolean</span></span>|<span data-ttu-id="b3eb8-370">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-370">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="b3eb8-371">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b3eb8-371">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="b3eb8-372">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-372">Boolean</span></span>|<span data-ttu-id="b3eb8-373">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-373">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="b3eb8-374">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-374">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="b3eb8-375">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="b3eb8-375">edgeFavoritesListLocation</span></span>|<span data-ttu-id="b3eb8-376">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-376">String</span></span>|<span data-ttu-id="b3eb8-377">设置的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-377">The location of the favorites list to provision.</span></span> <span data-ttu-id="b3eb8-378">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-378">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b3eb8-379">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="b3eb8-379">edgeBlockEditFavorites</span></span>|<span data-ttu-id="b3eb8-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-380">Boolean</span></span>|<span data-ttu-id="b3eb8-381">指示阻止用户更改收藏夹。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-381">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="b3eb8-382">edgeNewTabPageURL</span><span class="sxs-lookup"><span data-stu-id="b3eb8-382">edgeNewTabPageURL</span></span>|<span data-ttu-id="b3eb8-383">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-383">String</span></span>|<span data-ttu-id="b3eb8-384">指定当创建新选项卡打开该页。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-384">Specify the page opened when new tabs are created.</span></span>|
|<span data-ttu-id="b3eb8-385">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3eb8-385">edgeHomeButtonConfiguration</span></span>|[<span data-ttu-id="b3eb8-386">edgeHomeButtonConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3eb8-386">edgeHomeButtonConfiguration</span></span>](../resources/intune-deviceconfig-edgehomebuttonconfiguration.md)|<span data-ttu-id="b3eb8-387">使主页按钮来隐藏、 加载默认起始页、 加载新的选项卡上页上或自定义 URL</span><span class="sxs-lookup"><span data-stu-id="b3eb8-387">Causes the Home button to either hide, load the default Start page, load a New tab page, or a custom URL</span></span>|
|<span data-ttu-id="b3eb8-388">edgeHomeButtonConfigurationEnabled</span><span class="sxs-lookup"><span data-stu-id="b3eb8-388">edgeHomeButtonConfigurationEnabled</span></span>|<span data-ttu-id="b3eb8-389">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-389">Boolean</span></span>|<span data-ttu-id="b3eb8-390">启用主页按钮配置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-390">Enable the Home button configuration.</span></span>|
|<span data-ttu-id="b3eb8-391">edgeOpensWith</span><span class="sxs-lookup"><span data-stu-id="b3eb8-391">edgeOpensWith</span></span>|[<span data-ttu-id="b3eb8-392">edgeOpenOptions</span><span class="sxs-lookup"><span data-stu-id="b3eb8-392">edgeOpenOptions</span></span>](../resources/intune-deviceconfig-edgeopenoptions.md)|<span data-ttu-id="b3eb8-393">指定在启动时打开了哪种类型的页面。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-393">Specify what kind of pages are open at start.</span></span> <span data-ttu-id="b3eb8-394">可取值为：`notConfigured`、`startPage`、`newTabPage`、`previousPages`、`specificPages`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-394">Possible values are: `notConfigured`, `startPage`, `newTabPage`, `previousPages`, `specificPages`.</span></span>|
|<span data-ttu-id="b3eb8-395">edgeBlockSideloadingExtensions</span><span class="sxs-lookup"><span data-stu-id="b3eb8-395">edgeBlockSideloadingExtensions</span></span>|<span data-ttu-id="b3eb8-396">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-396">Boolean</span></span>|<span data-ttu-id="b3eb8-397">指示用户是否可以 sideload 扩展。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-397">Indicates whether the user can sideload extensions.</span></span>|
|<span data-ttu-id="b3eb8-398">edgeRequiredExtensionPackageFamilyNames</span><span class="sxs-lookup"><span data-stu-id="b3eb8-398">edgeRequiredExtensionPackageFamilyNames</span></span>|<span data-ttu-id="b3eb8-399">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-399">String collection</span></span>|<span data-ttu-id="b3eb8-400">指定的所需并不能由用户关闭浏览器扩展的程序包系列名称的列表。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-400">Specify the list of package family names of browser extensions that are required and cannot be turned off by the user.</span></span>|
|<span data-ttu-id="b3eb8-401">edgeBlockPrinting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-401">edgeBlockPrinting</span></span>|<span data-ttu-id="b3eb8-402">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-402">Boolean</span></span>|<span data-ttu-id="b3eb8-403">若要允许或阻止打印的边缘配置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-403">Configure Edge to allow or block printing.</span></span>|
|<span data-ttu-id="b3eb8-404">edgeFavoritesBarVisibility</span><span class="sxs-lookup"><span data-stu-id="b3eb8-404">edgeFavoritesBarVisibility</span></span>|[<span data-ttu-id="b3eb8-405">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-405">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-406">获取或设置一个值，指定是否设置为总是可见还是隐藏任何页面上的收藏夹栏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-406">Get or set a value that specifies whether to set the favorites bar to always be visible or hidden on any page.</span></span> <span data-ttu-id="b3eb8-407">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-407">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-408">edgeBlockSavingHistory</span><span class="sxs-lookup"><span data-stu-id="b3eb8-408">edgeBlockSavingHistory</span></span>|<span data-ttu-id="b3eb8-409">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-409">Boolean</span></span>|<span data-ttu-id="b3eb8-410">配置边缘允许浏览历史记录保存或永远不会保存浏览历史记录。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-410">Configure Edge to allow browsing history to be saved or to never save browsing history.</span></span>|
|<span data-ttu-id="b3eb8-411">edgeBlockFullScreenMode</span><span class="sxs-lookup"><span data-stu-id="b3eb8-411">edgeBlockFullScreenMode</span></span>|<span data-ttu-id="b3eb8-412">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-412">Boolean</span></span>|<span data-ttu-id="b3eb8-413">允许或阻止边缘输入全屏显示模式。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-413">Allow or prevent Edge from entering the full screen mode.</span></span>|
|<span data-ttu-id="b3eb8-414">edgeBlockWebContentOnNewTabPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-414">edgeBlockWebContentOnNewTabPage</span></span>|<span data-ttu-id="b3eb8-415">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-415">Boolean</span></span>|<span data-ttu-id="b3eb8-416">配置 Microsoft 边缘打开新选项卡时显示的内容。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-416">Configure what appears when Microsoft Edge opens a new tab.</span></span>|
|<span data-ttu-id="b3eb8-417">edgeBlockTabPreloading</span><span class="sxs-lookup"><span data-stu-id="b3eb8-417">edgeBlockTabPreloading</span></span>|<span data-ttu-id="b3eb8-418">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-418">Boolean</span></span>|<span data-ttu-id="b3eb8-419">配置是否边缘将 Windows 启动时的新选项卡页。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-419">Configure whether Edge preloads the new tab page at Windows startup.</span></span>|
|<span data-ttu-id="b3eb8-420">edgeBlockPrelaunch</span><span class="sxs-lookup"><span data-stu-id="b3eb8-420">edgeBlockPrelaunch</span></span>|<span data-ttu-id="b3eb8-421">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-421">Boolean</span></span>|<span data-ttu-id="b3eb8-422">决定是否将 Microsoft 边缘 prelaunched Windows 启动时。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-422">Decide whether Microsoft Edge is prelaunched at Windows startup.</span></span>|
|<span data-ttu-id="b3eb8-423">edgeShowMessageWhenOpeningInternetExplorerSites</span><span class="sxs-lookup"><span data-stu-id="b3eb8-423">edgeShowMessageWhenOpeningInternetExplorerSites</span></span>|[<span data-ttu-id="b3eb8-424">internetExplorerMessageSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-424">internetExplorerMessageSetting</span></span>](../resources/intune-deviceconfig-internetexplorermessagesetting.md)|<span data-ttu-id="b3eb8-425">控制切换到 Internet Explorer 之前显示边缘的消息。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-425">Controls the message displayed by Edge before switching to Internet Explorer.</span></span> <span data-ttu-id="b3eb8-426">可取值为：`notConfigured`、`disabled`、`enabled`、`keepGoing`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-426">Possible values are: `notConfigured`, `disabled`, `enabled`, `keepGoing`.</span></span>|
|<span data-ttu-id="b3eb8-427">edgePreventCertificateErrorOverride</span><span class="sxs-lookup"><span data-stu-id="b3eb8-427">edgePreventCertificateErrorOverride</span></span>|<span data-ttu-id="b3eb8-428">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-428">Boolean</span></span>|<span data-ttu-id="b3eb8-429">允许或阻止用户替代证书错误。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-429">Allow or prevent users from overriding certificate errors.</span></span>|
|<span data-ttu-id="b3eb8-430">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="b3eb8-430">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="b3eb8-431">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-431">Boolean</span></span>|<span data-ttu-id="b3eb8-432">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-432">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="b3eb8-433">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="b3eb8-433">cellularBlockVpn</span></span>|<span data-ttu-id="b3eb8-434">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-434">Boolean</span></span>|<span data-ttu-id="b3eb8-435">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-435">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="b3eb8-436">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="b3eb8-436">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="b3eb8-437">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-437">Boolean</span></span>|<span data-ttu-id="b3eb8-438">是否阻止用户在通过手机网络漫游时使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-438">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="b3eb8-439">cellularData</span><span class="sxs-lookup"><span data-stu-id="b3eb8-439">cellularData</span></span>|[<span data-ttu-id="b3eb8-440">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-440">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="b3eb8-441">是否在设备上允许移动数据信道。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-441">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="b3eb8-442">如果未配置，允许移动数据通道，用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-442">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="b3eb8-443">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-443">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="b3eb8-444">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="b3eb8-444">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="b3eb8-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-445">Boolean</span></span>|<span data-ttu-id="b3eb8-446">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-446">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="b3eb8-447">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="b3eb8-447">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="b3eb8-448">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-448">Int32</span></span>|<span data-ttu-id="b3eb8-449">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-449">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="b3eb8-450">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="b3eb8-450">Valid values 0 to 90</span></span>|
|<span data-ttu-id="b3eb8-451">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="b3eb8-451">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="b3eb8-452">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="b3eb8-452">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="b3eb8-453">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-453">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="b3eb8-454">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="b3eb8-454">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="b3eb8-455">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="b3eb8-455">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="b3eb8-456">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-456">Defender day of the week for the system scan.</span></span> <span data-ttu-id="b3eb8-457">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-457">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="b3eb8-458">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="b3eb8-458">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="b3eb8-459">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-459">String collection</span></span>|<span data-ttu-id="b3eb8-460">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-460">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b3eb8-461">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="b3eb8-461">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="b3eb8-462">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-462">String collection</span></span>|<span data-ttu-id="b3eb8-463">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-463">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b3eb8-464">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="b3eb8-464">defenderScanMaxCpu</span></span>|<span data-ttu-id="b3eb8-465">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-465">Int32</span></span>|<span data-ttu-id="b3eb8-466">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-466">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="b3eb8-467">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="b3eb8-467">Valid values 0 to 100</span></span>|
|<span data-ttu-id="b3eb8-468">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="b3eb8-468">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="b3eb8-469">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="b3eb8-469">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="b3eb8-470">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-470">Value for monitoring file activity.</span></span> <span data-ttu-id="b3eb8-471">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-471">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="b3eb8-472">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="b3eb8-472">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="b3eb8-473">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="b3eb8-473">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="b3eb8-474">获取或设置要执行上可能不需要应用程序 (PUA)，其中包括与 ad 注入，软件捆绑、 持久请求的付款或订阅等的行为的软件的 Defender 的操作。PUA 正在下载，或尝试自行安装时，则 defender 通知用户。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-474">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="b3eb8-475">添加 Windows 10 中的桌面。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-475">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="b3eb8-476">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-476">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="b3eb8-477">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-477">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="b3eb8-478">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-478">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="b3eb8-479">获取或设置要执行上可能不需要应用程序 (PUA)，其中包括与 ad 注入，软件捆绑、 持久请求的付款或订阅等的行为的软件的 Defender 的操作。PUA 正在下载，或尝试自行安装时，则 defender 通知用户。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-479">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="b3eb8-480">添加 Windows 10 中的桌面。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-480">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="b3eb8-481">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-481">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="b3eb8-482">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="b3eb8-482">defenderProcessesToExclude</span></span>|<span data-ttu-id="b3eb8-483">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-483">String collection</span></span>|<span data-ttu-id="b3eb8-484">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-484">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="b3eb8-485">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="b3eb8-485">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="b3eb8-486">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="b3eb8-486">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="b3eb8-487">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-487">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="b3eb8-488">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-488">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="b3eb8-489">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="b3eb8-489">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="b3eb8-490">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-490">Boolean</span></span>|<span data-ttu-id="b3eb8-491">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-491">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="b3eb8-492">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="b3eb8-492">defenderRequireCloudProtection</span></span>|<span data-ttu-id="b3eb8-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-493">Boolean</span></span>|<span data-ttu-id="b3eb8-494">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-494">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="b3eb8-495">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="b3eb8-495">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="b3eb8-496">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-496">Boolean</span></span>|<span data-ttu-id="b3eb8-497">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-497">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="b3eb8-498">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="b3eb8-498">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="b3eb8-499">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-499">Boolean</span></span>|<span data-ttu-id="b3eb8-500">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-500">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="b3eb8-501">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="b3eb8-501">defenderScanArchiveFiles</span></span>|<span data-ttu-id="b3eb8-502">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-502">Boolean</span></span>|<span data-ttu-id="b3eb8-503">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-503">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="b3eb8-504">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="b3eb8-504">defenderScanDownloads</span></span>|<span data-ttu-id="b3eb8-505">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-505">Boolean</span></span>|<span data-ttu-id="b3eb8-506">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-506">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="b3eb8-507">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="b3eb8-507">defenderScanNetworkFiles</span></span>|<span data-ttu-id="b3eb8-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-508">Boolean</span></span>|<span data-ttu-id="b3eb8-509">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-509">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="b3eb8-510">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="b3eb8-510">defenderScanIncomingMail</span></span>|<span data-ttu-id="b3eb8-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-511">Boolean</span></span>|<span data-ttu-id="b3eb8-512">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-512">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="b3eb8-513">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="b3eb8-513">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="b3eb8-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-514">Boolean</span></span>|<span data-ttu-id="b3eb8-515">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-515">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="b3eb8-516">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="b3eb8-516">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="b3eb8-517">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-517">Boolean</span></span>|<span data-ttu-id="b3eb8-518">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-518">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="b3eb8-519">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b3eb8-519">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="b3eb8-520">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-520">Boolean</span></span>|<span data-ttu-id="b3eb8-521">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-521">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="b3eb8-522">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="b3eb8-522">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="b3eb8-523">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-523">Int32</span></span>|<span data-ttu-id="b3eb8-524">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-524">The signature update interval in hours.</span></span> <span data-ttu-id="b3eb8-525">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-525">Specify 0 not to check.</span></span> <span data-ttu-id="b3eb8-526">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="b3eb8-526">Valid values 0 to 24</span></span>|
|<span data-ttu-id="b3eb8-527">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-527">defenderScanType</span></span>|[<span data-ttu-id="b3eb8-528">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-528">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="b3eb8-529">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-529">The defender system scan type.</span></span> <span data-ttu-id="b3eb8-530">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-530">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="b3eb8-531">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="b3eb8-531">defenderScheduledScanTime</span></span>|<span data-ttu-id="b3eb8-532">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b3eb8-532">TimeOfDay</span></span>|<span data-ttu-id="b3eb8-533">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-533">The defender time for the system scan.</span></span>|
|<span data-ttu-id="b3eb8-534">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="b3eb8-534">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="b3eb8-535">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="b3eb8-535">TimeOfDay</span></span>|<span data-ttu-id="b3eb8-536">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-536">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="b3eb8-537">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="b3eb8-537">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="b3eb8-538">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-538">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="b3eb8-539">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-539">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="b3eb8-540">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-540">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="b3eb8-541">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="b3eb8-541">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="b3eb8-542">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-542">Int32</span></span>|<span data-ttu-id="b3eb8-543">超时的云扫描的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-543">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="b3eb8-544">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b3eb8-544">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b3eb8-545">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b3eb8-545">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="b3eb8-546">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-546">Int32</span></span>|<span data-ttu-id="b3eb8-547">超时的云扫描的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-547">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="b3eb8-548">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b3eb8-548">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b3eb8-549">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="b3eb8-549">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="b3eb8-550">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-550">Boolean</span></span>|<span data-ttu-id="b3eb8-551">允许或禁止 Windows Defender 上访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-551">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="b3eb8-552">defenderScheduleScanDay</span><span class="sxs-lookup"><span data-stu-id="b3eb8-552">defenderScheduleScanDay</span></span>|[<span data-ttu-id="b3eb8-553">defenderScheduleScanDay</span><span class="sxs-lookup"><span data-stu-id="b3eb8-553">defenderScheduleScanDay</span></span>](../resources/intune-deviceconfig-defenderschedulescanday.md)|<span data-ttu-id="b3eb8-554">选择应在运行 Windows Defender 扫描的日期。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-554">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="b3eb8-555">可取值为：`everyday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`sunday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-555">Possible values are: `everyday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="b3eb8-556">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-556">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="b3eb8-557">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-557">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="b3eb8-558">检查用户同意中发送数据的 Windows Defender 级别。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-558">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="b3eb8-559">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-559">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="b3eb8-560">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3eb8-560">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="b3eb8-561">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-561">Boolean</span></span>|<span data-ttu-id="b3eb8-562">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-562">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="b3eb8-563">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-563">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="b3eb8-564">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="b3eb8-564">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="b3eb8-565">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-565">Boolean</span></span>|<span data-ttu-id="b3eb8-566">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-566">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="b3eb8-567">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="b3eb8-567">lockScreenBlockCortana</span></span>|<span data-ttu-id="b3eb8-568">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-568">Boolean</span></span>|<span data-ttu-id="b3eb8-569">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-569">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="b3eb8-570">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="b3eb8-570">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="b3eb8-571">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-571">Boolean</span></span>|<span data-ttu-id="b3eb8-572">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-572">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="b3eb8-573">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="b3eb8-573">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="b3eb8-574">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-574">Int32</span></span>|<span data-ttu-id="b3eb8-575">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-575">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="b3eb8-576">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-576">Supported values are 11-1800.</span></span> <span data-ttu-id="b3eb8-577">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="b3eb8-577">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="b3eb8-578">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="b3eb8-578">passwordBlockSimple</span></span>|<span data-ttu-id="b3eb8-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-579">Boolean</span></span>|<span data-ttu-id="b3eb8-580">指定是否允许 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-580">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="b3eb8-581">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-581">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="b3eb8-582">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="b3eb8-582">passwordExpirationDays</span></span>|<span data-ttu-id="b3eb8-583">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-583">Int32</span></span>|<span data-ttu-id="b3eb8-584">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-584">The password expiration in days.</span></span> <span data-ttu-id="b3eb8-585">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="b3eb8-585">Valid values 0 to 730</span></span>|
|<span data-ttu-id="b3eb8-586">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="b3eb8-586">passwordMinimumLength</span></span>|<span data-ttu-id="b3eb8-587">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-587">Int32</span></span>|<span data-ttu-id="b3eb8-588">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-588">The minimum password length.</span></span> <span data-ttu-id="b3eb8-589">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="b3eb8-589">Valid values 4 to 16</span></span>|
|<span data-ttu-id="b3eb8-590">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="b3eb8-590">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="b3eb8-591">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-591">Int32</span></span>|<span data-ttu-id="b3eb8-592">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-592">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="b3eb8-593">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="b3eb8-593">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="b3eb8-594">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-594">Int32</span></span>|<span data-ttu-id="b3eb8-595">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-595">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="b3eb8-596">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="b3eb8-596">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="b3eb8-597">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-597">Int32</span></span>|<span data-ttu-id="b3eb8-598">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-598">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="b3eb8-599">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="b3eb8-599">Valid values 0 to 50</span></span>|
|<span data-ttu-id="b3eb8-600">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="b3eb8-600">passwordRequired</span></span>|<span data-ttu-id="b3eb8-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-601">Boolean</span></span>|<span data-ttu-id="b3eb8-602">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-602">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="b3eb8-603">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="b3eb8-603">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="b3eb8-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-604">Boolean</span></span>|<span data-ttu-id="b3eb8-605">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-605">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="b3eb8-606">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-606">passwordRequiredType</span></span>|[<span data-ttu-id="b3eb8-607">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-607">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="b3eb8-608">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-608">The required password type.</span></span> <span data-ttu-id="b3eb8-609">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-609">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="b3eb8-610">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="b3eb8-610">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="b3eb8-611">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-611">Int32</span></span>|<span data-ttu-id="b3eb8-612">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-612">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="b3eb8-613">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="b3eb8-613">Valid values 0 to 999</span></span>|
|<span data-ttu-id="b3eb8-614">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="b3eb8-614">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="b3eb8-615">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-615">Int32</span></span>|<span data-ttu-id="b3eb8-616">此安全设置确定的时间 （以天为单位） 的密码必须使用之前的用户可以更改它。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-616">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="b3eb8-617">有效的值 0 到 998</span><span class="sxs-lookup"><span data-stu-id="b3eb8-617">Valid values 0 to 998</span></span>|
|<span data-ttu-id="b3eb8-618">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="b3eb8-618">privacyAdvertisingId</span></span>|[<span data-ttu-id="b3eb8-619">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-619">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b3eb8-620">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-620">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="b3eb8-621">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-621">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="b3eb8-622">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-622">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b3eb8-623">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="b3eb8-623">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="b3eb8-624">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-624">Boolean</span></span>|<span data-ttu-id="b3eb8-625">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-625">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="b3eb8-626">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="b3eb8-626">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="b3eb8-627">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-627">Boolean</span></span>|<span data-ttu-id="b3eb8-628">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-628">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="b3eb8-629">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="b3eb8-629">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="b3eb8-630">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-630">Boolean</span></span>|<span data-ttu-id="b3eb8-631">阻止共享的体验/发现最近使用过中的资源任务切换器等。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-631">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="b3eb8-632">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="b3eb8-632">privacyBlockActivityFeed</span></span>|<span data-ttu-id="b3eb8-633">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-633">Boolean</span></span>|<span data-ttu-id="b3eb8-634">阻止对 Cortana、 口述或存储应用程序的基于云语音服务的使用情况。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-634">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="b3eb8-635">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="b3eb8-635">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="b3eb8-636">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-636">Boolean</span></span>|<span data-ttu-id="b3eb8-637">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-637">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="b3eb8-638">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="b3eb8-638">startMenuAppListVisibility</span></span>|[<span data-ttu-id="b3eb8-639">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-639">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="b3eb8-640">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-640">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="b3eb8-641">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-641">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="b3eb8-642">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="b3eb8-642">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="b3eb8-643">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-643">Boolean</span></span>|<span data-ttu-id="b3eb8-644">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-644">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-645">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="b3eb8-645">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="b3eb8-646">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-646">Boolean</span></span>|<span data-ttu-id="b3eb8-647">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-647">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b3eb8-648">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="b3eb8-648">startMenuHideHibernate</span></span>|<span data-ttu-id="b3eb8-649">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-649">Boolean</span></span>|<span data-ttu-id="b3eb8-650">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-650">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-651">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="b3eb8-651">startMenuHideLock</span></span>|<span data-ttu-id="b3eb8-652">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-652">Boolean</span></span>|<span data-ttu-id="b3eb8-653">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-653">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-654">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="b3eb8-654">startMenuHidePowerButton</span></span>|<span data-ttu-id="b3eb8-655">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-655">Boolean</span></span>|<span data-ttu-id="b3eb8-656">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-656">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-657">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="b3eb8-657">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="b3eb8-658">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-658">Boolean</span></span>|<span data-ttu-id="b3eb8-659">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-659">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b3eb8-660">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="b3eb8-660">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="b3eb8-661">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-661">Boolean</span></span>|<span data-ttu-id="b3eb8-662">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-662">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="b3eb8-663">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="b3eb8-663">startMenuHideRestartOptions</span></span>|<span data-ttu-id="b3eb8-664">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-664">Boolean</span></span>|<span data-ttu-id="b3eb8-665">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-665">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-666">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="b3eb8-666">startMenuHideShutDown</span></span>|<span data-ttu-id="b3eb8-667">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-667">Boolean</span></span>|<span data-ttu-id="b3eb8-668">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-668">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-669">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="b3eb8-669">startMenuHideSignOut</span></span>|<span data-ttu-id="b3eb8-670">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-670">Boolean</span></span>|<span data-ttu-id="b3eb8-671">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-671">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-672">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="b3eb8-672">startMenuHideSleep</span></span>|<span data-ttu-id="b3eb8-673">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-673">Boolean</span></span>|<span data-ttu-id="b3eb8-674">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-674">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-675">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="b3eb8-675">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="b3eb8-676">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-676">Boolean</span></span>|<span data-ttu-id="b3eb8-677">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-677">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-678">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="b3eb8-678">startMenuHideUserTile</span></span>|<span data-ttu-id="b3eb8-679">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-679">Boolean</span></span>|<span data-ttu-id="b3eb8-680">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-680">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="b3eb8-681">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="b3eb8-681">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="b3eb8-682">Binary</span><span class="sxs-lookup"><span data-stu-id="b3eb8-682">Binary</span></span>|<span data-ttu-id="b3eb8-683">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-683">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="b3eb8-684">开始布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-684">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="b3eb8-685">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-685">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="b3eb8-686">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-686">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="b3eb8-687">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-687">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="b3eb8-688">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="b3eb8-688">startMenuLayoutXml</span></span>|<span data-ttu-id="b3eb8-689">Binary</span><span class="sxs-lookup"><span data-stu-id="b3eb8-689">Binary</span></span>|<span data-ttu-id="b3eb8-690">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-690">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="b3eb8-691">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-691">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="b3eb8-692">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-692">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="b3eb8-693">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="b3eb8-693">startMenuMode</span></span>|[<span data-ttu-id="b3eb8-694">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-694">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="b3eb8-695">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-695">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="b3eb8-696">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-696">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="b3eb8-697">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="b3eb8-697">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="b3eb8-698">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-698">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-699">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-699">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-700">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-700">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-701">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="b3eb8-701">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="b3eb8-702">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-702">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-703">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-703">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-704">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-704">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-705">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="b3eb8-705">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="b3eb8-706">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-706">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-707">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-707">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-708">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-708">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-709">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="b3eb8-709">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="b3eb8-710">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-710">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-711">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-711">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-712">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-712">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-713">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="b3eb8-713">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="b3eb8-714">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-714">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-715">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-715">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-716">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-716">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-717">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="b3eb8-717">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="b3eb8-718">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-718">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-719">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-719">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-720">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-720">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-721">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="b3eb8-721">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="b3eb8-722">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-722">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-723">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-723">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-724">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-724">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-725">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="b3eb8-725">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="b3eb8-726">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-726">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-727">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-727">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-728">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-728">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-729">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="b3eb8-729">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="b3eb8-730">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-730">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-731">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-731">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-732">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-732">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-733">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="b3eb8-733">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="b3eb8-734">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-734">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="b3eb8-735">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-735">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="b3eb8-736">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-736">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="b3eb8-737">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="b3eb8-737">settingsBlockSettingsApp</span></span>|<span data-ttu-id="b3eb8-738">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-738">Boolean</span></span>|<span data-ttu-id="b3eb8-739">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-739">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="b3eb8-740">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-740">settingsBlockSystemPage</span></span>|<span data-ttu-id="b3eb8-741">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-741">Boolean</span></span>|<span data-ttu-id="b3eb8-742">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-742">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-743">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-743">settingsBlockDevicesPage</span></span>|<span data-ttu-id="b3eb8-744">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-744">Boolean</span></span>|<span data-ttu-id="b3eb8-745">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-745">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-746">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-746">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="b3eb8-747">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-747">Boolean</span></span>|<span data-ttu-id="b3eb8-748">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-748">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-749">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-749">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="b3eb8-750">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-750">Boolean</span></span>|<span data-ttu-id="b3eb8-751">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-751">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-752">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-752">settingsBlockAccountsPage</span></span>|<span data-ttu-id="b3eb8-753">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-753">Boolean</span></span>|<span data-ttu-id="b3eb8-754">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-754">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-755">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-755">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="b3eb8-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-756">Boolean</span></span>|<span data-ttu-id="b3eb8-757">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-757">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-758">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-758">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="b3eb8-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-759">Boolean</span></span>|<span data-ttu-id="b3eb8-760">指示是否阻止在“设置”应用中访问“辅助功能”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-760">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-761">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-761">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="b3eb8-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-762">Boolean</span></span>|<span data-ttu-id="b3eb8-763">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-763">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-764">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-764">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="b3eb8-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-765">Boolean</span></span>|<span data-ttu-id="b3eb8-766">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-766">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-767">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-767">settingsBlockAppsPage</span></span>|<span data-ttu-id="b3eb8-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-768">Boolean</span></span>|<span data-ttu-id="b3eb8-769">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-769">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-770">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-770">settingsBlockGamingPage</span></span>|<span data-ttu-id="b3eb8-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-771">Boolean</span></span>|<span data-ttu-id="b3eb8-772">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-772">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="b3eb8-773">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="b3eb8-773">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="b3eb8-774">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-774">Boolean</span></span>|<span data-ttu-id="b3eb8-775">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-775">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="b3eb8-776">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-776">windowsSpotlightBlocked</span></span>|<span data-ttu-id="b3eb8-777">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-777">Boolean</span></span>|<span data-ttu-id="b3eb8-778">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="b3eb8-778">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="b3eb8-779">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="b3eb8-779">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="b3eb8-780">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-780">Boolean</span></span>|<span data-ttu-id="b3eb8-781">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="b3eb8-781">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="b3eb8-782">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="b3eb8-782">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="b3eb8-783">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-783">Boolean</span></span>|<span data-ttu-id="b3eb8-784">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-784">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="b3eb8-785">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="b3eb8-785">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="b3eb8-786">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-786">Boolean</span></span>|<span data-ttu-id="b3eb8-787">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="b3eb8-787">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="b3eb8-788">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="b3eb8-788">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="b3eb8-789">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-789">Boolean</span></span>|<span data-ttu-id="b3eb8-790">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="b3eb8-790">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="b3eb8-791">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="b3eb8-791">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="b3eb8-792">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-792">Boolean</span></span>|<span data-ttu-id="b3eb8-793">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-793">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="b3eb8-794">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="b3eb8-794">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="b3eb8-795">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="b3eb8-795">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="b3eb8-796">指定聚焦的类型。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-796">Specifies the type of Spotlight.</span></span> <span data-ttu-id="b3eb8-797">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-797">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="b3eb8-798">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="b3eb8-798">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="b3eb8-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-799">Boolean</span></span>|<span data-ttu-id="b3eb8-800">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-800">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="b3eb8-801">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-801">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="b3eb8-802">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="b3eb8-802">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="b3eb8-803">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-803">Boolean</span></span>|<span data-ttu-id="b3eb8-804">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-804">Disable automatic detection of settings.</span></span> <span data-ttu-id="b3eb8-805">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-805">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="b3eb8-806">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="b3eb8-806">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="b3eb8-807">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-807">String</span></span>|<span data-ttu-id="b3eb8-808">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-808">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="b3eb8-809">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="b3eb8-809">networkProxyServer</span></span>|[<span data-ttu-id="b3eb8-810">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="b3eb8-810">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="b3eb8-811">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-811">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="b3eb8-812">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="b3eb8-812">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="b3eb8-813">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-813">Boolean</span></span>|<span data-ttu-id="b3eb8-814">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-814">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="b3eb8-815">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-815">antiTheftModeBlocked</span></span>|<span data-ttu-id="b3eb8-816">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-816">Boolean</span></span>|<span data-ttu-id="b3eb8-817">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-817">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="b3eb8-818">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-818">bluetoothBlocked</span></span>|<span data-ttu-id="b3eb8-819">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-819">Boolean</span></span>|<span data-ttu-id="b3eb8-820">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-820">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="b3eb8-821">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-821">cameraBlocked</span></span>|<span data-ttu-id="b3eb8-822">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-822">Boolean</span></span>|<span data-ttu-id="b3eb8-823">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-823">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="b3eb8-824">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-824">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="b3eb8-825">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-825">Boolean</span></span>|<span data-ttu-id="b3eb8-826">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-826">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="b3eb8-827">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="b3eb8-827">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="b3eb8-828">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-828">Boolean</span></span>|<span data-ttu-id="b3eb8-829">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-829">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="b3eb8-830">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-830">copyPasteBlocked</span></span>|<span data-ttu-id="b3eb8-831">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-831">Boolean</span></span>|<span data-ttu-id="b3eb8-832">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-832">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="b3eb8-833">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-833">cortanaBlocked</span></span>|<span data-ttu-id="b3eb8-834">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-834">Boolean</span></span>|<span data-ttu-id="b3eb8-835">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-835">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="b3eb8-836">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="b3eb8-836">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="b3eb8-837">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-837">Boolean</span></span>|<span data-ttu-id="b3eb8-838">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-838">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="b3eb8-839">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="b3eb8-839">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="b3eb8-840">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-840">Boolean</span></span>|<span data-ttu-id="b3eb8-841">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-841">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="b3eb8-842">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="b3eb8-842">safeSearchFilter</span></span>|[<span data-ttu-id="b3eb8-843">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="b3eb8-843">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="b3eb8-844">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-844">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="b3eb8-845">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-845">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="b3eb8-846">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="b3eb8-846">edgeBlockPopups</span></span>|<span data-ttu-id="b3eb8-847">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-847">Boolean</span></span>|<span data-ttu-id="b3eb8-848">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-848">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="b3eb8-849">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="b3eb8-849">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="b3eb8-850">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-850">Boolean</span></span>|<span data-ttu-id="b3eb8-851">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-851">Indicates whether or not to Block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="b3eb8-852">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b3eb8-852">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="b3eb8-853">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-853">Boolean</span></span>|<span data-ttu-id="b3eb8-854">指示切换从边缘到 Internet Explorer 的 intranet 通信。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-854">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span> <span data-ttu-id="b3eb8-855">注意： 该属性的名称令人误解;属性已过时，而是使用 EdgeSendIntranetTrafficToInternetExplorer。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-855">Note: the name of this property is misleading; the property is obsolete, use EdgeSendIntranetTrafficToInternetExplorer instead.</span></span>|
|<span data-ttu-id="b3eb8-856">edgeSendIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="b3eb8-856">edgeSendIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="b3eb8-857">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-857">Boolean</span></span>|<span data-ttu-id="b3eb8-858">指示切换从边缘到 Internet Explorer 的 intranet 通信。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-858">Indicates whether or not to switch the intranet traffic from Edge to Internet Explorer.</span></span>|
|<span data-ttu-id="b3eb8-859">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="b3eb8-859">edgeRequireSmartScreen</span></span>|<span data-ttu-id="b3eb8-860">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-860">Boolean</span></span>|<span data-ttu-id="b3eb8-861">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-861">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="b3eb8-862">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="b3eb8-862">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="b3eb8-863">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-863">String</span></span>|<span data-ttu-id="b3eb8-864">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-864">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="b3eb8-865">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-865">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="b3eb8-866">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="b3eb8-866">edgeFirstRunUrl</span></span>|<span data-ttu-id="b3eb8-867">String</span><span class="sxs-lookup"><span data-stu-id="b3eb8-867">String</span></span>|<span data-ttu-id="b3eb8-868">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-868">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="b3eb8-869">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="b3eb8-869">edgeSearchEngine</span></span>|[<span data-ttu-id="b3eb8-870">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="b3eb8-870">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="b3eb8-871">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-871">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="b3eb8-872">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-872">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="b3eb8-873">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="b3eb8-873">edgeHomepageUrls</span></span>|<span data-ttu-id="b3eb8-874">String 集合</span><span class="sxs-lookup"><span data-stu-id="b3eb8-874">String collection</span></span>|<span data-ttu-id="b3eb8-875">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-875">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="b3eb8-876">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="b3eb8-876">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="b3eb8-877">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-877">Boolean</span></span>|<span data-ttu-id="b3eb8-878">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-878">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="b3eb8-879">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="b3eb8-879">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="b3eb8-880">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-880">Boolean</span></span>|<span data-ttu-id="b3eb8-881">指示用户是否可以覆盖有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-881">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="b3eb8-882">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="b3eb8-882">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="b3eb8-883">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-883">Boolean</span></span>|<span data-ttu-id="b3eb8-884">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="b3eb8-884">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="b3eb8-885">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="b3eb8-885">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="b3eb8-886">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-886">Boolean</span></span>|<span data-ttu-id="b3eb8-887">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="b3eb8-887">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="b3eb8-888">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-888">internetSharingBlocked</span></span>|<span data-ttu-id="b3eb8-889">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-889">Boolean</span></span>|<span data-ttu-id="b3eb8-890">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-890">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="b3eb8-891">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-891">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="b3eb8-892">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-892">Boolean</span></span>|<span data-ttu-id="b3eb8-893">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-893">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="b3eb8-894">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-894">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="b3eb8-895">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-895">Boolean</span></span>|<span data-ttu-id="b3eb8-896">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-896">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="b3eb8-897">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="b3eb8-897">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="b3eb8-898">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-898">Boolean</span></span>|<span data-ttu-id="b3eb8-899">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-899">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="b3eb8-900">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="b3eb8-900">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="b3eb8-901">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-901">Boolean</span></span>|<span data-ttu-id="b3eb8-902">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-902">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="b3eb8-903">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="b3eb8-903">settingsBlockChangeRegion</span></span>|<span data-ttu-id="b3eb8-904">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-904">Boolean</span></span>|<span data-ttu-id="b3eb8-905">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-905">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="b3eb8-906">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-906">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="b3eb8-907">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-907">Boolean</span></span>|<span data-ttu-id="b3eb8-908">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-908">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="b3eb8-909">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="b3eb8-909">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="b3eb8-910">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-910">Boolean</span></span>|<span data-ttu-id="b3eb8-911">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-911">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="b3eb8-912">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-912">locationServicesBlocked</span></span>|<span data-ttu-id="b3eb8-913">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-913">Boolean</span></span>|<span data-ttu-id="b3eb8-914">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-914">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="b3eb8-915">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-915">microsoftAccountBlocked</span></span>|<span data-ttu-id="b3eb8-916">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-916">Boolean</span></span>|<span data-ttu-id="b3eb8-917">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-917">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="b3eb8-918">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="b3eb8-918">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="b3eb8-919">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-919">Boolean</span></span>|<span data-ttu-id="b3eb8-920">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-920">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="b3eb8-921">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-921">nfcBlocked</span></span>|<span data-ttu-id="b3eb8-922">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-922">Boolean</span></span>|<span data-ttu-id="b3eb8-923">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-923">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="b3eb8-924">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-924">resetProtectionModeBlocked</span></span>|<span data-ttu-id="b3eb8-925">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-925">Boolean</span></span>|<span data-ttu-id="b3eb8-926">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-926">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="b3eb8-927">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-927">screenCaptureBlocked</span></span>|<span data-ttu-id="b3eb8-928">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-928">Boolean</span></span>|<span data-ttu-id="b3eb8-929">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-929">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="b3eb8-930">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="b3eb8-930">storageBlockRemovableStorage</span></span>|<span data-ttu-id="b3eb8-931">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-931">Boolean</span></span>|<span data-ttu-id="b3eb8-932">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-932">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="b3eb8-933">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="b3eb8-933">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="b3eb8-934">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-934">Boolean</span></span>|<span data-ttu-id="b3eb8-935">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-935">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="b3eb8-936">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-936">usbBlocked</span></span>|<span data-ttu-id="b3eb8-937">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-937">Boolean</span></span>|<span data-ttu-id="b3eb8-938">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-938">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="b3eb8-939">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-939">voiceRecordingBlocked</span></span>|<span data-ttu-id="b3eb8-940">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-940">Boolean</span></span>|<span data-ttu-id="b3eb8-941">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-941">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="b3eb8-942">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="b3eb8-942">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="b3eb8-943">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-943">Boolean</span></span>|<span data-ttu-id="b3eb8-944">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-944">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="b3eb8-945">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-945">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="b3eb8-946">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-946">wiFiBlocked</span></span>|<span data-ttu-id="b3eb8-947">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-947">Boolean</span></span>|<span data-ttu-id="b3eb8-948">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-948">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="b3eb8-949">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="b3eb8-949">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="b3eb8-950">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-950">Boolean</span></span>|<span data-ttu-id="b3eb8-951">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-951">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="b3eb8-952">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="b3eb8-952">wiFiScanInterval</span></span>|<span data-ttu-id="b3eb8-953">Int32</span><span class="sxs-lookup"><span data-stu-id="b3eb8-953">Int32</span></span>|<span data-ttu-id="b3eb8-954">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-954">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="b3eb8-955">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-955">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="b3eb8-956">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="b3eb8-956">Valid values 1 to 500</span></span>|
|<span data-ttu-id="b3eb8-957">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="b3eb8-957">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="b3eb8-958">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-958">Boolean</span></span>|<span data-ttu-id="b3eb8-959">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-959">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="b3eb8-960">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="b3eb8-960">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="b3eb8-961">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-961">Boolean</span></span>|<span data-ttu-id="b3eb8-962">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-962">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="b3eb8-963">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="b3eb8-963">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="b3eb8-964">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-964">Boolean</span></span>|<span data-ttu-id="b3eb8-965">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-965">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="b3eb8-966">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-966">windowsStoreBlocked</span></span>|<span data-ttu-id="b3eb8-967">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-967">Boolean</span></span>|<span data-ttu-id="b3eb8-968">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-968">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="b3eb8-969">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="b3eb8-969">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="b3eb8-970">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-970">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b3eb8-971">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-971">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="b3eb8-972">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-972">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b3eb8-973">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="b3eb8-973">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="b3eb8-974">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-974">Boolean</span></span>|<span data-ttu-id="b3eb8-975">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-975">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="b3eb8-976">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-976">developerUnlockSetting</span></span>|[<span data-ttu-id="b3eb8-977">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="b3eb8-977">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="b3eb8-978">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-978">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="b3eb8-979">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-979">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="b3eb8-980">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="b3eb8-980">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="b3eb8-981">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-981">Boolean</span></span>|<span data-ttu-id="b3eb8-982">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-982">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="b3eb8-983">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="b3eb8-983">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="b3eb8-984">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-984">Boolean</span></span>|<span data-ttu-id="b3eb8-985">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-985">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="b3eb8-986">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="b3eb8-986">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="b3eb8-987">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-987">Boolean</span></span>|<span data-ttu-id="b3eb8-988">指示是否启用“仅限私人应用商店”。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-988">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="b3eb8-989">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="b3eb8-989">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="b3eb8-990">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-990">Boolean</span></span>|<span data-ttu-id="b3eb8-991">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-991">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="b3eb8-992">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="b3eb8-992">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="b3eb8-993">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-993">Boolean</span></span>|<span data-ttu-id="b3eb8-994">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-994">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="b3eb8-995">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="b3eb8-995">gameDvrBlocked</span></span>|<span data-ttu-id="b3eb8-996">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-996">Boolean</span></span>|<span data-ttu-id="b3eb8-997">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-997">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="b3eb8-998">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="b3eb8-998">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="b3eb8-999">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-999">Boolean</span></span>|<span data-ttu-id="b3eb8-1000">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1000">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="b3eb8-1001">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1001">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="b3eb8-1002">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1002">Boolean</span></span>|<span data-ttu-id="b3eb8-1003">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1003">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="b3eb8-1004">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1004">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="b3eb8-1005">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1005">Boolean</span></span>|<span data-ttu-id="b3eb8-1006">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1006">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="b3eb8-1007">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1007">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="b3eb8-1008">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1008">Boolean</span></span>|<span data-ttu-id="b3eb8-1009">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1009">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="b3eb8-1010">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1010">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="b3eb8-1011">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1011">Boolean</span></span>|<span data-ttu-id="b3eb8-1012">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1012">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="b3eb8-1013">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1013">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="b3eb8-1014">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1014">Boolean</span></span>|<span data-ttu-id="b3eb8-1015">此策略设置允许用户更改通常只能由系统管理员的安装选项。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1015">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="b3eb8-1016">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1016">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="b3eb8-1017">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1017">Boolean</span></span>|<span data-ttu-id="b3eb8-1018">此策略设置指示 Windows Installer 系统上安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1018">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="b3eb8-1019">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1019">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="b3eb8-1020">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1020">Boolean</span></span>|<span data-ttu-id="b3eb8-1021">此策略设置允许您阻止直接内存访问 (DMA) 的所有热 pluggable PCI 下游端口直到用户登录到 Windows。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1021">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="b3eb8-1022">响应</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1022">Response</span></span>
<span data-ttu-id="b3eb8-1023">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1023">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3eb8-1024">示例</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1024">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3eb8-1025">请求</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1025">Request</span></span>
<span data-ttu-id="b3eb8-1026">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1026">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 13056

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

### <a name="response"></a><span data-ttu-id="b3eb8-1027">响应</span><span class="sxs-lookup"><span data-stu-id="b3eb8-1027">Response</span></span>
<span data-ttu-id="b3eb8-p178">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3eb8-p178">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 13228

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




