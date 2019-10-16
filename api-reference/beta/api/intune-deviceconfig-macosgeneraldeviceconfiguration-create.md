---
title: 创建 macOSGeneralDeviceConfiguration
description: 创建新的 macOSGeneralDeviceConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 183013fb06d1fef856ab4f2d5c717d627bab0ddd
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37533586"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="e11e3-103">创建 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e11e3-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e11e3-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e11e3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e11e3-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e11e3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e11e3-106">创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e11e3-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e11e3-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e11e3-107">Prerequisites</span></span>
<span data-ttu-id="e11e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e11e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e11e3-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e11e3-110">Permission type</span></span>|<span data-ttu-id="e11e3-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e11e3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e11e3-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e11e3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e11e3-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e11e3-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e11e3-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e11e3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e11e3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e11e3-115">Not supported.</span></span>|
|<span data-ttu-id="e11e3-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e11e3-116">Application</span></span>|<span data-ttu-id="e11e3-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e11e3-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e11e3-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e11e3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e11e3-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e11e3-119">Request headers</span></span>
|<span data-ttu-id="e11e3-120">标头</span><span class="sxs-lookup"><span data-stu-id="e11e3-120">Header</span></span>|<span data-ttu-id="e11e3-121">值</span><span class="sxs-lookup"><span data-stu-id="e11e3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e11e3-122">授权</span><span class="sxs-lookup"><span data-stu-id="e11e3-122">Authorization</span></span>|<span data-ttu-id="e11e3-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e11e3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e11e3-124">接受</span><span class="sxs-lookup"><span data-stu-id="e11e3-124">Accept</span></span>|<span data-ttu-id="e11e3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e11e3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e11e3-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e11e3-126">Request body</span></span>
<span data-ttu-id="e11e3-127">在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e11e3-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="e11e3-128">下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e11e3-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="e11e3-129">属性</span><span class="sxs-lookup"><span data-stu-id="e11e3-129">Property</span></span>|<span data-ttu-id="e11e3-130">类型</span><span class="sxs-lookup"><span data-stu-id="e11e3-130">Type</span></span>|<span data-ttu-id="e11e3-131">说明</span><span class="sxs-lookup"><span data-stu-id="e11e3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e11e3-132">id</span><span class="sxs-lookup"><span data-stu-id="e11e3-132">id</span></span>|<span data-ttu-id="e11e3-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e11e3-133">String</span></span>|<span data-ttu-id="e11e3-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e11e3-134">Key of the entity.</span></span> <span data-ttu-id="e11e3-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e11e3-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e11e3-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e11e3-137">DateTimeOffset</span></span>|<span data-ttu-id="e11e3-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e11e3-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e11e3-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e11e3-140">roleScopeTagIds</span></span>|<span data-ttu-id="e11e3-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="e11e3-141">String collection</span></span>|<span data-ttu-id="e11e3-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e11e3-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e11e3-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e11e3-144">supportsScopeTags</span></span>|<span data-ttu-id="e11e3-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-145">Boolean</span></span>|<span data-ttu-id="e11e3-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e11e3-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e11e3-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e11e3-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e11e3-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e11e3-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e11e3-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e11e3-149">This property is read-only.</span></span> <span data-ttu-id="e11e3-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e11e3-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e11e3-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e11e3-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e11e3-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e11e3-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e11e3-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e11e3-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e11e3-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e11e3-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e11e3-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e11e3-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e11e3-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e11e3-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e11e3-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e11e3-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e11e3-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e11e3-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e11e3-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e11e3-163">createdDateTime</span></span>|<span data-ttu-id="e11e3-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e11e3-164">DateTimeOffset</span></span>|<span data-ttu-id="e11e3-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e11e3-165">DateTime the object was created.</span></span> <span data-ttu-id="e11e3-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-167">说明</span><span class="sxs-lookup"><span data-stu-id="e11e3-167">description</span></span>|<span data-ttu-id="e11e3-168">String</span><span class="sxs-lookup"><span data-stu-id="e11e3-168">String</span></span>|<span data-ttu-id="e11e3-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e11e3-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e11e3-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e11e3-171">displayName</span></span>|<span data-ttu-id="e11e3-172">String</span><span class="sxs-lookup"><span data-stu-id="e11e3-172">String</span></span>|<span data-ttu-id="e11e3-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e11e3-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e11e3-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-175">version</span><span class="sxs-lookup"><span data-stu-id="e11e3-175">version</span></span>|<span data-ttu-id="e11e3-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e3-176">Int32</span></span>|<span data-ttu-id="e11e3-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e11e3-177">Version of the device configuration.</span></span> <span data-ttu-id="e11e3-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e11e3-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e11e3-179">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="e11e3-179">compliantAppsList</span></span>|<span data-ttu-id="e11e3-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e11e3-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e11e3-181">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="e11e3-181">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="e11e3-182">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="e11e3-182">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e11e3-183">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="e11e3-183">compliantAppListType</span></span>|[<span data-ttu-id="e11e3-184">appListType</span><span class="sxs-lookup"><span data-stu-id="e11e3-184">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="e11e3-185">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="e11e3-185">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="e11e3-186">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="e11e3-186">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="e11e3-187">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="e11e3-187">emailInDomainSuffixes</span></span>|<span data-ttu-id="e11e3-188">String 集合</span><span class="sxs-lookup"><span data-stu-id="e11e3-188">String collection</span></span>|<span data-ttu-id="e11e3-189">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="e11e3-189">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="e11e3-190">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e11e3-190">passwordBlockSimple</span></span>|<span data-ttu-id="e11e3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-191">Boolean</span></span>|<span data-ttu-id="e11e3-192">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="e11e3-192">Block simple passwords.</span></span>|
|<span data-ttu-id="e11e3-193">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e11e3-193">passwordExpirationDays</span></span>|<span data-ttu-id="e11e3-194">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e3-194">Int32</span></span>|<span data-ttu-id="e11e3-195">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e11e3-195">Number of days before the password expires.</span></span>|
|<span data-ttu-id="e11e3-196">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e11e3-196">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e11e3-197">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e3-197">Int32</span></span>|<span data-ttu-id="e11e3-198">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="e11e3-198">Number of character sets a password must contain.</span></span> <span data-ttu-id="e11e3-199">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="e11e3-199">Valid values 0 to 4</span></span>|
|<span data-ttu-id="e11e3-200">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e11e3-200">passwordMinimumLength</span></span>|<span data-ttu-id="e11e3-201">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e3-201">Int32</span></span>|<span data-ttu-id="e11e3-202">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e11e3-202">Minimum length of passwords.</span></span>|
|<span data-ttu-id="e11e3-203">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e11e3-203">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e11e3-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e3-204">Int32</span></span>|<span data-ttu-id="e11e3-205">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e11e3-205">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="e11e3-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e11e3-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e11e3-207">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e3-207">Int32</span></span>|<span data-ttu-id="e11e3-208">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e11e3-208">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="e11e3-209">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e11e3-209">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e11e3-210">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e3-210">Int32</span></span>|<span data-ttu-id="e11e3-211">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e11e3-211">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="e11e3-212">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e11e3-212">passwordRequiredType</span></span>|[<span data-ttu-id="e11e3-213">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e11e3-213">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e11e3-214">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e11e3-214">Type of password that is required.</span></span> <span data-ttu-id="e11e3-215">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="e11e3-215">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e11e3-216">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e11e3-216">passwordRequired</span></span>|<span data-ttu-id="e11e3-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-217">Boolean</span></span>|<span data-ttu-id="e11e3-218">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="e11e3-218">Whether or not to require a password.</span></span>|
|<span data-ttu-id="e11e3-219">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="e11e3-219">keychainBlockCloudSync</span></span>|<span data-ttu-id="e11e3-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-220">Boolean</span></span>|<span data-ttu-id="e11e3-221">指示是否阻止 iCloud 密钥链同步（macOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e11e3-221">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="e11e3-222">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="e11e3-222">airPrintBlocked</span></span>|<span data-ttu-id="e11e3-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-223">Boolean</span></span>|<span data-ttu-id="e11e3-224">指示是否阻止 AirPrint （macOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e11e3-224">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="e11e3-225">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="e11e3-225">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="e11e3-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-226">Boolean</span></span>|<span data-ttu-id="e11e3-227">指示 TLS 打印通信是否需要受信任的证书（macOS 10.13 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e11e3-227">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="e11e3-228">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="e11e3-228">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="e11e3-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-229">Boolean</span></span>|<span data-ttu-id="e11e3-230">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="e11e3-230">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="e11e3-231">这可防止来自网络流量的虚假 AirPrint 蓝牙信号（macOS 10.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e11e3-231">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="e11e3-232">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="e11e3-232">safariBlockAutofill</span></span>|<span data-ttu-id="e11e3-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-233">Boolean</span></span>|<span data-ttu-id="e11e3-234">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="e11e3-234">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="e11e3-235">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e11e3-235">cameraBlocked</span></span>|<span data-ttu-id="e11e3-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-236">Boolean</span></span>|<span data-ttu-id="e11e3-237">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="e11e3-237">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="e11e3-238">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="e11e3-238">iTunesBlockMusicService</span></span>|<span data-ttu-id="e11e3-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-239">Boolean</span></span>|<span data-ttu-id="e11e3-240">指示是否阻止音乐服务并将音乐应用还原到经典模式。</span><span class="sxs-lookup"><span data-stu-id="e11e3-240">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="e11e3-241">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="e11e3-241">spotlightBlockInternetResults</span></span>|<span data-ttu-id="e11e3-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-242">Boolean</span></span>|<span data-ttu-id="e11e3-243">指示是否阻止聚光灯从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="e11e3-243">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="e11e3-244">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="e11e3-244">keyboardBlockDictation</span></span>|<span data-ttu-id="e11e3-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-245">Boolean</span></span>|<span data-ttu-id="e11e3-246">指示是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="e11e3-246">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="e11e3-247">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="e11e3-247">definitionLookupBlocked</span></span>|<span data-ttu-id="e11e3-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-248">Boolean</span></span>|<span data-ttu-id="e11e3-249">指示是否阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="e11e3-249">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="e11e3-250">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="e11e3-250">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="e11e3-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-251">Boolean</span></span>|<span data-ttu-id="e11e3-252">指示是否阻止用户使用 Apple Watch 解锁其 Mac。</span><span class="sxs-lookup"><span data-stu-id="e11e3-252">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="e11e3-253">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="e11e3-253">iTunesBlockFileSharing</span></span>|<span data-ttu-id="e11e3-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-254">Boolean</span></span>|<span data-ttu-id="e11e3-255">指示是否阻止使用 iTunes 传输文件。</span><span class="sxs-lookup"><span data-stu-id="e11e3-255">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="e11e3-256">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="e11e3-256">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="e11e3-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-257">Boolean</span></span>|<span data-ttu-id="e11e3-258">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="e11e3-258">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="e11e3-259">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="e11e3-259">iCloudBlockMail</span></span>|<span data-ttu-id="e11e3-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-260">Boolean</span></span>|<span data-ttu-id="e11e3-261">指示是否阻止 iCloud 同步邮件。</span><span class="sxs-lookup"><span data-stu-id="e11e3-261">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="e11e3-262">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="e11e3-262">iCloudBlockAddressBook</span></span>|<span data-ttu-id="e11e3-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-263">Boolean</span></span>|<span data-ttu-id="e11e3-264">指示是否阻止 iCloud 同步联系人。</span><span class="sxs-lookup"><span data-stu-id="e11e3-264">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="e11e3-265">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="e11e3-265">iCloudBlockCalendar</span></span>|<span data-ttu-id="e11e3-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-266">Boolean</span></span>|<span data-ttu-id="e11e3-267">指示是否阻止 iCloud 同步日历。</span><span class="sxs-lookup"><span data-stu-id="e11e3-267">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="e11e3-268">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="e11e3-268">iCloudBlockReminders</span></span>|<span data-ttu-id="e11e3-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-269">Boolean</span></span>|<span data-ttu-id="e11e3-270">指示是否阻止 iCloud 同步提醒。</span><span class="sxs-lookup"><span data-stu-id="e11e3-270">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="e11e3-271">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="e11e3-271">iCloudBlockBookmarks</span></span>|<span data-ttu-id="e11e3-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-272">Boolean</span></span>|<span data-ttu-id="e11e3-273">指示是否阻止 iCloud 同步书签。</span><span class="sxs-lookup"><span data-stu-id="e11e3-273">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="e11e3-274">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="e11e3-274">iCloudBlockNotes</span></span>|<span data-ttu-id="e11e3-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-275">Boolean</span></span>|<span data-ttu-id="e11e3-276">指示是否阻止 iCloud 同步笔记。</span><span class="sxs-lookup"><span data-stu-id="e11e3-276">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="e11e3-277">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="e11e3-277">airDropBlocked</span></span>|<span data-ttu-id="e11e3-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-278">Boolean</span></span>|<span data-ttu-id="e11e3-279">指示是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="e11e3-279">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="e11e3-280">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="e11e3-280">passwordBlockModification</span></span>|<span data-ttu-id="e11e3-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-281">Boolean</span></span>|<span data-ttu-id="e11e3-282">指示是否允许修改密码。</span><span class="sxs-lookup"><span data-stu-id="e11e3-282">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="e11e3-283">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e11e3-283">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e11e3-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-284">Boolean</span></span>|<span data-ttu-id="e11e3-285">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="e11e3-285">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e11e3-286">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="e11e3-286">passwordBlockAutoFill</span></span>|<span data-ttu-id="e11e3-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-287">Boolean</span></span>|<span data-ttu-id="e11e3-288">指示是否阻止自动填充密码功能。</span><span class="sxs-lookup"><span data-stu-id="e11e3-288">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="e11e3-289">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="e11e3-289">passwordBlockProximityRequests</span></span>|<span data-ttu-id="e11e3-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-290">Boolean</span></span>|<span data-ttu-id="e11e3-291">指示是否阻止来自附近设备的请求密码。</span><span class="sxs-lookup"><span data-stu-id="e11e3-291">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="e11e3-292">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="e11e3-292">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="e11e3-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-293">Boolean</span></span>|<span data-ttu-id="e11e3-294">指示是否阻止使用 AirDrop 密码功能的共享密码。</span><span class="sxs-lookup"><span data-stu-id="e11e3-294">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="e11e3-295">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="e11e3-295">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="e11e3-296">Int32</span><span class="sxs-lookup"><span data-stu-id="e11e3-296">Int32</span></span>|<span data-ttu-id="e11e3-297">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="e11e3-297">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="e11e3-298">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="e11e3-298">Valid values 0 to 90</span></span>|
|<span data-ttu-id="e11e3-299">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="e11e3-299">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="e11e3-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-300">Boolean</span></span>|<span data-ttu-id="e11e3-301">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="e11e3-301">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e11e3-302">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="e11e3-302">contentCachingBlocked</span></span>|<span data-ttu-id="e11e3-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-303">Boolean</span></span>|<span data-ttu-id="e11e3-304">指示是否允许内容缓存。</span><span class="sxs-lookup"><span data-stu-id="e11e3-304">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="e11e3-305">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="e11e3-305">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="e11e3-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-306">Boolean</span></span>|<span data-ttu-id="e11e3-307">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="e11e3-307">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="e11e3-308">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e11e3-308">screenCaptureBlocked</span></span>|<span data-ttu-id="e11e3-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-309">Boolean</span></span>|<span data-ttu-id="e11e3-310">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="e11e3-310">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="e11e3-311">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e11e3-311">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="e11e3-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-312">Boolean</span></span>|<span data-ttu-id="e11e3-313">指示是否允许教室应用进行远程屏幕观察。</span><span class="sxs-lookup"><span data-stu-id="e11e3-313">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="e11e3-314">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e11e3-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e11e3-315">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e11e3-315">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="e11e3-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-316">Boolean</span></span>|<span data-ttu-id="e11e3-317">指示是否自动向教师授予对教室应用程序中的托管课程的权限，以便在不提示的情况下查看学生的屏幕。</span><span class="sxs-lookup"><span data-stu-id="e11e3-317">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="e11e3-318">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e11e3-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e11e3-319">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="e11e3-319">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="e11e3-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-320">Boolean</span></span>|<span data-ttu-id="e11e3-321">指示是否在不提示学生的情况下自动向教师的请求授予权限。</span><span class="sxs-lookup"><span data-stu-id="e11e3-321">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="e11e3-322">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e11e3-322">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e11e3-323">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="e11e3-323">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="e11e3-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-324">Boolean</span></span>|<span data-ttu-id="e11e3-325">指示在非托管课程中通过课堂注册的学生是否需要在尝试离开本课程时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="e11e3-325">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="e11e3-326">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e11e3-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e11e3-327">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="e11e3-327">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="e11e3-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-328">Boolean</span></span>|<span data-ttu-id="e11e3-329">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="e11e3-329">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="e11e3-330">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e11e3-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e11e3-331">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="e11e3-331">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="e11e3-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="e11e3-332">Boolean</span></span>|<span data-ttu-id="e11e3-333">指示是否阻止用户继续在另一台 iOS 或 MacOS 设备（MacOS 10.15 或更高版本）上的 MacOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="e11e3-333">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="e11e3-334">响应</span><span class="sxs-lookup"><span data-stu-id="e11e3-334">Response</span></span>
<span data-ttu-id="e11e3-335">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e11e3-335">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e11e3-336">示例</span><span class="sxs-lookup"><span data-stu-id="e11e3-336">Example</span></span>

### <a name="request"></a><span data-ttu-id="e11e3-337">请求</span><span class="sxs-lookup"><span data-stu-id="e11e3-337">Request</span></span>
<span data-ttu-id="e11e3-338">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e11e3-338">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="e11e3-339">响应</span><span class="sxs-lookup"><span data-stu-id="e11e3-339">Response</span></span>
<span data-ttu-id="e11e3-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e11e3-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






