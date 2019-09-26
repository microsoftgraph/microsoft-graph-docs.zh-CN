---
title: 更新 macOSGeneralDeviceConfiguration
description: 更新 macOSGeneralDeviceConfiguration 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d8062cea749ff314ec2089be5cfd4efccac22ac7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37181999"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="e61d4-103">更新 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e61d4-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e61d4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e61d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e61d4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e61d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e61d4-106">更新 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e61d4-106">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e61d4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e61d4-107">Prerequisites</span></span>
<span data-ttu-id="e61d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e61d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e61d4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e61d4-110">Permission type</span></span>|<span data-ttu-id="e61d4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e61d4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e61d4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e61d4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e61d4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e61d4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e61d4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e61d4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e61d4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e61d4-115">Not supported.</span></span>|
|<span data-ttu-id="e61d4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e61d4-116">Application</span></span>|<span data-ttu-id="e61d4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e61d4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e61d4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e61d4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e61d4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e61d4-119">Request headers</span></span>
|<span data-ttu-id="e61d4-120">标头</span><span class="sxs-lookup"><span data-stu-id="e61d4-120">Header</span></span>|<span data-ttu-id="e61d4-121">值</span><span class="sxs-lookup"><span data-stu-id="e61d4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e61d4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e61d4-122">Authorization</span></span>|<span data-ttu-id="e61d4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e61d4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e61d4-124">接受</span><span class="sxs-lookup"><span data-stu-id="e61d4-124">Accept</span></span>|<span data-ttu-id="e61d4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e61d4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e61d4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e61d4-126">Request body</span></span>
<span data-ttu-id="e61d4-127">在请求正文中，提供 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e61d4-127">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="e61d4-128">下表显示创建 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e61d4-128">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="e61d4-129">属性</span><span class="sxs-lookup"><span data-stu-id="e61d4-129">Property</span></span>|<span data-ttu-id="e61d4-130">类型</span><span class="sxs-lookup"><span data-stu-id="e61d4-130">Type</span></span>|<span data-ttu-id="e61d4-131">说明</span><span class="sxs-lookup"><span data-stu-id="e61d4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e61d4-132">id</span><span class="sxs-lookup"><span data-stu-id="e61d4-132">id</span></span>|<span data-ttu-id="e61d4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e61d4-133">String</span></span>|<span data-ttu-id="e61d4-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e61d4-134">Key of the entity.</span></span> <span data-ttu-id="e61d4-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e61d4-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e61d4-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e61d4-137">DateTimeOffset</span></span>|<span data-ttu-id="e61d4-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e61d4-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e61d4-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e61d4-140">roleScopeTagIds</span></span>|<span data-ttu-id="e61d4-141">String collection</span><span class="sxs-lookup"><span data-stu-id="e61d4-141">String collection</span></span>|<span data-ttu-id="e61d4-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e61d4-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e61d4-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e61d4-144">supportsScopeTags</span></span>|<span data-ttu-id="e61d4-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-145">Boolean</span></span>|<span data-ttu-id="e61d4-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e61d4-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e61d4-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e61d4-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e61d4-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e61d4-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e61d4-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e61d4-149">This property is read-only.</span></span> <span data-ttu-id="e61d4-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e61d4-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e61d4-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e61d4-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e61d4-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e61d4-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e61d4-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e61d4-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e61d4-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e61d4-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e61d4-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e61d4-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e61d4-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e61d4-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e61d4-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e61d4-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e61d4-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e61d4-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e61d4-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e61d4-163">createdDateTime</span></span>|<span data-ttu-id="e61d4-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e61d4-164">DateTimeOffset</span></span>|<span data-ttu-id="e61d4-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e61d4-165">DateTime the object was created.</span></span> <span data-ttu-id="e61d4-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-167">说明</span><span class="sxs-lookup"><span data-stu-id="e61d4-167">description</span></span>|<span data-ttu-id="e61d4-168">String</span><span class="sxs-lookup"><span data-stu-id="e61d4-168">String</span></span>|<span data-ttu-id="e61d4-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e61d4-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e61d4-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-171">displayName</span><span class="sxs-lookup"><span data-stu-id="e61d4-171">displayName</span></span>|<span data-ttu-id="e61d4-172">String</span><span class="sxs-lookup"><span data-stu-id="e61d4-172">String</span></span>|<span data-ttu-id="e61d4-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e61d4-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e61d4-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-175">version</span><span class="sxs-lookup"><span data-stu-id="e61d4-175">version</span></span>|<span data-ttu-id="e61d4-176">Int32</span><span class="sxs-lookup"><span data-stu-id="e61d4-176">Int32</span></span>|<span data-ttu-id="e61d4-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e61d4-177">Version of the device configuration.</span></span> <span data-ttu-id="e61d4-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e61d4-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e61d4-179">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="e61d4-179">compliantAppsList</span></span>|<span data-ttu-id="e61d4-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e61d4-180">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="e61d4-181">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="e61d4-181">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="e61d4-182">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="e61d4-182">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="e61d4-183">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="e61d4-183">compliantAppListType</span></span>|[<span data-ttu-id="e61d4-184">appListType</span><span class="sxs-lookup"><span data-stu-id="e61d4-184">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="e61d4-185">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="e61d4-185">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="e61d4-186">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="e61d4-186">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="e61d4-187">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="e61d4-187">emailInDomainSuffixes</span></span>|<span data-ttu-id="e61d4-188">String 集合</span><span class="sxs-lookup"><span data-stu-id="e61d4-188">String collection</span></span>|<span data-ttu-id="e61d4-189">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="e61d4-189">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="e61d4-190">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="e61d4-190">passwordBlockSimple</span></span>|<span data-ttu-id="e61d4-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-191">Boolean</span></span>|<span data-ttu-id="e61d4-192">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="e61d4-192">Block simple passwords.</span></span>|
|<span data-ttu-id="e61d4-193">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e61d4-193">passwordExpirationDays</span></span>|<span data-ttu-id="e61d4-194">Int32</span><span class="sxs-lookup"><span data-stu-id="e61d4-194">Int32</span></span>|<span data-ttu-id="e61d4-195">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="e61d4-195">Number of days before the password expires.</span></span>|
|<span data-ttu-id="e61d4-196">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="e61d4-196">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="e61d4-197">Int32</span><span class="sxs-lookup"><span data-stu-id="e61d4-197">Int32</span></span>|<span data-ttu-id="e61d4-198">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="e61d4-198">Number of character sets a password must contain.</span></span> <span data-ttu-id="e61d4-199">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="e61d4-199">Valid values 0 to 4</span></span>|
|<span data-ttu-id="e61d4-200">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e61d4-200">passwordMinimumLength</span></span>|<span data-ttu-id="e61d4-201">Int32</span><span class="sxs-lookup"><span data-stu-id="e61d4-201">Int32</span></span>|<span data-ttu-id="e61d4-202">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="e61d4-202">Minimum length of passwords.</span></span>|
|<span data-ttu-id="e61d4-203">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="e61d4-203">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="e61d4-204">Int32</span><span class="sxs-lookup"><span data-stu-id="e61d4-204">Int32</span></span>|<span data-ttu-id="e61d4-205">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e61d4-205">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="e61d4-206">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e61d4-206">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e61d4-207">Int32</span><span class="sxs-lookup"><span data-stu-id="e61d4-207">Int32</span></span>|<span data-ttu-id="e61d4-208">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="e61d4-208">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="e61d4-209">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e61d4-209">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e61d4-210">Int32</span><span class="sxs-lookup"><span data-stu-id="e61d4-210">Int32</span></span>|<span data-ttu-id="e61d4-211">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="e61d4-211">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="e61d4-212">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e61d4-212">passwordRequiredType</span></span>|[<span data-ttu-id="e61d4-213">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e61d4-213">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="e61d4-214">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="e61d4-214">Type of password that is required.</span></span> <span data-ttu-id="e61d4-215">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="e61d4-215">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="e61d4-216">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="e61d4-216">passwordRequired</span></span>|<span data-ttu-id="e61d4-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-217">Boolean</span></span>|<span data-ttu-id="e61d4-218">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="e61d4-218">Whether or not to require a password.</span></span>|
|<span data-ttu-id="e61d4-219">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="e61d4-219">keychainBlockCloudSync</span></span>|<span data-ttu-id="e61d4-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-220">Boolean</span></span>|<span data-ttu-id="e61d4-221">指示是否阻止 iCloud 密钥链同步（macOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e61d4-221">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="e61d4-222">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="e61d4-222">airPrintBlocked</span></span>|<span data-ttu-id="e61d4-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-223">Boolean</span></span>|<span data-ttu-id="e61d4-224">指示是否阻止 AirPrint （macOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e61d4-224">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="e61d4-225">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="e61d4-225">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="e61d4-226">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-226">Boolean</span></span>|<span data-ttu-id="e61d4-227">指示 TLS 打印通信是否需要受信任的证书（macOS 10.13 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e61d4-227">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="e61d4-228">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="e61d4-228">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="e61d4-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-229">Boolean</span></span>|<span data-ttu-id="e61d4-230">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="e61d4-230">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="e61d4-231">这可防止来自网络流量的虚假 AirPrint 蓝牙信号（macOS 10.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="e61d4-231">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="e61d4-232">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="e61d4-232">safariBlockAutofill</span></span>|<span data-ttu-id="e61d4-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-233">Boolean</span></span>|<span data-ttu-id="e61d4-234">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="e61d4-234">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="e61d4-235">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="e61d4-235">cameraBlocked</span></span>|<span data-ttu-id="e61d4-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-236">Boolean</span></span>|<span data-ttu-id="e61d4-237">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="e61d4-237">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="e61d4-238">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="e61d4-238">iTunesBlockMusicService</span></span>|<span data-ttu-id="e61d4-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-239">Boolean</span></span>|<span data-ttu-id="e61d4-240">指示是否阻止音乐服务并将音乐应用还原到经典模式。</span><span class="sxs-lookup"><span data-stu-id="e61d4-240">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="e61d4-241">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="e61d4-241">spotlightBlockInternetResults</span></span>|<span data-ttu-id="e61d4-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-242">Boolean</span></span>|<span data-ttu-id="e61d4-243">指示是否阻止聚光灯从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="e61d4-243">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="e61d4-244">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="e61d4-244">keyboardBlockDictation</span></span>|<span data-ttu-id="e61d4-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-245">Boolean</span></span>|<span data-ttu-id="e61d4-246">指示是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="e61d4-246">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="e61d4-247">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="e61d4-247">definitionLookupBlocked</span></span>|<span data-ttu-id="e61d4-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-248">Boolean</span></span>|<span data-ttu-id="e61d4-249">指示是否阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="e61d4-249">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="e61d4-250">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="e61d4-250">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="e61d4-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-251">Boolean</span></span>|<span data-ttu-id="e61d4-252">指示是否阻止用户使用 Apple Watch 解锁其 Mac。</span><span class="sxs-lookup"><span data-stu-id="e61d4-252">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="e61d4-253">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="e61d4-253">iTunesBlockFileSharing</span></span>|<span data-ttu-id="e61d4-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-254">Boolean</span></span>|<span data-ttu-id="e61d4-255">指示是否阻止使用 iTunes 传输文件。</span><span class="sxs-lookup"><span data-stu-id="e61d4-255">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="e61d4-256">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="e61d4-256">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="e61d4-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-257">Boolean</span></span>|<span data-ttu-id="e61d4-258">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="e61d4-258">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="e61d4-259">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="e61d4-259">iCloudBlockMail</span></span>|<span data-ttu-id="e61d4-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-260">Boolean</span></span>|<span data-ttu-id="e61d4-261">指示是否阻止 iCloud 同步邮件。</span><span class="sxs-lookup"><span data-stu-id="e61d4-261">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="e61d4-262">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="e61d4-262">iCloudBlockAddressBook</span></span>|<span data-ttu-id="e61d4-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-263">Boolean</span></span>|<span data-ttu-id="e61d4-264">指示是否阻止 iCloud 同步联系人。</span><span class="sxs-lookup"><span data-stu-id="e61d4-264">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="e61d4-265">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="e61d4-265">iCloudBlockCalendar</span></span>|<span data-ttu-id="e61d4-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-266">Boolean</span></span>|<span data-ttu-id="e61d4-267">指示是否阻止 iCloud 同步日历。</span><span class="sxs-lookup"><span data-stu-id="e61d4-267">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="e61d4-268">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="e61d4-268">iCloudBlockReminders</span></span>|<span data-ttu-id="e61d4-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-269">Boolean</span></span>|<span data-ttu-id="e61d4-270">指示是否阻止 iCloud 同步提醒。</span><span class="sxs-lookup"><span data-stu-id="e61d4-270">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="e61d4-271">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="e61d4-271">iCloudBlockBookmarks</span></span>|<span data-ttu-id="e61d4-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-272">Boolean</span></span>|<span data-ttu-id="e61d4-273">指示是否阻止 iCloud 同步书签。</span><span class="sxs-lookup"><span data-stu-id="e61d4-273">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="e61d4-274">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="e61d4-274">iCloudBlockNotes</span></span>|<span data-ttu-id="e61d4-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-275">Boolean</span></span>|<span data-ttu-id="e61d4-276">指示是否阻止 iCloud 同步笔记。</span><span class="sxs-lookup"><span data-stu-id="e61d4-276">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="e61d4-277">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="e61d4-277">airDropBlocked</span></span>|<span data-ttu-id="e61d4-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-278">Boolean</span></span>|<span data-ttu-id="e61d4-279">指示是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="e61d4-279">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="e61d4-280">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="e61d4-280">passwordBlockModification</span></span>|<span data-ttu-id="e61d4-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-281">Boolean</span></span>|<span data-ttu-id="e61d4-282">指示是否允许修改密码。</span><span class="sxs-lookup"><span data-stu-id="e61d4-282">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="e61d4-283">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e61d4-283">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e61d4-284">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-284">Boolean</span></span>|<span data-ttu-id="e61d4-285">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="e61d4-285">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e61d4-286">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="e61d4-286">passwordBlockAutoFill</span></span>|<span data-ttu-id="e61d4-287">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-287">Boolean</span></span>|<span data-ttu-id="e61d4-288">指示是否阻止自动填充密码功能。</span><span class="sxs-lookup"><span data-stu-id="e61d4-288">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="e61d4-289">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="e61d4-289">passwordBlockProximityRequests</span></span>|<span data-ttu-id="e61d4-290">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-290">Boolean</span></span>|<span data-ttu-id="e61d4-291">指示是否阻止来自附近设备的请求密码。</span><span class="sxs-lookup"><span data-stu-id="e61d4-291">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="e61d4-292">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="e61d4-292">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="e61d4-293">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-293">Boolean</span></span>|<span data-ttu-id="e61d4-294">指示是否阻止使用 AirDrop 密码功能的共享密码。</span><span class="sxs-lookup"><span data-stu-id="e61d4-294">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="e61d4-295">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="e61d4-295">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="e61d4-296">Int32</span><span class="sxs-lookup"><span data-stu-id="e61d4-296">Int32</span></span>|<span data-ttu-id="e61d4-297">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="e61d4-297">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="e61d4-298">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="e61d4-298">Valid values 0 to 90</span></span>|
|<span data-ttu-id="e61d4-299">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="e61d4-299">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="e61d4-300">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-300">Boolean</span></span>|<span data-ttu-id="e61d4-301">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="e61d4-301">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="e61d4-302">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="e61d4-302">contentCachingBlocked</span></span>|<span data-ttu-id="e61d4-303">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-303">Boolean</span></span>|<span data-ttu-id="e61d4-304">指示是否允许内容缓存。</span><span class="sxs-lookup"><span data-stu-id="e61d4-304">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="e61d4-305">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="e61d4-305">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="e61d4-306">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-306">Boolean</span></span>|<span data-ttu-id="e61d4-307">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="e61d4-307">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="e61d4-308">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="e61d4-308">screenCaptureBlocked</span></span>|<span data-ttu-id="e61d4-309">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-309">Boolean</span></span>|<span data-ttu-id="e61d4-310">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="e61d4-310">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="e61d4-311">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e61d4-311">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="e61d4-312">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-312">Boolean</span></span>|<span data-ttu-id="e61d4-313">指示是否允许教室应用进行远程屏幕观察。</span><span class="sxs-lookup"><span data-stu-id="e61d4-313">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="e61d4-314">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e61d4-314">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e61d4-315">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="e61d4-315">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="e61d4-316">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-316">Boolean</span></span>|<span data-ttu-id="e61d4-317">指示是否自动向教师授予对教室应用程序中的托管课程的权限，以便在不提示的情况下查看学生的屏幕。</span><span class="sxs-lookup"><span data-stu-id="e61d4-317">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="e61d4-318">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e61d4-318">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e61d4-319">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="e61d4-319">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="e61d4-320">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-320">Boolean</span></span>|<span data-ttu-id="e61d4-321">指示是否在不提示学生的情况下自动向教师的请求授予权限。</span><span class="sxs-lookup"><span data-stu-id="e61d4-321">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="e61d4-322">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e61d4-322">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e61d4-323">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="e61d4-323">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="e61d4-324">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-324">Boolean</span></span>|<span data-ttu-id="e61d4-325">指示在非托管课程中通过课堂注册的学生是否需要在尝试离开本课程时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="e61d4-325">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="e61d4-326">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e61d4-326">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e61d4-327">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="e61d4-327">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="e61d4-328">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-328">Boolean</span></span>|<span data-ttu-id="e61d4-329">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="e61d4-329">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="e61d4-330">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="e61d4-330">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="e61d4-331">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="e61d4-331">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="e61d4-332">Boolean</span><span class="sxs-lookup"><span data-stu-id="e61d4-332">Boolean</span></span>|<span data-ttu-id="e61d4-333">指示是否阻止用户继续在另一台 iOS 或 MacOS 设备（MacOS 10.15 或更高版本）上的 MacOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="e61d4-333">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|



## <a name="response"></a><span data-ttu-id="e61d4-334">响应</span><span class="sxs-lookup"><span data-stu-id="e61d4-334">Response</span></span>
<span data-ttu-id="e61d4-335">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e61d4-335">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e61d4-336">示例</span><span class="sxs-lookup"><span data-stu-id="e61d4-336">Example</span></span>

### <a name="request"></a><span data-ttu-id="e61d4-337">请求</span><span class="sxs-lookup"><span data-stu-id="e61d4-337">Request</span></span>
<span data-ttu-id="e61d4-338">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e61d4-338">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e61d4-339">响应</span><span class="sxs-lookup"><span data-stu-id="e61d4-339">Response</span></span>
<span data-ttu-id="e61d4-p124">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e61d4-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




