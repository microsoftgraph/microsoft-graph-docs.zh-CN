---
title: 创建 windows10SecureAssessmentConfiguration
description: 创建新的 windows10SecureAssessmentConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 50db5375419346f63af9783a02c6af4953ea0155
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48065576"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="f5036-103">创建 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="f5036-103">Create windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="f5036-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5036-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5036-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5036-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5036-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5036-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5036-107">创建新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5036-107">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f5036-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f5036-108">Prerequisites</span></span>
<span data-ttu-id="f5036-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5036-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5036-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5036-111">Permission type</span></span>|<span data-ttu-id="f5036-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f5036-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f5036-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5036-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f5036-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5036-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f5036-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5036-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f5036-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f5036-116">Not supported.</span></span>|
|<span data-ttu-id="f5036-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5036-117">Application</span></span>|<span data-ttu-id="f5036-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5036-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f5036-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5036-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f5036-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5036-120">Request headers</span></span>
|<span data-ttu-id="f5036-121">标头</span><span class="sxs-lookup"><span data-stu-id="f5036-121">Header</span></span>|<span data-ttu-id="f5036-122">值</span><span class="sxs-lookup"><span data-stu-id="f5036-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f5036-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5036-123">Authorization</span></span>|<span data-ttu-id="f5036-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f5036-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f5036-125">接受</span><span class="sxs-lookup"><span data-stu-id="f5036-125">Accept</span></span>|<span data-ttu-id="f5036-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f5036-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f5036-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5036-127">Request body</span></span>
<span data-ttu-id="f5036-128">在请求正文中，提供 windows10SecureAssessmentConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f5036-128">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="f5036-129">下表显示创建 windows10SecureAssessmentConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f5036-129">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="f5036-130">属性</span><span class="sxs-lookup"><span data-stu-id="f5036-130">Property</span></span>|<span data-ttu-id="f5036-131">类型</span><span class="sxs-lookup"><span data-stu-id="f5036-131">Type</span></span>|<span data-ttu-id="f5036-132">说明</span><span class="sxs-lookup"><span data-stu-id="f5036-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5036-133">id</span><span class="sxs-lookup"><span data-stu-id="f5036-133">id</span></span>|<span data-ttu-id="f5036-134">String</span><span class="sxs-lookup"><span data-stu-id="f5036-134">String</span></span>|<span data-ttu-id="f5036-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f5036-135">Key of the entity.</span></span> <span data-ttu-id="f5036-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f5036-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f5036-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5036-138">DateTimeOffset</span></span>|<span data-ttu-id="f5036-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f5036-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f5036-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f5036-141">roleScopeTagIds</span></span>|<span data-ttu-id="f5036-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="f5036-142">String collection</span></span>|<span data-ttu-id="f5036-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="f5036-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f5036-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f5036-145">supportsScopeTags</span></span>|<span data-ttu-id="f5036-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5036-146">Boolean</span></span>|<span data-ttu-id="f5036-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="f5036-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f5036-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="f5036-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f5036-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="f5036-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f5036-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="f5036-150">This property is read-only.</span></span> <span data-ttu-id="f5036-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5036-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="f5036-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="f5036-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="f5036-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="f5036-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="f5036-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5036-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="f5036-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="f5036-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="f5036-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f5036-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="f5036-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f5036-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="f5036-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="f5036-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="f5036-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="f5036-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="f5036-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f5036-164">createdDateTime</span></span>|<span data-ttu-id="f5036-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f5036-165">DateTimeOffset</span></span>|<span data-ttu-id="f5036-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f5036-166">DateTime the object was created.</span></span> <span data-ttu-id="f5036-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-168">说明</span><span class="sxs-lookup"><span data-stu-id="f5036-168">description</span></span>|<span data-ttu-id="f5036-169">String</span><span class="sxs-lookup"><span data-stu-id="f5036-169">String</span></span>|<span data-ttu-id="f5036-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f5036-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f5036-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-172">displayName</span><span class="sxs-lookup"><span data-stu-id="f5036-172">displayName</span></span>|<span data-ttu-id="f5036-173">String</span><span class="sxs-lookup"><span data-stu-id="f5036-173">String</span></span>|<span data-ttu-id="f5036-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f5036-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f5036-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-176">version</span><span class="sxs-lookup"><span data-stu-id="f5036-176">version</span></span>|<span data-ttu-id="f5036-177">Int32</span><span class="sxs-lookup"><span data-stu-id="f5036-177">Int32</span></span>|<span data-ttu-id="f5036-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f5036-178">Version of the device configuration.</span></span> <span data-ttu-id="f5036-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f5036-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f5036-180">launchUri</span><span class="sxs-lookup"><span data-stu-id="f5036-180">launchUri</span></span>|<span data-ttu-id="f5036-181">String</span><span class="sxs-lookup"><span data-stu-id="f5036-181">String</span></span>|<span data-ttu-id="f5036-182">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="f5036-182">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="f5036-183">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="f5036-183">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="f5036-184">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="f5036-184">configurationAccount</span></span>|<span data-ttu-id="f5036-185">String</span><span class="sxs-lookup"><span data-stu-id="f5036-185">String</span></span>|<span data-ttu-id="f5036-186">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="f5036-186">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="f5036-187">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="f5036-187">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="f5036-188">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="f5036-188">configurationAccountType</span></span>|[<span data-ttu-id="f5036-189">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="f5036-189">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="f5036-190">由 ConfigurationAccount 使用的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="f5036-190">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="f5036-191">可取值为：`azureADAccount`、`domainAccount`、`localAccount`、`localGuestAccount`。</span><span class="sxs-lookup"><span data-stu-id="f5036-191">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="f5036-192">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="f5036-192">allowPrinting</span></span>|<span data-ttu-id="f5036-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5036-193">Boolean</span></span>|<span data-ttu-id="f5036-194">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="f5036-194">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="f5036-195">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="f5036-195">allowScreenCapture</span></span>|<span data-ttu-id="f5036-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5036-196">Boolean</span></span>|<span data-ttu-id="f5036-197">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="f5036-197">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="f5036-198">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="f5036-198">allowTextSuggestion</span></span>|<span data-ttu-id="f5036-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="f5036-199">Boolean</span></span>|<span data-ttu-id="f5036-200">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="f5036-200">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="f5036-201">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="f5036-201">localGuestAccountName</span></span>|<span data-ttu-id="f5036-202">String</span><span class="sxs-lookup"><span data-stu-id="f5036-202">String</span></span>|<span data-ttu-id="f5036-203">指定在登录屏幕上显示的本地来宾帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="f5036-203">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="f5036-204">通常是评估的名称。</span><span class="sxs-lookup"><span data-stu-id="f5036-204">Typically is the name of an assessment.</span></span> <span data-ttu-id="f5036-205">当用户在登录屏幕上单击本地来宾帐户时，将使用指定的评估 URL 启动评估应用程序。</span><span class="sxs-lookup"><span data-stu-id="f5036-205">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="f5036-206">只能在运行 Windows 10 版本1903或更高版本的设备上使用本地来宾帐户登录来配置安全评估。</span><span class="sxs-lookup"><span data-stu-id="f5036-206">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="f5036-207">重要说明：必须使用 assessmentAppUserModelID 设置此属性，才能使本地来宾帐户登录体验正常工作以进行安全评估。</span><span class="sxs-lookup"><span data-stu-id="f5036-207">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="f5036-208">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="f5036-208">assessmentAppUserModelId</span></span>|<span data-ttu-id="f5036-209">String</span><span class="sxs-lookup"><span data-stu-id="f5036-209">String</span></span>|<span data-ttu-id="f5036-210">指定当用户使用本地来宾帐户登录安全评估时启动的评估应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="f5036-210">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="f5036-211">重要说明：必须使用 localGuestAccountName 设置此属性，才能使本地来宾帐户登录体验正常工作以进行安全评估。</span><span class="sxs-lookup"><span data-stu-id="f5036-211">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="f5036-212">响应</span><span class="sxs-lookup"><span data-stu-id="f5036-212">Response</span></span>
<span data-ttu-id="f5036-213">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f5036-213">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5036-214">示例</span><span class="sxs-lookup"><span data-stu-id="f5036-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="f5036-215">请求</span><span class="sxs-lookup"><span data-stu-id="f5036-215">Request</span></span>
<span data-ttu-id="f5036-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5036-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f5036-217">响应</span><span class="sxs-lookup"><span data-stu-id="f5036-217">Response</span></span>
<span data-ttu-id="f5036-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5036-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






