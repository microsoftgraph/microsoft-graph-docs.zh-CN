---
title: 更新 macOSGeneralDeviceConfiguration
description: 更新 macOSGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5b58f7606909d5c40777ed37e4b5d49da39f76f0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32518609"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="a8f73-103">更新 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="a8f73-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="a8f73-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a8f73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a8f73-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8f73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8f73-106">更新 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a8f73-106">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a8f73-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8f73-107">Prerequisites</span></span>
<span data-ttu-id="a8f73-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a8f73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a8f73-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8f73-110">Permission type</span></span>|<span data-ttu-id="a8f73-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a8f73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8f73-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8f73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a8f73-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8f73-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a8f73-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8f73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8f73-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8f73-115">Not supported.</span></span>|
|<span data-ttu-id="a8f73-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8f73-116">Application</span></span>|<span data-ttu-id="a8f73-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8f73-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8f73-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8f73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a8f73-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8f73-119">Request headers</span></span>
|<span data-ttu-id="a8f73-120">标头</span><span class="sxs-lookup"><span data-stu-id="a8f73-120">Header</span></span>|<span data-ttu-id="a8f73-121">值</span><span class="sxs-lookup"><span data-stu-id="a8f73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8f73-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8f73-122">Authorization</span></span>|<span data-ttu-id="a8f73-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8f73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a8f73-124">接受</span><span class="sxs-lookup"><span data-stu-id="a8f73-124">Accept</span></span>|<span data-ttu-id="a8f73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a8f73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8f73-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8f73-126">Request body</span></span>
<span data-ttu-id="a8f73-127">在请求正文中，提供 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8f73-127">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="a8f73-128">下表显示创建 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a8f73-128">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="a8f73-129">属性</span><span class="sxs-lookup"><span data-stu-id="a8f73-129">Property</span></span>|<span data-ttu-id="a8f73-130">类型</span><span class="sxs-lookup"><span data-stu-id="a8f73-130">Type</span></span>|<span data-ttu-id="a8f73-131">说明</span><span class="sxs-lookup"><span data-stu-id="a8f73-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8f73-132">id</span><span class="sxs-lookup"><span data-stu-id="a8f73-132">id</span></span>|<span data-ttu-id="a8f73-133">String</span><span class="sxs-lookup"><span data-stu-id="a8f73-133">String</span></span>|<span data-ttu-id="a8f73-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a8f73-134">Key of the entity.</span></span> <span data-ttu-id="a8f73-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f73-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8f73-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a8f73-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a8f73-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8f73-137">DateTimeOffset</span></span>|<span data-ttu-id="a8f73-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a8f73-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a8f73-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f73-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8f73-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a8f73-140">roleScopeTagIds</span></span>|<span data-ttu-id="a8f73-141">String collection</span><span class="sxs-lookup"><span data-stu-id="a8f73-141">String collection</span></span>|<span data-ttu-id="a8f73-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="a8f73-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="a8f73-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f73-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8f73-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="a8f73-144">supportsScopeTags</span></span>|<span data-ttu-id="a8f73-145">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-145">Boolean</span></span>|<span data-ttu-id="a8f73-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="a8f73-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="a8f73-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="a8f73-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="a8f73-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="a8f73-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="a8f73-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="a8f73-149">This property is read-only.</span></span> <span data-ttu-id="a8f73-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f73-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8f73-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a8f73-151">createdDateTime</span></span>|<span data-ttu-id="a8f73-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a8f73-152">DateTimeOffset</span></span>|<span data-ttu-id="a8f73-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a8f73-153">DateTime the object was created.</span></span> <span data-ttu-id="a8f73-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f73-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8f73-155">description</span><span class="sxs-lookup"><span data-stu-id="a8f73-155">description</span></span>|<span data-ttu-id="a8f73-156">字符串</span><span class="sxs-lookup"><span data-stu-id="a8f73-156">String</span></span>|<span data-ttu-id="a8f73-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a8f73-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a8f73-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f73-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8f73-159">displayName</span><span class="sxs-lookup"><span data-stu-id="a8f73-159">displayName</span></span>|<span data-ttu-id="a8f73-160">String</span><span class="sxs-lookup"><span data-stu-id="a8f73-160">String</span></span>|<span data-ttu-id="a8f73-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a8f73-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a8f73-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f73-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8f73-163">version</span><span class="sxs-lookup"><span data-stu-id="a8f73-163">version</span></span>|<span data-ttu-id="a8f73-164">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f73-164">Int32</span></span>|<span data-ttu-id="a8f73-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a8f73-165">Version of the device configuration.</span></span> <span data-ttu-id="a8f73-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a8f73-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a8f73-167">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="a8f73-167">compliantAppsList</span></span>|<span data-ttu-id="a8f73-168">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a8f73-168">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="a8f73-169">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="a8f73-169">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="a8f73-170">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a8f73-170">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="a8f73-171">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="a8f73-171">compliantAppListType</span></span>|[<span data-ttu-id="a8f73-172">appListType</span><span class="sxs-lookup"><span data-stu-id="a8f73-172">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="a8f73-173">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="a8f73-173">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="a8f73-174">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="a8f73-174">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="a8f73-175">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="a8f73-175">emailInDomainSuffixes</span></span>|<span data-ttu-id="a8f73-176">String 集合</span><span class="sxs-lookup"><span data-stu-id="a8f73-176">String collection</span></span>|<span data-ttu-id="a8f73-177">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="a8f73-177">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="a8f73-178">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="a8f73-178">passwordBlockSimple</span></span>|<span data-ttu-id="a8f73-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8f73-179">Boolean</span></span>|<span data-ttu-id="a8f73-180">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="a8f73-180">Block simple passwords.</span></span>|
|<span data-ttu-id="a8f73-181">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a8f73-181">passwordExpirationDays</span></span>|<span data-ttu-id="a8f73-182">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f73-182">Int32</span></span>|<span data-ttu-id="a8f73-183">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="a8f73-183">Number of days before the password expires.</span></span>|
|<span data-ttu-id="a8f73-184">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="a8f73-184">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="a8f73-185">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f73-185">Int32</span></span>|<span data-ttu-id="a8f73-186">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="a8f73-186">Number of character sets a password must contain.</span></span> <span data-ttu-id="a8f73-187">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="a8f73-187">Valid values 0 to 4</span></span>|
|<span data-ttu-id="a8f73-188">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a8f73-188">passwordMinimumLength</span></span>|<span data-ttu-id="a8f73-189">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f73-189">Int32</span></span>|<span data-ttu-id="a8f73-190">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="a8f73-190">Minimum length of passwords.</span></span>|
|<span data-ttu-id="a8f73-191">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="a8f73-191">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="a8f73-192">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f73-192">Int32</span></span>|<span data-ttu-id="a8f73-193">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a8f73-193">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="a8f73-194">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a8f73-194">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a8f73-195">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f73-195">Int32</span></span>|<span data-ttu-id="a8f73-196">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="a8f73-196">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="a8f73-197">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a8f73-197">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a8f73-198">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f73-198">Int32</span></span>|<span data-ttu-id="a8f73-199">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="a8f73-199">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="a8f73-200">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a8f73-200">passwordRequiredType</span></span>|[<span data-ttu-id="a8f73-201">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a8f73-201">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="a8f73-202">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="a8f73-202">Type of password that is required.</span></span> <span data-ttu-id="a8f73-203">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="a8f73-203">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="a8f73-204">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="a8f73-204">passwordRequired</span></span>|<span data-ttu-id="a8f73-205">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-205">Boolean</span></span>|<span data-ttu-id="a8f73-206">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="a8f73-206">Whether or not to require a password.</span></span>|
|<span data-ttu-id="a8f73-207">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="a8f73-207">keychainBlockCloudSync</span></span>|<span data-ttu-id="a8f73-208">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-208">Boolean</span></span>|<span data-ttu-id="a8f73-209">指示是否阻止 iCloud 密钥链同步 (macOS 10.12 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="a8f73-209">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="a8f73-210">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="a8f73-210">airPrintBlocked</span></span>|<span data-ttu-id="a8f73-211">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-211">Boolean</span></span>|<span data-ttu-id="a8f73-212">指示是否阻止 AirPrint (macOS 10.12 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="a8f73-212">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="a8f73-213">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="a8f73-213">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="a8f73-214">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-214">Boolean</span></span>|<span data-ttu-id="a8f73-215">指示 TLS 打印通信是否需要受信任的证书 (macOS 10.13 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="a8f73-215">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="a8f73-216">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="a8f73-216">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="a8f73-217">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-217">Boolean</span></span>|<span data-ttu-id="a8f73-218">指示是否阻止 AirPrint 打印机的 iBeacon 发现。</span><span class="sxs-lookup"><span data-stu-id="a8f73-218">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="a8f73-219">这可防止来自网络流量的虚假 AirPrint 蓝牙信号 (macOS 10.3 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="a8f73-219">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="a8f73-220">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="a8f73-220">safariBlockAutofill</span></span>|<span data-ttu-id="a8f73-221">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-221">Boolean</span></span>|<span data-ttu-id="a8f73-222">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="a8f73-222">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="a8f73-223">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="a8f73-223">cameraBlocked</span></span>|<span data-ttu-id="a8f73-224">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-224">Boolean</span></span>|<span data-ttu-id="a8f73-225">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="a8f73-225">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="a8f73-226">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="a8f73-226">iTunesBlockMusicService</span></span>|<span data-ttu-id="a8f73-227">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-227">Boolean</span></span>|<span data-ttu-id="a8f73-228">指示是否阻止音乐服务并将音乐应用还原到经典模式。</span><span class="sxs-lookup"><span data-stu-id="a8f73-228">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="a8f73-229">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="a8f73-229">spotlightBlockInternetResults</span></span>|<span data-ttu-id="a8f73-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8f73-230">Boolean</span></span>|<span data-ttu-id="a8f73-231">指示是否阻止聚光灯从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="a8f73-231">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="a8f73-232">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="a8f73-232">keyboardBlockDictation</span></span>|<span data-ttu-id="a8f73-233">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-233">Boolean</span></span>|<span data-ttu-id="a8f73-234">指示是否阻止用户使用听写输入。</span><span class="sxs-lookup"><span data-stu-id="a8f73-234">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="a8f73-235">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="a8f73-235">definitionLookupBlocked</span></span>|<span data-ttu-id="a8f73-236">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-236">Boolean</span></span>|<span data-ttu-id="a8f73-237">指示是否阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="a8f73-237">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="a8f73-238">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="a8f73-238">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="a8f73-239">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-239">Boolean</span></span>|<span data-ttu-id="a8f73-240">指示是否阻止用户使用 Apple Watch 解锁其 Mac。</span><span class="sxs-lookup"><span data-stu-id="a8f73-240">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="a8f73-241">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="a8f73-241">iTunesBlockFileSharing</span></span>|<span data-ttu-id="a8f73-242">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-242">Boolean</span></span>|<span data-ttu-id="a8f73-243">指示是否阻止使用 iTunes 传输文件。</span><span class="sxs-lookup"><span data-stu-id="a8f73-243">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="a8f73-244">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="a8f73-244">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="a8f73-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="a8f73-245">Boolean</span></span>|<span data-ttu-id="a8f73-246">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="a8f73-246">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="a8f73-247">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="a8f73-247">iCloudBlockMail</span></span>|<span data-ttu-id="a8f73-248">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-248">Boolean</span></span>|<span data-ttu-id="a8f73-249">指示是否阻止 iCloud 同步邮件。</span><span class="sxs-lookup"><span data-stu-id="a8f73-249">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="a8f73-250">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="a8f73-250">iCloudBlockAddressBook</span></span>|<span data-ttu-id="a8f73-251">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-251">Boolean</span></span>|<span data-ttu-id="a8f73-252">指示是否阻止 iCloud 同步联系人。</span><span class="sxs-lookup"><span data-stu-id="a8f73-252">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="a8f73-253">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="a8f73-253">iCloudBlockCalendar</span></span>|<span data-ttu-id="a8f73-254">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-254">Boolean</span></span>|<span data-ttu-id="a8f73-255">指示是否阻止 iCloud 同步日历。</span><span class="sxs-lookup"><span data-stu-id="a8f73-255">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="a8f73-256">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="a8f73-256">iCloudBlockReminders</span></span>|<span data-ttu-id="a8f73-257">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-257">Boolean</span></span>|<span data-ttu-id="a8f73-258">指示是否阻止 iCloud 同步提醒。</span><span class="sxs-lookup"><span data-stu-id="a8f73-258">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="a8f73-259">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="a8f73-259">iCloudBlockBookmarks</span></span>|<span data-ttu-id="a8f73-260">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-260">Boolean</span></span>|<span data-ttu-id="a8f73-261">指示是否阻止 iCloud 同步书签。</span><span class="sxs-lookup"><span data-stu-id="a8f73-261">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="a8f73-262">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="a8f73-262">iCloudBlockNotes</span></span>|<span data-ttu-id="a8f73-263">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-263">Boolean</span></span>|<span data-ttu-id="a8f73-264">指示是否阻止 iCloud 同步笔记。</span><span class="sxs-lookup"><span data-stu-id="a8f73-264">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="a8f73-265">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="a8f73-265">airDropBlocked</span></span>|<span data-ttu-id="a8f73-266">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-266">Boolean</span></span>|<span data-ttu-id="a8f73-267">指示是否允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="a8f73-267">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="a8f73-268">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="a8f73-268">passwordBlockModification</span></span>|<span data-ttu-id="a8f73-269">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-269">Boolean</span></span>|<span data-ttu-id="a8f73-270">指示是否允许修改密码。</span><span class="sxs-lookup"><span data-stu-id="a8f73-270">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="a8f73-271">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a8f73-271">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a8f73-272">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-272">Boolean</span></span>|<span data-ttu-id="a8f73-273">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="a8f73-273">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a8f73-274">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="a8f73-274">passwordBlockAutoFill</span></span>|<span data-ttu-id="a8f73-275">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-275">Boolean</span></span>|<span data-ttu-id="a8f73-276">指示是否阻止自动填充密码功能。</span><span class="sxs-lookup"><span data-stu-id="a8f73-276">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="a8f73-277">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="a8f73-277">passwordBlockProximityRequests</span></span>|<span data-ttu-id="a8f73-278">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-278">Boolean</span></span>|<span data-ttu-id="a8f73-279">指示是否阻止来自附近设备的请求密码。</span><span class="sxs-lookup"><span data-stu-id="a8f73-279">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="a8f73-280">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="a8f73-280">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="a8f73-281">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-281">Boolean</span></span>|<span data-ttu-id="a8f73-282">指示是否阻止使用 AirDrop 密码功能的共享密码。</span><span class="sxs-lookup"><span data-stu-id="a8f73-282">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|
|<span data-ttu-id="a8f73-283">softwareUpdatesEnforcedDelayInDays</span><span class="sxs-lookup"><span data-stu-id="a8f73-283">softwareUpdatesEnforcedDelayInDays</span></span>|<span data-ttu-id="a8f73-284">Int32</span><span class="sxs-lookup"><span data-stu-id="a8f73-284">Int32</span></span>|<span data-ttu-id="a8f73-285">设置受监督的设备 delyed 软件更新的天数。</span><span class="sxs-lookup"><span data-stu-id="a8f73-285">Sets how many days a software update will be delyed for a supervised device.</span></span> <span data-ttu-id="a8f73-286">有效值为 0 至 90</span><span class="sxs-lookup"><span data-stu-id="a8f73-286">Valid values 0 to 90</span></span>|
|<span data-ttu-id="a8f73-287">softwareUpdatesForceDelayed</span><span class="sxs-lookup"><span data-stu-id="a8f73-287">softwareUpdatesForceDelayed</span></span>|<span data-ttu-id="a8f73-288">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-288">Boolean</span></span>|<span data-ttu-id="a8f73-289">指示设备处于监督模式时是否延迟用户对软件更新的可见性。</span><span class="sxs-lookup"><span data-stu-id="a8f73-289">Indicates whether or not to delay user visibility of software updates when the device is in supervised mode.</span></span>|
|<span data-ttu-id="a8f73-290">contentCachingBlocked</span><span class="sxs-lookup"><span data-stu-id="a8f73-290">contentCachingBlocked</span></span>|<span data-ttu-id="a8f73-291">布尔</span><span class="sxs-lookup"><span data-stu-id="a8f73-291">Boolean</span></span>|<span data-ttu-id="a8f73-292">指示是否允许内容缓存。</span><span class="sxs-lookup"><span data-stu-id="a8f73-292">Indicates whether or not to allow content caching.</span></span>|



## <a name="response"></a><span data-ttu-id="a8f73-293">响应</span><span class="sxs-lookup"><span data-stu-id="a8f73-293">Response</span></span>
<span data-ttu-id="a8f73-294">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8f73-294">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8f73-295">示例</span><span class="sxs-lookup"><span data-stu-id="a8f73-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="a8f73-296">请求</span><span class="sxs-lookup"><span data-stu-id="a8f73-296">Request</span></span>
<span data-ttu-id="a8f73-297">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8f73-297">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1988

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "contentCachingBlocked": true
}
```

### <a name="response"></a><span data-ttu-id="a8f73-298">响应</span><span class="sxs-lookup"><span data-stu-id="a8f73-298">Response</span></span>
<span data-ttu-id="a8f73-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8f73-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2160

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "contentCachingBlocked": true
}
```





