---
title: 创建 macOSGeneralDeviceConfiguration
description: 创建新的 macOSGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bf82fccec0e8658aa14bc5d4a5577c0ec6a849d9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49290915"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="76513-103">创建 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="76513-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="76513-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76513-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="76513-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76513-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76513-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76513-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76513-107">创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76513-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76513-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="76513-108">Prerequisites</span></span>
<span data-ttu-id="76513-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76513-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76513-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="76513-111">Permission type</span></span>|<span data-ttu-id="76513-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="76513-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76513-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="76513-113">Delegated (work or school account)</span></span>|<span data-ttu-id="76513-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76513-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76513-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="76513-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76513-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="76513-116">Not supported.</span></span>|
|<span data-ttu-id="76513-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="76513-117">Application</span></span>|<span data-ttu-id="76513-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76513-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76513-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76513-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="76513-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="76513-120">Request headers</span></span>
|<span data-ttu-id="76513-121">标头</span><span class="sxs-lookup"><span data-stu-id="76513-121">Header</span></span>|<span data-ttu-id="76513-122">值</span><span class="sxs-lookup"><span data-stu-id="76513-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76513-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="76513-123">Authorization</span></span>|<span data-ttu-id="76513-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="76513-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76513-125">接受</span><span class="sxs-lookup"><span data-stu-id="76513-125">Accept</span></span>|<span data-ttu-id="76513-126">application/json</span><span class="sxs-lookup"><span data-stu-id="76513-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76513-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="76513-127">Request body</span></span>
<span data-ttu-id="76513-128">在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="76513-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="76513-129">下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="76513-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="76513-130">属性</span><span class="sxs-lookup"><span data-stu-id="76513-130">Property</span></span>|<span data-ttu-id="76513-131">类型</span><span class="sxs-lookup"><span data-stu-id="76513-131">Type</span></span>|<span data-ttu-id="76513-132">说明</span><span class="sxs-lookup"><span data-stu-id="76513-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76513-133">id</span><span class="sxs-lookup"><span data-stu-id="76513-133">id</span></span>|<span data-ttu-id="76513-134">字符串</span><span class="sxs-lookup"><span data-stu-id="76513-134">String</span></span>|<span data-ttu-id="76513-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="76513-135">Key of the entity.</span></span> <span data-ttu-id="76513-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76513-137">lastModifiedDateTime</span></span>|<span data-ttu-id="76513-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76513-138">DateTimeOffset</span></span>|<span data-ttu-id="76513-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="76513-139">DateTime the object was last modified.</span></span> <span data-ttu-id="76513-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="76513-141">roleScopeTagIds</span></span>|<span data-ttu-id="76513-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="76513-142">String collection</span></span>|<span data-ttu-id="76513-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="76513-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="76513-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="76513-145">supportsScopeTags</span></span>|<span data-ttu-id="76513-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-146">Boolean</span></span>|<span data-ttu-id="76513-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="76513-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="76513-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="76513-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="76513-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="76513-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="76513-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="76513-150">This property is read-only.</span></span> <span data-ttu-id="76513-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76513-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="76513-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="76513-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="76513-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="76513-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="76513-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76513-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="76513-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="76513-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="76513-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="76513-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="76513-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76513-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="76513-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="76513-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="76513-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="76513-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="76513-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76513-164">createdDateTime</span></span>|<span data-ttu-id="76513-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76513-165">DateTimeOffset</span></span>|<span data-ttu-id="76513-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="76513-166">DateTime the object was created.</span></span> <span data-ttu-id="76513-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-168">description</span><span class="sxs-lookup"><span data-stu-id="76513-168">description</span></span>|<span data-ttu-id="76513-169">字符串</span><span class="sxs-lookup"><span data-stu-id="76513-169">String</span></span>|<span data-ttu-id="76513-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="76513-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76513-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-172">displayName</span><span class="sxs-lookup"><span data-stu-id="76513-172">displayName</span></span>|<span data-ttu-id="76513-173">字符串</span><span class="sxs-lookup"><span data-stu-id="76513-173">String</span></span>|<span data-ttu-id="76513-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="76513-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76513-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-176">version</span><span class="sxs-lookup"><span data-stu-id="76513-176">version</span></span>|<span data-ttu-id="76513-177">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-177">Int32</span></span>|<span data-ttu-id="76513-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="76513-178">Version of the device configuration.</span></span> <span data-ttu-id="76513-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76513-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76513-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="76513-180">compliantAppsList</span></span>|<span data-ttu-id="76513-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76513-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="76513-182">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="76513-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="76513-183">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="76513-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="76513-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="76513-184">compliantAppListType</span></span>|[<span data-ttu-id="76513-185">appListType</span><span class="sxs-lookup"><span data-stu-id="76513-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="76513-186">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="76513-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="76513-187">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="76513-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="76513-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="76513-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="76513-189">String 集合</span><span class="sxs-lookup"><span data-stu-id="76513-189">String collection</span></span>|<span data-ttu-id="76513-190">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="76513-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="76513-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="76513-191">passwordBlockSimple</span></span>|<span data-ttu-id="76513-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-192">Boolean</span></span>|<span data-ttu-id="76513-193">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="76513-193">Block simple passwords.</span></span>|
|<span data-ttu-id="76513-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="76513-194">passwordExpirationDays</span></span>|<span data-ttu-id="76513-195">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-195">Int32</span></span>|<span data-ttu-id="76513-196">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="76513-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="76513-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="76513-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="76513-198">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-198">Int32</span></span>|<span data-ttu-id="76513-199">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="76513-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="76513-200">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="76513-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="76513-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="76513-201">passwordMinimumLength</span></span>|<span data-ttu-id="76513-202">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-202">Int32</span></span>|<span data-ttu-id="76513-203">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="76513-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="76513-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="76513-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="76513-205">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-205">Int32</span></span>|<span data-ttu-id="76513-206">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="76513-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="76513-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="76513-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="76513-208">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-208">Int32</span></span>|<span data-ttu-id="76513-209">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="76513-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="76513-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="76513-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="76513-211">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-211">Int32</span></span>|<span data-ttu-id="76513-212">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="76513-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="76513-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="76513-213">passwordRequiredType</span></span>|[<span data-ttu-id="76513-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="76513-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="76513-215">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="76513-215">Type of password that is required.</span></span> <span data-ttu-id="76513-216">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="76513-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="76513-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="76513-217">passwordRequired</span></span>|<span data-ttu-id="76513-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-218">Boolean</span></span>|<span data-ttu-id="76513-219">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="76513-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="76513-220">passwordMaximumAttemptCount</span><span class="sxs-lookup"><span data-stu-id="76513-220">passwordMaximumAttemptCount</span></span>|<span data-ttu-id="76513-221">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-221">Int32</span></span>|<span data-ttu-id="76513-222">在设备的锁屏上尝试输入密码失败的次数。</span><span class="sxs-lookup"><span data-stu-id="76513-222">The number of allowed failed attempts to enter the passcode at the device's lock screen.</span></span> <span data-ttu-id="76513-223">有效的值为2到11</span><span class="sxs-lookup"><span data-stu-id="76513-223">Valid values 2 to 11</span></span>|
|<span data-ttu-id="76513-224">passwordMinutesUntilFailedLoginReset</span><span class="sxs-lookup"><span data-stu-id="76513-224">passwordMinutesUntilFailedLoginReset</span></span>|<span data-ttu-id="76513-225">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-225">Int32</span></span>|<span data-ttu-id="76513-226">达到最大失败登录尝试次数后重置登录前的分钟数。</span><span class="sxs-lookup"><span data-stu-id="76513-226">The number of minutes before the login is reset after the maximum number of unsuccessful login attempts is reached.</span></span>|
|<span data-ttu-id="76513-227">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="76513-227">keychainBlockCloudSync</span></span>|<span data-ttu-id="76513-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-228">Boolean</span></span>|<span data-ttu-id="76513-229">指示是否阻止 (macOS 10.12 及更高版本) 的 iCloud 密钥链同步。</span><span class="sxs-lookup"><span data-stu-id="76513-229">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="76513-230">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="76513-230">airPrintBlocked</span></span>|<span data-ttu-id="76513-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-231">Boolean</span></span>|<span data-ttu-id="76513-232">指示是否阻止 AirPrint (macOS 10.12 及更高版本中) 。</span><span class="sxs-lookup"><span data-stu-id="76513-232">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="76513-233">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="76513-233">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="76513-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-234">Boolean</span></span>|<span data-ttu-id="76513-235">指示 TLS 打印通信 (macOS 10.13 及更高版本) 是否需要受信任的证书。</span><span class="sxs-lookup"><span data-stu-id="76513-235">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="76513-236">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="76513-236">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="76513-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-237">Boolean</span></span>|<span data-ttu-id="76513-238">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="76513-238">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="76513-239">这样可以防止在网络流量 (macOS 10.3 及更高版本) 中出现虚假的 AirPrint 蓝牙信号。</span><span class="sxs-lookup"><span data-stu-id="76513-239">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="76513-240">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="76513-240">safariBlockAutofill</span></span>|<span data-ttu-id="76513-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-241">Boolean</span></span>|<span data-ttu-id="76513-242">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="76513-242">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="76513-243">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="76513-243">cameraBlocked</span></span>|<span data-ttu-id="76513-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-244">Boolean</span></span>|<span data-ttu-id="76513-245">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="76513-245">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="76513-246">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="76513-246">iTunesBlockMusicService</span></span>|<span data-ttu-id="76513-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-247">Boolean</span></span>|<span data-ttu-id="76513-248">指示是否阻止音乐服务并将音乐应用还原到经典模式。</span><span class="sxs-lookup"><span data-stu-id="76513-248">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="76513-249">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="76513-249">spotlightBlockInternetResults</span></span>|<span data-ttu-id="76513-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-250">Boolean</span></span>|<span data-ttu-id="76513-251">指示是否阻止聚光灯从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="76513-251">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="76513-252">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="76513-252">keyboardBlockDictation</span></span>|<span data-ttu-id="76513-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-253">Boolean</span></span>|<span data-ttu-id="76513-254">指示是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="76513-254">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="76513-255">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="76513-255">definitionLookupBlocked</span></span>|<span data-ttu-id="76513-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-256">Boolean</span></span>|<span data-ttu-id="76513-257">指示是否阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="76513-257">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="76513-258">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="76513-258">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="76513-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-259">Boolean</span></span>|<span data-ttu-id="76513-260">指示是否阻止用户使用 Apple Watch 解锁其 Mac。</span><span class="sxs-lookup"><span data-stu-id="76513-260">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="76513-261">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="76513-261">iTunesBlockFileSharing</span></span>|<span data-ttu-id="76513-262">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-262">Boolean</span></span>|<span data-ttu-id="76513-263">指示是否阻止使用 iTunes 传输文件。</span><span class="sxs-lookup"><span data-stu-id="76513-263">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="76513-264">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="76513-264">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="76513-265">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-265">Boolean</span></span>|<span data-ttu-id="76513-266">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="76513-266">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="76513-267">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="76513-267">iCloudBlockMail</span></span>|<span data-ttu-id="76513-268">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-268">Boolean</span></span>|<span data-ttu-id="76513-269">指示是否阻止 iCloud 同步邮件。</span><span class="sxs-lookup"><span data-stu-id="76513-269">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="76513-270">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="76513-270">iCloudBlockAddressBook</span></span>|<span data-ttu-id="76513-271">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-271">Boolean</span></span>|<span data-ttu-id="76513-272">指示是否阻止 iCloud 同步联系人。</span><span class="sxs-lookup"><span data-stu-id="76513-272">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="76513-273">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="76513-273">iCloudBlockCalendar</span></span>|<span data-ttu-id="76513-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-274">Boolean</span></span>|<span data-ttu-id="76513-275">指示是否阻止 iCloud 同步日历。</span><span class="sxs-lookup"><span data-stu-id="76513-275">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="76513-276">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="76513-276">iCloudBlockReminders</span></span>|<span data-ttu-id="76513-277">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-277">Boolean</span></span>|<span data-ttu-id="76513-278">指示是否阻止 iCloud 同步提醒。</span><span class="sxs-lookup"><span data-stu-id="76513-278">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="76513-279">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="76513-279">iCloudBlockBookmarks</span></span>|<span data-ttu-id="76513-280">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-280">Boolean</span></span>|<span data-ttu-id="76513-281">指示是否阻止 iCloud 同步书签。</span><span class="sxs-lookup"><span data-stu-id="76513-281">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="76513-282">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="76513-282">iCloudBlockNotes</span></span>|<span data-ttu-id="76513-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-283">Boolean</span></span>|<span data-ttu-id="76513-284">指示是否阻止 iCloud 同步笔记。</span><span class="sxs-lookup"><span data-stu-id="76513-284">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="76513-285">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="76513-285">airDropBlocked</span></span>|<span data-ttu-id="76513-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-286">Boolean</span></span>|<span data-ttu-id="76513-287">指示是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="76513-287">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="76513-288">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="76513-288">passwordBlockModification</span></span>|<span data-ttu-id="76513-289">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-289">Boolean</span></span>|<span data-ttu-id="76513-290">指示是否允许修改密码。</span><span class="sxs-lookup"><span data-stu-id="76513-290">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="76513-291">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="76513-291">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="76513-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-292">Boolean</span></span>|<span data-ttu-id="76513-293">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="76513-293">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="76513-294">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="76513-294">passwordBlockAutoFill</span></span>|<span data-ttu-id="76513-295">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-295">Boolean</span></span>|<span data-ttu-id="76513-296">指示是否阻止自动填充密码功能。</span><span class="sxs-lookup"><span data-stu-id="76513-296">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="76513-297">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="76513-297">passwordBlockProximityRequests</span></span>|<span data-ttu-id="76513-298">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-298">Boolean</span></span>|<span data-ttu-id="76513-299">指示是否阻止来自附近设备的请求密码。</span><span class="sxs-lookup"><span data-stu-id="76513-299">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="76513-300">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="76513-300">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="76513-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-301">Boolean</span></span>|<span data-ttu-id="76513-302">指示是否阻止使用 AirDrop 密码功能的共享密码。</span><span class="sxs-lookup"><span data-stu-id="76513-302">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="76513-303">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="76513-303">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="76513-304">Int32</span><span class="sxs-lookup"><span data-stu-id="76513-304">Int32</span></span>|<span data-ttu-id="76513-305">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="76513-305">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="76513-306">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="76513-306">Valid values 0 to 90</span></span>|
|<span data-ttu-id="76513-307">updateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="76513-307">updateDelayPolicy</span></span>|[<span data-ttu-id="76513-308">macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="76513-308">macOSSoftwareUpdateDelayPolicy</span></span>](../resources/intune-deviceconfig-macossoftwareupdatedelaypolicy.md)|<span data-ttu-id="76513-309">确定是否延迟 macOS 的 OS 和/或应用更新。</span><span class="sxs-lookup"><span data-stu-id="76513-309">Determines whether to delay OS and/or app updates for macOS.</span></span> <span data-ttu-id="76513-310">可取值为：`none`、`delayOSUpdateVisibility`、`delayAppUpdateVisibility`。</span><span class="sxs-lookup"><span data-stu-id="76513-310">Possible values are: `none`, `delayOSUpdateVisibility`, `delayAppUpdateVisibility`.</span></span>|
|<span data-ttu-id="76513-311">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="76513-311">contentCachingBlocked</span></span>|<span data-ttu-id="76513-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-312">Boolean</span></span>|<span data-ttu-id="76513-313">指示是否允许内容缓存。</span><span class="sxs-lookup"><span data-stu-id="76513-313">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="76513-314">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="76513-314">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="76513-315">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-315">Boolean</span></span>|<span data-ttu-id="76513-316">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="76513-316">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="76513-317">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="76513-317">screenCaptureBlocked</span></span>|<span data-ttu-id="76513-318">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-318">Boolean</span></span>|<span data-ttu-id="76513-319">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="76513-319">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="76513-320">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="76513-320">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="76513-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-321">Boolean</span></span>|<span data-ttu-id="76513-322">指示是否允许教室应用进行远程屏幕观察。</span><span class="sxs-lookup"><span data-stu-id="76513-322">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="76513-323">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="76513-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="76513-324">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="76513-324">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="76513-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-325">Boolean</span></span>|<span data-ttu-id="76513-326">指示是否自动向教师授予对教室应用程序中的托管课程的权限，以便在不提示的情况下查看学生的屏幕。</span><span class="sxs-lookup"><span data-stu-id="76513-326">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="76513-327">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="76513-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="76513-328">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="76513-328">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="76513-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-329">Boolean</span></span>|<span data-ttu-id="76513-330">指示是否在不提示学生的情况下自动向教师的请求授予权限。</span><span class="sxs-lookup"><span data-stu-id="76513-330">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="76513-331">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="76513-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="76513-332">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="76513-332">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="76513-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-333">Boolean</span></span>|<span data-ttu-id="76513-334">指示在非托管课程中通过课堂注册的学生是否需要在尝试离开本课程时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="76513-334">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="76513-335">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="76513-335">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="76513-336">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="76513-336">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="76513-337">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-337">Boolean</span></span>|<span data-ttu-id="76513-338">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="76513-338">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="76513-339">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="76513-339">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="76513-340">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="76513-340">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="76513-341">Boolean</span><span class="sxs-lookup"><span data-stu-id="76513-341">Boolean</span></span>|<span data-ttu-id="76513-342">指示是否阻止用户继续在另一台 iOS 或 MacOS 设备上的 MacOS 设备上启动的工作， (MacOS 10.15 或更高版本) 。</span><span class="sxs-lookup"><span data-stu-id="76513-342">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="76513-343">privacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="76513-343">privacyAccessControls</span></span>|<span data-ttu-id="76513-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="76513-344">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="76513-345">隐私首选项策略控制的列表。</span><span class="sxs-lookup"><span data-stu-id="76513-345">List of privacy preference policy controls.</span></span> <span data-ttu-id="76513-346">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="76513-346">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="76513-347">响应</span><span class="sxs-lookup"><span data-stu-id="76513-347">Response</span></span>
<span data-ttu-id="76513-348">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="76513-348">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76513-349">示例</span><span class="sxs-lookup"><span data-stu-id="76513-349">Example</span></span>

### <a name="request"></a><span data-ttu-id="76513-350">请求</span><span class="sxs-lookup"><span data-stu-id="76513-350">Request</span></span>
<span data-ttu-id="76513-351">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="76513-351">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4640

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="76513-352">响应</span><span class="sxs-lookup"><span data-stu-id="76513-352">Response</span></span>
<span data-ttu-id="76513-p127">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76513-p127">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4812

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
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
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true,
  "passwordMaximumAttemptCount": 11,
  "passwordMinutesUntilFailedLoginReset": 4,
  "keychainBlockCloudSync": true,
  "airPrintBlocked": true,
  "airPrintForceTrustedTLS": true,
  "airPrintBlockiBeaconDiscovery": true,
  "safariBlockAutofill": true,
  "cameraBlocked": true,
  "iTunesBlockMusicService": true,
  "spotlightBlockInternetResults": true,
  "keyboardBlockDictation": true,
  "definitionLookupBlocked": true,
  "appleWatchBlockAutoUnlock": true,
  "iTunesBlockFileSharing": true,
  "iCloudBlockDocumentSync": true,
  "iCloudBlockMail": true,
  "iCloudBlockAddressBook": true,
  "iCloudBlockCalendar": true,
  "iCloudBlockReminders": true,
  "iCloudBlockBookmarks": true,
  "iCloudBlockNotes": true,
  "airDropBlocked": true,
  "passwordBlockModification": true,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockAutoFill": true,
  "passwordBlockProximityRequests": true,
  "passwordBlockAirDropSharing": true,
  "softwareUpdatesEnforcedDelayInDays": 2,
  "updateDelayPolicy": "delayOSUpdateVisibility",
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true,
  "privacyAccessControls": [
    {
      "@odata.type": "microsoft.graph.macOSPrivacyAccessControlItem",
      "displayName": "Display Name value",
      "identifier": "Identifier value",
      "identifierType": "path",
      "codeRequirement": "Code Requirement value",
      "staticCodeValidation": true,
      "blockCamera": true,
      "blockMicrophone": true,
      "blockScreenCapture": true,
      "blockListenEvent": true,
      "speechRecognition": "enabled",
      "accessibility": "enabled",
      "addressBook": "enabled",
      "calendar": "enabled",
      "reminders": "enabled",
      "photos": "enabled",
      "mediaLibrary": "enabled",
      "fileProviderPresence": "enabled",
      "systemPolicyAllFiles": "enabled",
      "systemPolicySystemAdminFiles": "enabled",
      "systemPolicyDesktopFolder": "enabled",
      "systemPolicyDocumentsFolder": "enabled",
      "systemPolicyDownloadsFolder": "enabled",
      "systemPolicyNetworkVolumes": "enabled",
      "systemPolicyRemovableVolumes": "enabled",
      "postEvent": "enabled",
      "appleEventsAllowedReceivers": [
        {
          "@odata.type": "microsoft.graph.macOSAppleEventReceiver",
          "codeRequirement": "Code Requirement value",
          "identifier": "Identifier value",
          "identifierType": "path",
          "allowed": true
        }
      ]
    }
  ]
}
```




