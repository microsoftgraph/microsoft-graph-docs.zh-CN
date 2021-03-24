---
title: 更新 windows10SecureAssessmentConfiguration
description: 更新 windows10SecureAssessmentConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc91366f1d7ae9e827795f10b95cd352f9d97b42
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127443"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="37841-103">更新 windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="37841-103">Update windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="37841-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37841-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37841-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37841-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37841-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37841-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37841-107">更新 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="37841-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37841-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="37841-108">Prerequisites</span></span>
<span data-ttu-id="37841-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37841-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37841-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="37841-111">Permission type</span></span>|<span data-ttu-id="37841-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="37841-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37841-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37841-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37841-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37841-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="37841-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37841-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37841-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37841-116">Not supported.</span></span>|
|<span data-ttu-id="37841-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="37841-117">Application</span></span>|<span data-ttu-id="37841-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37841-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37841-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37841-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="37841-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="37841-120">Request headers</span></span>
|<span data-ttu-id="37841-121">标头</span><span class="sxs-lookup"><span data-stu-id="37841-121">Header</span></span>|<span data-ttu-id="37841-122">值</span><span class="sxs-lookup"><span data-stu-id="37841-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37841-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37841-123">Authorization</span></span>|<span data-ttu-id="37841-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="37841-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37841-125">接受</span><span class="sxs-lookup"><span data-stu-id="37841-125">Accept</span></span>|<span data-ttu-id="37841-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37841-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37841-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37841-127">Request body</span></span>
<span data-ttu-id="37841-128">在请求正文中，提供 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37841-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="37841-129">下表显示创建 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="37841-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="37841-130">属性</span><span class="sxs-lookup"><span data-stu-id="37841-130">Property</span></span>|<span data-ttu-id="37841-131">类型</span><span class="sxs-lookup"><span data-stu-id="37841-131">Type</span></span>|<span data-ttu-id="37841-132">说明</span><span class="sxs-lookup"><span data-stu-id="37841-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37841-133">id</span><span class="sxs-lookup"><span data-stu-id="37841-133">id</span></span>|<span data-ttu-id="37841-134">String</span><span class="sxs-lookup"><span data-stu-id="37841-134">String</span></span>|<span data-ttu-id="37841-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="37841-135">Key of the entity.</span></span> <span data-ttu-id="37841-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="37841-137">lastModifiedDateTime</span></span>|<span data-ttu-id="37841-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37841-138">DateTimeOffset</span></span>|<span data-ttu-id="37841-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="37841-139">DateTime the object was last modified.</span></span> <span data-ttu-id="37841-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="37841-141">roleScopeTagIds</span></span>|<span data-ttu-id="37841-142">String collection</span><span class="sxs-lookup"><span data-stu-id="37841-142">String collection</span></span>|<span data-ttu-id="37841-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="37841-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="37841-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="37841-145">supportsScopeTags</span></span>|<span data-ttu-id="37841-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="37841-146">Boolean</span></span>|<span data-ttu-id="37841-147">指示基础设备配置是否支持分配范围标记。</span><span class="sxs-lookup"><span data-stu-id="37841-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="37841-148">当此值为 false 且实体对作用域用户不可见时，不允许分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="37841-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="37841-149">这适用于在 Silverlight 中创建的旧版策略，可通过在 Azure 门户中删除和重新创建策略来解决。</span><span class="sxs-lookup"><span data-stu-id="37841-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="37841-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="37841-150">This property is read-only.</span></span> <span data-ttu-id="37841-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37841-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="37841-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="37841-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="37841-154">此策略的操作系统版本适用性。</span><span class="sxs-lookup"><span data-stu-id="37841-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="37841-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37841-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="37841-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="37841-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="37841-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="37841-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="37841-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37841-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="37841-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="37841-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="37841-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="37841-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="37841-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="37841-164">createdDateTime</span></span>|<span data-ttu-id="37841-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="37841-165">DateTimeOffset</span></span>|<span data-ttu-id="37841-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="37841-166">DateTime the object was created.</span></span> <span data-ttu-id="37841-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-168">说明</span><span class="sxs-lookup"><span data-stu-id="37841-168">description</span></span>|<span data-ttu-id="37841-169">String</span><span class="sxs-lookup"><span data-stu-id="37841-169">String</span></span>|<span data-ttu-id="37841-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="37841-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="37841-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-172">displayName</span><span class="sxs-lookup"><span data-stu-id="37841-172">displayName</span></span>|<span data-ttu-id="37841-173">String</span><span class="sxs-lookup"><span data-stu-id="37841-173">String</span></span>|<span data-ttu-id="37841-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="37841-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="37841-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-176">version</span><span class="sxs-lookup"><span data-stu-id="37841-176">version</span></span>|<span data-ttu-id="37841-177">Int32</span><span class="sxs-lookup"><span data-stu-id="37841-177">Int32</span></span>|<span data-ttu-id="37841-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="37841-178">Version of the device configuration.</span></span> <span data-ttu-id="37841-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="37841-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="37841-180">launchUri</span><span class="sxs-lookup"><span data-stu-id="37841-180">launchUri</span></span>|<span data-ttu-id="37841-181">String</span><span class="sxs-lookup"><span data-stu-id="37841-181">String</span></span>|<span data-ttu-id="37841-182">启动安全评估浏览器时指向自动加载的评估的 URL 链接。</span><span class="sxs-lookup"><span data-stu-id="37841-182">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="37841-183">它必须是有效的 URL (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="37841-183">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="37841-184">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="37841-184">configurationAccount</span></span>|<span data-ttu-id="37841-185">String</span><span class="sxs-lookup"><span data-stu-id="37841-185">String</span></span>|<span data-ttu-id="37841-186">用于配置 Windows 设备进行测试的帐户。</span><span class="sxs-lookup"><span data-stu-id="37841-186">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="37841-187">用户可以是域帐户（域\用户）、AAD 帐户 (username@tenant.com) 或本地帐户（用户名）。</span><span class="sxs-lookup"><span data-stu-id="37841-187">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="37841-188">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="37841-188">configurationAccountType</span></span>|[<span data-ttu-id="37841-189">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="37841-189">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="37841-190">ConfigurationAccount 所使用的帐户类型。</span><span class="sxs-lookup"><span data-stu-id="37841-190">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="37841-191">可取值为：`azureADAccount`、`domainAccount`、`localAccount`、`localGuestAccount`。</span><span class="sxs-lookup"><span data-stu-id="37841-191">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="37841-192">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="37841-192">allowPrinting</span></span>|<span data-ttu-id="37841-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="37841-193">Boolean</span></span>|<span data-ttu-id="37841-194">指示在测试期间是否允许应用打印。</span><span class="sxs-lookup"><span data-stu-id="37841-194">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="37841-195">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="37841-195">allowScreenCapture</span></span>|<span data-ttu-id="37841-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="37841-196">Boolean</span></span>|<span data-ttu-id="37841-197">指示在测试期间是否允许屏幕捕获功能。</span><span class="sxs-lookup"><span data-stu-id="37841-197">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="37841-198">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="37841-198">allowTextSuggestion</span></span>|<span data-ttu-id="37841-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="37841-199">Boolean</span></span>|<span data-ttu-id="37841-200">指示在测试期间是否允许文本建议。</span><span class="sxs-lookup"><span data-stu-id="37841-200">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="37841-201">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="37841-201">localGuestAccountName</span></span>|<span data-ttu-id="37841-202">String</span><span class="sxs-lookup"><span data-stu-id="37841-202">String</span></span>|<span data-ttu-id="37841-203">指定登录屏幕上显示的本地来宾帐户的显示文本。</span><span class="sxs-lookup"><span data-stu-id="37841-203">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="37841-204">通常是评估的名称。</span><span class="sxs-lookup"><span data-stu-id="37841-204">Typically is the name of an assessment.</span></span> <span data-ttu-id="37841-205">当用户在登录屏幕上单击本地来宾帐户时，会使用指定的评估 URL 启动评估应用。</span><span class="sxs-lookup"><span data-stu-id="37841-205">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="37841-206">安全评估只能在运行 Windows 10 版本 1903 或更高版本的设备上使用本地来宾帐户登录进行配置。</span><span class="sxs-lookup"><span data-stu-id="37841-206">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="37841-207">重要说明：此属性必须使用 assessmentAppUserModelID 进行设置，以便本地来宾帐户登录体验能够正常进行安全评估。</span><span class="sxs-lookup"><span data-stu-id="37841-207">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="37841-208">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="37841-208">assessmentAppUserModelId</span></span>|<span data-ttu-id="37841-209">String</span><span class="sxs-lookup"><span data-stu-id="37841-209">String</span></span>|<span data-ttu-id="37841-210">指定当用户使用本地来宾帐户登录安全评估时启动的评估应用的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="37841-210">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="37841-211">重要说明：此属性必须使用 localGuestAccountName 进行设置，以便本地来宾帐户登录体验能够正常进行安全评估。</span><span class="sxs-lookup"><span data-stu-id="37841-211">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="37841-212">响应</span><span class="sxs-lookup"><span data-stu-id="37841-212">Response</span></span>
<span data-ttu-id="37841-213">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37841-213">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37841-214">示例</span><span class="sxs-lookup"><span data-stu-id="37841-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="37841-215">请求</span><span class="sxs-lookup"><span data-stu-id="37841-215">Request</span></span>
<span data-ttu-id="37841-216">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37841-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37841-217">响应</span><span class="sxs-lookup"><span data-stu-id="37841-217">Response</span></span>
<span data-ttu-id="37841-p118">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37841-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




