---
title: 创建 androidWorkProfileNineWorkEasConfiguration
description: 创建新的 androidWorkProfileNineWorkEasConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a2324b36a32dbeb9479d2634f7beb84465eeacd0
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42758416"
---
# <a name="create-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="4ae7e-103">创建 androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="4ae7e-103">Create androidWorkProfileNineWorkEasConfiguration</span></span>

> <span data-ttu-id="4ae7e-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ae7e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ae7e-106">创建新的[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-106">Create a new [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4ae7e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4ae7e-107">Prerequisites</span></span>
<span data-ttu-id="4ae7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4ae7e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4ae7e-110">Permission type</span></span>|<span data-ttu-id="4ae7e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4ae7e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4ae7e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae7e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4ae7e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae7e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4ae7e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4ae7e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4ae7e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-115">Not supported.</span></span>|
|<span data-ttu-id="4ae7e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4ae7e-116">Application</span></span>|<span data-ttu-id="4ae7e-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4ae7e-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4ae7e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4ae7e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4ae7e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4ae7e-119">Request headers</span></span>
|<span data-ttu-id="4ae7e-120">标头</span><span class="sxs-lookup"><span data-stu-id="4ae7e-120">Header</span></span>|<span data-ttu-id="4ae7e-121">值</span><span class="sxs-lookup"><span data-stu-id="4ae7e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4ae7e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4ae7e-122">Authorization</span></span>|<span data-ttu-id="4ae7e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4ae7e-124">接受</span><span class="sxs-lookup"><span data-stu-id="4ae7e-124">Accept</span></span>|<span data-ttu-id="4ae7e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4ae7e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4ae7e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4ae7e-126">Request body</span></span>
<span data-ttu-id="4ae7e-127">在请求正文中，提供 androidWorkProfileNineWorkEasConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-127">In the request body, supply a JSON representation for the androidWorkProfileNineWorkEasConfiguration object.</span></span>

<span data-ttu-id="4ae7e-128">下表显示创建 androidWorkProfileNineWorkEasConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-128">The following table shows the properties that are required when you create the androidWorkProfileNineWorkEasConfiguration.</span></span>

|<span data-ttu-id="4ae7e-129">属性</span><span class="sxs-lookup"><span data-stu-id="4ae7e-129">Property</span></span>|<span data-ttu-id="4ae7e-130">类型</span><span class="sxs-lookup"><span data-stu-id="4ae7e-130">Type</span></span>|<span data-ttu-id="4ae7e-131">说明</span><span class="sxs-lookup"><span data-stu-id="4ae7e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ae7e-132">id</span><span class="sxs-lookup"><span data-stu-id="4ae7e-132">id</span></span>|<span data-ttu-id="4ae7e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4ae7e-133">String</span></span>|<span data-ttu-id="4ae7e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-134">Key of the entity.</span></span> <span data-ttu-id="4ae7e-135">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4ae7e-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4ae7e-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ae7e-137">DateTimeOffset</span></span>|<span data-ttu-id="4ae7e-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4ae7e-139">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="4ae7e-140">roleScopeTagIds</span></span>|<span data-ttu-id="4ae7e-141">String collection</span><span class="sxs-lookup"><span data-stu-id="4ae7e-141">String collection</span></span>|<span data-ttu-id="4ae7e-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="4ae7e-143">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="4ae7e-144">supportsScopeTags</span></span>|<span data-ttu-id="4ae7e-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="4ae7e-145">Boolean</span></span>|<span data-ttu-id="4ae7e-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="4ae7e-147">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="4ae7e-148">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="4ae7e-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-149">This property is read-only.</span></span> <span data-ttu-id="4ae7e-150">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ae7e-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="4ae7e-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="4ae7e-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="4ae7e-153">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="4ae7e-154">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ae7e-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="4ae7e-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="4ae7e-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="4ae7e-157">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="4ae7e-158">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ae7e-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="4ae7e-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="4ae7e-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="4ae7e-161">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="4ae7e-162">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4ae7e-163">createdDateTime</span></span>|<span data-ttu-id="4ae7e-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4ae7e-164">DateTimeOffset</span></span>|<span data-ttu-id="4ae7e-165">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-165">DateTime the object was created.</span></span> <span data-ttu-id="4ae7e-166">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-167">说明</span><span class="sxs-lookup"><span data-stu-id="4ae7e-167">description</span></span>|<span data-ttu-id="4ae7e-168">String</span><span class="sxs-lookup"><span data-stu-id="4ae7e-168">String</span></span>|<span data-ttu-id="4ae7e-169">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4ae7e-170">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-171">displayName</span><span class="sxs-lookup"><span data-stu-id="4ae7e-171">displayName</span></span>|<span data-ttu-id="4ae7e-172">String</span><span class="sxs-lookup"><span data-stu-id="4ae7e-172">String</span></span>|<span data-ttu-id="4ae7e-173">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4ae7e-174">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-175">version</span><span class="sxs-lookup"><span data-stu-id="4ae7e-175">version</span></span>|<span data-ttu-id="4ae7e-176">Int32</span><span class="sxs-lookup"><span data-stu-id="4ae7e-176">Int32</span></span>|<span data-ttu-id="4ae7e-177">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-177">Version of the device configuration.</span></span> <span data-ttu-id="4ae7e-178">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4ae7e-179">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ae7e-179">authenticationMethod</span></span>|[<span data-ttu-id="4ae7e-180">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="4ae7e-180">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="4ae7e-181">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-181">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="4ae7e-182">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-182">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="4ae7e-183">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-183">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="4ae7e-184">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="4ae7e-184">durationOfEmailToSync</span></span>|[<span data-ttu-id="4ae7e-185">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="4ae7e-185">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="4ae7e-186">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-186">Duration of time email should be synced to.</span></span> <span data-ttu-id="4ae7e-187">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-187">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="4ae7e-188">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-188">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="4ae7e-189">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="4ae7e-189">emailAddressSource</span></span>|[<span data-ttu-id="4ae7e-190">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="4ae7e-190">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="4ae7e-191">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-191">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4ae7e-192">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-192">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="4ae7e-193">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-193">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4ae7e-194">hostName</span><span class="sxs-lookup"><span data-stu-id="4ae7e-194">hostName</span></span>|<span data-ttu-id="4ae7e-195">String</span><span class="sxs-lookup"><span data-stu-id="4ae7e-195">String</span></span>|<span data-ttu-id="4ae7e-196">邮件应用程序连接到的 Exchange 位置（URL）。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-196">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="4ae7e-197">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-197">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="4ae7e-198">requireSsl</span><span class="sxs-lookup"><span data-stu-id="4ae7e-198">requireSsl</span></span>|<span data-ttu-id="4ae7e-199">布尔值</span><span class="sxs-lookup"><span data-stu-id="4ae7e-199">Boolean</span></span>|<span data-ttu-id="4ae7e-200">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-200">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="4ae7e-201">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="4ae7e-201">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="4ae7e-202">usernameSource</span><span class="sxs-lookup"><span data-stu-id="4ae7e-202">usernameSource</span></span>|[<span data-ttu-id="4ae7e-203">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="4ae7e-203">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="4ae7e-204">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-204">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="4ae7e-205">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-205">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="4ae7e-206">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-206">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="4ae7e-207">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="4ae7e-207">syncCalendar</span></span>|<span data-ttu-id="4ae7e-208">布尔值</span><span class="sxs-lookup"><span data-stu-id="4ae7e-208">Boolean</span></span>|<span data-ttu-id="4ae7e-209">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-209">Toggles syncing the calendar.</span></span> <span data-ttu-id="4ae7e-210">如果设置为 false，则表示设备上的日历处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-210">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="4ae7e-211">syncContacts</span><span class="sxs-lookup"><span data-stu-id="4ae7e-211">syncContacts</span></span>|<span data-ttu-id="4ae7e-212">布尔值</span><span class="sxs-lookup"><span data-stu-id="4ae7e-212">Boolean</span></span>|<span data-ttu-id="4ae7e-213">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-213">Toggles syncing contacts.</span></span> <span data-ttu-id="4ae7e-214">如果设置为 false，则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-214">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="4ae7e-215">syncTasks</span><span class="sxs-lookup"><span data-stu-id="4ae7e-215">syncTasks</span></span>|<span data-ttu-id="4ae7e-216">布尔值</span><span class="sxs-lookup"><span data-stu-id="4ae7e-216">Boolean</span></span>|<span data-ttu-id="4ae7e-217">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-217">Toggles syncing tasks.</span></span> <span data-ttu-id="4ae7e-218">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-218">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="4ae7e-219">响应</span><span class="sxs-lookup"><span data-stu-id="4ae7e-219">Response</span></span>
<span data-ttu-id="4ae7e-220">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-220">If successful, this method returns a `201 Created` response code and a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4ae7e-221">示例</span><span class="sxs-lookup"><span data-stu-id="4ae7e-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="4ae7e-222">请求</span><span class="sxs-lookup"><span data-stu-id="4ae7e-222">Request</span></span>
<span data-ttu-id="4ae7e-223">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1343

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```

### <a name="response"></a><span data-ttu-id="4ae7e-224">响应</span><span class="sxs-lookup"><span data-stu-id="4ae7e-224">Response</span></span>
<span data-ttu-id="4ae7e-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4ae7e-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1515

{
  "@odata.type": "#microsoft.graph.androidWorkProfileNineWorkEasConfiguration",
  "id": "3d9e3a30-3a30-3d9e-303a-9e3d303a9e3d",
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
  "authenticationMethod": "certificate",
  "durationOfEmailToSync": "oneDay",
  "emailAddressSource": "primarySmtpAddress",
  "hostName": "Host Name value",
  "requireSsl": true,
  "usernameSource": "userPrincipalName",
  "syncCalendar": true,
  "syncContacts": true,
  "syncTasks": true
}
```




