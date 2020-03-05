---
title: 更新 windows10SecureAssessmentConfiguration
description: 更新 windows10SecureAssessmentConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f818fa67e9f6a4f99038282a42f757301bd03a99
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42477922"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="dfbee-103">更新 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="dfbee-103">Update windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="dfbee-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dfbee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dfbee-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dfbee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dfbee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dfbee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dfbee-107">更新 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dfbee-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dfbee-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dfbee-108">Prerequisites</span></span>
<span data-ttu-id="dfbee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfbee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfbee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfbee-111">Permission type</span></span>|<span data-ttu-id="dfbee-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dfbee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfbee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfbee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dfbee-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfbee-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dfbee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfbee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfbee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfbee-116">Not supported.</span></span>|
|<span data-ttu-id="dfbee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfbee-117">Application</span></span>|<span data-ttu-id="dfbee-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dfbee-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfbee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfbee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="dfbee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfbee-120">Request headers</span></span>
|<span data-ttu-id="dfbee-121">标头</span><span class="sxs-lookup"><span data-stu-id="dfbee-121">Header</span></span>|<span data-ttu-id="dfbee-122">值</span><span class="sxs-lookup"><span data-stu-id="dfbee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfbee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfbee-123">Authorization</span></span>|<span data-ttu-id="dfbee-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dfbee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfbee-125">接受</span><span class="sxs-lookup"><span data-stu-id="dfbee-125">Accept</span></span>|<span data-ttu-id="dfbee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dfbee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfbee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfbee-127">Request body</span></span>
<span data-ttu-id="dfbee-128">在请求正文中，提供 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfbee-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="dfbee-129">下表显示创建 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dfbee-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="dfbee-130">属性</span><span class="sxs-lookup"><span data-stu-id="dfbee-130">Property</span></span>|<span data-ttu-id="dfbee-131">类型</span><span class="sxs-lookup"><span data-stu-id="dfbee-131">Type</span></span>|<span data-ttu-id="dfbee-132">说明</span><span class="sxs-lookup"><span data-stu-id="dfbee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dfbee-133">id</span><span class="sxs-lookup"><span data-stu-id="dfbee-133">id</span></span>|<span data-ttu-id="dfbee-134">字符串</span><span class="sxs-lookup"><span data-stu-id="dfbee-134">String</span></span>|<span data-ttu-id="dfbee-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="dfbee-135">Key of the entity.</span></span> <span data-ttu-id="dfbee-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dfbee-137">lastModifiedDateTime</span></span>|<span data-ttu-id="dfbee-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfbee-138">DateTimeOffset</span></span>|<span data-ttu-id="dfbee-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dfbee-139">DateTime the object was last modified.</span></span> <span data-ttu-id="dfbee-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dfbee-141">roleScopeTagIds</span></span>|<span data-ttu-id="dfbee-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="dfbee-142">String collection</span></span>|<span data-ttu-id="dfbee-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="dfbee-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="dfbee-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="dfbee-145">supportsScopeTags</span></span>|<span data-ttu-id="dfbee-146">布尔</span><span class="sxs-lookup"><span data-stu-id="dfbee-146">Boolean</span></span>|<span data-ttu-id="dfbee-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="dfbee-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="dfbee-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="dfbee-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="dfbee-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="dfbee-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="dfbee-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="dfbee-150">This property is read-only.</span></span> <span data-ttu-id="dfbee-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dfbee-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="dfbee-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="dfbee-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="dfbee-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="dfbee-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="dfbee-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dfbee-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="dfbee-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="dfbee-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="dfbee-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="dfbee-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="dfbee-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dfbee-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="dfbee-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="dfbee-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="dfbee-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="dfbee-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="dfbee-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dfbee-164">createdDateTime</span></span>|<span data-ttu-id="dfbee-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dfbee-165">DateTimeOffset</span></span>|<span data-ttu-id="dfbee-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="dfbee-166">DateTime the object was created.</span></span> <span data-ttu-id="dfbee-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-168">说明</span><span class="sxs-lookup"><span data-stu-id="dfbee-168">description</span></span>|<span data-ttu-id="dfbee-169">String</span><span class="sxs-lookup"><span data-stu-id="dfbee-169">String</span></span>|<span data-ttu-id="dfbee-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="dfbee-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="dfbee-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-172">displayName</span><span class="sxs-lookup"><span data-stu-id="dfbee-172">displayName</span></span>|<span data-ttu-id="dfbee-173">字符串</span><span class="sxs-lookup"><span data-stu-id="dfbee-173">String</span></span>|<span data-ttu-id="dfbee-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="dfbee-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="dfbee-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-176">version</span><span class="sxs-lookup"><span data-stu-id="dfbee-176">version</span></span>|<span data-ttu-id="dfbee-177">Int32</span><span class="sxs-lookup"><span data-stu-id="dfbee-177">Int32</span></span>|<span data-ttu-id="dfbee-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="dfbee-178">Version of the device configuration.</span></span> <span data-ttu-id="dfbee-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="dfbee-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="dfbee-180">launchUri</span><span class="sxs-lookup"><span data-stu-id="dfbee-180">launchUri</span></span>|<span data-ttu-id="dfbee-181">String</span><span class="sxs-lookup"><span data-stu-id="dfbee-181">String</span></span>|<span data-ttu-id="dfbee-182">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="dfbee-182">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="dfbee-183">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="dfbee-183">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="dfbee-184">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="dfbee-184">configurationAccount</span></span>|<span data-ttu-id="dfbee-185">String</span><span class="sxs-lookup"><span data-stu-id="dfbee-185">String</span></span>|<span data-ttu-id="dfbee-186">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="dfbee-186">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="dfbee-187">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="dfbee-187">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="dfbee-188">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="dfbee-188">configurationAccountType</span></span>|[<span data-ttu-id="dfbee-189">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="dfbee-189">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="dfbee-190">由 ConfigurationAccount 使用的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="dfbee-190">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="dfbee-191">可取值为：`azureADAccount`、`domainAccount`、`localAccount`、`localGuestAccount`。</span><span class="sxs-lookup"><span data-stu-id="dfbee-191">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="dfbee-192">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="dfbee-192">allowPrinting</span></span>|<span data-ttu-id="dfbee-193">布尔</span><span class="sxs-lookup"><span data-stu-id="dfbee-193">Boolean</span></span>|<span data-ttu-id="dfbee-194">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="dfbee-194">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="dfbee-195">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="dfbee-195">allowScreenCapture</span></span>|<span data-ttu-id="dfbee-196">布尔</span><span class="sxs-lookup"><span data-stu-id="dfbee-196">Boolean</span></span>|<span data-ttu-id="dfbee-197">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="dfbee-197">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="dfbee-198">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="dfbee-198">allowTextSuggestion</span></span>|<span data-ttu-id="dfbee-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="dfbee-199">Boolean</span></span>|<span data-ttu-id="dfbee-200">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="dfbee-200">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="dfbee-201">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="dfbee-201">localGuestAccountName</span></span>|<span data-ttu-id="dfbee-202">String</span><span class="sxs-lookup"><span data-stu-id="dfbee-202">String</span></span>|<span data-ttu-id="dfbee-203">指定在登录屏幕上显示的本地来宾帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="dfbee-203">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="dfbee-204">通常是评估的名称。</span><span class="sxs-lookup"><span data-stu-id="dfbee-204">Typically is the name of an assessment.</span></span> <span data-ttu-id="dfbee-205">当用户在登录屏幕上单击本地来宾帐户时，将使用指定的评估 URL 启动评估应用程序。</span><span class="sxs-lookup"><span data-stu-id="dfbee-205">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="dfbee-206">只能在运行 Windows 10 版本1903或更高版本的设备上使用本地来宾帐户登录来配置安全评估。</span><span class="sxs-lookup"><span data-stu-id="dfbee-206">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="dfbee-207">重要说明：必须使用 assessmentAppUserModelID 设置此属性，才能使本地来宾帐户登录体验正常工作以进行安全评估。</span><span class="sxs-lookup"><span data-stu-id="dfbee-207">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="dfbee-208">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="dfbee-208">assessmentAppUserModelId</span></span>|<span data-ttu-id="dfbee-209">String</span><span class="sxs-lookup"><span data-stu-id="dfbee-209">String</span></span>|<span data-ttu-id="dfbee-210">指定当用户使用本地来宾帐户登录安全评估时启动的评估应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="dfbee-210">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="dfbee-211">重要说明：必须使用 localGuestAccountName 设置此属性，才能使本地来宾帐户登录体验正常工作以进行安全评估。</span><span class="sxs-lookup"><span data-stu-id="dfbee-211">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="dfbee-212">响应</span><span class="sxs-lookup"><span data-stu-id="dfbee-212">Response</span></span>
<span data-ttu-id="dfbee-213">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dfbee-213">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfbee-214">示例</span><span class="sxs-lookup"><span data-stu-id="dfbee-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="dfbee-215">请求</span><span class="sxs-lookup"><span data-stu-id="dfbee-215">Request</span></span>
<span data-ttu-id="dfbee-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfbee-216">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1403

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
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
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true,
  "localGuestAccountName": "Local Guest Account Name value",
  "assessmentAppUserModelId": "Assessment App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="dfbee-217">响应</span><span class="sxs-lookup"><span data-stu-id="dfbee-217">Response</span></span>
<span data-ttu-id="dfbee-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfbee-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1575

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
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
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true,
  "localGuestAccountName": "Local Guest Account Name value",
  "assessmentAppUserModelId": "Assessment App User Model Id value"
}
```





