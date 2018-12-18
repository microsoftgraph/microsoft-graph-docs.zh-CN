---
title: 更新 windows10GeneralConfiguration
description: 更新 windows10GeneralConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: c135256fa93c202537729048caeac12ec169ba17
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322734"
---
# <a name="update-windows10generalconfiguration"></a><span data-ttu-id="82fcc-103">更新 windows10GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="82fcc-103">Update windows10GeneralConfiguration</span></span>

> <span data-ttu-id="82fcc-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="82fcc-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="82fcc-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="82fcc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="82fcc-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="82fcc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82fcc-107">更新 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82fcc-107">Update the properties of a [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="82fcc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="82fcc-108">Prerequisites</span></span>
<span data-ttu-id="82fcc-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="82fcc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82fcc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="82fcc-111">Permission type</span></span>|<span data-ttu-id="82fcc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82fcc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82fcc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82fcc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="82fcc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82fcc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82fcc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82fcc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82fcc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="82fcc-116">Not supported.</span></span>|
|<span data-ttu-id="82fcc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="82fcc-117">Application</span></span>|<span data-ttu-id="82fcc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="82fcc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82fcc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82fcc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82fcc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="82fcc-120">Request headers</span></span>
|<span data-ttu-id="82fcc-121">标头</span><span class="sxs-lookup"><span data-stu-id="82fcc-121">Header</span></span>|<span data-ttu-id="82fcc-122">值</span><span class="sxs-lookup"><span data-stu-id="82fcc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82fcc-123">授权</span><span class="sxs-lookup"><span data-stu-id="82fcc-123">Authorization</span></span>|<span data-ttu-id="82fcc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="82fcc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82fcc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="82fcc-125">Accept</span></span>|<span data-ttu-id="82fcc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="82fcc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82fcc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="82fcc-127">Request body</span></span>
<span data-ttu-id="82fcc-128">在请求正文中，提供 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82fcc-128">In the request body, supply a JSON representation for the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object.</span></span>

<span data-ttu-id="82fcc-129">下表显示了创建 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="82fcc-129">The following table shows the properties that are required when you create the [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md).</span></span>

|<span data-ttu-id="82fcc-130">属性</span><span class="sxs-lookup"><span data-stu-id="82fcc-130">Property</span></span>|<span data-ttu-id="82fcc-131">类型</span><span class="sxs-lookup"><span data-stu-id="82fcc-131">Type</span></span>|<span data-ttu-id="82fcc-132">说明</span><span class="sxs-lookup"><span data-stu-id="82fcc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82fcc-133">id</span><span class="sxs-lookup"><span data-stu-id="82fcc-133">id</span></span>|<span data-ttu-id="82fcc-134">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-134">String</span></span>|<span data-ttu-id="82fcc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="82fcc-135">Key of the entity.</span></span> <span data-ttu-id="82fcc-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82fcc-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82fcc-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82fcc-137">lastModifiedDateTime</span></span>|<span data-ttu-id="82fcc-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82fcc-138">DateTimeOffset</span></span>|<span data-ttu-id="82fcc-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82fcc-139">DateTime the object was last modified.</span></span> <span data-ttu-id="82fcc-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82fcc-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82fcc-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="82fcc-141">roleScopeTagIds</span></span>|<span data-ttu-id="82fcc-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-142">String collection</span></span>|<span data-ttu-id="82fcc-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="82fcc-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="82fcc-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82fcc-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82fcc-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="82fcc-145">supportsScopeTags</span></span>|<span data-ttu-id="82fcc-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-146">Boolean</span></span>|<span data-ttu-id="82fcc-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="82fcc-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="82fcc-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="82fcc-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="82fcc-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="82fcc-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="82fcc-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="82fcc-150">This property is read-only.</span></span> <span data-ttu-id="82fcc-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82fcc-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82fcc-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82fcc-152">createdDateTime</span></span>|<span data-ttu-id="82fcc-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82fcc-153">DateTimeOffset</span></span>|<span data-ttu-id="82fcc-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82fcc-154">DateTime the object was created.</span></span> <span data-ttu-id="82fcc-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82fcc-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82fcc-156">description</span><span class="sxs-lookup"><span data-stu-id="82fcc-156">description</span></span>|<span data-ttu-id="82fcc-157">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-157">String</span></span>|<span data-ttu-id="82fcc-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="82fcc-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82fcc-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82fcc-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82fcc-160">displayName</span><span class="sxs-lookup"><span data-stu-id="82fcc-160">displayName</span></span>|<span data-ttu-id="82fcc-161">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-161">String</span></span>|<span data-ttu-id="82fcc-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="82fcc-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82fcc-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82fcc-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82fcc-164">version</span><span class="sxs-lookup"><span data-stu-id="82fcc-164">version</span></span>|<span data-ttu-id="82fcc-165">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-165">Int32</span></span>|<span data-ttu-id="82fcc-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="82fcc-166">Version of the device configuration.</span></span> <span data-ttu-id="82fcc-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82fcc-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82fcc-168">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="82fcc-168">windows10AppsForceUpdateSchedule</span></span>|[<span data-ttu-id="82fcc-169">windows10AppsForceUpdateSchedule</span><span class="sxs-lookup"><span data-stu-id="82fcc-169">windows10AppsForceUpdateSchedule</span></span>](../resources/intune-deviceconfig-windows10appsforceupdateschedule.md)|<span data-ttu-id="82fcc-170">应用程序的 Windows 10 强制更新计划。</span><span class="sxs-lookup"><span data-stu-id="82fcc-170">Windows 10 force update schedule for Apps.</span></span>|
|<span data-ttu-id="82fcc-171">enableAutomaticRedeployment</span><span class="sxs-lookup"><span data-stu-id="82fcc-171">enableAutomaticRedeployment</span></span>|<span data-ttu-id="82fcc-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-172">Boolean</span></span>|<span data-ttu-id="82fcc-173">允许用户具有管理权限，以删除所有用户数据和设置在设备锁定屏幕上使用 CTRL + Win + R，以便可以自动重新配置和管理到 re-enrolled 设备。</span><span class="sxs-lookup"><span data-stu-id="82fcc-173">Allow users with administrative rights to delete all user data and settings using CTRL + Win + R at the device lock screen so that the device can be automatically re-configured and re-enrolled into management.</span></span>|
|<span data-ttu-id="82fcc-174">assignedAccessSingleModeUserName</span><span class="sxs-lookup"><span data-stu-id="82fcc-174">assignedAccessSingleModeUserName</span></span>|<span data-ttu-id="82fcc-175">字符串</span><span class="sxs-lookup"><span data-stu-id="82fcc-175">String</span></span>|<span data-ttu-id="82fcc-176">此策略设置允许为单个应用程序展台模式定义的用户帐户将被锁定。</span><span class="sxs-lookup"><span data-stu-id="82fcc-176">This policy setting allows to define the user account that will be locked to Single App Kiosk Mode.</span></span>|
|<span data-ttu-id="82fcc-177">assignedAccessSingleModeAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="82fcc-177">assignedAccessSingleModeAppUserModelId</span></span>|<span data-ttu-id="82fcc-178">字符串</span><span class="sxs-lookup"><span data-stu-id="82fcc-178">String</span></span>|<span data-ttu-id="82fcc-179">此策略设置允许为单个应用程序展台模式定义应用程序用户模型 ID (AUMID)，将被锁定。</span><span class="sxs-lookup"><span data-stu-id="82fcc-179">This policy setting allows to define the Application User Model ID (AUMID) that will be locked to Single App Kiosk Mode.</span></span>|
|<span data-ttu-id="82fcc-180">microsoftAccountSignInAssistantSettings</span><span class="sxs-lookup"><span data-stu-id="82fcc-180">microsoftAccountSignInAssistantSettings</span></span>|[<span data-ttu-id="82fcc-181">signInAssistantOptions</span><span class="sxs-lookup"><span data-stu-id="82fcc-181">signInAssistantOptions</span></span>](../resources/intune-deviceconfig-signinassistantoptions.md)|<span data-ttu-id="82fcc-182">控制 Microsoft 帐户登录助手 (wlidsvc) NT 服务。</span><span class="sxs-lookup"><span data-stu-id="82fcc-182">Controls the Microsoft Account Sign-In Assistant (wlidsvc) NT service.</span></span> <span data-ttu-id="82fcc-183">可取值为：`notConfigured`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-183">Possible values are: `notConfigured`, `disabled`.</span></span>|
|<span data-ttu-id="82fcc-184">authenticationAllowSecondaryDevice</span><span class="sxs-lookup"><span data-stu-id="82fcc-184">authenticationAllowSecondaryDevice</span></span>|<span data-ttu-id="82fcc-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-185">Boolean</span></span>|<span data-ttu-id="82fcc-186">允许使用 Windows 的辅助身份验证设备。</span><span class="sxs-lookup"><span data-stu-id="82fcc-186">Allows secondary authentication devices to work with Windows.</span></span>|
|<span data-ttu-id="82fcc-187">authenticationAllowFIDODevice</span><span class="sxs-lookup"><span data-stu-id="82fcc-187">authenticationAllowFIDODevice</span></span>|<span data-ttu-id="82fcc-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-188">Boolean</span></span>|<span data-ttu-id="82fcc-189">指示允许使用 FIDO 身份验证设备 （https://fidoalliance.org/)</span><span class="sxs-lookup"><span data-stu-id="82fcc-189">Indicates whether or not to allow authentication using FIDO device (https://fidoalliance.org/)</span></span>|
|<span data-ttu-id="82fcc-190">cryptographyAllowFipsAlgorithmPolicy</span><span class="sxs-lookup"><span data-stu-id="82fcc-190">cryptographyAllowFipsAlgorithmPolicy</span></span>|<span data-ttu-id="82fcc-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-191">Boolean</span></span>|<span data-ttu-id="82fcc-192">指定是否允许或禁止联邦信息处理标准 (FIPS) 策略。</span><span class="sxs-lookup"><span data-stu-id="82fcc-192">Specify whether to allow or disallow the Federal Information Processing Standard (FIPS) policy.</span></span>|
|<span data-ttu-id="82fcc-193">displayAppListWithGdiDPIScalingTurnedOn</span><span class="sxs-lookup"><span data-stu-id="82fcc-193">displayAppListWithGdiDPIScalingTurnedOn</span></span>|<span data-ttu-id="82fcc-194">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-194">String collection</span></span>|<span data-ttu-id="82fcc-195">已打开 GDI DPI 缩放比例的旧应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="82fcc-195">List of legacy applications that have GDI DPI Scaling turned on.</span></span>|
|<span data-ttu-id="82fcc-196">displayAppListWithGdiDPIScalingTurnedOff</span><span class="sxs-lookup"><span data-stu-id="82fcc-196">displayAppListWithGdiDPIScalingTurnedOff</span></span>|<span data-ttu-id="82fcc-197">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-197">String collection</span></span>|<span data-ttu-id="82fcc-198">已关闭 GDI DPI 缩放比例的旧应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="82fcc-198">List of legacy applications that have GDI DPI Scaling turned off.</span></span>|
|<span data-ttu-id="82fcc-199">enterpriseCloudPrintDiscoveryEndPoint</span><span class="sxs-lookup"><span data-stu-id="82fcc-199">enterpriseCloudPrintDiscoveryEndPoint</span></span>|<span data-ttu-id="82fcc-200">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-200">String</span></span>|<span data-ttu-id="82fcc-201">发现云打印机的终结点。</span><span class="sxs-lookup"><span data-stu-id="82fcc-201">Endpoint for discovering cloud printers.</span></span>|
|<span data-ttu-id="82fcc-202">enterpriseCloudPrintOAuthAuthority</span><span class="sxs-lookup"><span data-stu-id="82fcc-202">enterpriseCloudPrintOAuthAuthority</span></span>|<span data-ttu-id="82fcc-203">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-203">String</span></span>|<span data-ttu-id="82fcc-204">获取 OAuth 令牌的身份验证终结点。</span><span class="sxs-lookup"><span data-stu-id="82fcc-204">Authentication endpoint for acquiring OAuth tokens.</span></span>|
|<span data-ttu-id="82fcc-205">enterpriseCloudPrintOAuthClientIdentifier</span><span class="sxs-lookup"><span data-stu-id="82fcc-205">enterpriseCloudPrintOAuthClientIdentifier</span></span>|<span data-ttu-id="82fcc-206">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-206">String</span></span>|<span data-ttu-id="82fcc-207">被授权从 OAuth 机构检索 OAuth 令牌的客户端应用程序的 GUID。</span><span class="sxs-lookup"><span data-stu-id="82fcc-207">GUID of a client application authorized to retrieve OAuth tokens from the OAuth Authority.</span></span>|
|<span data-ttu-id="82fcc-208">enterpriseCloudPrintResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="82fcc-208">enterpriseCloudPrintResourceIdentifier</span></span>|<span data-ttu-id="82fcc-209">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-209">String</span></span>|<span data-ttu-id="82fcc-210">在 Azure 门户中配置的用于打印服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="82fcc-210">OAuth resource URI for print service as configured in the Azure portal.</span></span>|
|<span data-ttu-id="82fcc-211">enterpriseCloudPrintDiscoveryMaxLimit</span><span class="sxs-lookup"><span data-stu-id="82fcc-211">enterpriseCloudPrintDiscoveryMaxLimit</span></span>|<span data-ttu-id="82fcc-212">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-212">Int32</span></span>|<span data-ttu-id="82fcc-213">应该从发现终结点查询的打印机最大数量。</span><span class="sxs-lookup"><span data-stu-id="82fcc-213">Maximum number of printers that should be queried from a discovery endpoint.</span></span> <span data-ttu-id="82fcc-214">此设置仅限移动设备。</span><span class="sxs-lookup"><span data-stu-id="82fcc-214">This is a mobile only setting.</span></span> <span data-ttu-id="82fcc-215">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="82fcc-215">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="82fcc-216">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span><span class="sxs-lookup"><span data-stu-id="82fcc-216">enterpriseCloudPrintMopriaDiscoveryResourceIdentifier</span></span>|<span data-ttu-id="82fcc-217">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-217">String</span></span>|<span data-ttu-id="82fcc-218">在 Azure 门户中配置的用于打印机发现服务的 OAuth 资源 URI。</span><span class="sxs-lookup"><span data-stu-id="82fcc-218">OAuth resource URI for printer discovery service as configured in Azure portal.</span></span>|
|<span data-ttu-id="82fcc-219">messagingBlockSync</span><span class="sxs-lookup"><span data-stu-id="82fcc-219">messagingBlockSync</span></span>|<span data-ttu-id="82fcc-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-220">Boolean</span></span>|<span data-ttu-id="82fcc-221">指示阻止短信备份和还原和消息无处不在。</span><span class="sxs-lookup"><span data-stu-id="82fcc-221">Indicates whether or not to block text message back up and restore and Messaging Everywhere.</span></span>|
|<span data-ttu-id="82fcc-222">messagingBlockMMS</span><span class="sxs-lookup"><span data-stu-id="82fcc-222">messagingBlockMMS</span></span>|<span data-ttu-id="82fcc-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-223">Boolean</span></span>|<span data-ttu-id="82fcc-224">指示是否阻止 MMS 发送/接收的设备上的功能。</span><span class="sxs-lookup"><span data-stu-id="82fcc-224">Indicates whether or not to block the the MMS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="82fcc-225">messagingBlockRichCommunicationServices</span><span class="sxs-lookup"><span data-stu-id="82fcc-225">messagingBlockRichCommunicationServices</span></span>|<span data-ttu-id="82fcc-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-226">Boolean</span></span>|<span data-ttu-id="82fcc-227">指示是否阻止 RC 发送/接收的设备上的功能。</span><span class="sxs-lookup"><span data-stu-id="82fcc-227">Indicates whether or not to block the the RCS send/receive functionality on the device.</span></span>|
|<span data-ttu-id="82fcc-228">printerNames</span><span class="sxs-lookup"><span data-stu-id="82fcc-228">printerNames</span></span>|<span data-ttu-id="82fcc-229">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-229">String collection</span></span>|<span data-ttu-id="82fcc-230">自动设置打印机根据其名称 （网络主机名）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-230">Automatically provision printers based on their names (network host names).</span></span>|
|<span data-ttu-id="82fcc-231">printerDefaultName</span><span class="sxs-lookup"><span data-stu-id="82fcc-231">printerDefaultName</span></span>|<span data-ttu-id="82fcc-232">字符串</span><span class="sxs-lookup"><span data-stu-id="82fcc-232">String</span></span>|<span data-ttu-id="82fcc-233">已安装的打印机的名称 （网络主机名）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-233">Name (network host name) of an installed printer.</span></span>|
|<span data-ttu-id="82fcc-234">printerBlockAddition</span><span class="sxs-lookup"><span data-stu-id="82fcc-234">printerBlockAddition</span></span>|<span data-ttu-id="82fcc-235">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-235">Boolean</span></span>|<span data-ttu-id="82fcc-236">阻止用户安装的打印机设置中的其他打印机。</span><span class="sxs-lookup"><span data-stu-id="82fcc-236">Prevent user installation of additional printers from printers settings.</span></span>|
|<span data-ttu-id="82fcc-237">searchBlockDiacritics</span><span class="sxs-lookup"><span data-stu-id="82fcc-237">searchBlockDiacritics</span></span>|<span data-ttu-id="82fcc-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-238">Boolean</span></span>|<span data-ttu-id="82fcc-239">指定搜索是否可以使用音调符号。</span><span class="sxs-lookup"><span data-stu-id="82fcc-239">Specifies if search can use diacritics.</span></span>|
|<span data-ttu-id="82fcc-240">searchDisableAutoLanguageDetection</span><span class="sxs-lookup"><span data-stu-id="82fcc-240">searchDisableAutoLanguageDetection</span></span>|<span data-ttu-id="82fcc-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-241">Boolean</span></span>|<span data-ttu-id="82fcc-242">指定建立内容和属性索引时是否使用自动语言检测。</span><span class="sxs-lookup"><span data-stu-id="82fcc-242">Specifies whether to use automatic language detection when indexing content and properties.</span></span>|
|<span data-ttu-id="82fcc-243">searchDisableIndexingEncryptedItems</span><span class="sxs-lookup"><span data-stu-id="82fcc-243">searchDisableIndexingEncryptedItems</span></span>|<span data-ttu-id="82fcc-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-244">Boolean</span></span>|<span data-ttu-id="82fcc-245">指示是否阻止建立 WIP 保护项的索引，以阻止它们出现在 Cortana 或资源管理器的搜索结果中。</span><span class="sxs-lookup"><span data-stu-id="82fcc-245">Indicates whether or not to block indexing of WIP-protected items to prevent them from appearing in search results for Cortana or Explorer.</span></span>|
|<span data-ttu-id="82fcc-246">searchEnableRemoteQueries</span><span class="sxs-lookup"><span data-stu-id="82fcc-246">searchEnableRemoteQueries</span></span>|<span data-ttu-id="82fcc-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-247">Boolean</span></span>|<span data-ttu-id="82fcc-248">指示是否阻止此计算机索引的远程查询。</span><span class="sxs-lookup"><span data-stu-id="82fcc-248">Indicates whether or not to block remote queries of this computer’s index.</span></span>|
|<span data-ttu-id="82fcc-249">searchDisableUseLocation</span><span class="sxs-lookup"><span data-stu-id="82fcc-249">searchDisableUseLocation</span></span>|<span data-ttu-id="82fcc-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-250">Boolean</span></span>|<span data-ttu-id="82fcc-251">指定搜索可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="82fcc-251">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="82fcc-252">searchDisableLocation</span><span class="sxs-lookup"><span data-stu-id="82fcc-252">searchDisableLocation</span></span>|<span data-ttu-id="82fcc-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-253">Boolean</span></span>|<span data-ttu-id="82fcc-254">指定搜索可以使用位置信息。</span><span class="sxs-lookup"><span data-stu-id="82fcc-254">Specifies if search can use location information.</span></span>|
|<span data-ttu-id="82fcc-255">searchDisableIndexerBackoff</span><span class="sxs-lookup"><span data-stu-id="82fcc-255">searchDisableIndexerBackoff</span></span>|<span data-ttu-id="82fcc-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-256">Boolean</span></span>|<span data-ttu-id="82fcc-257">指示是否禁用搜索索引器回退功能。</span><span class="sxs-lookup"><span data-stu-id="82fcc-257">Indicates whether or not to disable the search indexer backoff feature.</span></span>|
|<span data-ttu-id="82fcc-258">searchDisableIndexingRemovableDrive</span><span class="sxs-lookup"><span data-stu-id="82fcc-258">searchDisableIndexingRemovableDrive</span></span>|<span data-ttu-id="82fcc-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-259">Boolean</span></span>|<span data-ttu-id="82fcc-260">指示是否允许用户将可移动驱动器上的位置添加到库并建立索引。</span><span class="sxs-lookup"><span data-stu-id="82fcc-260">Indicates whether or not to allow users to add locations on removable drives to libraries and to be indexed.</span></span>|
|<span data-ttu-id="82fcc-261">searchEnableAutomaticIndexSizeManangement</span><span class="sxs-lookup"><span data-stu-id="82fcc-261">searchEnableAutomaticIndexSizeManangement</span></span>|<span data-ttu-id="82fcc-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-262">Boolean</span></span>|<span data-ttu-id="82fcc-263">在建立索引停止之前，指定与索引位置相同的驱动器上的最小硬盘空间量。</span><span class="sxs-lookup"><span data-stu-id="82fcc-263">Specifies minimum amount of hard drive space on the same drive as the index location before indexing stops.</span></span>|
|<span data-ttu-id="82fcc-264">searchBlockWebResults</span><span class="sxs-lookup"><span data-stu-id="82fcc-264">searchBlockWebResults</span></span>|<span data-ttu-id="82fcc-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-265">Boolean</span></span>|<span data-ttu-id="82fcc-266">指示阻止 web 搜索。</span><span class="sxs-lookup"><span data-stu-id="82fcc-266">Indicates whether or not to block the web search.</span></span>|
|<span data-ttu-id="82fcc-267">securityBlockAzureADJoinedDevicesAutoEncryption</span><span class="sxs-lookup"><span data-stu-id="82fcc-267">securityBlockAzureADJoinedDevicesAutoEncryption</span></span>|<span data-ttu-id="82fcc-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-268">Boolean</span></span>|<span data-ttu-id="82fcc-269">指定是否允许设备自动加密期间 OOBE 设备时 Azure AD 加入 （仅适用于桌面）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-269">Specify whether to allow automatic device encryption during OOBE when the device is Azure AD joined (desktop only).</span></span>|
|<span data-ttu-id="82fcc-270">diagnosticsDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="82fcc-270">diagnosticsDataSubmissionMode</span></span>|[<span data-ttu-id="82fcc-271">diagnosticDataSubmissionMode</span><span class="sxs-lookup"><span data-stu-id="82fcc-271">diagnosticDataSubmissionMode</span></span>](../resources/intune-deviceconfig-diagnosticdatasubmissionmode.md)|<span data-ttu-id="82fcc-272">获取或设置允许设备发送诊断和使用遥测数据的值，如 Watson。</span><span class="sxs-lookup"><span data-stu-id="82fcc-272">Gets or sets a value allowing the device to send diagnostic and usage telemetry data, such as Watson.</span></span> <span data-ttu-id="82fcc-273">可取值为：`userDefined`、`none`、`basic`、`enhanced`、`full`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-273">Possible values are: `userDefined`, `none`, `basic`, `enhanced`, `full`.</span></span>|
|<span data-ttu-id="82fcc-274">oneDriveDisableFileSync</span><span class="sxs-lookup"><span data-stu-id="82fcc-274">oneDriveDisableFileSync</span></span>|<span data-ttu-id="82fcc-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-275">Boolean</span></span>|<span data-ttu-id="82fcc-276">获取或设置一个值，允许 IT 管理员阻止应用和功能使用 OneDrive 上的文件。</span><span class="sxs-lookup"><span data-stu-id="82fcc-276">Gets or sets a value allowing IT admins to prevent apps and features from working with files on OneDrive.</span></span>|
|<span data-ttu-id="82fcc-277">systemTelemetryProxyServer</span><span class="sxs-lookup"><span data-stu-id="82fcc-277">systemTelemetryProxyServer</span></span>|<span data-ttu-id="82fcc-278">字符串</span><span class="sxs-lookup"><span data-stu-id="82fcc-278">String</span></span>|<span data-ttu-id="82fcc-279">获取或设置的完全限定的域名 (FQDN) 或代理服务器连接的用户体验和遥测请求转发的 IP 地址。</span><span class="sxs-lookup"><span data-stu-id="82fcc-279">Gets or sets the fully qualified domain name (FQDN) or IP address of a proxy server to forward Connected User Experiences and Telemetry requests.</span></span>|
|<span data-ttu-id="82fcc-280">inkWorkspaceAccess</span><span class="sxs-lookup"><span data-stu-id="82fcc-280">inkWorkspaceAccess</span></span>|[<span data-ttu-id="82fcc-281">inkAccessSetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-281">inkAccessSetting</span></span>](../resources/intune-deviceconfig-inkaccesssetting.md)|<span data-ttu-id="82fcc-282">控制用户访问墨迹工作区中，在桌面上，然后从锁定屏幕上上述。</span><span class="sxs-lookup"><span data-stu-id="82fcc-282">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="82fcc-283">可取值为：`notConfigured`、`enabled`、`disabled`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-283">Possible values are: `notConfigured`, `enabled`, `disabled`.</span></span>|
|<span data-ttu-id="82fcc-284">inkWorkspaceAccessState</span><span class="sxs-lookup"><span data-stu-id="82fcc-284">inkWorkspaceAccessState</span></span>|[<span data-ttu-id="82fcc-285">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-285">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="82fcc-286">控制用户访问墨迹工作区中，在桌面上，然后从锁定屏幕上上述。</span><span class="sxs-lookup"><span data-stu-id="82fcc-286">Controls the user access to the ink workspace, from the desktop and from above the lock screen.</span></span> <span data-ttu-id="82fcc-287">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-287">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="82fcc-288">inkWorkspaceBlockSuggestedApps</span><span class="sxs-lookup"><span data-stu-id="82fcc-288">inkWorkspaceBlockSuggestedApps</span></span>|<span data-ttu-id="82fcc-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-289">Boolean</span></span>|<span data-ttu-id="82fcc-290">指定是否在墨迹工作区中显示建议的应用程序建议。</span><span class="sxs-lookup"><span data-stu-id="82fcc-290">Specify whether to show recommended app suggestions in the ink workspace.</span></span>|
|<span data-ttu-id="82fcc-291">smartScreenEnableAppInstallControl</span><span class="sxs-lookup"><span data-stu-id="82fcc-291">smartScreenEnableAppInstallControl</span></span>|<span data-ttu-id="82fcc-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-292">Boolean</span></span>|<span data-ttu-id="82fcc-293">允许 IT 管理员控制是否允许用户从应用商店以外的地方安装应用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-293">Allows IT Admins to control whether users are allowed to install apps from places other than the Store.</span></span>|
|<span data-ttu-id="82fcc-294">personalizationDesktopImageUrl</span><span class="sxs-lookup"><span data-stu-id="82fcc-294">personalizationDesktopImageUrl</span></span>|<span data-ttu-id="82fcc-295">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-295">String</span></span>|<span data-ttu-id="82fcc-296">指向需要下载并用作桌面图像的 http 或 https URL，或指向需要用作桌面图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="82fcc-296">A http or https Url to a jpg, jpeg or png image that needs to be downloaded and used as the Desktop Image or a file Url to a local image on the file system that needs to used as the Desktop Image.</span></span>|
|<span data-ttu-id="82fcc-297">personalizationLockScreenImageUrl</span><span class="sxs-lookup"><span data-stu-id="82fcc-297">personalizationLockScreenImageUrl</span></span>|<span data-ttu-id="82fcc-298">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-298">String</span></span>|<span data-ttu-id="82fcc-299">指向需要下载并用作锁屏图像的 jpg、jpeg 或 png 图像的 http 或 https URL，或指向需要用作锁屏图像的文件系统上的本地图像的文件 URL。</span><span class="sxs-lookup"><span data-stu-id="82fcc-299">A http or https Url to a jpg, jpeg or png image that neeeds to be downloaded and used as the Lock Screen Image or a file Url to a local image on the file system that needs to be used as the Lock Screen Image.</span></span>|
|<span data-ttu-id="82fcc-300">bluetoothAllowedServices</span><span class="sxs-lookup"><span data-stu-id="82fcc-300">bluetoothAllowedServices</span></span>|<span data-ttu-id="82fcc-301">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-301">String collection</span></span>|<span data-ttu-id="82fcc-302">以十六进制格式的字符串指定允许的蓝牙服务和配置文件的列表。</span><span class="sxs-lookup"><span data-stu-id="82fcc-302">Specify a list of allowed Bluetooth services and profiles in hex formatted strings.</span></span>|
|<span data-ttu-id="82fcc-303">bluetoothBlockAdvertising</span><span class="sxs-lookup"><span data-stu-id="82fcc-303">bluetoothBlockAdvertising</span></span>|<span data-ttu-id="82fcc-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-304">Boolean</span></span>|<span data-ttu-id="82fcc-305">是否阻止用户使用蓝牙广告。</span><span class="sxs-lookup"><span data-stu-id="82fcc-305">Whether or not to Block the user from using bluetooth advertising.</span></span>|
|<span data-ttu-id="82fcc-306">bluetoothBlockDiscoverableMode</span><span class="sxs-lookup"><span data-stu-id="82fcc-306">bluetoothBlockDiscoverableMode</span></span>|<span data-ttu-id="82fcc-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-307">Boolean</span></span>|<span data-ttu-id="82fcc-308">是否阻止用户使用蓝牙可发现模式。</span><span class="sxs-lookup"><span data-stu-id="82fcc-308">Whether or not to Block the user from using bluetooth discoverable mode.</span></span>|
|<span data-ttu-id="82fcc-309">bluetoothBlockPrePairing</span><span class="sxs-lookup"><span data-stu-id="82fcc-309">bluetoothBlockPrePairing</span></span>|<span data-ttu-id="82fcc-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-310">Boolean</span></span>|<span data-ttu-id="82fcc-311">是否阻止特定的捆绑蓝牙外围设备自动与主机设备配对。</span><span class="sxs-lookup"><span data-stu-id="82fcc-311">Whether or not to block specific bundled Bluetooth peripherals to automatically pair with the host device.</span></span>|
|<span data-ttu-id="82fcc-312">edgeBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="82fcc-312">edgeBlockAutofill</span></span>|<span data-ttu-id="82fcc-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-313">Boolean</span></span>|<span data-ttu-id="82fcc-314">指示是否阻止自动填充。</span><span class="sxs-lookup"><span data-stu-id="82fcc-314">Indicates whether or not to block auto fill.</span></span>|
|<span data-ttu-id="82fcc-315">edgeBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-315">edgeBlocked</span></span>|<span data-ttu-id="82fcc-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-316">Boolean</span></span>|<span data-ttu-id="82fcc-317">指示是否阻止用户使用 Edge 浏览器。</span><span class="sxs-lookup"><span data-stu-id="82fcc-317">Indicates whether or not to Block the user from using the Edge browser.</span></span>|
|<span data-ttu-id="82fcc-318">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="82fcc-318">edgeCookiePolicy</span></span>|[<span data-ttu-id="82fcc-319">edgeCookiePolicy</span><span class="sxs-lookup"><span data-stu-id="82fcc-319">edgeCookiePolicy</span></span>](../resources/intune-deviceconfig-edgecookiepolicy.md)|<span data-ttu-id="82fcc-320">指示要在 Edge 浏览器中阻止的 Cookie。</span><span class="sxs-lookup"><span data-stu-id="82fcc-320">Indicates which cookies to block in the Edge browser.</span></span> <span data-ttu-id="82fcc-321">可取值为：`userDefined`、`allow`、`blockThirdParty`、`blockAll`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-321">Possible values are: `userDefined`, `allow`, `blockThirdParty`, `blockAll`.</span></span>|
|<span data-ttu-id="82fcc-322">edgeBlockDeveloperTools</span><span class="sxs-lookup"><span data-stu-id="82fcc-322">edgeBlockDeveloperTools</span></span>|<span data-ttu-id="82fcc-323">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-323">Boolean</span></span>|<span data-ttu-id="82fcc-324">指示是否在 Edge 浏览器中阻止开发人员工具。</span><span class="sxs-lookup"><span data-stu-id="82fcc-324">Indicates whether or not to block developer tools in the Edge browser.</span></span>|
|<span data-ttu-id="82fcc-325">edgeBlockSendingDoNotTrackHeader</span><span class="sxs-lookup"><span data-stu-id="82fcc-325">edgeBlockSendingDoNotTrackHeader</span></span>|<span data-ttu-id="82fcc-326">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-326">Boolean</span></span>|<span data-ttu-id="82fcc-327">指示是否阻止用户发送 Do Not Track 标头。</span><span class="sxs-lookup"><span data-stu-id="82fcc-327">Indicates whether or not to Block the user from sending the do not track header.</span></span>|
|<span data-ttu-id="82fcc-328">edgeBlockExtensions</span><span class="sxs-lookup"><span data-stu-id="82fcc-328">edgeBlockExtensions</span></span>|<span data-ttu-id="82fcc-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-329">Boolean</span></span>|<span data-ttu-id="82fcc-330">指示是否在 Edge 浏览器中阻止扩展。</span><span class="sxs-lookup"><span data-stu-id="82fcc-330">Indicates whether or not to block extensions in the Edge browser.</span></span>|
|<span data-ttu-id="82fcc-331">edgeBlockInPrivateBrowsing</span><span class="sxs-lookup"><span data-stu-id="82fcc-331">edgeBlockInPrivateBrowsing</span></span>|<span data-ttu-id="82fcc-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-332">Boolean</span></span>|<span data-ttu-id="82fcc-333">指示是否在 Edge 浏览器中阻止公司网络上的 InPrivate 浏览。</span><span class="sxs-lookup"><span data-stu-id="82fcc-333">Indicates whether or not to block InPrivate browsing on corporate networks, in the Edge browser.</span></span>|
|<span data-ttu-id="82fcc-334">edgeBlockJavaScript</span><span class="sxs-lookup"><span data-stu-id="82fcc-334">edgeBlockJavaScript</span></span>|<span data-ttu-id="82fcc-335">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-335">Boolean</span></span>|<span data-ttu-id="82fcc-336">指示是否阻止用户使用 JavaScript。</span><span class="sxs-lookup"><span data-stu-id="82fcc-336">Indicates whether or not to Block the user from using JavaScript.</span></span>|
|<span data-ttu-id="82fcc-337">edgeBlockPasswordManager</span><span class="sxs-lookup"><span data-stu-id="82fcc-337">edgeBlockPasswordManager</span></span>|<span data-ttu-id="82fcc-338">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-338">Boolean</span></span>|<span data-ttu-id="82fcc-339">指示是否阻止密码管理器。</span><span class="sxs-lookup"><span data-stu-id="82fcc-339">Indicates whether or not to Block password manager.</span></span>|
|<span data-ttu-id="82fcc-340">edgeBlockAddressBarDropdown</span><span class="sxs-lookup"><span data-stu-id="82fcc-340">edgeBlockAddressBarDropdown</span></span>|<span data-ttu-id="82fcc-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-341">Boolean</span></span>|<span data-ttu-id="82fcc-342">阻止 Microsoft Edge 中的地址栏下拉功能。</span><span class="sxs-lookup"><span data-stu-id="82fcc-342">Block the address bar dropdown functionality in Microsoft Edge.</span></span> <span data-ttu-id="82fcc-343">禁用此设置可最大限度地减少从 Microsoft Edge 到 Microsoft 服务的网络连接。</span><span class="sxs-lookup"><span data-stu-id="82fcc-343">Disable this settings to minimize network connections from Microsoft Edge to Microsoft services.</span></span>|
|<span data-ttu-id="82fcc-344">edgeBlockCompatibilityList</span><span class="sxs-lookup"><span data-stu-id="82fcc-344">edgeBlockCompatibilityList</span></span>|<span data-ttu-id="82fcc-345">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-345">Boolean</span></span>|<span data-ttu-id="82fcc-346">阻止 Microsoft Edge 中的 Microsoft 兼容性列表。</span><span class="sxs-lookup"><span data-stu-id="82fcc-346">Block Microsoft compatibility list in Microsoft Edge.</span></span> <span data-ttu-id="82fcc-347">Microsoft 提供的此列表可帮助 Edge 正确显示具有已知兼容性问题的网站。</span><span class="sxs-lookup"><span data-stu-id="82fcc-347">This list from Microsoft helps Edge properly display sites with known compatibility issues.</span></span>|
|<span data-ttu-id="82fcc-348">edgeClearBrowsingDataOnExit</span><span class="sxs-lookup"><span data-stu-id="82fcc-348">edgeClearBrowsingDataOnExit</span></span>|<span data-ttu-id="82fcc-349">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-349">Boolean</span></span>|<span data-ttu-id="82fcc-350">退出 Microsoft Edge 时清除浏览数据。</span><span class="sxs-lookup"><span data-stu-id="82fcc-350">Clear browsing data on exiting Microsoft Edge.</span></span>|
|<span data-ttu-id="82fcc-351">edgeAllowStartPagesModification</span><span class="sxs-lookup"><span data-stu-id="82fcc-351">edgeAllowStartPagesModification</span></span>|<span data-ttu-id="82fcc-352">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-352">Boolean</span></span>|<span data-ttu-id="82fcc-353">允许用户更改 Edge 上的开始页面。</span><span class="sxs-lookup"><span data-stu-id="82fcc-353">Allow users to change Start pages on Edge.</span></span> <span data-ttu-id="82fcc-354">使用 EdgeHomepageUrls 指定用户在打开 Edge 时默认会看到的开始页面。</span><span class="sxs-lookup"><span data-stu-id="82fcc-354">Use the EdgeHomepageUrls to specify the Start pages that the user would see by default when they open Edge.</span></span>|
|<span data-ttu-id="82fcc-355">edgeDisableFirstRunPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-355">edgeDisableFirstRunPage</span></span>|<span data-ttu-id="82fcc-356">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-356">Boolean</span></span>|<span data-ttu-id="82fcc-357">阻止首次使用 Microsoft Edge 时打开的 Microsoft 网页。</span><span class="sxs-lookup"><span data-stu-id="82fcc-357">Block the Microsoft web page that opens on the first use of Microsoft Edge.</span></span> <span data-ttu-id="82fcc-358">此策略允许企业（如那些参与零排放配置的企业）阻止此页面。</span><span class="sxs-lookup"><span data-stu-id="82fcc-358">This policy allows enterprises, like those enrolled in zero emissions configurations, to block this page.</span></span>|
|<span data-ttu-id="82fcc-359">edgeBlockLiveTileDataCollection</span><span class="sxs-lookup"><span data-stu-id="82fcc-359">edgeBlockLiveTileDataCollection</span></span>|<span data-ttu-id="82fcc-360">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-360">Boolean</span></span>|<span data-ttu-id="82fcc-361">当用户将某个网站固定为从 Microsoft Edge 启动时，阻止 Microsoft 收集用于实时磁贴创建的信息。</span><span class="sxs-lookup"><span data-stu-id="82fcc-361">Block the collection of information by Microsoft for live tile creation when users pin a site to Start from Microsoft Edge.</span></span>|
|<span data-ttu-id="82fcc-362">edgeSyncFavoritesWithInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="82fcc-362">edgeSyncFavoritesWithInternetExplorer</span></span>|<span data-ttu-id="82fcc-363">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-363">Boolean</span></span>|<span data-ttu-id="82fcc-364">在 Internet Explorer 和 Microsoft Edge 之间启用收藏夹同步。</span><span class="sxs-lookup"><span data-stu-id="82fcc-364">Enable favorites sync between Internet Explorer and Microsoft Edge.</span></span> <span data-ttu-id="82fcc-365">在浏览器之间共享对收藏夹的添加、删除、修改和顺序更改。</span><span class="sxs-lookup"><span data-stu-id="82fcc-365">Additions, deletions, modifications and order changes to favorites are shared between browsers.</span></span>|
|<span data-ttu-id="82fcc-366">edgeFavoritesListLocation</span><span class="sxs-lookup"><span data-stu-id="82fcc-366">edgeFavoritesListLocation</span></span>|<span data-ttu-id="82fcc-367">字符串</span><span class="sxs-lookup"><span data-stu-id="82fcc-367">String</span></span>|<span data-ttu-id="82fcc-368">设置的收藏夹列表的位置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-368">The location of the favorites list to provision.</span></span> <span data-ttu-id="82fcc-369">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-369">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="82fcc-370">edgeBlockEditFavorites</span><span class="sxs-lookup"><span data-stu-id="82fcc-370">edgeBlockEditFavorites</span></span>|<span data-ttu-id="82fcc-371">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-371">Boolean</span></span>|<span data-ttu-id="82fcc-372">指示阻止用户更改收藏夹。</span><span class="sxs-lookup"><span data-stu-id="82fcc-372">Indicates whether or not to Block the user from making changes to Favorites.</span></span>|
|<span data-ttu-id="82fcc-373">cellularBlockDataWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="82fcc-373">cellularBlockDataWhenRoaming</span></span>|<span data-ttu-id="82fcc-374">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-374">Boolean</span></span>|<span data-ttu-id="82fcc-375">是否阻止用户在漫游时通过手机网络使用数据。</span><span class="sxs-lookup"><span data-stu-id="82fcc-375">Whether or not to Block the user from using data over cellular while roaming.</span></span>|
|<span data-ttu-id="82fcc-376">cellularBlockVpn</span><span class="sxs-lookup"><span data-stu-id="82fcc-376">cellularBlockVpn</span></span>|<span data-ttu-id="82fcc-377">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-377">Boolean</span></span>|<span data-ttu-id="82fcc-378">是否阻止用户通过手机网络使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="82fcc-378">Whether or not to Block the user from using VPN over cellular.</span></span>|
|<span data-ttu-id="82fcc-379">cellularBlockVpnWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="82fcc-379">cellularBlockVpnWhenRoaming</span></span>|<span data-ttu-id="82fcc-380">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-380">Boolean</span></span>|<span data-ttu-id="82fcc-381">是否阻止用户在通过手机网络漫游时使用 VPN。</span><span class="sxs-lookup"><span data-stu-id="82fcc-381">Whether or not to Block the user from using VPN when roaming over cellular.</span></span>|
|<span data-ttu-id="82fcc-382">cellularData</span><span class="sxs-lookup"><span data-stu-id="82fcc-382">cellularData</span></span>|[<span data-ttu-id="82fcc-383">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="82fcc-383">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="82fcc-384">是否在设备上允许移动数据信道。</span><span class="sxs-lookup"><span data-stu-id="82fcc-384">Whether or not to allow the cellular data channel on the device.</span></span> <span data-ttu-id="82fcc-385">如果未配置，允许移动数据通道，用户可以将其关闭。</span><span class="sxs-lookup"><span data-stu-id="82fcc-385">If not configured, the cellular data channel is allowed and the user can turn it off.</span></span> <span data-ttu-id="82fcc-386">可取值为：`blocked`、`required`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-386">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="82fcc-387">defenderBlockEndUserAccess</span><span class="sxs-lookup"><span data-stu-id="82fcc-387">defenderBlockEndUserAccess</span></span>|<span data-ttu-id="82fcc-388">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-388">Boolean</span></span>|<span data-ttu-id="82fcc-389">是否阻止最终用户访问 Defender。</span><span class="sxs-lookup"><span data-stu-id="82fcc-389">Whether or not to block end user access to Defender.</span></span>|
|<span data-ttu-id="82fcc-390">defenderDaysBeforeDeletingQuarantinedMalware</span><span class="sxs-lookup"><span data-stu-id="82fcc-390">defenderDaysBeforeDeletingQuarantinedMalware</span></span>|<span data-ttu-id="82fcc-391">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-391">Int32</span></span>|<span data-ttu-id="82fcc-392">删除隔离的恶意软件之前的天数。</span><span class="sxs-lookup"><span data-stu-id="82fcc-392">Number of days before deleting quarantined malware.</span></span> <span data-ttu-id="82fcc-393">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="82fcc-393">Valid values 0 to 90</span></span>|
|<span data-ttu-id="82fcc-394">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="82fcc-394">defenderDetectedMalwareActions</span></span>|[<span data-ttu-id="82fcc-395">defenderDetectedMalwareActions</span><span class="sxs-lookup"><span data-stu-id="82fcc-395">defenderDetectedMalwareActions</span></span>](../resources/intune-deviceconfig-defenderdetectedmalwareactions.md)|<span data-ttu-id="82fcc-396">获取或设置要按威胁级别对检测到的恶意软件执行的 Defender 操作。</span><span class="sxs-lookup"><span data-stu-id="82fcc-396">Gets or sets Defender’s actions to take on detected Malware per threat level.</span></span>|
|<span data-ttu-id="82fcc-397">defenderSystemScanSchedule</span><span class="sxs-lookup"><span data-stu-id="82fcc-397">defenderSystemScanSchedule</span></span>|[<span data-ttu-id="82fcc-398">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="82fcc-398">weeklySchedule</span></span>](../resources/intune-deviceconfig-weeklyschedule.md)|<span data-ttu-id="82fcc-399">Defender 进行系统扫描的星期几。</span><span class="sxs-lookup"><span data-stu-id="82fcc-399">Defender day of the week for the system scan.</span></span> <span data-ttu-id="82fcc-400">可取值为：`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-400">Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="82fcc-401">defenderFilesAndFoldersToExclude</span><span class="sxs-lookup"><span data-stu-id="82fcc-401">defenderFilesAndFoldersToExclude</span></span>|<span data-ttu-id="82fcc-402">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-402">String collection</span></span>|<span data-ttu-id="82fcc-403">要从扫描和实时保护中排除的文件和文件夹。</span><span class="sxs-lookup"><span data-stu-id="82fcc-403">Files and folder to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="82fcc-404">defenderFileExtensionsToExclude</span><span class="sxs-lookup"><span data-stu-id="82fcc-404">defenderFileExtensionsToExclude</span></span>|<span data-ttu-id="82fcc-405">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-405">String collection</span></span>|<span data-ttu-id="82fcc-406">要从扫描和实时保护中排除的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="82fcc-406">File extensions to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="82fcc-407">defenderScanMaxCpu</span><span class="sxs-lookup"><span data-stu-id="82fcc-407">defenderScanMaxCpu</span></span>|<span data-ttu-id="82fcc-408">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-408">Int32</span></span>|<span data-ttu-id="82fcc-409">扫描期间最大 CPU 使用率。</span><span class="sxs-lookup"><span data-stu-id="82fcc-409">Max CPU usage percentage during scan.</span></span> <span data-ttu-id="82fcc-410">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="82fcc-410">Valid values 0 to 100</span></span>|
|<span data-ttu-id="82fcc-411">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="82fcc-411">defenderMonitorFileActivity</span></span>|[<span data-ttu-id="82fcc-412">defenderMonitorFileActivity</span><span class="sxs-lookup"><span data-stu-id="82fcc-412">defenderMonitorFileActivity</span></span>](../resources/intune-deviceconfig-defendermonitorfileactivity.md)|<span data-ttu-id="82fcc-413">监视文件活动的值。</span><span class="sxs-lookup"><span data-stu-id="82fcc-413">Value for monitoring file activity.</span></span> <span data-ttu-id="82fcc-414">可取值为：`userDefined`、`disable`、`monitorAllFiles`、`monitorIncomingFilesOnly`、`monitorOutgoingFilesOnly`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-414">Possible values are: `userDefined`, `disable`, `monitorAllFiles`, `monitorIncomingFilesOnly`, `monitorOutgoingFilesOnly`.</span></span>|
|<span data-ttu-id="82fcc-415">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="82fcc-415">defenderPotentiallyUnwantedAppAction</span></span>|[<span data-ttu-id="82fcc-416">defenderPotentiallyUnwantedAppAction</span><span class="sxs-lookup"><span data-stu-id="82fcc-416">defenderPotentiallyUnwantedAppAction</span></span>](../resources/intune-deviceconfig-defenderpotentiallyunwantedappaction.md)|<span data-ttu-id="82fcc-417">获取或设置要执行上可能不需要应用程序 (PUA)，其中包括与 ad 注入，软件捆绑、 持久请求的付款或订阅等的行为的软件的 Defender 的操作。PUA 正在下载，或尝试自行安装时，则 defender 通知用户。</span><span class="sxs-lookup"><span data-stu-id="82fcc-417">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="82fcc-418">添加 Windows 10 中的桌面。</span><span class="sxs-lookup"><span data-stu-id="82fcc-418">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="82fcc-419">可取值为：`deviceDefault`、`block`、`audit`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-419">Possible values are: `deviceDefault`, `block`, `audit`.</span></span>|
|<span data-ttu-id="82fcc-420">defenderPotentiallyUnwantedAppActionSetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-420">defenderPotentiallyUnwantedAppActionSetting</span></span>|[<span data-ttu-id="82fcc-421">defenderProtectionType</span><span class="sxs-lookup"><span data-stu-id="82fcc-421">defenderProtectionType</span></span>](../resources/intune-deviceconfig-defenderprotectiontype.md)|<span data-ttu-id="82fcc-422">获取或设置要执行上可能不需要应用程序 (PUA)，其中包括与 ad 注入，软件捆绑、 持久请求的付款或订阅等的行为的软件的 Defender 的操作。PUA 正在下载，或尝试自行安装时，则 defender 通知用户。</span><span class="sxs-lookup"><span data-stu-id="82fcc-422">Gets or sets Defender’s action to take on Potentially Unwanted Application (PUA), which includes software with behaviors of ad-injection, software bundling, persistent solicitation for payment or subscription, etc. Defender alerts user when PUA is being downloaded or attempts to install itself.</span></span> <span data-ttu-id="82fcc-423">添加 Windows 10 中的桌面。</span><span class="sxs-lookup"><span data-stu-id="82fcc-423">Added in Windows 10 for desktop.</span></span> <span data-ttu-id="82fcc-424">可取值为：`userDefined`、`enable`、`auditMode`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-424">Possible values are: `userDefined`, `enable`, `auditMode`.</span></span>|
|<span data-ttu-id="82fcc-425">defenderProcessesToExclude</span><span class="sxs-lookup"><span data-stu-id="82fcc-425">defenderProcessesToExclude</span></span>|<span data-ttu-id="82fcc-426">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-426">String collection</span></span>|<span data-ttu-id="82fcc-427">要从扫描和实时保护中排除的进程。</span><span class="sxs-lookup"><span data-stu-id="82fcc-427">Processes to exclude from scans and real time protection.</span></span>|
|<span data-ttu-id="82fcc-428">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="82fcc-428">defenderPromptForSampleSubmission</span></span>|[<span data-ttu-id="82fcc-429">defenderPromptForSampleSubmission</span><span class="sxs-lookup"><span data-stu-id="82fcc-429">defenderPromptForSampleSubmission</span></span>](../resources/intune-deviceconfig-defenderpromptforsamplesubmission.md)|<span data-ttu-id="82fcc-430">如何提示用户提交样本的配置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-430">The configuration for how to prompt user for sample submission.</span></span> <span data-ttu-id="82fcc-431">可取值为：`userDefined`、`alwaysPrompt`、`promptBeforeSendingPersonalData`、`neverSendData`、`sendAllDataWithoutPrompting`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-431">Possible values are: `userDefined`, `alwaysPrompt`, `promptBeforeSendingPersonalData`, `neverSendData`, `sendAllDataWithoutPrompting`.</span></span>|
|<span data-ttu-id="82fcc-432">defenderRequireBehaviorMonitoring</span><span class="sxs-lookup"><span data-stu-id="82fcc-432">defenderRequireBehaviorMonitoring</span></span>|<span data-ttu-id="82fcc-433">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-433">Boolean</span></span>|<span data-ttu-id="82fcc-434">指示是否需要行为监控。</span><span class="sxs-lookup"><span data-stu-id="82fcc-434">Indicates whether or not to require behavior monitoring.</span></span>|
|<span data-ttu-id="82fcc-435">defenderRequireCloudProtection</span><span class="sxs-lookup"><span data-stu-id="82fcc-435">defenderRequireCloudProtection</span></span>|<span data-ttu-id="82fcc-436">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-436">Boolean</span></span>|<span data-ttu-id="82fcc-437">指示是否需要云保护。</span><span class="sxs-lookup"><span data-stu-id="82fcc-437">Indicates whether or not to require cloud protection.</span></span>|
|<span data-ttu-id="82fcc-438">defenderRequireNetworkInspectionSystem</span><span class="sxs-lookup"><span data-stu-id="82fcc-438">defenderRequireNetworkInspectionSystem</span></span>|<span data-ttu-id="82fcc-439">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-439">Boolean</span></span>|<span data-ttu-id="82fcc-440">指示是否需要网络检查系统。</span><span class="sxs-lookup"><span data-stu-id="82fcc-440">Indicates whether or not to require network inspection system.</span></span>|
|<span data-ttu-id="82fcc-441">defenderRequireRealTimeMonitoring</span><span class="sxs-lookup"><span data-stu-id="82fcc-441">defenderRequireRealTimeMonitoring</span></span>|<span data-ttu-id="82fcc-442">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-442">Boolean</span></span>|<span data-ttu-id="82fcc-443">指示是否需要实时监控。</span><span class="sxs-lookup"><span data-stu-id="82fcc-443">Indicates whether or not to require real time monitoring.</span></span>|
|<span data-ttu-id="82fcc-444">defenderScanArchiveFiles</span><span class="sxs-lookup"><span data-stu-id="82fcc-444">defenderScanArchiveFiles</span></span>|<span data-ttu-id="82fcc-445">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-445">Boolean</span></span>|<span data-ttu-id="82fcc-446">指示是否扫描存档文件。</span><span class="sxs-lookup"><span data-stu-id="82fcc-446">Indicates whether or not to scan archive files.</span></span>|
|<span data-ttu-id="82fcc-447">defenderScanDownloads</span><span class="sxs-lookup"><span data-stu-id="82fcc-447">defenderScanDownloads</span></span>|<span data-ttu-id="82fcc-448">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-448">Boolean</span></span>|<span data-ttu-id="82fcc-449">指示是否扫描下载内容。</span><span class="sxs-lookup"><span data-stu-id="82fcc-449">Indicates whether or not to scan downloads.</span></span>|
|<span data-ttu-id="82fcc-450">defenderScanNetworkFiles</span><span class="sxs-lookup"><span data-stu-id="82fcc-450">defenderScanNetworkFiles</span></span>|<span data-ttu-id="82fcc-451">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-451">Boolean</span></span>|<span data-ttu-id="82fcc-452">指示是否扫描从网络文件夹打开的文件。</span><span class="sxs-lookup"><span data-stu-id="82fcc-452">Indicates whether or not to scan files opened from a network folder.</span></span>|
|<span data-ttu-id="82fcc-453">defenderScanIncomingMail</span><span class="sxs-lookup"><span data-stu-id="82fcc-453">defenderScanIncomingMail</span></span>|<span data-ttu-id="82fcc-454">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-454">Boolean</span></span>|<span data-ttu-id="82fcc-455">指示是否扫描传入的邮件。</span><span class="sxs-lookup"><span data-stu-id="82fcc-455">Indicates whether or not to scan incoming mail messages.</span></span>|
|<span data-ttu-id="82fcc-456">defenderScanMappedNetworkDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="82fcc-456">defenderScanMappedNetworkDrivesDuringFullScan</span></span>|<span data-ttu-id="82fcc-457">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-457">Boolean</span></span>|<span data-ttu-id="82fcc-458">指示在全面扫描期间是否扫描映射的网络驱动器。</span><span class="sxs-lookup"><span data-stu-id="82fcc-458">Indicates whether or not to scan mapped network drives during full scan.</span></span>|
|<span data-ttu-id="82fcc-459">defenderScanRemovableDrivesDuringFullScan</span><span class="sxs-lookup"><span data-stu-id="82fcc-459">defenderScanRemovableDrivesDuringFullScan</span></span>|<span data-ttu-id="82fcc-460">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-460">Boolean</span></span>|<span data-ttu-id="82fcc-461">指示在全面扫描期间是否扫描可移动驱动器。</span><span class="sxs-lookup"><span data-stu-id="82fcc-461">Indicates whether or not to scan removable drives during full scan.</span></span>|
|<span data-ttu-id="82fcc-462">defenderScanScriptsLoadedInInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="82fcc-462">defenderScanScriptsLoadedInInternetExplorer</span></span>|<span data-ttu-id="82fcc-463">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-463">Boolean</span></span>|<span data-ttu-id="82fcc-464">指示是否扫描在 Internet Explorer 浏览器中加载的脚本。</span><span class="sxs-lookup"><span data-stu-id="82fcc-464">Indicates whether or not to scan scripts loaded in Internet Explorer browser.</span></span>|
|<span data-ttu-id="82fcc-465">defenderSignatureUpdateIntervalInHours</span><span class="sxs-lookup"><span data-stu-id="82fcc-465">defenderSignatureUpdateIntervalInHours</span></span>|<span data-ttu-id="82fcc-466">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-466">Int32</span></span>|<span data-ttu-id="82fcc-467">签名更新间隔（以小时为单位）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-467">The signature update interval in hours.</span></span> <span data-ttu-id="82fcc-468">指定 0 不检查。</span><span class="sxs-lookup"><span data-stu-id="82fcc-468">Specify 0 not to check.</span></span> <span data-ttu-id="82fcc-469">有效值为 0 至 24</span><span class="sxs-lookup"><span data-stu-id="82fcc-469">Valid values 0 to 24</span></span>|
|<span data-ttu-id="82fcc-470">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="82fcc-470">defenderScanType</span></span>|[<span data-ttu-id="82fcc-471">defenderScanType</span><span class="sxs-lookup"><span data-stu-id="82fcc-471">defenderScanType</span></span>](../resources/intune-deviceconfig-defenderscantype.md)|<span data-ttu-id="82fcc-472">Defender 系统扫描类型。</span><span class="sxs-lookup"><span data-stu-id="82fcc-472">The defender system scan type.</span></span> <span data-ttu-id="82fcc-473">可取值为：`userDefined`、`disabled`、`quick`、`full`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-473">Possible values are: `userDefined`, `disabled`, `quick`, `full`.</span></span>|
|<span data-ttu-id="82fcc-474">defenderScheduledScanTime</span><span class="sxs-lookup"><span data-stu-id="82fcc-474">defenderScheduledScanTime</span></span>|<span data-ttu-id="82fcc-475">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="82fcc-475">TimeOfDay</span></span>|<span data-ttu-id="82fcc-476">系统扫描的 Defender 时间。</span><span class="sxs-lookup"><span data-stu-id="82fcc-476">The defender time for the system scan.</span></span>|
|<span data-ttu-id="82fcc-477">defenderScheduledQuickScanTime</span><span class="sxs-lookup"><span data-stu-id="82fcc-477">defenderScheduledQuickScanTime</span></span>|<span data-ttu-id="82fcc-478">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="82fcc-478">TimeOfDay</span></span>|<span data-ttu-id="82fcc-479">执行每日快速扫描的时间。</span><span class="sxs-lookup"><span data-stu-id="82fcc-479">The time to perform a daily quick scan.</span></span>|
|<span data-ttu-id="82fcc-480">defenderCloudBlockLevel</span><span class="sxs-lookup"><span data-stu-id="82fcc-480">defenderCloudBlockLevel</span></span>|[<span data-ttu-id="82fcc-481">defenderCloudBlockLevelType</span><span class="sxs-lookup"><span data-stu-id="82fcc-481">defenderCloudBlockLevelType</span></span>](../resources/intune-deviceconfig-defendercloudblockleveltype.md)|<span data-ttu-id="82fcc-482">指定云提供的保护级别。</span><span class="sxs-lookup"><span data-stu-id="82fcc-482">Specifies the level of cloud-delivered protection.</span></span> <span data-ttu-id="82fcc-483">可取值为：`notConfigured`、`high`、`highPlus`、`zeroTolerance`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-483">Possible values are: `notConfigured`, `high`, `highPlus`, `zeroTolerance`.</span></span>|
|<span data-ttu-id="82fcc-484">defenderCloudExtendedTimeout</span><span class="sxs-lookup"><span data-stu-id="82fcc-484">defenderCloudExtendedTimeout</span></span>|<span data-ttu-id="82fcc-485">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-485">Int32</span></span>|<span data-ttu-id="82fcc-486">超时的云扫描的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="82fcc-486">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="82fcc-487">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="82fcc-487">Valid values 0 to 50</span></span>|
|<span data-ttu-id="82fcc-488">defenderCloudExtendedTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="82fcc-488">defenderCloudExtendedTimeoutInSeconds</span></span>|<span data-ttu-id="82fcc-489">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-489">Int32</span></span>|<span data-ttu-id="82fcc-490">超时的云扫描的文件扩展名。</span><span class="sxs-lookup"><span data-stu-id="82fcc-490">Timeout extension for file scanning by the cloud.</span></span> <span data-ttu-id="82fcc-491">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="82fcc-491">Valid values 0 to 50</span></span>|
|<span data-ttu-id="82fcc-492">defenderBlockOnAccessProtection</span><span class="sxs-lookup"><span data-stu-id="82fcc-492">defenderBlockOnAccessProtection</span></span>|<span data-ttu-id="82fcc-493">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-493">Boolean</span></span>|<span data-ttu-id="82fcc-494">允许或禁止 Windows Defender 上访问保护功能。</span><span class="sxs-lookup"><span data-stu-id="82fcc-494">Allows or disallows Windows Defender On Access Protection functionality.</span></span>|
|<span data-ttu-id="82fcc-495">defenderScheduleScanDay</span><span class="sxs-lookup"><span data-stu-id="82fcc-495">defenderScheduleScanDay</span></span>|[<span data-ttu-id="82fcc-496">defenderScheduleScanDay</span><span class="sxs-lookup"><span data-stu-id="82fcc-496">defenderScheduleScanDay</span></span>](../resources/intune-deviceconfig-defenderschedulescanday.md)|<span data-ttu-id="82fcc-497">选择应在运行 Windows Defender 扫描的日期。</span><span class="sxs-lookup"><span data-stu-id="82fcc-497">Selects the day that the Windows Defender scan should run.</span></span> <span data-ttu-id="82fcc-498">可取值为：`everyday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`、`sunday`、`noScheduledScan`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-498">Possible values are: `everyday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, `sunday`, `noScheduledScan`.</span></span>|
|<span data-ttu-id="82fcc-499">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="82fcc-499">defenderSubmitSamplesConsentType</span></span>|[<span data-ttu-id="82fcc-500">defenderSubmitSamplesConsentType</span><span class="sxs-lookup"><span data-stu-id="82fcc-500">defenderSubmitSamplesConsentType</span></span>](../resources/intune-deviceconfig-defendersubmitsamplesconsenttype.md)|<span data-ttu-id="82fcc-501">检查用户同意中发送数据的 Windows Defender 级别。</span><span class="sxs-lookup"><span data-stu-id="82fcc-501">Checks for the user consent level in Windows Defender to send data.</span></span> <span data-ttu-id="82fcc-502">可取值为：`sendSafeSamplesAutomatically`、`alwaysPrompt`、`neverSend`、`sendAllSamplesAutomatically`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-502">Possible values are: `sendSafeSamplesAutomatically`, `alwaysPrompt`, `neverSend`, `sendAllSamplesAutomatically`.</span></span>|
|<span data-ttu-id="82fcc-503">lockScreenAllowTimeoutConfiguration</span><span class="sxs-lookup"><span data-stu-id="82fcc-503">lockScreenAllowTimeoutConfiguration</span></span>|<span data-ttu-id="82fcc-504">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-504">Boolean</span></span>|<span data-ttu-id="82fcc-505">指定是否在 Windows 10 移动版设备的锁定屏幕上显示用户可配置设置以控制屏幕超时。</span><span class="sxs-lookup"><span data-stu-id="82fcc-505">Specify whether to show a user-configurable setting to control the screen timeout while on the lock screen of Windows 10 Mobile devices.</span></span> <span data-ttu-id="82fcc-506">如果此策略设置为 Allow，则由 lockScreenTimeoutInSeconds 设置的值将被忽略。</span><span class="sxs-lookup"><span data-stu-id="82fcc-506">If this policy is set to Allow, the value set by lockScreenTimeoutInSeconds is ignored.</span></span>|
|<span data-ttu-id="82fcc-507">lockScreenBlockActionCenterNotifications</span><span class="sxs-lookup"><span data-stu-id="82fcc-507">lockScreenBlockActionCenterNotifications</span></span>|<span data-ttu-id="82fcc-508">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-508">Boolean</span></span>|<span data-ttu-id="82fcc-509">指示在锁定屏幕上是否阻止操作中心通知。</span><span class="sxs-lookup"><span data-stu-id="82fcc-509">Indicates whether or not to block action center notifications over lock screen.</span></span>|
|<span data-ttu-id="82fcc-510">lockScreenBlockCortana</span><span class="sxs-lookup"><span data-stu-id="82fcc-510">lockScreenBlockCortana</span></span>|<span data-ttu-id="82fcc-511">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-511">Boolean</span></span>|<span data-ttu-id="82fcc-512">指示系统锁定时用户是否可以使用语音与 Cortana 进行交互。</span><span class="sxs-lookup"><span data-stu-id="82fcc-512">Indicates whether or not the user can interact with Cortana using speech while the system is locked.</span></span>|
|<span data-ttu-id="82fcc-513">lockScreenBlockToastNotifications</span><span class="sxs-lookup"><span data-stu-id="82fcc-513">lockScreenBlockToastNotifications</span></span>|<span data-ttu-id="82fcc-514">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-514">Boolean</span></span>|<span data-ttu-id="82fcc-515">指示是否允许设备锁定屏幕上方的 Toast 通知。</span><span class="sxs-lookup"><span data-stu-id="82fcc-515">Indicates whether to allow toast notifications above the device lock screen.</span></span>|
|<span data-ttu-id="82fcc-516">lockScreenTimeoutInSeconds</span><span class="sxs-lookup"><span data-stu-id="82fcc-516">lockScreenTimeoutInSeconds</span></span>|<span data-ttu-id="82fcc-517">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-517">Int32</span></span>|<span data-ttu-id="82fcc-518">设置从 Windows 10 移动版设备的屏幕锁定到屏幕关闭的持续时间（以秒为单位）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-518">Set the duration (in seconds) from the screen locking to the screen turning off for Windows 10 Mobile devices.</span></span> <span data-ttu-id="82fcc-519">支持的值为 11-1800。</span><span class="sxs-lookup"><span data-stu-id="82fcc-519">Supported values are 11-1800.</span></span> <span data-ttu-id="82fcc-520">有效值为 11 至 1800</span><span class="sxs-lookup"><span data-stu-id="82fcc-520">Valid values 11 to 1800</span></span>|
|<span data-ttu-id="82fcc-521">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="82fcc-521">passwordBlockSimple</span></span>|<span data-ttu-id="82fcc-522">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-522">Boolean</span></span>|<span data-ttu-id="82fcc-523">指定是否允许 PIN 或密码，例如“1111”或“1234”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-523">Specify whether PINs or passwords such as "1111" or "1234" are allowed.</span></span> <span data-ttu-id="82fcc-524">对于 Windows 10 台式机，它也控制图片密码的使用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-524">For Windows 10 desktops, it also controls the use of picture passwords.</span></span>|
|<span data-ttu-id="82fcc-525">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="82fcc-525">passwordExpirationDays</span></span>|<span data-ttu-id="82fcc-526">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-526">Int32</span></span>|<span data-ttu-id="82fcc-527">密码过期天数。</span><span class="sxs-lookup"><span data-stu-id="82fcc-527">The password expiration in days.</span></span> <span data-ttu-id="82fcc-528">有效值为 0 至 730</span><span class="sxs-lookup"><span data-stu-id="82fcc-528">Valid values 0 to 730</span></span>|
|<span data-ttu-id="82fcc-529">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="82fcc-529">passwordMinimumLength</span></span>|<span data-ttu-id="82fcc-530">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-530">Int32</span></span>|<span data-ttu-id="82fcc-531">最短密码长度。</span><span class="sxs-lookup"><span data-stu-id="82fcc-531">The minimum password length.</span></span> <span data-ttu-id="82fcc-532">有效值为 4 至 16</span><span class="sxs-lookup"><span data-stu-id="82fcc-532">Valid values 4 to 16</span></span>|
|<span data-ttu-id="82fcc-533">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="82fcc-533">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="82fcc-534">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-534">Int32</span></span>|<span data-ttu-id="82fcc-535">屏幕超时之前的不活动分钟数。</span><span class="sxs-lookup"><span data-stu-id="82fcc-535">The minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="82fcc-536">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="82fcc-536">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="82fcc-537">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-537">Int32</span></span>|<span data-ttu-id="82fcc-538">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="82fcc-538">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="82fcc-539">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="82fcc-539">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="82fcc-540">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-540">Int32</span></span>|<span data-ttu-id="82fcc-541">防止重复使用的先前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="82fcc-541">The number of previous passwords to prevent reuse of.</span></span> <span data-ttu-id="82fcc-542">有效值为 0 至 50</span><span class="sxs-lookup"><span data-stu-id="82fcc-542">Valid values 0 to 50</span></span>|
|<span data-ttu-id="82fcc-543">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="82fcc-543">passwordRequired</span></span>|<span data-ttu-id="82fcc-544">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-544">Boolean</span></span>|<span data-ttu-id="82fcc-545">指示是否要求用户输入密码。</span><span class="sxs-lookup"><span data-stu-id="82fcc-545">Indicates whether or not to require the user to have a password.</span></span>|
|<span data-ttu-id="82fcc-546">passwordRequireWhenResumeFromIdleState</span><span class="sxs-lookup"><span data-stu-id="82fcc-546">passwordRequireWhenResumeFromIdleState</span></span>|<span data-ttu-id="82fcc-547">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-547">Boolean</span></span>|<span data-ttu-id="82fcc-548">指示从空闲状态恢复时是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="82fcc-548">Indicates whether or not to require a password upon resuming from an idle state.</span></span>|
|<span data-ttu-id="82fcc-549">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="82fcc-549">passwordRequiredType</span></span>|[<span data-ttu-id="82fcc-550">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="82fcc-550">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="82fcc-551">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="82fcc-551">The required password type.</span></span> <span data-ttu-id="82fcc-552">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-552">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="82fcc-553">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="82fcc-553">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="82fcc-554">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-554">Int32</span></span>|<span data-ttu-id="82fcc-555">恢复出厂设置之前登录失败的次数。</span><span class="sxs-lookup"><span data-stu-id="82fcc-555">The number of sign in failures before factory reset.</span></span> <span data-ttu-id="82fcc-556">有效值为 0 至 999</span><span class="sxs-lookup"><span data-stu-id="82fcc-556">Valid values 0 to 999</span></span>|
|<span data-ttu-id="82fcc-557">passwordMinimumAgeInDays</span><span class="sxs-lookup"><span data-stu-id="82fcc-557">passwordMinimumAgeInDays</span></span>|<span data-ttu-id="82fcc-558">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-558">Int32</span></span>|<span data-ttu-id="82fcc-559">此安全设置确定的时间 （以天为单位） 的密码必须使用之前的用户可以更改它。</span><span class="sxs-lookup"><span data-stu-id="82fcc-559">This security setting determines the period of time (in days) that a password must be used before the user can change it.</span></span> <span data-ttu-id="82fcc-560">有效的值 0 到 998</span><span class="sxs-lookup"><span data-stu-id="82fcc-560">Valid values 0 to 998</span></span>|
|<span data-ttu-id="82fcc-561">privacyAdvertisingId</span><span class="sxs-lookup"><span data-stu-id="82fcc-561">privacyAdvertisingId</span></span>|[<span data-ttu-id="82fcc-562">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-562">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="82fcc-563">启用或禁用广告 ID 的使用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-563">Enables or disables the use of advertising ID.</span></span> <span data-ttu-id="82fcc-564">已添加到 Windows 10 版本 1607 中。</span><span class="sxs-lookup"><span data-stu-id="82fcc-564">Added in Windows 10, version 1607.</span></span> <span data-ttu-id="82fcc-565">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-565">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="82fcc-566">privacyAutoAcceptPairingAndConsentPrompts</span><span class="sxs-lookup"><span data-stu-id="82fcc-566">privacyAutoAcceptPairingAndConsentPrompts</span></span>|<span data-ttu-id="82fcc-567">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-567">Boolean</span></span>|<span data-ttu-id="82fcc-568">指示在启动应用时是否允许自动接受配对和隐私用户许可对话框。</span><span class="sxs-lookup"><span data-stu-id="82fcc-568">Indicates whether or not to allow the automatic acceptance of the pairing and privacy user consent dialog when launching apps.</span></span>|
|<span data-ttu-id="82fcc-569">privacyBlockInputPersonalization</span><span class="sxs-lookup"><span data-stu-id="82fcc-569">privacyBlockInputPersonalization</span></span>|<span data-ttu-id="82fcc-570">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-570">Boolean</span></span>|<span data-ttu-id="82fcc-571">指示是否阻止 Cortana、Dictation 或 Store 应用程序使用基于云的语音服务。</span><span class="sxs-lookup"><span data-stu-id="82fcc-571">Indicates whether or not to block the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="82fcc-572">privacyBlockPublishUserActivities</span><span class="sxs-lookup"><span data-stu-id="82fcc-572">privacyBlockPublishUserActivities</span></span>|<span data-ttu-id="82fcc-573">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-573">Boolean</span></span>|<span data-ttu-id="82fcc-574">阻止共享的体验/发现最近使用过中的资源任务切换器等。</span><span class="sxs-lookup"><span data-stu-id="82fcc-574">Blocks the shared experiences/discovery of recently used resources in task switcher etc.</span></span>|
|<span data-ttu-id="82fcc-575">privacyBlockActivityFeed</span><span class="sxs-lookup"><span data-stu-id="82fcc-575">privacyBlockActivityFeed</span></span>|<span data-ttu-id="82fcc-576">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-576">Boolean</span></span>|<span data-ttu-id="82fcc-577">阻止对 Cortana、 口述或存储应用程序的基于云语音服务的使用情况。</span><span class="sxs-lookup"><span data-stu-id="82fcc-577">Blocks the usage of cloud based speech services for Cortana, Dictation, or Store applications.</span></span>|
|<span data-ttu-id="82fcc-578">startBlockUnpinningAppsFromTaskbar</span><span class="sxs-lookup"><span data-stu-id="82fcc-578">startBlockUnpinningAppsFromTaskbar</span></span>|<span data-ttu-id="82fcc-579">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-579">Boolean</span></span>|<span data-ttu-id="82fcc-580">指示是否阻止用户从任务栏取消固定应用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-580">Indicates whether or not to block the user from unpinning apps from taskbar.</span></span>|
|<span data-ttu-id="82fcc-581">startMenuAppListVisibility</span><span class="sxs-lookup"><span data-stu-id="82fcc-581">startMenuAppListVisibility</span></span>|[<span data-ttu-id="82fcc-582">windowsStartMenuAppListVisibilityType</span><span class="sxs-lookup"><span data-stu-id="82fcc-582">windowsStartMenuAppListVisibilityType</span></span>](../resources/intune-deviceconfig-windowsstartmenuapplistvisibilitytype.md)|<span data-ttu-id="82fcc-583">设置此值会折叠应用列表，完全删除应用列表，或者在“设置”应用中禁用相应的切换。</span><span class="sxs-lookup"><span data-stu-id="82fcc-583">Setting the value of this collapses the app list, removes the app list entirely, or disables the corresponding toggle in the Settings app.</span></span> <span data-ttu-id="82fcc-584">可取值为：`userDefined`、`collapse`、`remove`、`disableSettingsApp`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-584">Possible values are: `userDefined`, `collapse`, `remove`, `disableSettingsApp`.</span></span>|
|<span data-ttu-id="82fcc-585">startMenuHideChangeAccountSettings</span><span class="sxs-lookup"><span data-stu-id="82fcc-585">startMenuHideChangeAccountSettings</span></span>|<span data-ttu-id="82fcc-586">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-586">Boolean</span></span>|<span data-ttu-id="82fcc-587">启用此策略会将更改帐户设置从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-587">Enabling this policy hides the change account setting from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="82fcc-588">startMenuHideFrequentlyUsedApps</span><span class="sxs-lookup"><span data-stu-id="82fcc-588">startMenuHideFrequentlyUsedApps</span></span>|<span data-ttu-id="82fcc-589">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-589">Boolean</span></span>|<span data-ttu-id="82fcc-590">启用此策略会将最常用的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="82fcc-590">Enabling this policy hides the most used apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="82fcc-591">startMenuHideHibernate</span><span class="sxs-lookup"><span data-stu-id="82fcc-591">startMenuHideHibernate</span></span>|<span data-ttu-id="82fcc-592">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-592">Boolean</span></span>|<span data-ttu-id="82fcc-593">启用此策略会将休眠从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-593">Enabling this policy hides hibernate from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="82fcc-594">startMenuHideLock</span><span class="sxs-lookup"><span data-stu-id="82fcc-594">startMenuHideLock</span></span>|<span data-ttu-id="82fcc-595">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-595">Boolean</span></span>|<span data-ttu-id="82fcc-596">启用此策略会将锁定从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-596">Enabling this policy hides lock from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="82fcc-597">startMenuHidePowerButton</span><span class="sxs-lookup"><span data-stu-id="82fcc-597">startMenuHidePowerButton</span></span>|<span data-ttu-id="82fcc-598">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-598">Boolean</span></span>|<span data-ttu-id="82fcc-599">启用此策略会将电源按钮从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-599">Enabling this policy hides the power button from appearing in the start menu.</span></span>|
|<span data-ttu-id="82fcc-600">startMenuHideRecentJumpLists</span><span class="sxs-lookup"><span data-stu-id="82fcc-600">startMenuHideRecentJumpLists</span></span>|<span data-ttu-id="82fcc-601">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-601">Boolean</span></span>|<span data-ttu-id="82fcc-602">启用此策略会将最近的跳转列表从开始菜单/任务栏中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="82fcc-602">Enabling this policy hides recent jump lists from appearing on the start menu/taskbar and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="82fcc-603">startMenuHideRecentlyAddedApps</span><span class="sxs-lookup"><span data-stu-id="82fcc-603">startMenuHideRecentlyAddedApps</span></span>|<span data-ttu-id="82fcc-604">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-604">Boolean</span></span>|<span data-ttu-id="82fcc-605">启用此策略会将最近添加的应用从开始菜单中隐藏，并会禁用“设置”应用中的相应切换。</span><span class="sxs-lookup"><span data-stu-id="82fcc-605">Enabling this policy hides recently added apps from appearing on the start menu and disables the corresponding toggle in the Settings app.</span></span>|
|<span data-ttu-id="82fcc-606">startMenuHideRestartOptions</span><span class="sxs-lookup"><span data-stu-id="82fcc-606">startMenuHideRestartOptions</span></span>|<span data-ttu-id="82fcc-607">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-607">Boolean</span></span>|<span data-ttu-id="82fcc-608">启用此策略会将“重启/更新并重启”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-608">Enabling this policy hides “Restart/Update and Restart” from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="82fcc-609">startMenuHideShutDown</span><span class="sxs-lookup"><span data-stu-id="82fcc-609">startMenuHideShutDown</span></span>|<span data-ttu-id="82fcc-610">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-610">Boolean</span></span>|<span data-ttu-id="82fcc-611">启用此策略会将“关机/更新并关机”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-611">Enabling this policy hides shut down/update and shut down from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="82fcc-612">startMenuHideSignOut</span><span class="sxs-lookup"><span data-stu-id="82fcc-612">startMenuHideSignOut</span></span>|<span data-ttu-id="82fcc-613">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-613">Boolean</span></span>|<span data-ttu-id="82fcc-614">启用此策略会将“注销”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-614">Enabling this policy hides sign out from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="82fcc-615">startMenuHideSleep</span><span class="sxs-lookup"><span data-stu-id="82fcc-615">startMenuHideSleep</span></span>|<span data-ttu-id="82fcc-616">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-616">Boolean</span></span>|<span data-ttu-id="82fcc-617">启用此策略会将“休眠”从开始菜单的电源按钮中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-617">Enabling this policy hides sleep from appearing in the power button in the start menu.</span></span>|
|<span data-ttu-id="82fcc-618">startMenuHideSwitchAccount</span><span class="sxs-lookup"><span data-stu-id="82fcc-618">startMenuHideSwitchAccount</span></span>|<span data-ttu-id="82fcc-619">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-619">Boolean</span></span>|<span data-ttu-id="82fcc-620">启用此策略会将“切换帐户”从开始菜单的用户磁贴中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-620">Enabling this policy hides switch account from appearing in the user tile in the start menu.</span></span>|
|<span data-ttu-id="82fcc-621">startMenuHideUserTile</span><span class="sxs-lookup"><span data-stu-id="82fcc-621">startMenuHideUserTile</span></span>|<span data-ttu-id="82fcc-622">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-622">Boolean</span></span>|<span data-ttu-id="82fcc-623">启用此策略会将用户磁贴从开始菜单中隐藏。</span><span class="sxs-lookup"><span data-stu-id="82fcc-623">Enabling this policy hides the user tile from appearing in the start menu.</span></span>|
|<span data-ttu-id="82fcc-624">startMenuLayoutEdgeAssetsXml</span><span class="sxs-lookup"><span data-stu-id="82fcc-624">startMenuLayoutEdgeAssetsXml</span></span>|<span data-ttu-id="82fcc-625">Binary</span><span class="sxs-lookup"><span data-stu-id="82fcc-625">Binary</span></span>|<span data-ttu-id="82fcc-626">此策略设置使用户可以导入 Edge 资产以与 startMenuLayoutXml 策略一起使用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-626">This policy setting allows you to import Edge assets to be used with startMenuLayoutXml policy.</span></span> <span data-ttu-id="82fcc-627">开始布局可以包含查找 Edge 本地资产文件的 Edge 应用中的辅助磁贴。</span><span class="sxs-lookup"><span data-stu-id="82fcc-627">Start layout can contain secondary tile from Edge app which looks for Edge local asset file.</span></span> <span data-ttu-id="82fcc-628">在这种情况下，Edge 本地资产不存在并导致 Edge 辅助磁贴显示为空。</span><span class="sxs-lookup"><span data-stu-id="82fcc-628">Edge local asset would not exist and cause Edge secondary tile to appear empty in this case.</span></span> <span data-ttu-id="82fcc-629">仅当修改 startMenuLayoutXml 策略时才应用此策略。</span><span class="sxs-lookup"><span data-stu-id="82fcc-629">This policy only gets applied when startMenuLayoutXml policy is modified.</span></span> <span data-ttu-id="82fcc-630">该值应该是一个 UTF-8 Base64 编码的字节数组。</span><span class="sxs-lookup"><span data-stu-id="82fcc-630">The value should be a UTF-8 Base64 encoded byte array.</span></span>|
|<span data-ttu-id="82fcc-631">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="82fcc-631">startMenuLayoutXml</span></span>|<span data-ttu-id="82fcc-632">Binary</span><span class="sxs-lookup"><span data-stu-id="82fcc-632">Binary</span></span>|<span data-ttu-id="82fcc-633">允许管理员覆盖默认的“开始”菜单布局并阻止用户对其进行更改。</span><span class="sxs-lookup"><span data-stu-id="82fcc-633">Allows admins to override the default Start menu layout and prevents the user from changing it.</span></span> <span data-ttu-id="82fcc-634">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="82fcc-634">The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="82fcc-635">XML 需要采用 UTF8 编码的字节数组格式。</span><span class="sxs-lookup"><span data-stu-id="82fcc-635">XML needs to be in a UTF8 encoded byte array format.</span></span>|
|<span data-ttu-id="82fcc-636">startMenuMode</span><span class="sxs-lookup"><span data-stu-id="82fcc-636">startMenuMode</span></span>|[<span data-ttu-id="82fcc-637">windowsStartMenuModeType</span><span class="sxs-lookup"><span data-stu-id="82fcc-637">windowsStartMenuModeType</span></span>](../resources/intune-deviceconfig-windowsstartmenumodetype.md)|<span data-ttu-id="82fcc-638">允许管理员决定显示“开始”菜单的方式。</span><span class="sxs-lookup"><span data-stu-id="82fcc-638">Allows admins to decide how the Start menu is displayed.</span></span> <span data-ttu-id="82fcc-639">可取值为：`userDefined`、`fullScreen`、`nonFullScreen`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-639">Possible values are: `userDefined`, `fullScreen`, `nonFullScreen`.</span></span>|
|<span data-ttu-id="82fcc-640">startMenuPinnedFolderDocuments</span><span class="sxs-lookup"><span data-stu-id="82fcc-640">startMenuPinnedFolderDocuments</span></span>|[<span data-ttu-id="82fcc-641">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-641">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-642">强制“开始”菜单上的文档文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-642">Enforces the visibility (Show/Hide) of the Documents folder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-643">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-643">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-644">startMenuPinnedFolderDownloads</span><span class="sxs-lookup"><span data-stu-id="82fcc-644">startMenuPinnedFolderDownloads</span></span>|[<span data-ttu-id="82fcc-645">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-645">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-646">强制“开始”菜单上的下载文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-646">Enforces the visibility (Show/Hide) of the Downloads folder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-647">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-647">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-648">startMenuPinnedFolderFileExplorer</span><span class="sxs-lookup"><span data-stu-id="82fcc-648">startMenuPinnedFolderFileExplorer</span></span>|[<span data-ttu-id="82fcc-649">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-649">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-650">强制“开始”菜单上的 FileExplorer 快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-650">Enforces the visibility (Show/Hide) of the FileExplorer shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-651">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-651">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-652">startMenuPinnedFolderHomeGroup</span><span class="sxs-lookup"><span data-stu-id="82fcc-652">startMenuPinnedFolderHomeGroup</span></span>|[<span data-ttu-id="82fcc-653">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-653">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-654">强制“开始”菜单上的 HomeGroup 文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-654">Enforces the visibility (Show/Hide) of the HomeGroup folder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-655">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-655">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-656">startMenuPinnedFolderMusic</span><span class="sxs-lookup"><span data-stu-id="82fcc-656">startMenuPinnedFolderMusic</span></span>|[<span data-ttu-id="82fcc-657">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-657">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-658">强制“开始”菜单上的音乐文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-658">Enforces the visibility (Show/Hide) of the Music folder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-659">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-659">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-660">startMenuPinnedFolderNetwork</span><span class="sxs-lookup"><span data-stu-id="82fcc-660">startMenuPinnedFolderNetwork</span></span>|[<span data-ttu-id="82fcc-661">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-661">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-662">强制“开始”菜单上的网络文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-662">Enforces the visibility (Show/Hide) of the Network folder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-663">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-663">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-664">startMenuPinnedFolderPersonalFolder</span><span class="sxs-lookup"><span data-stu-id="82fcc-664">startMenuPinnedFolderPersonalFolder</span></span>|[<span data-ttu-id="82fcc-665">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-665">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-666">强制“开始”菜单上的个人文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-666">Enforces the visibility (Show/Hide) of the PersonalFolder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-667">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-667">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-668">startMenuPinnedFolderPictures</span><span class="sxs-lookup"><span data-stu-id="82fcc-668">startMenuPinnedFolderPictures</span></span>|[<span data-ttu-id="82fcc-669">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-669">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-670">强制“开始”菜单上的图片文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-670">Enforces the visibility (Show/Hide) of the Pictures folder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-671">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-671">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-672">startMenuPinnedFolderSettings</span><span class="sxs-lookup"><span data-stu-id="82fcc-672">startMenuPinnedFolderSettings</span></span>|[<span data-ttu-id="82fcc-673">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-673">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-674">强制“开始”菜单上的设置文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-674">Enforces the visibility (Show/Hide) of the Settings folder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-675">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-675">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-676">startMenuPinnedFolderVideos</span><span class="sxs-lookup"><span data-stu-id="82fcc-676">startMenuPinnedFolderVideos</span></span>|[<span data-ttu-id="82fcc-677">visibilitySetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-677">visibilitySetting</span></span>](../resources/intune-deviceconfig-visibilitysetting.md)|<span data-ttu-id="82fcc-678">强制“开始”菜单上的视频文件夹快捷方式的可见性（显示/隐藏）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-678">Enforces the visibility (Show/Hide) of the Videos folder shortcut on the Start menu.</span></span> <span data-ttu-id="82fcc-679">可取值为：`notConfigured`、`hide`、`show`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-679">Possible values are: `notConfigured`, `hide`, `show`.</span></span>|
|<span data-ttu-id="82fcc-680">settingsBlockSettingsApp</span><span class="sxs-lookup"><span data-stu-id="82fcc-680">settingsBlockSettingsApp</span></span>|<span data-ttu-id="82fcc-681">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-681">Boolean</span></span>|<span data-ttu-id="82fcc-682">指示是否阻止访问“设置”应用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-682">Indicates whether or not to block access to Settings app.</span></span>|
|<span data-ttu-id="82fcc-683">settingsBlockSystemPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-683">settingsBlockSystemPage</span></span>|<span data-ttu-id="82fcc-684">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-684">Boolean</span></span>|<span data-ttu-id="82fcc-685">指示是否阻止在“设置”应用中访问系统。</span><span class="sxs-lookup"><span data-stu-id="82fcc-685">Indicates whether or not to block access to System in Settings app.</span></span>|
|<span data-ttu-id="82fcc-686">settingsBlockDevicesPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-686">settingsBlockDevicesPage</span></span>|<span data-ttu-id="82fcc-687">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-687">Boolean</span></span>|<span data-ttu-id="82fcc-688">指示是否阻止在“设置”应用中访问设备。</span><span class="sxs-lookup"><span data-stu-id="82fcc-688">Indicates whether or not to block access to Devices in Settings app.</span></span>|
|<span data-ttu-id="82fcc-689">settingsBlockNetworkInternetPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-689">settingsBlockNetworkInternetPage</span></span>|<span data-ttu-id="82fcc-690">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-690">Boolean</span></span>|<span data-ttu-id="82fcc-691">指示是否阻止在“设置”应用中访问“网络和 Internet”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-691">Indicates whether or not to block access to Network & Internet in Settings app.</span></span>|
|<span data-ttu-id="82fcc-692">settingsBlockPersonalizationPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-692">settingsBlockPersonalizationPage</span></span>|<span data-ttu-id="82fcc-693">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-693">Boolean</span></span>|<span data-ttu-id="82fcc-694">指示是否阻止在“设置”应用中访问“个性化”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-694">Indicates whether or not to block access to Personalization in Settings app.</span></span>|
|<span data-ttu-id="82fcc-695">settingsBlockAccountsPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-695">settingsBlockAccountsPage</span></span>|<span data-ttu-id="82fcc-696">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-696">Boolean</span></span>|<span data-ttu-id="82fcc-697">指示是否阻止在“设置”应用中访问“帐户”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-697">Indicates whether or not to block access to Accounts in Settings app.</span></span>|
|<span data-ttu-id="82fcc-698">settingsBlockTimeLanguagePage</span><span class="sxs-lookup"><span data-stu-id="82fcc-698">settingsBlockTimeLanguagePage</span></span>|<span data-ttu-id="82fcc-699">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-699">Boolean</span></span>|<span data-ttu-id="82fcc-700">指示是否阻止在“设置”应用中访问“时间和语言”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-700">Indicates whether or not to block access to Time & Language in Settings app.</span></span>|
|<span data-ttu-id="82fcc-701">settingsBlockEaseOfAccessPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-701">settingsBlockEaseOfAccessPage</span></span>|<span data-ttu-id="82fcc-702">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-702">Boolean</span></span>|<span data-ttu-id="82fcc-703">指示是否阻止在“设置”应用中访问“辅助功能”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-703">Indicates whether or not to block access to Ease of Access in Settings app.</span></span>|
|<span data-ttu-id="82fcc-704">settingsBlockPrivacyPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-704">settingsBlockPrivacyPage</span></span>|<span data-ttu-id="82fcc-705">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-705">Boolean</span></span>|<span data-ttu-id="82fcc-706">指示是否阻止在“设置”应用中访问“隐私”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-706">Indicates whether or not to block access to Privacy in Settings app.</span></span>|
|<span data-ttu-id="82fcc-707">settingsBlockUpdateSecurityPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-707">settingsBlockUpdateSecurityPage</span></span>|<span data-ttu-id="82fcc-708">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-708">Boolean</span></span>|<span data-ttu-id="82fcc-709">指示是否阻止在“设置”应用中访问“更新和安全”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-709">Indicates whether or not to block access to Update & Security in Settings app.</span></span>|
|<span data-ttu-id="82fcc-710">settingsBlockAppsPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-710">settingsBlockAppsPage</span></span>|<span data-ttu-id="82fcc-711">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-711">Boolean</span></span>|<span data-ttu-id="82fcc-712">指示是否阻止在“设置”应用中访问“应用”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-712">Indicates whether or not to block access to Apps in Settings app.</span></span>|
|<span data-ttu-id="82fcc-713">settingsBlockGamingPage</span><span class="sxs-lookup"><span data-stu-id="82fcc-713">settingsBlockGamingPage</span></span>|<span data-ttu-id="82fcc-714">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-714">Boolean</span></span>|<span data-ttu-id="82fcc-715">指示是否阻止在“设置”应用中访问“游戏”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-715">Indicates whether or not to block access to Gaming in Settings app.</span></span>|
|<span data-ttu-id="82fcc-716">windowsSpotlightBlockConsumerSpecificFeatures</span><span class="sxs-lookup"><span data-stu-id="82fcc-716">windowsSpotlightBlockConsumerSpecificFeatures</span></span>|<span data-ttu-id="82fcc-717">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-717">Boolean</span></span>|<span data-ttu-id="82fcc-718">允许 IT 管理员阻止通常仅供消费者使用的体验，例如开始建议、会员通知、Post-OOBE 应用安装和重定向磁贴。</span><span class="sxs-lookup"><span data-stu-id="82fcc-718">Allows IT admins to block experiences that are typically for consumers only, such as Start suggestions, Membership notifications, Post-OOBE app install and redirect tiles.</span></span>|
|<span data-ttu-id="82fcc-719">windowsSpotlightBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-719">windowsSpotlightBlocked</span></span>|<span data-ttu-id="82fcc-720">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-720">Boolean</span></span>|<span data-ttu-id="82fcc-721">允许 IT 管理员关闭所有 Windows 聚焦功能</span><span class="sxs-lookup"><span data-stu-id="82fcc-721">Allows IT admins to turn off all Windows Spotlight features</span></span>|
|<span data-ttu-id="82fcc-722">windowsSpotlightBlockOnActionCenter</span><span class="sxs-lookup"><span data-stu-id="82fcc-722">windowsSpotlightBlockOnActionCenter</span></span>|<span data-ttu-id="82fcc-723">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-723">Boolean</span></span>|<span data-ttu-id="82fcc-724">阻止 Microsoft 在每次操作系统全新安装、升级或持续推出后显示的建议，以向用户介绍新增功能或更改功能</span><span class="sxs-lookup"><span data-stu-id="82fcc-724">Block suggestions from Microsoft that show after each OS clean install, upgrade or in an on-going basis to introduce users to what is new or changed</span></span>|
|<span data-ttu-id="82fcc-725">windowsSpotlightBlockTailoredExperiences</span><span class="sxs-lookup"><span data-stu-id="82fcc-725">windowsSpotlightBlockTailoredExperiences</span></span>|<span data-ttu-id="82fcc-726">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-726">Boolean</span></span>|<span data-ttu-id="82fcc-727">基于用户的设备使用情况，在 Windows 聚焦中阻止个性化内容。</span><span class="sxs-lookup"><span data-stu-id="82fcc-727">Block personalized content in Windows spotlight based on user’s device usage.</span></span>|
|<span data-ttu-id="82fcc-728">windowsSpotlightBlockThirdPartyNotifications</span><span class="sxs-lookup"><span data-stu-id="82fcc-728">windowsSpotlightBlockThirdPartyNotifications</span></span>|<span data-ttu-id="82fcc-729">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-729">Boolean</span></span>|<span data-ttu-id="82fcc-730">阻止通过 Windows 聚焦投放的第三方内容</span><span class="sxs-lookup"><span data-stu-id="82fcc-730">Block third party content delivered via Windows Spotlight</span></span>|
|<span data-ttu-id="82fcc-731">windowsSpotlightBlockWelcomeExperience</span><span class="sxs-lookup"><span data-stu-id="82fcc-731">windowsSpotlightBlockWelcomeExperience</span></span>|<span data-ttu-id="82fcc-732">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-732">Boolean</span></span>|<span data-ttu-id="82fcc-733">阻止 Windows 聚焦 Windows 欢迎体验</span><span class="sxs-lookup"><span data-stu-id="82fcc-733">Block Windows Spotlight Windows welcome experience</span></span>|
|<span data-ttu-id="82fcc-734">windowsSpotlightBlockWindowsTips</span><span class="sxs-lookup"><span data-stu-id="82fcc-734">windowsSpotlightBlockWindowsTips</span></span>|<span data-ttu-id="82fcc-735">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-735">Boolean</span></span>|<span data-ttu-id="82fcc-736">允许 IT 管理员关闭 Windows 提示的弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="82fcc-736">Allows IT admins to turn off the popup of Windows Tips.</span></span>|
|<span data-ttu-id="82fcc-737">windowsSpotlightConfigureOnLockScreen</span><span class="sxs-lookup"><span data-stu-id="82fcc-737">windowsSpotlightConfigureOnLockScreen</span></span>|[<span data-ttu-id="82fcc-738">windowsSpotlightEnablementSettings</span><span class="sxs-lookup"><span data-stu-id="82fcc-738">windowsSpotlightEnablementSettings</span></span>](../resources/intune-deviceconfig-windowsspotlightenablementsettings.md)|<span data-ttu-id="82fcc-739">指定聚焦的类型。</span><span class="sxs-lookup"><span data-stu-id="82fcc-739">Specifies the type of Spotlight.</span></span> <span data-ttu-id="82fcc-740">可取值为：`notConfigured`、`disabled`、`enabled`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-740">Possible values are: `notConfigured`, `disabled`, `enabled`.</span></span>|
|<span data-ttu-id="82fcc-741">networkProxyApplySettingsDeviceWide</span><span class="sxs-lookup"><span data-stu-id="82fcc-741">networkProxyApplySettingsDeviceWide</span></span>|<span data-ttu-id="82fcc-742">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-742">Boolean</span></span>|<span data-ttu-id="82fcc-743">如果设置，代理设置将应用于设备中的所有进程和帐户。</span><span class="sxs-lookup"><span data-stu-id="82fcc-743">If set, proxy settings will be applied to all processes and accounts in the device.</span></span> <span data-ttu-id="82fcc-744">否则，它将应用于注册到 MDM 中的用户帐户。</span><span class="sxs-lookup"><span data-stu-id="82fcc-744">Otherwise, it will be applied to the user account that’s enrolled into MDM.</span></span>|
|<span data-ttu-id="82fcc-745">networkProxyDisableAutoDetect</span><span class="sxs-lookup"><span data-stu-id="82fcc-745">networkProxyDisableAutoDetect</span></span>|<span data-ttu-id="82fcc-746">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-746">Boolean</span></span>|<span data-ttu-id="82fcc-747">禁用自动检测设置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-747">Disable automatic detection of settings.</span></span> <span data-ttu-id="82fcc-748">如果启用，系统将尝试查找代理自动配置 (PAC) 脚本的路径。</span><span class="sxs-lookup"><span data-stu-id="82fcc-748">If enabled, the system will try to find the path to a proxy auto-config (PAC) script.</span></span>|
|<span data-ttu-id="82fcc-749">networkProxyAutomaticConfigurationUrl</span><span class="sxs-lookup"><span data-stu-id="82fcc-749">networkProxyAutomaticConfigurationUrl</span></span>|<span data-ttu-id="82fcc-750">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-750">String</span></span>|<span data-ttu-id="82fcc-751">指向你要使用的代理自动配置 (PAC) 脚本的地址。</span><span class="sxs-lookup"><span data-stu-id="82fcc-751">Address to the proxy auto-config (PAC) script you want to use.</span></span>|
|<span data-ttu-id="82fcc-752">networkProxyServer</span><span class="sxs-lookup"><span data-stu-id="82fcc-752">networkProxyServer</span></span>|[<span data-ttu-id="82fcc-753">windows10NetworkProxyServer</span><span class="sxs-lookup"><span data-stu-id="82fcc-753">windows10NetworkProxyServer</span></span>](../resources/intune-deviceconfig-windows10networkproxyserver.md)|<span data-ttu-id="82fcc-754">指定手动代理服务器设置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-754">Specifies manual proxy server settings.</span></span>|
|<span data-ttu-id="82fcc-755">accountsBlockAddingNonMicrosoftAccountEmail</span><span class="sxs-lookup"><span data-stu-id="82fcc-755">accountsBlockAddingNonMicrosoftAccountEmail</span></span>|<span data-ttu-id="82fcc-756">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-756">Boolean</span></span>|<span data-ttu-id="82fcc-757">指示是否阻止用户将电子邮件帐户添加到未与 Microsoft 帐户关联的设备。</span><span class="sxs-lookup"><span data-stu-id="82fcc-757">Indicates whether or not to Block the user from adding email accounts to the device that are not associated with a Microsoft account.</span></span>|
|<span data-ttu-id="82fcc-758">antiTheftModeBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-758">antiTheftModeBlocked</span></span>|<span data-ttu-id="82fcc-759">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-759">Boolean</span></span>|<span data-ttu-id="82fcc-760">指示是否阻止用户选择 AntiTheft 模式首选项（仅限 Windows 10 移动版）。</span><span class="sxs-lookup"><span data-stu-id="82fcc-760">Indicates whether or not to block the user from selecting an AntiTheft mode preference (Windows 10 Mobile only).</span></span>|
|<span data-ttu-id="82fcc-761">bluetoothBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-761">bluetoothBlocked</span></span>|<span data-ttu-id="82fcc-762">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-762">Boolean</span></span>|<span data-ttu-id="82fcc-763">是否阻止用户使用蓝牙。</span><span class="sxs-lookup"><span data-stu-id="82fcc-763">Whether or not to Block the user from using bluetooth.</span></span>|
|<span data-ttu-id="82fcc-764">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-764">cameraBlocked</span></span>|<span data-ttu-id="82fcc-765">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-765">Boolean</span></span>|<span data-ttu-id="82fcc-766">是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="82fcc-766">Whether or not to Block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="82fcc-767">connectedDevicesServiceBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-767">connectedDevicesServiceBlocked</span></span>|<span data-ttu-id="82fcc-768">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-768">Boolean</span></span>|<span data-ttu-id="82fcc-769">是否阻止能够发现并连接到其他设备、远程消息、远程应用会话和其他跨设备体验的连接设备服务。</span><span class="sxs-lookup"><span data-stu-id="82fcc-769">Whether or not to block Connected Devices Service which enables discovery and connection to other devices, remote messaging, remote app sessions and other cross-device experiences.</span></span>|
|<span data-ttu-id="82fcc-770">certificatesBlockManualRootCertificateInstallation</span><span class="sxs-lookup"><span data-stu-id="82fcc-770">certificatesBlockManualRootCertificateInstallation</span></span>|<span data-ttu-id="82fcc-771">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-771">Boolean</span></span>|<span data-ttu-id="82fcc-772">是否阻止用户执行手动根证书安装。</span><span class="sxs-lookup"><span data-stu-id="82fcc-772">Whether or not to Block the user from doing manual root certificate installation.</span></span>|
|<span data-ttu-id="82fcc-773">copyPasteBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-773">copyPasteBlocked</span></span>|<span data-ttu-id="82fcc-774">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-774">Boolean</span></span>|<span data-ttu-id="82fcc-775">是否阻止用户使用复制粘贴。</span><span class="sxs-lookup"><span data-stu-id="82fcc-775">Whether or not to Block the user from using copy paste.</span></span>|
|<span data-ttu-id="82fcc-776">cortanaBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-776">cortanaBlocked</span></span>|<span data-ttu-id="82fcc-777">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-777">Boolean</span></span>|<span data-ttu-id="82fcc-778">是否阻止用户使用 Cortana。</span><span class="sxs-lookup"><span data-stu-id="82fcc-778">Whether or not to Block the user from using Cortana.</span></span>|
|<span data-ttu-id="82fcc-779">deviceManagementBlockFactoryResetOnMobile</span><span class="sxs-lookup"><span data-stu-id="82fcc-779">deviceManagementBlockFactoryResetOnMobile</span></span>|<span data-ttu-id="82fcc-780">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-780">Boolean</span></span>|<span data-ttu-id="82fcc-781">指示是否阻止用户重置手机。</span><span class="sxs-lookup"><span data-stu-id="82fcc-781">Indicates whether or not to Block the user from resetting their phone.</span></span>|
|<span data-ttu-id="82fcc-782">deviceManagementBlockManualUnenroll</span><span class="sxs-lookup"><span data-stu-id="82fcc-782">deviceManagementBlockManualUnenroll</span></span>|<span data-ttu-id="82fcc-783">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-783">Boolean</span></span>|<span data-ttu-id="82fcc-784">指示是否阻止用户从设备管理手动取消注册。</span><span class="sxs-lookup"><span data-stu-id="82fcc-784">Indicates whether or not to Block the user from doing manual un-enrollment from device management.</span></span>|
|<span data-ttu-id="82fcc-785">safeSearchFilter</span><span class="sxs-lookup"><span data-stu-id="82fcc-785">safeSearchFilter</span></span>|[<span data-ttu-id="82fcc-786">safeSearchFilterType</span><span class="sxs-lookup"><span data-stu-id="82fcc-786">safeSearchFilterType</span></span>](../resources/intune-deviceconfig-safesearchfiltertype.md)|<span data-ttu-id="82fcc-787">指定需要的安全搜索筛选级别。</span><span class="sxs-lookup"><span data-stu-id="82fcc-787">Specifies what filter level of safe search is required.</span></span> <span data-ttu-id="82fcc-788">可取值为：`userDefined`、`strict`、`moderate`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-788">Possible values are: `userDefined`, `strict`, `moderate`.</span></span>|
|<span data-ttu-id="82fcc-789">edgeBlockPopups</span><span class="sxs-lookup"><span data-stu-id="82fcc-789">edgeBlockPopups</span></span>|<span data-ttu-id="82fcc-790">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-790">Boolean</span></span>|<span data-ttu-id="82fcc-791">指示是否阻止弹出窗口。</span><span class="sxs-lookup"><span data-stu-id="82fcc-791">Indicates whether or not to block popups.</span></span>|
|<span data-ttu-id="82fcc-792">edgeBlockSearchSuggestions</span><span class="sxs-lookup"><span data-stu-id="82fcc-792">edgeBlockSearchSuggestions</span></span>|<span data-ttu-id="82fcc-793">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-793">Boolean</span></span>|<span data-ttu-id="82fcc-794">指示是否阻止用户使用地址栏中的搜索建议。</span><span class="sxs-lookup"><span data-stu-id="82fcc-794">Indicates whether or not to Block the user from using the search suggestions in the address bar.</span></span>|
|<span data-ttu-id="82fcc-795">edgeBlockSendingIntranetTrafficToInternetExplorer</span><span class="sxs-lookup"><span data-stu-id="82fcc-795">edgeBlockSendingIntranetTrafficToInternetExplorer</span></span>|<span data-ttu-id="82fcc-796">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-796">Boolean</span></span>|<span data-ttu-id="82fcc-797">指示是否阻止用户将 Intranet 流量从 Edge 发送到 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="82fcc-797">Indicates whether or not to Block the user from sending Intranet traffic to Internet Explorer from Edge.</span></span>|
|<span data-ttu-id="82fcc-798">edgeRequireSmartScreen</span><span class="sxs-lookup"><span data-stu-id="82fcc-798">edgeRequireSmartScreen</span></span>|<span data-ttu-id="82fcc-799">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-799">Boolean</span></span>|<span data-ttu-id="82fcc-800">指示是否要求用户使用智能屏蔽筛选器。</span><span class="sxs-lookup"><span data-stu-id="82fcc-800">Indicates whether or not to Require the user to use the smart screen filter.</span></span>|
|<span data-ttu-id="82fcc-801">edgeEnterpriseModeSiteListLocation</span><span class="sxs-lookup"><span data-stu-id="82fcc-801">edgeEnterpriseModeSiteListLocation</span></span>|<span data-ttu-id="82fcc-802">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-802">String</span></span>|<span data-ttu-id="82fcc-803">指示企业模式站点列表位置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-803">Indicates the enterprise mode site list location.</span></span> <span data-ttu-id="82fcc-804">可能是本地文件、本地网络或 http 位置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-804">Could be a local file, local network or http location.</span></span>|
|<span data-ttu-id="82fcc-805">edgeFirstRunUrl</span><span class="sxs-lookup"><span data-stu-id="82fcc-805">edgeFirstRunUrl</span></span>|<span data-ttu-id="82fcc-806">String</span><span class="sxs-lookup"><span data-stu-id="82fcc-806">String</span></span>|<span data-ttu-id="82fcc-807">第一次打开 Edge 浏览器时的首个运行 URL。</span><span class="sxs-lookup"><span data-stu-id="82fcc-807">The first run URL for when Edge browser is opened for the first time.</span></span>|
|<span data-ttu-id="82fcc-808">edgeSearchEngine</span><span class="sxs-lookup"><span data-stu-id="82fcc-808">edgeSearchEngine</span></span>|[<span data-ttu-id="82fcc-809">edgeSearchEngineBase</span><span class="sxs-lookup"><span data-stu-id="82fcc-809">edgeSearchEngineBase</span></span>](../resources/intune-deviceconfig-edgesearchenginebase.md)|<span data-ttu-id="82fcc-810">允许 IT 管理员为 MDM 控制的设备设置默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="82fcc-810">Allows IT admins to set a default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="82fcc-811">如果未设置 AllowSearchEngineCustomization 策略，则用户可以替代此设置并更改其默认搜索引擎。</span><span class="sxs-lookup"><span data-stu-id="82fcc-811">Users can override this and change their default search engine provided the AllowSearchEngineCustomization policy is not set.</span></span>|
|<span data-ttu-id="82fcc-812">edgeHomepageUrls</span><span class="sxs-lookup"><span data-stu-id="82fcc-812">edgeHomepageUrls</span></span>|<span data-ttu-id="82fcc-813">String 集合</span><span class="sxs-lookup"><span data-stu-id="82fcc-813">String collection</span></span>|<span data-ttu-id="82fcc-814">Edge 浏览器上 MDM 注册设备上的主页 URL 列表。</span><span class="sxs-lookup"><span data-stu-id="82fcc-814">The list of URLs for homepages shodwn on MDM-enrolled devices on Edge browser.</span></span>|
|<span data-ttu-id="82fcc-815">edgeBlockAccessToAboutFlags</span><span class="sxs-lookup"><span data-stu-id="82fcc-815">edgeBlockAccessToAboutFlags</span></span>|<span data-ttu-id="82fcc-816">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-816">Boolean</span></span>|<span data-ttu-id="82fcc-817">指示是否阻止访问 Edge 浏览器上关于标志的信息。</span><span class="sxs-lookup"><span data-stu-id="82fcc-817">Indicates whether or not to prevent access to about flags on Edge browser.</span></span>|
|<span data-ttu-id="82fcc-818">smartScreenBlockPromptOverride</span><span class="sxs-lookup"><span data-stu-id="82fcc-818">smartScreenBlockPromptOverride</span></span>|<span data-ttu-id="82fcc-819">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-819">Boolean</span></span>|<span data-ttu-id="82fcc-820">指示用户是否可以覆盖有关潜在恶意网站的 SmartScreen 筛选器警告。</span><span class="sxs-lookup"><span data-stu-id="82fcc-820">Indicates whether or not users can override SmartScreen Filter warnings about potentially malicious websites.</span></span>|
|<span data-ttu-id="82fcc-821">smartScreenBlockPromptOverrideForFiles</span><span class="sxs-lookup"><span data-stu-id="82fcc-821">smartScreenBlockPromptOverrideForFiles</span></span>|<span data-ttu-id="82fcc-822">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-822">Boolean</span></span>|<span data-ttu-id="82fcc-823">指示用户是否可以覆盖关于下载未验证文件的 SmartScreen 筛选器警告</span><span class="sxs-lookup"><span data-stu-id="82fcc-823">Indicates whether or not users can override the SmartScreen Filter warnings about downloading unverified files</span></span>|
|<span data-ttu-id="82fcc-824">webRtcBlockLocalhostIpAddress</span><span class="sxs-lookup"><span data-stu-id="82fcc-824">webRtcBlockLocalhostIpAddress</span></span>|<span data-ttu-id="82fcc-825">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-825">Boolean</span></span>|<span data-ttu-id="82fcc-826">指示在使用 WebRTC 拨打电话时是否显示用户的本地主机 IP 地址</span><span class="sxs-lookup"><span data-stu-id="82fcc-826">Indicates whether or not user's localhost IP address is displayed while making phone calls using the WebRTC</span></span>|
|<span data-ttu-id="82fcc-827">internetSharingBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-827">internetSharingBlocked</span></span>|<span data-ttu-id="82fcc-828">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-828">Boolean</span></span>|<span data-ttu-id="82fcc-829">指示是否阻止用户使用 Internet 共享。</span><span class="sxs-lookup"><span data-stu-id="82fcc-829">Indicates whether or not to Block the user from using internet sharing.</span></span>|
|<span data-ttu-id="82fcc-830">settingsBlockAddProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="82fcc-830">settingsBlockAddProvisioningPackage</span></span>|<span data-ttu-id="82fcc-831">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-831">Boolean</span></span>|<span data-ttu-id="82fcc-832">指示是否阻止用户安装预配程序包。</span><span class="sxs-lookup"><span data-stu-id="82fcc-832">Indicates whether or not to block the user from installing provisioning packages.</span></span>|
|<span data-ttu-id="82fcc-833">settingsBlockRemoveProvisioningPackage</span><span class="sxs-lookup"><span data-stu-id="82fcc-833">settingsBlockRemoveProvisioningPackage</span></span>|<span data-ttu-id="82fcc-834">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-834">Boolean</span></span>|<span data-ttu-id="82fcc-835">指示是否阻止运行时配置代理删除预配程序包。</span><span class="sxs-lookup"><span data-stu-id="82fcc-835">Indicates whether or not to block the runtime configuration agent from removing provisioning packages.</span></span>|
|<span data-ttu-id="82fcc-836">settingsBlockChangeSystemTime</span><span class="sxs-lookup"><span data-stu-id="82fcc-836">settingsBlockChangeSystemTime</span></span>|<span data-ttu-id="82fcc-837">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-837">Boolean</span></span>|<span data-ttu-id="82fcc-838">指示是否阻止用户更改日期和时间设置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-838">Indicates whether or not to block the user from changing date and time settings.</span></span>|
|<span data-ttu-id="82fcc-839">settingsBlockEditDeviceName</span><span class="sxs-lookup"><span data-stu-id="82fcc-839">settingsBlockEditDeviceName</span></span>|<span data-ttu-id="82fcc-840">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-840">Boolean</span></span>|<span data-ttu-id="82fcc-841">指示是否阻止用户编辑设备名称。</span><span class="sxs-lookup"><span data-stu-id="82fcc-841">Indicates whether or not to block the user from editing the device name.</span></span>|
|<span data-ttu-id="82fcc-842">settingsBlockChangeRegion</span><span class="sxs-lookup"><span data-stu-id="82fcc-842">settingsBlockChangeRegion</span></span>|<span data-ttu-id="82fcc-843">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-843">Boolean</span></span>|<span data-ttu-id="82fcc-844">指示是否阻止用户更改区域设置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-844">Indicates whether or not to block the user from changing the region settings.</span></span>|
|<span data-ttu-id="82fcc-845">settingsBlockChangeLanguage</span><span class="sxs-lookup"><span data-stu-id="82fcc-845">settingsBlockChangeLanguage</span></span>|<span data-ttu-id="82fcc-846">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-846">Boolean</span></span>|<span data-ttu-id="82fcc-847">指示是否阻止用户更改语言设置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-847">Indicates whether or not to block the user from changing the language settings.</span></span>|
|<span data-ttu-id="82fcc-848">settingsBlockChangePowerSleep</span><span class="sxs-lookup"><span data-stu-id="82fcc-848">settingsBlockChangePowerSleep</span></span>|<span data-ttu-id="82fcc-849">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-849">Boolean</span></span>|<span data-ttu-id="82fcc-850">指示是否阻止用户更改电源和睡眠设置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-850">Indicates whether or not to block the user from changing power and sleep settings.</span></span>|
|<span data-ttu-id="82fcc-851">locationServicesBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-851">locationServicesBlocked</span></span>|<span data-ttu-id="82fcc-852">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-852">Boolean</span></span>|<span data-ttu-id="82fcc-853">指示是否阻止用户使用位置服务。</span><span class="sxs-lookup"><span data-stu-id="82fcc-853">Indicates whether or not to Block the user from location services.</span></span>|
|<span data-ttu-id="82fcc-854">microsoftAccountBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-854">microsoftAccountBlocked</span></span>|<span data-ttu-id="82fcc-855">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-855">Boolean</span></span>|<span data-ttu-id="82fcc-856">指示是否阻止 Microsoft 帐户。</span><span class="sxs-lookup"><span data-stu-id="82fcc-856">Indicates whether or not to Block a Microsoft account.</span></span>|
|<span data-ttu-id="82fcc-857">microsoftAccountBlockSettingsSync</span><span class="sxs-lookup"><span data-stu-id="82fcc-857">microsoftAccountBlockSettingsSync</span></span>|<span data-ttu-id="82fcc-858">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-858">Boolean</span></span>|<span data-ttu-id="82fcc-859">指示是否阻止 Microsoft 帐户设置同步。</span><span class="sxs-lookup"><span data-stu-id="82fcc-859">Indicates whether or not to Block Microsoft account settings sync.</span></span>|
|<span data-ttu-id="82fcc-860">nfcBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-860">nfcBlocked</span></span>|<span data-ttu-id="82fcc-861">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-861">Boolean</span></span>|<span data-ttu-id="82fcc-862">指示是否阻止用户使用近场通信。</span><span class="sxs-lookup"><span data-stu-id="82fcc-862">Indicates whether or not to Block the user from using near field communication.</span></span>|
|<span data-ttu-id="82fcc-863">resetProtectionModeBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-863">resetProtectionModeBlocked</span></span>|<span data-ttu-id="82fcc-864">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-864">Boolean</span></span>|<span data-ttu-id="82fcc-865">指示是否阻止用户进入重置保护模式。</span><span class="sxs-lookup"><span data-stu-id="82fcc-865">Indicates whether or not to Block the user from reset protection mode.</span></span>|
|<span data-ttu-id="82fcc-866">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-866">screenCaptureBlocked</span></span>|<span data-ttu-id="82fcc-867">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-867">Boolean</span></span>|<span data-ttu-id="82fcc-868">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="82fcc-868">Indicates whether or not to Block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="82fcc-869">storageBlockRemovableStorage</span><span class="sxs-lookup"><span data-stu-id="82fcc-869">storageBlockRemovableStorage</span></span>|<span data-ttu-id="82fcc-870">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-870">Boolean</span></span>|<span data-ttu-id="82fcc-871">指示是否阻止用户使用可移动存储。</span><span class="sxs-lookup"><span data-stu-id="82fcc-871">Indicates whether or not to Block the user from using removable storage.</span></span>|
|<span data-ttu-id="82fcc-872">storageRequireMobileDeviceEncryption</span><span class="sxs-lookup"><span data-stu-id="82fcc-872">storageRequireMobileDeviceEncryption</span></span>|<span data-ttu-id="82fcc-873">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-873">Boolean</span></span>|<span data-ttu-id="82fcc-874">指示是否需要在移动设备上进行加密。</span><span class="sxs-lookup"><span data-stu-id="82fcc-874">Indicating whether or not to require encryption on a mobile device.</span></span>|
|<span data-ttu-id="82fcc-875">usbBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-875">usbBlocked</span></span>|<span data-ttu-id="82fcc-876">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-876">Boolean</span></span>|<span data-ttu-id="82fcc-877">指示是否阻止用户使用 USB 连接。</span><span class="sxs-lookup"><span data-stu-id="82fcc-877">Indicates whether or not to Block the user from USB connection.</span></span>|
|<span data-ttu-id="82fcc-878">voiceRecordingBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-878">voiceRecordingBlocked</span></span>|<span data-ttu-id="82fcc-879">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-879">Boolean</span></span>|<span data-ttu-id="82fcc-880">指示是否阻止用户进行语音录制。</span><span class="sxs-lookup"><span data-stu-id="82fcc-880">Indicates whether or not to Block the user from voice recording.</span></span>|
|<span data-ttu-id="82fcc-881">wiFiBlockAutomaticConnectHotspots</span><span class="sxs-lookup"><span data-stu-id="82fcc-881">wiFiBlockAutomaticConnectHotspots</span></span>|<span data-ttu-id="82fcc-882">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-882">Boolean</span></span>|<span data-ttu-id="82fcc-883">指示是否阻止自动连接到 Wi-Fi 热点。</span><span class="sxs-lookup"><span data-stu-id="82fcc-883">Indicating whether or not to block automatically connecting to Wi-Fi hotspots.</span></span> <span data-ttu-id="82fcc-884">如果 Wi-Fi 被阻止，没有任何影响。</span><span class="sxs-lookup"><span data-stu-id="82fcc-884">Has no impact if Wi-Fi is blocked.</span></span>|
|<span data-ttu-id="82fcc-885">wiFiBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-885">wiFiBlocked</span></span>|<span data-ttu-id="82fcc-886">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-886">Boolean</span></span>|<span data-ttu-id="82fcc-887">指示是否阻止用户使用 Wi-Fi。</span><span class="sxs-lookup"><span data-stu-id="82fcc-887">Indicates whether or not to Block the user from using Wi-Fi.</span></span>|
|<span data-ttu-id="82fcc-888">wiFiBlockManualConfiguration</span><span class="sxs-lookup"><span data-stu-id="82fcc-888">wiFiBlockManualConfiguration</span></span>|<span data-ttu-id="82fcc-889">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-889">Boolean</span></span>|<span data-ttu-id="82fcc-890">指示是否阻止用户使用 Wi-Fi 手动配置。</span><span class="sxs-lookup"><span data-stu-id="82fcc-890">Indicates whether or not to Block the user from using Wi-Fi manual configuration.</span></span>|
|<span data-ttu-id="82fcc-891">wiFiScanInterval</span><span class="sxs-lookup"><span data-stu-id="82fcc-891">wiFiScanInterval</span></span>|<span data-ttu-id="82fcc-892">Int32</span><span class="sxs-lookup"><span data-stu-id="82fcc-892">Int32</span></span>|<span data-ttu-id="82fcc-893">指定设备扫描 Wi-Fi 网络的频率。</span><span class="sxs-lookup"><span data-stu-id="82fcc-893">Specify how often devices scan for Wi-Fi networks.</span></span> <span data-ttu-id="82fcc-894">支持的值是 1-500，其中 100 为默认值，500 为低频率。</span><span class="sxs-lookup"><span data-stu-id="82fcc-894">Supported values are 1-500, where 100 = default, and 500 = low frequency.</span></span> <span data-ttu-id="82fcc-895">有效值为 1 至 500</span><span class="sxs-lookup"><span data-stu-id="82fcc-895">Valid values 1 to 500</span></span>|
|<span data-ttu-id="82fcc-896">wirelessDisplayBlockProjectionToThisDevice</span><span class="sxs-lookup"><span data-stu-id="82fcc-896">wirelessDisplayBlockProjectionToThisDevice</span></span>|<span data-ttu-id="82fcc-897">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-897">Boolean</span></span>|<span data-ttu-id="82fcc-898">指示是否允许其他设备发现此电脑进行投影。</span><span class="sxs-lookup"><span data-stu-id="82fcc-898">Indicates whether or not to allow other devices from discovering this PC for projection.</span></span>|
|<span data-ttu-id="82fcc-899">wirelessDisplayBlockUserInputFromReceiver</span><span class="sxs-lookup"><span data-stu-id="82fcc-899">wirelessDisplayBlockUserInputFromReceiver</span></span>|<span data-ttu-id="82fcc-900">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-900">Boolean</span></span>|<span data-ttu-id="82fcc-901">指示是否允许来自无线显示接收器的用户输入。</span><span class="sxs-lookup"><span data-stu-id="82fcc-901">Indicates whether or not to allow user input from wireless display receiver.</span></span>|
|<span data-ttu-id="82fcc-902">wirelessDisplayRequirePinForPairing</span><span class="sxs-lookup"><span data-stu-id="82fcc-902">wirelessDisplayRequirePinForPairing</span></span>|<span data-ttu-id="82fcc-903">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-903">Boolean</span></span>|<span data-ttu-id="82fcc-904">指示是否需要新设备的 PIN 才能启动配对。</span><span class="sxs-lookup"><span data-stu-id="82fcc-904">Indicates whether or not to require a PIN for new devices to initiate pairing.</span></span>|
|<span data-ttu-id="82fcc-905">windowsStoreBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-905">windowsStoreBlocked</span></span>|<span data-ttu-id="82fcc-906">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-906">Boolean</span></span>|<span data-ttu-id="82fcc-907">指示是否阻止用户使用 Windows 应用商店。</span><span class="sxs-lookup"><span data-stu-id="82fcc-907">Indicates whether or not to Block the user from using the Windows store.</span></span>|
|<span data-ttu-id="82fcc-908">appsAllowTrustedAppsSideloading</span><span class="sxs-lookup"><span data-stu-id="82fcc-908">appsAllowTrustedAppsSideloading</span></span>|[<span data-ttu-id="82fcc-909">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-909">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="82fcc-910">指示是否可以旁加载使用可信证书签名的来自 AppX 程序包的应用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-910">Indicates whether apps from AppX packages signed with a trusted certificate can be side loaded.</span></span> <span data-ttu-id="82fcc-911">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-911">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="82fcc-912">windowsStoreBlockAutoUpdate</span><span class="sxs-lookup"><span data-stu-id="82fcc-912">windowsStoreBlockAutoUpdate</span></span>|<span data-ttu-id="82fcc-913">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-913">Boolean</span></span>|<span data-ttu-id="82fcc-914">指示是否阻止从 Windows 应用商店自动更新应用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-914">Indicates whether or not to block automatic update of apps from Windows Store.</span></span>|
|<span data-ttu-id="82fcc-915">developerUnlockSetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-915">developerUnlockSetting</span></span>|[<span data-ttu-id="82fcc-916">stateManagementSetting</span><span class="sxs-lookup"><span data-stu-id="82fcc-916">stateManagementSetting</span></span>](../resources/intune-deviceconfig-statemanagementsetting.md)|<span data-ttu-id="82fcc-917">指示是否允许开发人员解锁。</span><span class="sxs-lookup"><span data-stu-id="82fcc-917">Indicates whether or not to allow developer unlock.</span></span> <span data-ttu-id="82fcc-918">可取值为：`notConfigured`、`blocked`、`allowed`。</span><span class="sxs-lookup"><span data-stu-id="82fcc-918">Possible values are: `notConfigured`, `blocked`, `allowed`.</span></span>|
|<span data-ttu-id="82fcc-919">sharedUserAppDataAllowed</span><span class="sxs-lookup"><span data-stu-id="82fcc-919">sharedUserAppDataAllowed</span></span>|<span data-ttu-id="82fcc-920">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-920">Boolean</span></span>|<span data-ttu-id="82fcc-921">指示是否阻止同一应用的多个用户共享数据。</span><span class="sxs-lookup"><span data-stu-id="82fcc-921">Indicates whether or not to block multiple users of the same app to share data.</span></span>|
|<span data-ttu-id="82fcc-922">appsBlockWindowsStoreOriginatedApps</span><span class="sxs-lookup"><span data-stu-id="82fcc-922">appsBlockWindowsStoreOriginatedApps</span></span>|<span data-ttu-id="82fcc-923">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-923">Boolean</span></span>|<span data-ttu-id="82fcc-924">指示是否禁用启动 Windows 应用商店中预先安装或已下载的所有应用。</span><span class="sxs-lookup"><span data-stu-id="82fcc-924">Indicates whether or not to disable the launch of all apps from Windows Store that came pre-installed or were downloaded.</span></span>|
|<span data-ttu-id="82fcc-925">windowsStoreEnablePrivateStoreOnly</span><span class="sxs-lookup"><span data-stu-id="82fcc-925">windowsStoreEnablePrivateStoreOnly</span></span>|<span data-ttu-id="82fcc-926">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-926">Boolean</span></span>|<span data-ttu-id="82fcc-927">指示是否启用“仅限私人应用商店”。</span><span class="sxs-lookup"><span data-stu-id="82fcc-927">Indicates whether or not to enable Private Store Only.</span></span>|
|<span data-ttu-id="82fcc-928">storageRestrictAppDataToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="82fcc-928">storageRestrictAppDataToSystemVolume</span></span>|<span data-ttu-id="82fcc-929">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-929">Boolean</span></span>|<span data-ttu-id="82fcc-930">指示应用程序数据是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="82fcc-930">Indicates whether application data is restricted to the system drive.</span></span>|
|<span data-ttu-id="82fcc-931">storageRestrictAppInstallToSystemVolume</span><span class="sxs-lookup"><span data-stu-id="82fcc-931">storageRestrictAppInstallToSystemVolume</span></span>|<span data-ttu-id="82fcc-932">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-932">Boolean</span></span>|<span data-ttu-id="82fcc-933">指示应用程序的安装是否仅限于系统驱动器。</span><span class="sxs-lookup"><span data-stu-id="82fcc-933">Indicates whether the installation of applications is restricted to the system drive.</span></span>|
|<span data-ttu-id="82fcc-934">gameDvrBlocked</span><span class="sxs-lookup"><span data-stu-id="82fcc-934">gameDvrBlocked</span></span>|<span data-ttu-id="82fcc-935">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-935">Boolean</span></span>|<span data-ttu-id="82fcc-936">指示是否阻止 DVR 和广播。</span><span class="sxs-lookup"><span data-stu-id="82fcc-936">Indicates whether or not to block DVR and broadcasting.</span></span>|
|<span data-ttu-id="82fcc-937">experienceBlockDeviceDiscovery</span><span class="sxs-lookup"><span data-stu-id="82fcc-937">experienceBlockDeviceDiscovery</span></span>|<span data-ttu-id="82fcc-938">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-938">Boolean</span></span>|<span data-ttu-id="82fcc-939">指示是否启用设备发现 UX。</span><span class="sxs-lookup"><span data-stu-id="82fcc-939">Indicates whether or not to enable device discovery UX.</span></span>|
|<span data-ttu-id="82fcc-940">experienceBlockErrorDialogWhenNoSIM</span><span class="sxs-lookup"><span data-stu-id="82fcc-940">experienceBlockErrorDialogWhenNoSIM</span></span>|<span data-ttu-id="82fcc-941">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-941">Boolean</span></span>|<span data-ttu-id="82fcc-942">指示是否允许在未检测到 SIM 卡时显示错误对话框。</span><span class="sxs-lookup"><span data-stu-id="82fcc-942">Indicates whether or not to allow the error dialog from displaying if no SIM card is detected.</span></span>|
|<span data-ttu-id="82fcc-943">experienceBlockTaskSwitcher</span><span class="sxs-lookup"><span data-stu-id="82fcc-943">experienceBlockTaskSwitcher</span></span>|<span data-ttu-id="82fcc-944">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-944">Boolean</span></span>|<span data-ttu-id="82fcc-945">指示是否在设备上启用任务切换。</span><span class="sxs-lookup"><span data-stu-id="82fcc-945">Indicates whether or not to enable task switching on the device.</span></span>|
|<span data-ttu-id="82fcc-946">logonBlockFastUserSwitching</span><span class="sxs-lookup"><span data-stu-id="82fcc-946">logonBlockFastUserSwitching</span></span>|<span data-ttu-id="82fcc-947">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-947">Boolean</span></span>|<span data-ttu-id="82fcc-948">禁用在不注销的情况下在同时登录的用户之间快速切换的功能。</span><span class="sxs-lookup"><span data-stu-id="82fcc-948">Disables the ability to quickly switch between users that are logged on simultaneously without logging off.</span></span>|
|<span data-ttu-id="82fcc-949">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span><span class="sxs-lookup"><span data-stu-id="82fcc-949">tenantLockdownRequireNetworkDuringOutOfBoxExperience</span></span>|<span data-ttu-id="82fcc-950">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-950">Boolean</span></span>|<span data-ttu-id="82fcc-951">设备是否需要连接到网络。</span><span class="sxs-lookup"><span data-stu-id="82fcc-951">Whether the device is required to connect to the network.</span></span>|
|<span data-ttu-id="82fcc-952">appManagementMSIAllowUserControlOverInstall</span><span class="sxs-lookup"><span data-stu-id="82fcc-952">appManagementMSIAllowUserControlOverInstall</span></span>|<span data-ttu-id="82fcc-953">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-953">Boolean</span></span>|<span data-ttu-id="82fcc-954">此策略设置允许用户更改通常只能由系统管理员的安装选项。</span><span class="sxs-lookup"><span data-stu-id="82fcc-954">This policy setting permits users to change installation options that typically are available only to system administrators.</span></span>|
|<span data-ttu-id="82fcc-955">appManagementMSIAlwaysInstallWithElevatedPrivileges</span><span class="sxs-lookup"><span data-stu-id="82fcc-955">appManagementMSIAlwaysInstallWithElevatedPrivileges</span></span>|<span data-ttu-id="82fcc-956">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-956">Boolean</span></span>|<span data-ttu-id="82fcc-957">此策略设置指示 Windows Installer 系统上安装任何程序时使用提升的权限。</span><span class="sxs-lookup"><span data-stu-id="82fcc-957">This policy setting directs Windows Installer to use elevated permissions when it installs any program on the system.</span></span>|
|<span data-ttu-id="82fcc-958">dataProtectionBlockDirectMemoryAccess</span><span class="sxs-lookup"><span data-stu-id="82fcc-958">dataProtectionBlockDirectMemoryAccess</span></span>|<span data-ttu-id="82fcc-959">Boolean</span><span class="sxs-lookup"><span data-stu-id="82fcc-959">Boolean</span></span>|<span data-ttu-id="82fcc-960">此策略设置允许您阻止直接内存访问 (DMA) 的所有热 pluggable PCI 下游端口直到用户登录到 Windows。</span><span class="sxs-lookup"><span data-stu-id="82fcc-960">This policy setting allows you to block direct memory access (DMA) for all hot pluggable PCI downstream ports until a user logs into Windows.</span></span>|



## <a name="response"></a><span data-ttu-id="82fcc-961">响应</span><span class="sxs-lookup"><span data-stu-id="82fcc-961">Response</span></span>
<span data-ttu-id="82fcc-962">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="82fcc-962">If successful, this method returns a `200 OK` response code and an updated [windows10GeneralConfiguration](../resources/intune-deviceconfig-windows10generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82fcc-963">示例</span><span class="sxs-lookup"><span data-stu-id="82fcc-963">Example</span></span>
### <a name="request"></a><span data-ttu-id="82fcc-964">请求</span><span class="sxs-lookup"><span data-stu-id="82fcc-964">Request</span></span>
<span data-ttu-id="82fcc-965">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82fcc-965">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 12134

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "assignedAccessSingleModeUserName": "Assigned Access Single Mode User Name value",
  "assignedAccessSingleModeAppUserModelId": "Assigned Access Single Mode App User Model Id value",
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationAllowFIDODevice": true,
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

### <a name="response"></a><span data-ttu-id="82fcc-966">响应</span><span class="sxs-lookup"><span data-stu-id="82fcc-966">Response</span></span>
<span data-ttu-id="82fcc-p172">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82fcc-p172">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 12310

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
  "windows10AppsForceUpdateSchedule": {
    "@odata.type": "microsoft.graph.windows10AppsForceUpdateSchedule",
    "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
    "recurrence": "daily",
    "runImmediatelyIfAfterStartDateTime": true
  },
  "enableAutomaticRedeployment": true,
  "assignedAccessSingleModeUserName": "Assigned Access Single Mode User Name value",
  "assignedAccessSingleModeAppUserModelId": "Assigned Access Single Mode App User Model Id value",
  "microsoftAccountSignInAssistantSettings": "disabled",
  "authenticationAllowSecondaryDevice": true,
  "authenticationAllowFIDODevice": true,
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





