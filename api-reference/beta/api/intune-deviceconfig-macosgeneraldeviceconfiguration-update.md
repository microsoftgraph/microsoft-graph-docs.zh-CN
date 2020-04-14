---
title: 更新 macOSGeneralDeviceConfiguration
description: 更新 macOSGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 697b952af6227114ecd967b1597cac674688e208
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43432589"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="e0753-103">更新 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0753-103">Update macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="e0753-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e0753-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e0753-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e0753-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e0753-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e0753-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e0753-107">更新 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0753-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e0753-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0753-108">Prerequisites</span></span>
<span data-ttu-id="e0753-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e0753-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0753-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0753-111">Permission type</span></span>|<span data-ttu-id="e0753-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0753-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0753-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0753-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e0753-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0753-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0753-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0753-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0753-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0753-116">Not supported.</span></span>|
|<span data-ttu-id="e0753-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0753-117">Application</span></span>|<span data-ttu-id="e0753-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0753-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0753-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0753-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e0753-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0753-120">Request headers</span></span>
|<span data-ttu-id="e0753-121">标头</span><span class="sxs-lookup"><span data-stu-id="e0753-121">Header</span></span>|<span data-ttu-id="e0753-122">值</span><span class="sxs-lookup"><span data-stu-id="e0753-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0753-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0753-123">Authorization</span></span>|<span data-ttu-id="e0753-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0753-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0753-125">接受</span><span class="sxs-lookup"><span data-stu-id="e0753-125">Accept</span></span>|<span data-ttu-id="e0753-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e0753-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0753-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0753-127">Request body</span></span>
<span data-ttu-id="e0753-128">在请求正文中，提供 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0753-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="e0753-129">下表显示创建 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0753-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="e0753-130">属性</span><span class="sxs-lookup"><span data-stu-id="e0753-130">Property</span></span>|<span data-ttu-id="e0753-131">类型</span><span class="sxs-lookup"><span data-stu-id="e0753-131">Type</span></span>|<span data-ttu-id="e0753-132">说明</span><span class="sxs-lookup"><span data-stu-id="e0753-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0753-133">id</span><span class="sxs-lookup"><span data-stu-id="e0753-133">id</span></span>|<span data-ttu-id="e0753-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e0753-134">String</span></span>|<span data-ttu-id="e0753-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0753-135">Key of the entity.</span></span> <span data-ttu-id="e0753-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0753-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e0753-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0753-138">DateTimeOffset</span></span>|<span data-ttu-id="e0753-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e0753-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e0753-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e0753-141">roleScopeTagIds</span></span>|<span data-ttu-id="e0753-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="e0753-142">String collection</span></span>|<span data-ttu-id="e0753-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e0753-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e0753-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e0753-145">supportsScopeTags</span></span>|<span data-ttu-id="e0753-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-146">Boolean</span></span>|<span data-ttu-id="e0753-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e0753-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e0753-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e0753-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e0753-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e0753-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e0753-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e0753-150">This property is read-only.</span></span> <span data-ttu-id="e0753-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e0753-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e0753-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e0753-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e0753-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e0753-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e0753-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e0753-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e0753-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e0753-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e0753-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e0753-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e0753-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e0753-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e0753-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e0753-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e0753-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e0753-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e0753-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0753-164">createdDateTime</span></span>|<span data-ttu-id="e0753-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0753-165">DateTimeOffset</span></span>|<span data-ttu-id="e0753-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e0753-166">DateTime the object was created.</span></span> <span data-ttu-id="e0753-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-168">description</span><span class="sxs-lookup"><span data-stu-id="e0753-168">description</span></span>|<span data-ttu-id="e0753-169">String</span><span class="sxs-lookup"><span data-stu-id="e0753-169">String</span></span>|<span data-ttu-id="e0753-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e0753-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0753-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e0753-172">displayName</span></span>|<span data-ttu-id="e0753-173">String</span><span class="sxs-lookup"><span data-stu-id="e0753-173">String</span></span>|<span data-ttu-id="e0753-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e0753-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0753-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-176">version</span><span class="sxs-lookup"><span data-stu-id="e0753-176">version</span></span>|<span data-ttu-id="e0753-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e0753-177">Int32</span></span>|<span data-ttu-id="e0753-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e0753-178">Version of the device configuration.</span></span> <span data-ttu-id="e0753-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0753-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0753-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="e0753-180">compliantAppsList</span></span>|<span data-ttu-id="e0753-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e0753-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e0753-182">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="e0753-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="e0753-183">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="e0753-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e0753-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="e0753-184">compliantAppListType</span></span>|[<span data-ttu-id="e0753-185">appListType</span><span class="sxs-lookup"><span data-stu-id="e0753-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="e0753-186">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="e0753-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="e0753-187">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="e0753-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="e0753-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="e0753-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="e0753-189">String 集合</span><span class="sxs-lookup"><span data-stu-id="e0753-189">String collection</span></span>|<span data-ttu-id="e0753-190">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="e0753-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="e0753-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e0753-191">passwordBlockSimple</span></span>|<span data-ttu-id="e0753-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-192">Boolean</span></span>|<span data-ttu-id="e0753-193">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="e0753-193">Block simple passwords.</span></span>|
|<span data-ttu-id="e0753-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e0753-194">passwordExpirationDays</span></span>|<span data-ttu-id="e0753-195">Int32</span><span class="sxs-lookup"><span data-stu-id="e0753-195">Int32</span></span>|<span data-ttu-id="e0753-196">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e0753-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="e0753-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e0753-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e0753-198">Int32</span><span class="sxs-lookup"><span data-stu-id="e0753-198">Int32</span></span>|<span data-ttu-id="e0753-199">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="e0753-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="e0753-200">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="e0753-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="e0753-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e0753-201">passwordMinimumLength</span></span>|<span data-ttu-id="e0753-202">Int32</span><span class="sxs-lookup"><span data-stu-id="e0753-202">Int32</span></span>|<span data-ttu-id="e0753-203">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e0753-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="e0753-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e0753-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e0753-205">Int32</span><span class="sxs-lookup"><span data-stu-id="e0753-205">Int32</span></span>|<span data-ttu-id="e0753-206">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e0753-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="e0753-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e0753-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e0753-208">Int32</span><span class="sxs-lookup"><span data-stu-id="e0753-208">Int32</span></span>|<span data-ttu-id="e0753-209">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e0753-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="e0753-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e0753-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e0753-211">Int32</span><span class="sxs-lookup"><span data-stu-id="e0753-211">Int32</span></span>|<span data-ttu-id="e0753-212">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e0753-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="e0753-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e0753-213">passwordRequiredType</span></span>|[<span data-ttu-id="e0753-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e0753-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e0753-215">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e0753-215">Type of password that is required.</span></span> <span data-ttu-id="e0753-216">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="e0753-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e0753-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e0753-217">passwordRequired</span></span>|<span data-ttu-id="e0753-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-218">Boolean</span></span>|<span data-ttu-id="e0753-219">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="e0753-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="e0753-220">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="e0753-220">keychainBlockCloudSync</span></span>|<span data-ttu-id="e0753-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-221">Boolean</span></span>|<span data-ttu-id="e0753-222">指示是否阻止 iCloud 密钥链同步（macOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e0753-222">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="e0753-223">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="e0753-223">airPrintBlocked</span></span>|<span data-ttu-id="e0753-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-224">Boolean</span></span>|<span data-ttu-id="e0753-225">指示是否阻止 AirPrint （macOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e0753-225">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="e0753-226">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="e0753-226">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="e0753-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-227">Boolean</span></span>|<span data-ttu-id="e0753-228">指示 TLS 打印通信是否需要受信任的证书（macOS 10.13 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e0753-228">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="e0753-229">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="e0753-229">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="e0753-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-230">Boolean</span></span>|<span data-ttu-id="e0753-231">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="e0753-231">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="e0753-232">这可防止来自网络流量的虚假 AirPrint 蓝牙信号（macOS 10.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e0753-232">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="e0753-233">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="e0753-233">safariBlockAutofill</span></span>|<span data-ttu-id="e0753-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-234">Boolean</span></span>|<span data-ttu-id="e0753-235">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="e0753-235">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="e0753-236">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e0753-236">cameraBlocked</span></span>|<span data-ttu-id="e0753-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-237">Boolean</span></span>|<span data-ttu-id="e0753-238">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="e0753-238">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="e0753-239">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="e0753-239">iTunesBlockMusicService</span></span>|<span data-ttu-id="e0753-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-240">Boolean</span></span>|<span data-ttu-id="e0753-241">指示是否阻止音乐服务并将音乐应用还原到经典模式。</span><span class="sxs-lookup"><span data-stu-id="e0753-241">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="e0753-242">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="e0753-242">spotlightBlockInternetResults</span></span>|<span data-ttu-id="e0753-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-243">Boolean</span></span>|<span data-ttu-id="e0753-244">指示是否阻止聚光灯从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="e0753-244">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="e0753-245">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="e0753-245">keyboardBlockDictation</span></span>|<span data-ttu-id="e0753-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-246">Boolean</span></span>|<span data-ttu-id="e0753-247">指示是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="e0753-247">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="e0753-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="e0753-248">definitionLookupBlocked</span></span>|<span data-ttu-id="e0753-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-249">Boolean</span></span>|<span data-ttu-id="e0753-250">指示是否阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="e0753-250">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="e0753-251">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="e0753-251">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="e0753-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-252">Boolean</span></span>|<span data-ttu-id="e0753-253">指示是否阻止用户使用 Apple Watch 解锁其 Mac。</span><span class="sxs-lookup"><span data-stu-id="e0753-253">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="e0753-254">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="e0753-254">iTunesBlockFileSharing</span></span>|<span data-ttu-id="e0753-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-255">Boolean</span></span>|<span data-ttu-id="e0753-256">指示是否阻止使用 iTunes 传输文件。</span><span class="sxs-lookup"><span data-stu-id="e0753-256">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="e0753-257">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="e0753-257">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="e0753-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-258">Boolean</span></span>|<span data-ttu-id="e0753-259">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="e0753-259">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="e0753-260">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="e0753-260">iCloudBlockMail</span></span>|<span data-ttu-id="e0753-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-261">Boolean</span></span>|<span data-ttu-id="e0753-262">指示是否阻止 iCloud 同步邮件。</span><span class="sxs-lookup"><span data-stu-id="e0753-262">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="e0753-263">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="e0753-263">iCloudBlockAddressBook</span></span>|<span data-ttu-id="e0753-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-264">Boolean</span></span>|<span data-ttu-id="e0753-265">指示是否阻止 iCloud 同步联系人。</span><span class="sxs-lookup"><span data-stu-id="e0753-265">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="e0753-266">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="e0753-266">iCloudBlockCalendar</span></span>|<span data-ttu-id="e0753-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-267">Boolean</span></span>|<span data-ttu-id="e0753-268">指示是否阻止 iCloud 同步日历。</span><span class="sxs-lookup"><span data-stu-id="e0753-268">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="e0753-269">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="e0753-269">iCloudBlockReminders</span></span>|<span data-ttu-id="e0753-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-270">Boolean</span></span>|<span data-ttu-id="e0753-271">指示是否阻止 iCloud 同步提醒。</span><span class="sxs-lookup"><span data-stu-id="e0753-271">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="e0753-272">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="e0753-272">iCloudBlockBookmarks</span></span>|<span data-ttu-id="e0753-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-273">Boolean</span></span>|<span data-ttu-id="e0753-274">指示是否阻止 iCloud 同步书签。</span><span class="sxs-lookup"><span data-stu-id="e0753-274">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="e0753-275">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="e0753-275">iCloudBlockNotes</span></span>|<span data-ttu-id="e0753-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-276">Boolean</span></span>|<span data-ttu-id="e0753-277">指示是否阻止 iCloud 同步笔记。</span><span class="sxs-lookup"><span data-stu-id="e0753-277">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="e0753-278">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="e0753-278">airDropBlocked</span></span>|<span data-ttu-id="e0753-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-279">Boolean</span></span>|<span data-ttu-id="e0753-280">指示是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="e0753-280">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="e0753-281">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="e0753-281">passwordBlockModification</span></span>|<span data-ttu-id="e0753-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-282">Boolean</span></span>|<span data-ttu-id="e0753-283">指示是否允许修改密码。</span><span class="sxs-lookup"><span data-stu-id="e0753-283">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="e0753-284">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e0753-284">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e0753-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-285">Boolean</span></span>|<span data-ttu-id="e0753-286">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="e0753-286">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e0753-287">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="e0753-287">passwordBlockAutoFill</span></span>|<span data-ttu-id="e0753-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-288">Boolean</span></span>|<span data-ttu-id="e0753-289">指示是否阻止自动填充密码功能。</span><span class="sxs-lookup"><span data-stu-id="e0753-289">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="e0753-290">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="e0753-290">passwordBlockProximityRequests</span></span>|<span data-ttu-id="e0753-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-291">Boolean</span></span>|<span data-ttu-id="e0753-292">指示是否阻止来自附近设备的请求密码。</span><span class="sxs-lookup"><span data-stu-id="e0753-292">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="e0753-293">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="e0753-293">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="e0753-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-294">Boolean</span></span>|<span data-ttu-id="e0753-295">指示是否阻止使用 AirDrop 密码功能的共享密码。</span><span class="sxs-lookup"><span data-stu-id="e0753-295">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="e0753-296">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="e0753-296">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="e0753-297">Int32</span><span class="sxs-lookup"><span data-stu-id="e0753-297">Int32</span></span>|<span data-ttu-id="e0753-298">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="e0753-298">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="e0753-299">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="e0753-299">Valid values 0 to 90</span></span>|
|<span data-ttu-id="e0753-300">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="e0753-300">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="e0753-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-301">Boolean</span></span>|<span data-ttu-id="e0753-302">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="e0753-302">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e0753-303">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="e0753-303">contentCachingBlocked</span></span>|<span data-ttu-id="e0753-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-304">Boolean</span></span>|<span data-ttu-id="e0753-305">指示是否允许内容缓存。</span><span class="sxs-lookup"><span data-stu-id="e0753-305">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="e0753-306">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="e0753-306">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="e0753-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-307">Boolean</span></span>|<span data-ttu-id="e0753-308">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="e0753-308">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="e0753-309">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e0753-309">screenCaptureBlocked</span></span>|<span data-ttu-id="e0753-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-310">Boolean</span></span>|<span data-ttu-id="e0753-311">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="e0753-311">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="e0753-312">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e0753-312">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="e0753-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-313">Boolean</span></span>|<span data-ttu-id="e0753-314">指示是否允许教室应用进行远程屏幕观察。</span><span class="sxs-lookup"><span data-stu-id="e0753-314">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="e0753-315">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e0753-315">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e0753-316">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e0753-316">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="e0753-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-317">Boolean</span></span>|<span data-ttu-id="e0753-318">指示是否自动向教师授予对教室应用程序中的托管课程的权限，以便在不提示的情况下查看学生的屏幕。</span><span class="sxs-lookup"><span data-stu-id="e0753-318">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="e0753-319">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e0753-319">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e0753-320">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="e0753-320">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="e0753-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-321">Boolean</span></span>|<span data-ttu-id="e0753-322">指示是否在不提示学生的情况下自动向教师的请求授予权限。</span><span class="sxs-lookup"><span data-stu-id="e0753-322">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="e0753-323">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e0753-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e0753-324">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="e0753-324">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="e0753-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-325">Boolean</span></span>|<span data-ttu-id="e0753-326">指示在非托管课程中通过课堂注册的学生是否需要在尝试离开本课程时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="e0753-326">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="e0753-327">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e0753-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e0753-328">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="e0753-328">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="e0753-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-329">Boolean</span></span>|<span data-ttu-id="e0753-330">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="e0753-330">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="e0753-331">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e0753-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e0753-332">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="e0753-332">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="e0753-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="e0753-333">Boolean</span></span>|<span data-ttu-id="e0753-334">指示是否阻止用户继续在另一台 iOS 或 MacOS 设备（MacOS 10.15 或更高版本）上的 MacOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="e0753-334">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="e0753-335">响应</span><span class="sxs-lookup"><span data-stu-id="e0753-335">Response</span></span>
<span data-ttu-id="e0753-336">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0753-336">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0753-337">示例</span><span class="sxs-lookup"><span data-stu-id="e0753-337">Example</span></span>

### <a name="request"></a><span data-ttu-id="e0753-338">请求</span><span class="sxs-lookup"><span data-stu-id="e0753-338">Request</span></span>
<span data-ttu-id="e0753-339">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0753-339">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 3146

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
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```

### <a name="response"></a><span data-ttu-id="e0753-340">响应</span><span class="sxs-lookup"><span data-stu-id="e0753-340">Response</span></span>
<span data-ttu-id="e0753-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0753-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 3318

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
  "softwareUpdatesForceDelayed": true,
  "contentCachingBlocked": true,
  "iCloudBlockPhotoLibrary": true,
  "screenCaptureBlocked": true,
  "classroomAppBlockRemoteScreenObservation": true,
  "classroomAppForceUnpromptedScreenObservation": true,
  "classroomForceAutomaticallyJoinClasses": true,
  "classroomForceRequestPermissionToLeaveClasses": true,
  "classroomForceUnpromptedAppAndDeviceLock": true,
  "iCloudBlockActivityContinuation": true
}
```



