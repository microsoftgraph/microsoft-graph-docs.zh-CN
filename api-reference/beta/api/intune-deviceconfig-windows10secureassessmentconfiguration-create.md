---
title: 创建 windows10SecureAssessmentConfiguration
description: 创建新的 windows10SecureAssessmentConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 99d6e859fb0eb3f17650fe65d9c0e778fd225a51
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533100"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="4ebcf-103">创建 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ebcf-103">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="4ebcf-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ebcf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ebcf-106">创建新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-106">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ebcf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ebcf-107">Prerequisites</span></span>
<span data-ttu-id="4ebcf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ebcf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ebcf-110">Permission type</span></span>|<span data-ttu-id="4ebcf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ebcf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ebcf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ebcf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ebcf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ebcf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ebcf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ebcf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ebcf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-115">Not supported.</span></span>|
|<span data-ttu-id="4ebcf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ebcf-116">Application</span></span>|<span data-ttu-id="4ebcf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ebcf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ebcf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ebcf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ebcf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ebcf-119">Request headers</span></span>
|<span data-ttu-id="4ebcf-120">标头</span><span class="sxs-lookup"><span data-stu-id="4ebcf-120">Header</span></span>|<span data-ttu-id="4ebcf-121">值</span><span class="sxs-lookup"><span data-stu-id="4ebcf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ebcf-122">授权</span><span class="sxs-lookup"><span data-stu-id="4ebcf-122">Authorization</span></span>|<span data-ttu-id="4ebcf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ebcf-124">接受</span><span class="sxs-lookup"><span data-stu-id="4ebcf-124">Accept</span></span>|<span data-ttu-id="4ebcf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ebcf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ebcf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ebcf-126">Request body</span></span>
<span data-ttu-id="4ebcf-127">在请求正文中，提供 windows10SecureAssessmentConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-127">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="4ebcf-128">下表显示创建 windows10SecureAssessmentConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-128">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="4ebcf-129">属性</span><span class="sxs-lookup"><span data-stu-id="4ebcf-129">Property</span></span>|<span data-ttu-id="4ebcf-130">类型</span><span class="sxs-lookup"><span data-stu-id="4ebcf-130">Type</span></span>|<span data-ttu-id="4ebcf-131">说明</span><span class="sxs-lookup"><span data-stu-id="4ebcf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ebcf-132">id</span><span class="sxs-lookup"><span data-stu-id="4ebcf-132">id</span></span>|<span data-ttu-id="4ebcf-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4ebcf-133">String</span></span>|<span data-ttu-id="4ebcf-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-134">Key of the entity.</span></span> <span data-ttu-id="4ebcf-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ebcf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4ebcf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ebcf-137">DateTimeOffset</span></span>|<span data-ttu-id="4ebcf-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4ebcf-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ebcf-140">roleScopeTagIds</span></span>|<span data-ttu-id="4ebcf-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="4ebcf-141">String collection</span></span>|<span data-ttu-id="4ebcf-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ebcf-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ebcf-144">supportsScopeTags</span></span>|<span data-ttu-id="4ebcf-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ebcf-145">Boolean</span></span>|<span data-ttu-id="4ebcf-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ebcf-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ebcf-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ebcf-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-149">This property is read-only.</span></span> <span data-ttu-id="4ebcf-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ebcf-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4ebcf-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ebcf-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4ebcf-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4ebcf-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ebcf-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4ebcf-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ebcf-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4ebcf-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4ebcf-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ebcf-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4ebcf-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ebcf-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4ebcf-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4ebcf-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ebcf-163">createdDateTime</span></span>|<span data-ttu-id="4ebcf-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ebcf-164">DateTimeOffset</span></span>|<span data-ttu-id="4ebcf-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-165">DateTime the object was created.</span></span> <span data-ttu-id="4ebcf-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-167">说明</span><span class="sxs-lookup"><span data-stu-id="4ebcf-167">description</span></span>|<span data-ttu-id="4ebcf-168">String</span><span class="sxs-lookup"><span data-stu-id="4ebcf-168">String</span></span>|<span data-ttu-id="4ebcf-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ebcf-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4ebcf-171">displayName</span></span>|<span data-ttu-id="4ebcf-172">字符串</span><span class="sxs-lookup"><span data-stu-id="4ebcf-172">String</span></span>|<span data-ttu-id="4ebcf-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ebcf-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-175">version</span><span class="sxs-lookup"><span data-stu-id="4ebcf-175">version</span></span>|<span data-ttu-id="4ebcf-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4ebcf-176">Int32</span></span>|<span data-ttu-id="4ebcf-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-177">Version of the device configuration.</span></span> <span data-ttu-id="4ebcf-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ebcf-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ebcf-179">launchUri</span><span class="sxs-lookup"><span data-stu-id="4ebcf-179">launchUri</span></span>|<span data-ttu-id="4ebcf-180">字符串</span><span class="sxs-lookup"><span data-stu-id="4ebcf-180">String</span></span>|<span data-ttu-id="4ebcf-181">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-181">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="4ebcf-182">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-182">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="4ebcf-183">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="4ebcf-183">configurationAccount</span></span>|<span data-ttu-id="4ebcf-184">String</span><span class="sxs-lookup"><span data-stu-id="4ebcf-184">String</span></span>|<span data-ttu-id="4ebcf-185">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-185">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="4ebcf-186">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-186">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="4ebcf-187">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="4ebcf-187">configurationAccountType</span></span>|[<span data-ttu-id="4ebcf-188">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="4ebcf-188">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="4ebcf-189">由 ConfigurationAccount 使用的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-189">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="4ebcf-190">可取值为：`azureADAccount`、`domainAccount`、`localAccount`、`localGuestAccount`。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-190">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="4ebcf-191">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="4ebcf-191">allowPrinting</span></span>|<span data-ttu-id="4ebcf-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ebcf-192">Boolean</span></span>|<span data-ttu-id="4ebcf-193">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-193">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="4ebcf-194">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="4ebcf-194">allowScreenCapture</span></span>|<span data-ttu-id="4ebcf-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ebcf-195">Boolean</span></span>|<span data-ttu-id="4ebcf-196">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-196">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="4ebcf-197">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="4ebcf-197">allowTextSuggestion</span></span>|<span data-ttu-id="4ebcf-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="4ebcf-198">Boolean</span></span>|<span data-ttu-id="4ebcf-199">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-199">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="4ebcf-200">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="4ebcf-200">localGuestAccountName</span></span>|<span data-ttu-id="4ebcf-201">字符串</span><span class="sxs-lookup"><span data-stu-id="4ebcf-201">String</span></span>|<span data-ttu-id="4ebcf-202">指定在登录屏幕上显示的本地来宾帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-202">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="4ebcf-203">通常是评估的名称。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-203">Typically is the name of an assessment.</span></span> <span data-ttu-id="4ebcf-204">当用户在登录屏幕上单击本地来宾帐户时，将使用指定的评估 URL 启动评估应用程序。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-204">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="4ebcf-205">只能在运行 Windows 10 版本1903或更高版本的设备上使用本地来宾帐户登录来配置安全评估。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-205">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="4ebcf-206">重要说明：必须使用 assessmentAppUserModelID 设置此属性，才能使本地来宾帐户登录体验正常工作以进行安全评估。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-206">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="4ebcf-207">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="4ebcf-207">assessmentAppUserModelId</span></span>|<span data-ttu-id="4ebcf-208">字符串</span><span class="sxs-lookup"><span data-stu-id="4ebcf-208">String</span></span>|<span data-ttu-id="4ebcf-209">指定当用户使用本地来宾帐户登录安全评估时启动的评估应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-209">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="4ebcf-210">重要说明：必须使用 localGuestAccountName 设置此属性，才能使本地来宾帐户登录体验正常工作以进行安全评估。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-210">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="4ebcf-211">响应</span><span class="sxs-lookup"><span data-stu-id="4ebcf-211">Response</span></span>
<span data-ttu-id="4ebcf-212">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-212">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ebcf-213">示例</span><span class="sxs-lookup"><span data-stu-id="4ebcf-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ebcf-214">请求</span><span class="sxs-lookup"><span data-stu-id="4ebcf-214">Request</span></span>
<span data-ttu-id="4ebcf-215">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4ebcf-216">响应</span><span class="sxs-lookup"><span data-stu-id="4ebcf-216">Response</span></span>
<span data-ttu-id="4ebcf-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ebcf-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






