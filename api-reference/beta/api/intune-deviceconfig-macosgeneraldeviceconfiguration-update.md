---
title: 更新 macOSGeneralDeviceConfiguration
description: 更新 macOSGeneralDeviceConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: 84ea867f10a99f985e7789cab2071183b34751c9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27348487"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="542f2-103">更新 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="542f2-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="542f2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="542f2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="542f2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="542f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="542f2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="542f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="542f2-107">更新 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="542f2-107">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="542f2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="542f2-108">Prerequisites</span></span>
<span data-ttu-id="542f2-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="542f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="542f2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="542f2-111">Permission type</span></span>|<span data-ttu-id="542f2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="542f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="542f2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="542f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="542f2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="542f2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="542f2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="542f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="542f2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="542f2-116">Not supported.</span></span>|
|<span data-ttu-id="542f2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="542f2-117">Application</span></span>|<span data-ttu-id="542f2-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="542f2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="542f2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="542f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="542f2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="542f2-120">Request headers</span></span>
|<span data-ttu-id="542f2-121">标头</span><span class="sxs-lookup"><span data-stu-id="542f2-121">Header</span></span>|<span data-ttu-id="542f2-122">值</span><span class="sxs-lookup"><span data-stu-id="542f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="542f2-123">授权</span><span class="sxs-lookup"><span data-stu-id="542f2-123">Authorization</span></span>|<span data-ttu-id="542f2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="542f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="542f2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="542f2-125">Accept</span></span>|<span data-ttu-id="542f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="542f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="542f2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="542f2-127">Request body</span></span>
<span data-ttu-id="542f2-128">在请求正文中，提供 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="542f2-128">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="542f2-129">下表显示创建 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="542f2-129">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="542f2-130">属性</span><span class="sxs-lookup"><span data-stu-id="542f2-130">Property</span></span>|<span data-ttu-id="542f2-131">类型</span><span class="sxs-lookup"><span data-stu-id="542f2-131">Type</span></span>|<span data-ttu-id="542f2-132">说明</span><span class="sxs-lookup"><span data-stu-id="542f2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="542f2-133">id</span><span class="sxs-lookup"><span data-stu-id="542f2-133">id</span></span>|<span data-ttu-id="542f2-134">String</span><span class="sxs-lookup"><span data-stu-id="542f2-134">String</span></span>|<span data-ttu-id="542f2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="542f2-135">Key of the entity.</span></span> <span data-ttu-id="542f2-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542f2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="542f2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="542f2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="542f2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="542f2-138">DateTimeOffset</span></span>|<span data-ttu-id="542f2-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="542f2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="542f2-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542f2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="542f2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="542f2-141">roleScopeTagIds</span></span>|<span data-ttu-id="542f2-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="542f2-142">String collection</span></span>|<span data-ttu-id="542f2-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="542f2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="542f2-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542f2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="542f2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="542f2-145">supportsScopeTags</span></span>|<span data-ttu-id="542f2-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-146">Boolean</span></span>|<span data-ttu-id="542f2-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="542f2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="542f2-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="542f2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="542f2-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="542f2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="542f2-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="542f2-150">This property is read-only.</span></span> <span data-ttu-id="542f2-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542f2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="542f2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="542f2-152">createdDateTime</span></span>|<span data-ttu-id="542f2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="542f2-153">DateTimeOffset</span></span>|<span data-ttu-id="542f2-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="542f2-154">DateTime the object was created.</span></span> <span data-ttu-id="542f2-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542f2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="542f2-156">description</span><span class="sxs-lookup"><span data-stu-id="542f2-156">description</span></span>|<span data-ttu-id="542f2-157">String</span><span class="sxs-lookup"><span data-stu-id="542f2-157">String</span></span>|<span data-ttu-id="542f2-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="542f2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="542f2-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542f2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="542f2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="542f2-160">displayName</span></span>|<span data-ttu-id="542f2-161">String</span><span class="sxs-lookup"><span data-stu-id="542f2-161">String</span></span>|<span data-ttu-id="542f2-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="542f2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="542f2-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542f2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="542f2-164">version</span><span class="sxs-lookup"><span data-stu-id="542f2-164">version</span></span>|<span data-ttu-id="542f2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="542f2-165">Int32</span></span>|<span data-ttu-id="542f2-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="542f2-166">Version of the device configuration.</span></span> <span data-ttu-id="542f2-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="542f2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="542f2-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="542f2-168">compliantAppsList</span></span>|<span data-ttu-id="542f2-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="542f2-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="542f2-170">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="542f2-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="542f2-171">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="542f2-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="542f2-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="542f2-172">compliantAppListType</span></span>|[<span data-ttu-id="542f2-173">appListType</span><span class="sxs-lookup"><span data-stu-id="542f2-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="542f2-174">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="542f2-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="542f2-175">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="542f2-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="542f2-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="542f2-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="542f2-177">String 集合</span><span class="sxs-lookup"><span data-stu-id="542f2-177">String collection</span></span>|<span data-ttu-id="542f2-178">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="542f2-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="542f2-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="542f2-179">passwordBlockSimple</span></span>|<span data-ttu-id="542f2-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-180">Boolean</span></span>|<span data-ttu-id="542f2-181">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="542f2-181">Block simple passwords.</span></span>|
|<span data-ttu-id="542f2-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="542f2-182">passwordExpirationDays</span></span>|<span data-ttu-id="542f2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="542f2-183">Int32</span></span>|<span data-ttu-id="542f2-184">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="542f2-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="542f2-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="542f2-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="542f2-186">Int32</span><span class="sxs-lookup"><span data-stu-id="542f2-186">Int32</span></span>|<span data-ttu-id="542f2-187">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="542f2-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="542f2-188">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="542f2-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="542f2-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="542f2-189">passwordMinimumLength</span></span>|<span data-ttu-id="542f2-190">Int32</span><span class="sxs-lookup"><span data-stu-id="542f2-190">Int32</span></span>|<span data-ttu-id="542f2-191">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="542f2-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="542f2-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="542f2-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="542f2-193">Int32</span><span class="sxs-lookup"><span data-stu-id="542f2-193">Int32</span></span>|<span data-ttu-id="542f2-194">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="542f2-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="542f2-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="542f2-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="542f2-196">Int32</span><span class="sxs-lookup"><span data-stu-id="542f2-196">Int32</span></span>|<span data-ttu-id="542f2-197">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="542f2-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="542f2-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="542f2-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="542f2-199">Int32</span><span class="sxs-lookup"><span data-stu-id="542f2-199">Int32</span></span>|<span data-ttu-id="542f2-200">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="542f2-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="542f2-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="542f2-201">passwordRequiredType</span></span>|[<span data-ttu-id="542f2-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="542f2-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="542f2-203">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="542f2-203">Type of password that is required.</span></span> <span data-ttu-id="542f2-204">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="542f2-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="542f2-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="542f2-205">passwordRequired</span></span>|<span data-ttu-id="542f2-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-206">Boolean</span></span>|<span data-ttu-id="542f2-207">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="542f2-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="542f2-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="542f2-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="542f2-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-209">Boolean</span></span>|<span data-ttu-id="542f2-210">指示 iCloud 钥匙链同步阻止 (macOS 10.12 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="542f2-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="542f2-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="542f2-211">airPrintBlocked</span></span>|<span data-ttu-id="542f2-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-212">Boolean</span></span>|<span data-ttu-id="542f2-213">指示 AirPrint 阻止 (macOS 10.12 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="542f2-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="542f2-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="542f2-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="542f2-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-215">Boolean</span></span>|<span data-ttu-id="542f2-216">指示受信任的证书是否需要 TLS 打印通信 (macOS 10.13 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="542f2-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="542f2-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="542f2-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="542f2-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-218">Boolean</span></span>|<span data-ttu-id="542f2-219">指示阻止 iBeacon 发现 AirPrint 打印机。</span><span class="sxs-lookup"><span data-stu-id="542f2-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="542f2-220">这样可以防止在从网络流量 (macOS 10.3 及更高版本) 的网络钓鱼的虚假 AirPrint 蓝牙信号。</span><span class="sxs-lookup"><span data-stu-id="542f2-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="542f2-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="542f2-221">safariBlockAutofill</span></span>|<span data-ttu-id="542f2-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-222">Boolean</span></span>|<span data-ttu-id="542f2-223">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="542f2-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="542f2-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="542f2-224">cameraBlocked</span></span>|<span data-ttu-id="542f2-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-225">Boolean</span></span>|<span data-ttu-id="542f2-226">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="542f2-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="542f2-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="542f2-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="542f2-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-228">Boolean</span></span>|<span data-ttu-id="542f2-229">指示阻止音乐服务并还原为经典模式的音乐应用程序。</span><span class="sxs-lookup"><span data-stu-id="542f2-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="542f2-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="542f2-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="542f2-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-231">Boolean</span></span>|<span data-ttu-id="542f2-232">指示阻止聚焦从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="542f2-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="542f2-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="542f2-233">keyboardBlockDictation</span></span>|<span data-ttu-id="542f2-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-234">Boolean</span></span>|<span data-ttu-id="542f2-235">指示阻止用户使用口述输入。</span><span class="sxs-lookup"><span data-stu-id="542f2-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="542f2-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="542f2-236">definitionLookupBlocked</span></span>|<span data-ttu-id="542f2-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-237">Boolean</span></span>|<span data-ttu-id="542f2-238">指示阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="542f2-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="542f2-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="542f2-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="542f2-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-240">Boolean</span></span>|<span data-ttu-id="542f2-241">指示是否或阻止用户解锁与 Apple Watch 其 Mac。</span><span class="sxs-lookup"><span data-stu-id="542f2-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="542f2-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="542f2-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="542f2-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-243">Boolean</span></span>|<span data-ttu-id="542f2-244">指示阻止进行文件传输使用 iTunes。</span><span class="sxs-lookup"><span data-stu-id="542f2-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="542f2-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="542f2-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="542f2-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-246">Boolean</span></span>|<span data-ttu-id="542f2-247">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="542f2-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="542f2-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="542f2-248">iCloudBlockMail</span></span>|<span data-ttu-id="542f2-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-249">Boolean</span></span>|<span data-ttu-id="542f2-250">指示阻止 iCloud 从同步邮件。</span><span class="sxs-lookup"><span data-stu-id="542f2-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="542f2-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="542f2-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="542f2-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-252">Boolean</span></span>|<span data-ttu-id="542f2-253">指示阻止 iCloud 从同步联系人。</span><span class="sxs-lookup"><span data-stu-id="542f2-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="542f2-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="542f2-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="542f2-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-255">Boolean</span></span>|<span data-ttu-id="542f2-256">指示阻止 iCloud 从同步日历。</span><span class="sxs-lookup"><span data-stu-id="542f2-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="542f2-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="542f2-257">iCloudBlockReminders</span></span>|<span data-ttu-id="542f2-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-258">Boolean</span></span>|<span data-ttu-id="542f2-259">指示阻止 iCloud 从同步提醒。</span><span class="sxs-lookup"><span data-stu-id="542f2-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="542f2-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="542f2-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="542f2-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-261">Boolean</span></span>|<span data-ttu-id="542f2-262">指示阻止 iCloud 从同步书签。</span><span class="sxs-lookup"><span data-stu-id="542f2-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="542f2-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="542f2-263">iCloudBlockNotes</span></span>|<span data-ttu-id="542f2-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-264">Boolean</span></span>|<span data-ttu-id="542f2-265">指示阻止 iCloud 从同步注释。</span><span class="sxs-lookup"><span data-stu-id="542f2-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="542f2-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="542f2-266">airDropBlocked</span></span>|<span data-ttu-id="542f2-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-267">Boolean</span></span>|<span data-ttu-id="542f2-268">指示允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="542f2-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="542f2-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="542f2-269">passwordBlockModification</span></span>|<span data-ttu-id="542f2-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-270">Boolean</span></span>|<span data-ttu-id="542f2-271">指示允许密码修改。</span><span class="sxs-lookup"><span data-stu-id="542f2-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="542f2-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="542f2-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="542f2-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="542f2-273">Boolean</span></span>|<span data-ttu-id="542f2-274">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="542f2-274">Indicates whether or not to block fingerprint unlock.</span></span>|



## <a name="response"></a><span data-ttu-id="542f2-275">响应</span><span class="sxs-lookup"><span data-stu-id="542f2-275">Response</span></span>
<span data-ttu-id="542f2-276">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="542f2-276">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="542f2-277">示例</span><span class="sxs-lookup"><span data-stu-id="542f2-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="542f2-278">请求</span><span class="sxs-lookup"><span data-stu-id="542f2-278">Request</span></span>
<span data-ttu-id="542f2-279">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="542f2-279">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1747

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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
  "passwordBlockFingerprintUnlock": true
}
```

### <a name="response"></a><span data-ttu-id="542f2-280">响应</span><span class="sxs-lookup"><span data-stu-id="542f2-280">Response</span></span>
<span data-ttu-id="542f2-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="542f2-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1925

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
  "passwordBlockFingerprintUnlock": true
}
```





