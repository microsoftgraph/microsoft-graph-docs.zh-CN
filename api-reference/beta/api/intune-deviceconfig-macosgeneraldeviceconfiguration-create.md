---
title: 创建 macOSGeneralDeviceConfiguration
description: 创建新的 macOSGeneralDeviceConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 6dd521646246914508a24f4c9188defff04bad9f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406512"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="0ac1a-103">创建 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0ac1a-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="0ac1a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0ac1a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ac1a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0ac1a-107">创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-107">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ac1a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0ac1a-108">Prerequisites</span></span>
<span data-ttu-id="0ac1a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0ac1a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ac1a-111">Permission type</span></span>|<span data-ttu-id="0ac1a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0ac1a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ac1a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac1a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ac1a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ac1a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0ac1a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ac1a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ac1a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-116">Not supported.</span></span>|
|<span data-ttu-id="0ac1a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ac1a-117">Application</span></span>|<span data-ttu-id="0ac1a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ac1a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ac1a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0ac1a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ac1a-120">Request headers</span></span>
|<span data-ttu-id="0ac1a-121">标头</span><span class="sxs-lookup"><span data-stu-id="0ac1a-121">Header</span></span>|<span data-ttu-id="0ac1a-122">值</span><span class="sxs-lookup"><span data-stu-id="0ac1a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ac1a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ac1a-123">Authorization</span></span>|<span data-ttu-id="0ac1a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ac1a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ac1a-125">Accept</span></span>|<span data-ttu-id="0ac1a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ac1a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ac1a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ac1a-127">Request body</span></span>
<span data-ttu-id="0ac1a-128">在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-128">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="0ac1a-129">下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-129">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="0ac1a-130">属性</span><span class="sxs-lookup"><span data-stu-id="0ac1a-130">Property</span></span>|<span data-ttu-id="0ac1a-131">类型</span><span class="sxs-lookup"><span data-stu-id="0ac1a-131">Type</span></span>|<span data-ttu-id="0ac1a-132">说明</span><span class="sxs-lookup"><span data-stu-id="0ac1a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ac1a-133">id</span><span class="sxs-lookup"><span data-stu-id="0ac1a-133">id</span></span>|<span data-ttu-id="0ac1a-134">String</span><span class="sxs-lookup"><span data-stu-id="0ac1a-134">String</span></span>|<span data-ttu-id="0ac1a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-135">Key of the entity.</span></span> <span data-ttu-id="0ac1a-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac1a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac1a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0ac1a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0ac1a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ac1a-138">DateTimeOffset</span></span>|<span data-ttu-id="0ac1a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0ac1a-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac1a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac1a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0ac1a-141">roleScopeTagIds</span></span>|<span data-ttu-id="0ac1a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ac1a-142">String collection</span></span>|<span data-ttu-id="0ac1a-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0ac1a-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac1a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac1a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0ac1a-145">supportsScopeTags</span></span>|<span data-ttu-id="0ac1a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-146">Boolean</span></span>|<span data-ttu-id="0ac1a-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0ac1a-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0ac1a-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0ac1a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-150">This property is read-only.</span></span> <span data-ttu-id="0ac1a-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac1a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac1a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0ac1a-152">createdDateTime</span></span>|<span data-ttu-id="0ac1a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0ac1a-153">DateTimeOffset</span></span>|<span data-ttu-id="0ac1a-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-154">DateTime the object was created.</span></span> <span data-ttu-id="0ac1a-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac1a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac1a-156">description</span><span class="sxs-lookup"><span data-stu-id="0ac1a-156">description</span></span>|<span data-ttu-id="0ac1a-157">String</span><span class="sxs-lookup"><span data-stu-id="0ac1a-157">String</span></span>|<span data-ttu-id="0ac1a-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0ac1a-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac1a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac1a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0ac1a-160">displayName</span></span>|<span data-ttu-id="0ac1a-161">String</span><span class="sxs-lookup"><span data-stu-id="0ac1a-161">String</span></span>|<span data-ttu-id="0ac1a-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0ac1a-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac1a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac1a-164">version</span><span class="sxs-lookup"><span data-stu-id="0ac1a-164">version</span></span>|<span data-ttu-id="0ac1a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac1a-165">Int32</span></span>|<span data-ttu-id="0ac1a-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-166">Version of the device configuration.</span></span> <span data-ttu-id="0ac1a-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0ac1a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0ac1a-168">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="0ac1a-168">compliantAppsList</span></span>|<span data-ttu-id="0ac1a-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="0ac1a-169">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="0ac1a-170">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-170">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="0ac1a-171">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-171">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="0ac1a-172">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="0ac1a-172">compliantAppListType</span></span>|[<span data-ttu-id="0ac1a-173">appListType</span><span class="sxs-lookup"><span data-stu-id="0ac1a-173">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="0ac1a-174">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-174">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="0ac1a-175">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-175">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="0ac1a-176">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="0ac1a-176">emailInDomainSuffixes</span></span>|<span data-ttu-id="0ac1a-177">String 集合</span><span class="sxs-lookup"><span data-stu-id="0ac1a-177">String collection</span></span>|<span data-ttu-id="0ac1a-178">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-178">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="0ac1a-179">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="0ac1a-179">passwordBlockSimple</span></span>|<span data-ttu-id="0ac1a-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-180">Boolean</span></span>|<span data-ttu-id="0ac1a-181">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-181">Block simple passwords.</span></span>|
|<span data-ttu-id="0ac1a-182">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="0ac1a-182">passwordExpirationDays</span></span>|<span data-ttu-id="0ac1a-183">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac1a-183">Int32</span></span>|<span data-ttu-id="0ac1a-184">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-184">Number of days before the password expires.</span></span>|
|<span data-ttu-id="0ac1a-185">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="0ac1a-185">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="0ac1a-186">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac1a-186">Int32</span></span>|<span data-ttu-id="0ac1a-187">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-187">Number of character sets a password must contain.</span></span> <span data-ttu-id="0ac1a-188">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="0ac1a-188">Valid values 0 to 4</span></span>|
|<span data-ttu-id="0ac1a-189">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="0ac1a-189">passwordMinimumLength</span></span>|<span data-ttu-id="0ac1a-190">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac1a-190">Int32</span></span>|<span data-ttu-id="0ac1a-191">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-191">Minimum length of passwords.</span></span>|
|<span data-ttu-id="0ac1a-192">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="0ac1a-192">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="0ac1a-193">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac1a-193">Int32</span></span>|<span data-ttu-id="0ac1a-194">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-194">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="0ac1a-195">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="0ac1a-195">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="0ac1a-196">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac1a-196">Int32</span></span>|<span data-ttu-id="0ac1a-197">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-197">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="0ac1a-198">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="0ac1a-198">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="0ac1a-199">Int32</span><span class="sxs-lookup"><span data-stu-id="0ac1a-199">Int32</span></span>|<span data-ttu-id="0ac1a-200">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-200">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="0ac1a-201">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="0ac1a-201">passwordRequiredType</span></span>|[<span data-ttu-id="0ac1a-202">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="0ac1a-202">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="0ac1a-203">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-203">Type of password that is required.</span></span> <span data-ttu-id="0ac1a-204">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-204">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="0ac1a-205">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="0ac1a-205">passwordRequired</span></span>|<span data-ttu-id="0ac1a-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-206">Boolean</span></span>|<span data-ttu-id="0ac1a-207">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-207">Whether or not to require a password.</span></span>|
|<span data-ttu-id="0ac1a-208">keychainBlockCloudSync</span><span class="sxs-lookup"><span data-stu-id="0ac1a-208">keychainBlockCloudSync</span></span>|<span data-ttu-id="0ac1a-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-209">Boolean</span></span>|<span data-ttu-id="0ac1a-210">指示 iCloud 钥匙链同步阻止 (macOS 10.12 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-210">Indicates whether or not iCloud keychain synchronization is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="0ac1a-211">airPrintBlocked</span><span class="sxs-lookup"><span data-stu-id="0ac1a-211">airPrintBlocked</span></span>|<span data-ttu-id="0ac1a-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-212">Boolean</span></span>|<span data-ttu-id="0ac1a-213">指示 AirPrint 阻止 (macOS 10.12 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-213">Indicates whether or not AirPrint is blocked (macOS 10.12 and later).</span></span>|
|<span data-ttu-id="0ac1a-214">airPrintForceTrustedTLS</span><span class="sxs-lookup"><span data-stu-id="0ac1a-214">airPrintForceTrustedTLS</span></span>|<span data-ttu-id="0ac1a-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-215">Boolean</span></span>|<span data-ttu-id="0ac1a-216">指示受信任的证书是否需要 TLS 打印通信 (macOS 10.13 及更高版本)。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-216">Indicates if trusted certificates are required for TLS printing communication (macOS 10.13 and later).</span></span>|
|<span data-ttu-id="0ac1a-217">airPrintBlockiBeaconDiscovery</span><span class="sxs-lookup"><span data-stu-id="0ac1a-217">airPrintBlockiBeaconDiscovery</span></span>|<span data-ttu-id="0ac1a-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-218">Boolean</span></span>|<span data-ttu-id="0ac1a-219">指示阻止 iBeacon 发现 AirPrint 打印机。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-219">Indicates whether or not iBeacon discovery of AirPrint printers is blocked.</span></span> <span data-ttu-id="0ac1a-220">这样可以防止在从网络流量 (macOS 10.3 及更高版本) 的网络钓鱼的虚假 AirPrint 蓝牙信号。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-220">This prevents spurious AirPrint Bluetooth beacons from phishing for network traffic (macOS 10.3 and later).</span></span>|
|<span data-ttu-id="0ac1a-221">safariBlockAutofill</span><span class="sxs-lookup"><span data-stu-id="0ac1a-221">safariBlockAutofill</span></span>|<span data-ttu-id="0ac1a-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-222">Boolean</span></span>|<span data-ttu-id="0ac1a-223">指示在 Safari 中是否阻止用户使用自动填充。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-223">Indicates whether or not to block the user from using Auto fill in Safari.</span></span>|
|<span data-ttu-id="0ac1a-224">cameraBlocked</span><span class="sxs-lookup"><span data-stu-id="0ac1a-224">cameraBlocked</span></span>|<span data-ttu-id="0ac1a-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-225">Boolean</span></span>|<span data-ttu-id="0ac1a-226">指示是否阻止用户访问设备的照相机。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-226">Indicates whether or not to block the user from accessing the camera of the device.</span></span>|
|<span data-ttu-id="0ac1a-227">iTunesBlockMusicService</span><span class="sxs-lookup"><span data-stu-id="0ac1a-227">iTunesBlockMusicService</span></span>|<span data-ttu-id="0ac1a-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-228">Boolean</span></span>|<span data-ttu-id="0ac1a-229">指示阻止音乐服务并还原为经典模式的音乐应用程序。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-229">Indicates whether or not to block Music service and revert Music app to classic mode.</span></span>|
|<span data-ttu-id="0ac1a-230">spotlightBlockInternetResults</span><span class="sxs-lookup"><span data-stu-id="0ac1a-230">spotlightBlockInternetResults</span></span>|<span data-ttu-id="0ac1a-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-231">Boolean</span></span>|<span data-ttu-id="0ac1a-232">指示阻止聚焦从 Internet 搜索返回任何结果。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-232">Indicates whether or not to block Spotlight from returning any results from an Internet search.</span></span>|
|<span data-ttu-id="0ac1a-233">keyboardBlockDictation</span><span class="sxs-lookup"><span data-stu-id="0ac1a-233">keyboardBlockDictation</span></span>|<span data-ttu-id="0ac1a-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-234">Boolean</span></span>|<span data-ttu-id="0ac1a-235">指示阻止用户使用口述输入。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-235">Indicates whether or not to block the user from using dictation input.</span></span>|
|<span data-ttu-id="0ac1a-236">definitionLookupBlocked</span><span class="sxs-lookup"><span data-stu-id="0ac1a-236">definitionLookupBlocked</span></span>|<span data-ttu-id="0ac1a-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-237">Boolean</span></span>|<span data-ttu-id="0ac1a-238">指示阻止定义查找。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-238">Indicates whether or not to block definition lookup.</span></span>|
|<span data-ttu-id="0ac1a-239">appleWatchBlockAutoUnlock</span><span class="sxs-lookup"><span data-stu-id="0ac1a-239">appleWatchBlockAutoUnlock</span></span>|<span data-ttu-id="0ac1a-240">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-240">Boolean</span></span>|<span data-ttu-id="0ac1a-241">指示是否或阻止用户解锁与 Apple Watch 其 Mac。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-241">Indicates whether or to block users from unlocking their Mac with Apple Watch.</span></span>|
|<span data-ttu-id="0ac1a-242">iTunesBlockFileSharing</span><span class="sxs-lookup"><span data-stu-id="0ac1a-242">iTunesBlockFileSharing</span></span>|<span data-ttu-id="0ac1a-243">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-243">Boolean</span></span>|<span data-ttu-id="0ac1a-244">指示阻止进行文件传输使用 iTunes。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-244">Indicates whether or not to block files from being transferred using iTunes.</span></span>|
|<span data-ttu-id="0ac1a-245">iCloudBlockDocumentSync</span><span class="sxs-lookup"><span data-stu-id="0ac1a-245">iCloudBlockDocumentSync</span></span>|<span data-ttu-id="0ac1a-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-246">Boolean</span></span>|<span data-ttu-id="0ac1a-247">指示是否阻止 iCloud 文档同步。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-247">Indicates whether or not to block iCloud document sync.</span></span>|
|<span data-ttu-id="0ac1a-248">iCloudBlockMail</span><span class="sxs-lookup"><span data-stu-id="0ac1a-248">iCloudBlockMail</span></span>|<span data-ttu-id="0ac1a-249">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-249">Boolean</span></span>|<span data-ttu-id="0ac1a-250">指示阻止 iCloud 从同步邮件。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-250">Indicates whether or not to block iCloud from syncing mail.</span></span>|
|<span data-ttu-id="0ac1a-251">iCloudBlockAddressBook</span><span class="sxs-lookup"><span data-stu-id="0ac1a-251">iCloudBlockAddressBook</span></span>|<span data-ttu-id="0ac1a-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-252">Boolean</span></span>|<span data-ttu-id="0ac1a-253">指示阻止 iCloud 从同步联系人。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-253">Indicates whether or not to block iCloud from syncing contacts.</span></span>|
|<span data-ttu-id="0ac1a-254">iCloudBlockCalendar</span><span class="sxs-lookup"><span data-stu-id="0ac1a-254">iCloudBlockCalendar</span></span>|<span data-ttu-id="0ac1a-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-255">Boolean</span></span>|<span data-ttu-id="0ac1a-256">指示阻止 iCloud 从同步日历。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-256">Indicates whether or not to block iCloud from syncing calendars.</span></span>|
|<span data-ttu-id="0ac1a-257">iCloudBlockReminders</span><span class="sxs-lookup"><span data-stu-id="0ac1a-257">iCloudBlockReminders</span></span>|<span data-ttu-id="0ac1a-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-258">Boolean</span></span>|<span data-ttu-id="0ac1a-259">指示阻止 iCloud 从同步提醒。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-259">Indicates whether or not to block iCloud from syncing reminders.</span></span>|
|<span data-ttu-id="0ac1a-260">iCloudBlockBookmarks</span><span class="sxs-lookup"><span data-stu-id="0ac1a-260">iCloudBlockBookmarks</span></span>|<span data-ttu-id="0ac1a-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-261">Boolean</span></span>|<span data-ttu-id="0ac1a-262">指示阻止 iCloud 从同步书签。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-262">Indicates whether or not to block iCloud from syncing bookmarks.</span></span>|
|<span data-ttu-id="0ac1a-263">iCloudBlockNotes</span><span class="sxs-lookup"><span data-stu-id="0ac1a-263">iCloudBlockNotes</span></span>|<span data-ttu-id="0ac1a-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-264">Boolean</span></span>|<span data-ttu-id="0ac1a-265">指示阻止 iCloud 从同步注释。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-265">Indicates whether or not to block iCloud from syncing notes.</span></span>|
|<span data-ttu-id="0ac1a-266">airDropBlocked</span><span class="sxs-lookup"><span data-stu-id="0ac1a-266">airDropBlocked</span></span>|<span data-ttu-id="0ac1a-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-267">Boolean</span></span>|<span data-ttu-id="0ac1a-268">指示允许 AirDrop。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-268">Indicates whether or not to allow AirDrop.</span></span>|
|<span data-ttu-id="0ac1a-269">passwordBlockModification</span><span class="sxs-lookup"><span data-stu-id="0ac1a-269">passwordBlockModification</span></span>|<span data-ttu-id="0ac1a-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-270">Boolean</span></span>|<span data-ttu-id="0ac1a-271">指示允许密码修改。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-271">Indicates whether or not to allow passcode modification.</span></span>|
|<span data-ttu-id="0ac1a-272">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="0ac1a-272">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="0ac1a-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-273">Boolean</span></span>|<span data-ttu-id="0ac1a-274">指示是否阻止指纹解锁。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-274">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="0ac1a-275">passwordBlockAutoFill</span><span class="sxs-lookup"><span data-stu-id="0ac1a-275">passwordBlockAutoFill</span></span>|<span data-ttu-id="0ac1a-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-276">Boolean</span></span>|<span data-ttu-id="0ac1a-277">指示阻止自动填充密码功能。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-277">Indicates whether or not to block the AutoFill Passwords feature.</span></span>|
|<span data-ttu-id="0ac1a-278">passwordBlockProximityRequests</span><span class="sxs-lookup"><span data-stu-id="0ac1a-278">passwordBlockProximityRequests</span></span>|<span data-ttu-id="0ac1a-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-279">Boolean</span></span>|<span data-ttu-id="0ac1a-280">指示阻止请求从附近的设备的密码。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-280">Indicates whether or not to block requesting passwords from nearby devices.</span></span>|
|<span data-ttu-id="0ac1a-281">passwordBlockAirDropSharing</span><span class="sxs-lookup"><span data-stu-id="0ac1a-281">passwordBlockAirDropSharing</span></span>|<span data-ttu-id="0ac1a-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="0ac1a-282">Boolean</span></span>|<span data-ttu-id="0ac1a-283">指示阻止与 AirDrop 密码功能的共享密码。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-283">Indicates whether or not to block sharing passwords with the AirDrop passwords feature.</span></span>|



## <a name="response"></a><span data-ttu-id="0ac1a-284">响应</span><span class="sxs-lookup"><span data-stu-id="0ac1a-284">Response</span></span>
<span data-ttu-id="0ac1a-285">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-285">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ac1a-286">示例</span><span class="sxs-lookup"><span data-stu-id="0ac1a-286">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ac1a-287">请求</span><span class="sxs-lookup"><span data-stu-id="0ac1a-287">Request</span></span>
<span data-ttu-id="0ac1a-288">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-288">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1870

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
  "passwordBlockAirDropSharing": true
}
```

### <a name="response"></a><span data-ttu-id="0ac1a-289">响应</span><span class="sxs-lookup"><span data-stu-id="0ac1a-289">Response</span></span>
<span data-ttu-id="0ac1a-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ac1a-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2042

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
  "passwordBlockAirDropSharing": true
}
```




