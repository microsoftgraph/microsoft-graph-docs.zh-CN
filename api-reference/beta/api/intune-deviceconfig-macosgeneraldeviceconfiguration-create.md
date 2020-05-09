---
title: 创建 macOSGeneralDeviceConfiguration
description: 创建新的 macOSGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eb4f472594a57f3380c554b2187d99aa5d94f622
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177966"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="d241d-103">创建 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="d241d-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="d241d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d241d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d241d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d241d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d241d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d241d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d241d-107">创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d241d-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d241d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d241d-108">Prerequisites</span></span>
<span data-ttu-id="d241d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d241d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d241d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d241d-111">Permission type</span></span>|<span data-ttu-id="d241d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d241d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d241d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d241d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d241d-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d241d-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d241d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d241d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d241d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d241d-116">Not supported.</span></span>|
|<span data-ttu-id="d241d-117">Application</span><span class="sxs-lookup"><span data-stu-id="d241d-117">Application</span></span>|<span data-ttu-id="d241d-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d241d-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d241d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d241d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d241d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d241d-120">Request headers</span></span>
|<span data-ttu-id="d241d-121">标头</span><span class="sxs-lookup"><span data-stu-id="d241d-121">Header</span></span>|<span data-ttu-id="d241d-122">值</span><span class="sxs-lookup"><span data-stu-id="d241d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d241d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d241d-123">Authorization</span></span>|<span data-ttu-id="d241d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d241d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d241d-125">接受</span><span class="sxs-lookup"><span data-stu-id="d241d-125">Accept</span></span>|<span data-ttu-id="d241d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d241d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d241d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d241d-127">Request body</span></span>
<span data-ttu-id="d241d-128">在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d241d-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="d241d-129">下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d241d-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="d241d-130">属性</span><span class="sxs-lookup"><span data-stu-id="d241d-130">Property</span></span>|<span data-ttu-id="d241d-131">类型</span><span class="sxs-lookup"><span data-stu-id="d241d-131">Type</span></span>|<span data-ttu-id="d241d-132">说明</span><span class="sxs-lookup"><span data-stu-id="d241d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d241d-133">id</span><span class="sxs-lookup"><span data-stu-id="d241d-133">id</span></span>|<span data-ttu-id="d241d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="d241d-134">String</span></span>|<span data-ttu-id="d241d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d241d-135">Key of the entity.</span></span> <span data-ttu-id="d241d-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d241d-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d241d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d241d-138">DateTimeOffset</span></span>|<span data-ttu-id="d241d-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d241d-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d241d-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d241d-141">roleScopeTagIds</span></span>|<span data-ttu-id="d241d-142">字符串集合</span><span class="sxs-lookup"><span data-stu-id="d241d-142">String collection</span></span>|<span data-ttu-id="d241d-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="d241d-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d241d-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d241d-145">supportsScopeTags</span></span>|<span data-ttu-id="d241d-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-146">Boolean</span></span>|<span data-ttu-id="d241d-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="d241d-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d241d-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="d241d-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d241d-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="d241d-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d241d-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d241d-150">This property is read-only.</span></span> <span data-ttu-id="d241d-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d241d-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="d241d-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="d241d-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="d241d-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="d241d-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="d241d-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d241d-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="d241d-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="d241d-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="d241d-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d241d-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="d241d-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d241d-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="d241d-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="d241d-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="d241d-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="d241d-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="d241d-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d241d-164">createdDateTime</span></span>|<span data-ttu-id="d241d-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d241d-165">DateTimeOffset</span></span>|<span data-ttu-id="d241d-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d241d-166">DateTime the object was created.</span></span> <span data-ttu-id="d241d-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-168">说明</span><span class="sxs-lookup"><span data-stu-id="d241d-168">description</span></span>|<span data-ttu-id="d241d-169">String</span><span class="sxs-lookup"><span data-stu-id="d241d-169">String</span></span>|<span data-ttu-id="d241d-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d241d-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d241d-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-172">displayName</span><span class="sxs-lookup"><span data-stu-id="d241d-172">displayName</span></span>|<span data-ttu-id="d241d-173">String</span><span class="sxs-lookup"><span data-stu-id="d241d-173">String</span></span>|<span data-ttu-id="d241d-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d241d-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d241d-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-176">version</span><span class="sxs-lookup"><span data-stu-id="d241d-176">version</span></span>|<span data-ttu-id="d241d-177">Int32</span><span class="sxs-lookup"><span data-stu-id="d241d-177">Int32</span></span>|<span data-ttu-id="d241d-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d241d-178">Version of the device configuration.</span></span> <span data-ttu-id="d241d-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d241d-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d241d-180">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="d241d-180">compliantAppsList</span></span>|<span data-ttu-id="d241d-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d241d-181">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="d241d-182">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="d241d-182">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="d241d-183">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="d241d-183">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="d241d-184">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="d241d-184">compliantAppListType</span></span>|[<span data-ttu-id="d241d-185">appListType</span><span class="sxs-lookup"><span data-stu-id="d241d-185">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="d241d-186">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="d241d-186">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="d241d-187">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="d241d-187">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="d241d-188">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="d241d-188">emailInDomainSuffixes</span></span>|<span data-ttu-id="d241d-189">String 集合</span><span class="sxs-lookup"><span data-stu-id="d241d-189">String collection</span></span>|<span data-ttu-id="d241d-190">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="d241d-190">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="d241d-191">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="d241d-191">passwordBlockSimple</span></span>|<span data-ttu-id="d241d-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-192">Boolean</span></span>|<span data-ttu-id="d241d-193">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="d241d-193">Block simple passwords.</span></span>|
|<span data-ttu-id="d241d-194">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="d241d-194">passwordExpirationDays</span></span>|<span data-ttu-id="d241d-195">Int32</span><span class="sxs-lookup"><span data-stu-id="d241d-195">Int32</span></span>|<span data-ttu-id="d241d-196">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="d241d-196">Number of days before the password expires.</span></span>|
|<span data-ttu-id="d241d-197">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="d241d-197">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="d241d-198">Int32</span><span class="sxs-lookup"><span data-stu-id="d241d-198">Int32</span></span>|<span data-ttu-id="d241d-199">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="d241d-199">Number of character sets a password must contain.</span></span> <span data-ttu-id="d241d-200">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="d241d-200">Valid values 0 to 4</span></span>|
|<span data-ttu-id="d241d-201">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="d241d-201">passwordMinimumLength</span></span>|<span data-ttu-id="d241d-202">Int32</span><span class="sxs-lookup"><span data-stu-id="d241d-202">Int32</span></span>|<span data-ttu-id="d241d-203">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="d241d-203">Minimum length of passwords.</span></span>|
|<span data-ttu-id="d241d-204">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="d241d-204">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="d241d-205">Int32</span><span class="sxs-lookup"><span data-stu-id="d241d-205">Int32</span></span>|<span data-ttu-id="d241d-206">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="d241d-206">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="d241d-207">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="d241d-207">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="d241d-208">Int32</span><span class="sxs-lookup"><span data-stu-id="d241d-208">Int32</span></span>|<span data-ttu-id="d241d-209">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="d241d-209">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="d241d-210">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="d241d-210">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="d241d-211">Int32</span><span class="sxs-lookup"><span data-stu-id="d241d-211">Int32</span></span>|<span data-ttu-id="d241d-212">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="d241d-212">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="d241d-213">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="d241d-213">passwordRequiredType</span></span>|[<span data-ttu-id="d241d-214">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="d241d-214">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="d241d-215">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="d241d-215">Type of password that is required.</span></span> <span data-ttu-id="d241d-216">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="d241d-216">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="d241d-217">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="d241d-217">passwordRequired</span></span>|<span data-ttu-id="d241d-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-218">Boolean</span></span>|<span data-ttu-id="d241d-219">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="d241d-219">Whether or not to require a password.</span></span>|
|<span data-ttu-id="d241d-220">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="d241d-220">keychainBlockCloudSync</span></span>|<span data-ttu-id="d241d-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-221">Boolean</span></span>|<span data-ttu-id="d241d-222">指示是否阻止 iCloud 密钥链同步（macOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d241d-222">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="d241d-223">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="d241d-223">airPrintBlocked</span></span>|<span data-ttu-id="d241d-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-224">Boolean</span></span>|<span data-ttu-id="d241d-225">指示是否阻止 AirPrint （macOS 10.12 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d241d-225">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="d241d-226">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="d241d-226">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="d241d-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-227">Boolean</span></span>|<span data-ttu-id="d241d-228">指示 TLS 打印通信是否需要受信任的证书（macOS 10.13 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d241d-228">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="d241d-229">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="d241d-229">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="d241d-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-230">Boolean</span></span>|<span data-ttu-id="d241d-231">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="d241d-231">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="d241d-232">这可防止来自网络流量的虚假 AirPrint 蓝牙信号（macOS 10.3 及更高版本）。</span><span class="sxs-lookup"><span data-stu-id="d241d-232">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="d241d-233">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="d241d-233">safariBlockAutofill</span></span>|<span data-ttu-id="d241d-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-234">Boolean</span></span>|<span data-ttu-id="d241d-235">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="d241d-235">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="d241d-236">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="d241d-236">cameraBlocked</span></span>|<span data-ttu-id="d241d-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-237">Boolean</span></span>|<span data-ttu-id="d241d-238">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="d241d-238">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="d241d-239">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="d241d-239">iTunesBlockMusicService</span></span>|<span data-ttu-id="d241d-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-240">Boolean</span></span>|<span data-ttu-id="d241d-241">指示是否阻止音乐服务并将音乐应用还原到经典模式。</span><span class="sxs-lookup"><span data-stu-id="d241d-241">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="d241d-242">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="d241d-242">spotlightBlockInternetResults</span></span>|<span data-ttu-id="d241d-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-243">Boolean</span></span>|<span data-ttu-id="d241d-244">指示是否阻止聚光灯从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="d241d-244">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="d241d-245">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="d241d-245">keyboardBlockDictation</span></span>|<span data-ttu-id="d241d-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-246">Boolean</span></span>|<span data-ttu-id="d241d-247">指示是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="d241d-247">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="d241d-248">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="d241d-248">definitionLookupBlocked</span></span>|<span data-ttu-id="d241d-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-249">Boolean</span></span>|<span data-ttu-id="d241d-250">指示是否阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="d241d-250">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="d241d-251">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="d241d-251">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="d241d-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-252">Boolean</span></span>|<span data-ttu-id="d241d-253">指示是否阻止用户使用 Apple Watch 解锁其 Mac。</span><span class="sxs-lookup"><span data-stu-id="d241d-253">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="d241d-254">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="d241d-254">iTunesBlockFileSharing</span></span>|<span data-ttu-id="d241d-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-255">Boolean</span></span>|<span data-ttu-id="d241d-256">指示是否阻止使用 iTunes 传输文件。</span><span class="sxs-lookup"><span data-stu-id="d241d-256">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="d241d-257">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="d241d-257">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="d241d-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-258">Boolean</span></span>|<span data-ttu-id="d241d-259">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="d241d-259">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="d241d-260">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="d241d-260">iCloudBlockMail</span></span>|<span data-ttu-id="d241d-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-261">Boolean</span></span>|<span data-ttu-id="d241d-262">指示是否阻止 iCloud 同步邮件。</span><span class="sxs-lookup"><span data-stu-id="d241d-262">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="d241d-263">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="d241d-263">iCloudBlockAddressBook</span></span>|<span data-ttu-id="d241d-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-264">Boolean</span></span>|<span data-ttu-id="d241d-265">指示是否阻止 iCloud 同步联系人。</span><span class="sxs-lookup"><span data-stu-id="d241d-265">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="d241d-266">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="d241d-266">iCloudBlockCalendar</span></span>|<span data-ttu-id="d241d-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-267">Boolean</span></span>|<span data-ttu-id="d241d-268">指示是否阻止 iCloud 同步日历。</span><span class="sxs-lookup"><span data-stu-id="d241d-268">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="d241d-269">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="d241d-269">iCloudBlockReminders</span></span>|<span data-ttu-id="d241d-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-270">Boolean</span></span>|<span data-ttu-id="d241d-271">指示是否阻止 iCloud 同步提醒。</span><span class="sxs-lookup"><span data-stu-id="d241d-271">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="d241d-272">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="d241d-272">iCloudBlockBookmarks</span></span>|<span data-ttu-id="d241d-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-273">Boolean</span></span>|<span data-ttu-id="d241d-274">指示是否阻止 iCloud 同步书签。</span><span class="sxs-lookup"><span data-stu-id="d241d-274">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="d241d-275">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="d241d-275">iCloudBlockNotes</span></span>|<span data-ttu-id="d241d-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-276">Boolean</span></span>|<span data-ttu-id="d241d-277">指示是否阻止 iCloud 同步笔记。</span><span class="sxs-lookup"><span data-stu-id="d241d-277">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="d241d-278">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="d241d-278">airDropBlocked</span></span>|<span data-ttu-id="d241d-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-279">Boolean</span></span>|<span data-ttu-id="d241d-280">指示是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="d241d-280">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="d241d-281">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="d241d-281">passwordBlockModification</span></span>|<span data-ttu-id="d241d-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-282">Boolean</span></span>|<span data-ttu-id="d241d-283">指示是否允许修改密码。</span><span class="sxs-lookup"><span data-stu-id="d241d-283">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="d241d-284">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="d241d-284">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="d241d-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-285">Boolean</span></span>|<span data-ttu-id="d241d-286">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="d241d-286">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="d241d-287">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="d241d-287">passwordBlockAutoFill</span></span>|<span data-ttu-id="d241d-288">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-288">Boolean</span></span>|<span data-ttu-id="d241d-289">指示是否阻止自动填充密码功能。</span><span class="sxs-lookup"><span data-stu-id="d241d-289">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="d241d-290">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="d241d-290">passwordBlockProximityRequests</span></span>|<span data-ttu-id="d241d-291">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-291">Boolean</span></span>|<span data-ttu-id="d241d-292">指示是否阻止来自附近设备的请求密码。</span><span class="sxs-lookup"><span data-stu-id="d241d-292">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="d241d-293">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="d241d-293">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="d241d-294">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-294">Boolean</span></span>|<span data-ttu-id="d241d-295">指示是否阻止使用 AirDrop 密码功能的共享密码。</span><span class="sxs-lookup"><span data-stu-id="d241d-295">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="d241d-296">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="d241d-296">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="d241d-297">Int32</span><span class="sxs-lookup"><span data-stu-id="d241d-297">Int32</span></span>|<span data-ttu-id="d241d-298">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="d241d-298">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="d241d-299">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="d241d-299">Valid values 0 to 90</span></span>|
|<span data-ttu-id="d241d-300">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="d241d-300">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="d241d-301">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-301">Boolean</span></span>|<span data-ttu-id="d241d-302">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="d241d-302">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="d241d-303">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="d241d-303">contentCachingBlocked</span></span>|<span data-ttu-id="d241d-304">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-304">Boolean</span></span>|<span data-ttu-id="d241d-305">指示是否允许内容缓存。</span><span class="sxs-lookup"><span data-stu-id="d241d-305">Indicates whether or not to allow content caching.</span></span>|
|<span data-ttu-id="d241d-306">iCloudBlockPhotoLibrary</span><span class="sxs-lookup"><span data-stu-id="d241d-306">iCloudBlockPhotoLibrary</span></span>|<span data-ttu-id="d241d-307">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-307">Boolean</span></span>|<span data-ttu-id="d241d-308">指示是否阻止 iCloud 照片库。</span><span class="sxs-lookup"><span data-stu-id="d241d-308">Indicates whether or not to block iCloud Photo Library.</span></span>|
|<span data-ttu-id="d241d-309">screenCaptureBlocked</span><span class="sxs-lookup"><span data-stu-id="d241d-309">screenCaptureBlocked</span></span>|<span data-ttu-id="d241d-310">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-310">Boolean</span></span>|<span data-ttu-id="d241d-311">指示是否阻止用户进行屏幕截图。</span><span class="sxs-lookup"><span data-stu-id="d241d-311">Indicates whether or not to block the user from taking Screenshots.</span></span>|
|<span data-ttu-id="d241d-312">classroomAppBlockRemoteScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d241d-312">classroomAppBlockRemoteScreenObservation</span></span>|<span data-ttu-id="d241d-313">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-313">Boolean</span></span>|<span data-ttu-id="d241d-314">指示是否允许教室应用进行远程屏幕观察。</span><span class="sxs-lookup"><span data-stu-id="d241d-314">Indicates whether or not to allow remote screen observation by Classroom app.</span></span> <span data-ttu-id="d241d-315">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="d241d-315">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="d241d-316">classroomAppForceUnpromptedScreenObservation</span><span class="sxs-lookup"><span data-stu-id="d241d-316">classroomAppForceUnpromptedScreenObservation</span></span>|<span data-ttu-id="d241d-317">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-317">Boolean</span></span>|<span data-ttu-id="d241d-318">指示是否自动向教师授予对教室应用程序中的托管课程的权限，以便在不提示的情况下查看学生的屏幕。</span><span class="sxs-lookup"><span data-stu-id="d241d-318">Indicates whether or not to automatically give permission to the teacher of a managed course on the Classroom app to view a student's screen without prompting.</span></span> <span data-ttu-id="d241d-319">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="d241d-319">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="d241d-320">classroomForceAutomaticallyJoinClasses</span><span class="sxs-lookup"><span data-stu-id="d241d-320">classroomForceAutomaticallyJoinClasses</span></span>|<span data-ttu-id="d241d-321">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-321">Boolean</span></span>|<span data-ttu-id="d241d-322">指示是否在不提示学生的情况下自动向教师的请求授予权限。</span><span class="sxs-lookup"><span data-stu-id="d241d-322">Indicates whether or not to automatically give permission to the teacher's requests, without prompting the student.</span></span> <span data-ttu-id="d241d-323">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="d241d-323">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="d241d-324">classroomForceRequestPermissionToLeaveClasses</span><span class="sxs-lookup"><span data-stu-id="d241d-324">classroomForceRequestPermissionToLeaveClasses</span></span>|<span data-ttu-id="d241d-325">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-325">Boolean</span></span>|<span data-ttu-id="d241d-326">指示在非托管课程中通过课堂注册的学生是否需要在尝试离开本课程时向教师请求权限。</span><span class="sxs-lookup"><span data-stu-id="d241d-326">Indicates whether a student enrolled in an unmanaged course via Classroom will be required to request permission from the teacher when attempting to leave the course.</span></span> <span data-ttu-id="d241d-327">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="d241d-327">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="d241d-328">classroomForceUnpromptedAppAndDeviceLock</span><span class="sxs-lookup"><span data-stu-id="d241d-328">classroomForceUnpromptedAppAndDeviceLock</span></span>|<span data-ttu-id="d241d-329">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-329">Boolean</span></span>|<span data-ttu-id="d241d-330">指示是否允许教师在不提示学生的情况下锁定应用或设备。</span><span class="sxs-lookup"><span data-stu-id="d241d-330">Indicates whether or not to allow the teacher to lock apps or the device without prompting the student.</span></span> <span data-ttu-id="d241d-331">需要通过 Apple School Manager 或 Apple 商业版管理器进行 MDM 注册。</span><span class="sxs-lookup"><span data-stu-id="d241d-331">Requires MDM enrollment via Apple School Manager or Apple Business Manager.</span></span>|
|<span data-ttu-id="d241d-332">iCloudBlockActivityContinuation</span><span class="sxs-lookup"><span data-stu-id="d241d-332">iCloudBlockActivityContinuation</span></span>|<span data-ttu-id="d241d-333">Boolean</span><span class="sxs-lookup"><span data-stu-id="d241d-333">Boolean</span></span>|<span data-ttu-id="d241d-334">指示是否阻止用户继续在另一台 iOS 或 MacOS 设备（MacOS 10.15 或更高版本）上的 MacOS 设备上启动的工作。</span><span class="sxs-lookup"><span data-stu-id="d241d-334">Indicates whether or not to block the user from continuing work that they started on a MacOS device on another iOS or MacOS device (MacOS 10.15 or later).</span></span>|
|<span data-ttu-id="d241d-335">privacyAccessControls</span><span class="sxs-lookup"><span data-stu-id="d241d-335">privacyAccessControls</span></span>|<span data-ttu-id="d241d-336">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md)集合</span><span class="sxs-lookup"><span data-stu-id="d241d-336">[macOSPrivacyAccessControlItem](../resources/intune-deviceconfig-macosprivacyaccesscontrolitem.md) collection</span></span>|<span data-ttu-id="d241d-337">隐私首选项策略控制的列表。</span><span class="sxs-lookup"><span data-stu-id="d241d-337">List of privacy preference policy controls.</span></span> <span data-ttu-id="d241d-338">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="d241d-338">This collection can contain a maximum of 10000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="d241d-339">响应</span><span class="sxs-lookup"><span data-stu-id="d241d-339">Response</span></span>
<span data-ttu-id="d241d-340">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d241d-340">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d241d-341">示例</span><span class="sxs-lookup"><span data-stu-id="d241d-341">Example</span></span>

### <a name="request"></a><span data-ttu-id="d241d-342">请求</span><span class="sxs-lookup"><span data-stu-id="d241d-342">Request</span></span>
<span data-ttu-id="d241d-343">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d241d-343">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 4545

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

### <a name="response"></a><span data-ttu-id="d241d-344">响应</span><span class="sxs-lookup"><span data-stu-id="d241d-344">Response</span></span>
<span data-ttu-id="d241d-p125">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d241d-p125">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4717

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



