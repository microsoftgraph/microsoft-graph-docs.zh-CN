---
title: 创建 androidForWorkGmailEasConfiguration
description: 创建新的 androidForWorkGmailEasConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 108369f451a0316876153e2348414cc67c586d6a
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697019"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="ec96b-103">创建 androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="ec96b-103">Create androidForWorkGmailEasConfiguration</span></span>

<span data-ttu-id="ec96b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec96b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec96b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec96b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec96b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec96b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec96b-107">创建新的 [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec96b-107">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec96b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ec96b-108">Prerequisites</span></span>
<span data-ttu-id="ec96b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec96b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec96b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec96b-111">Permission type</span></span>|<span data-ttu-id="ec96b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ec96b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec96b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec96b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ec96b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec96b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ec96b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec96b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec96b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec96b-116">Not supported.</span></span>|
|<span data-ttu-id="ec96b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec96b-117">Application</span></span>|<span data-ttu-id="ec96b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec96b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec96b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec96b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ec96b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec96b-120">Request headers</span></span>
|<span data-ttu-id="ec96b-121">标头</span><span class="sxs-lookup"><span data-stu-id="ec96b-121">Header</span></span>|<span data-ttu-id="ec96b-122">值</span><span class="sxs-lookup"><span data-stu-id="ec96b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec96b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec96b-123">Authorization</span></span>|<span data-ttu-id="ec96b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ec96b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec96b-125">接受</span><span class="sxs-lookup"><span data-stu-id="ec96b-125">Accept</span></span>|<span data-ttu-id="ec96b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ec96b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec96b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec96b-127">Request body</span></span>
<span data-ttu-id="ec96b-128">在请求正文中，提供 androidForWorkGmailEasConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec96b-128">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="ec96b-129">下表显示创建 androidForWorkGmailEasConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ec96b-129">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="ec96b-130">属性</span><span class="sxs-lookup"><span data-stu-id="ec96b-130">Property</span></span>|<span data-ttu-id="ec96b-131">类型</span><span class="sxs-lookup"><span data-stu-id="ec96b-131">Type</span></span>|<span data-ttu-id="ec96b-132">说明</span><span class="sxs-lookup"><span data-stu-id="ec96b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec96b-133">id</span><span class="sxs-lookup"><span data-stu-id="ec96b-133">id</span></span>|<span data-ttu-id="ec96b-134">String</span><span class="sxs-lookup"><span data-stu-id="ec96b-134">String</span></span>|<span data-ttu-id="ec96b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ec96b-135">Key of the entity.</span></span> <span data-ttu-id="ec96b-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ec96b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="ec96b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec96b-138">DateTimeOffset</span></span>|<span data-ttu-id="ec96b-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ec96b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="ec96b-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ec96b-141">roleScopeTagIds</span></span>|<span data-ttu-id="ec96b-142">String collection</span><span class="sxs-lookup"><span data-stu-id="ec96b-142">String collection</span></span>|<span data-ttu-id="ec96b-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="ec96b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ec96b-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="ec96b-145">supportsScopeTags</span></span>|<span data-ttu-id="ec96b-146">布尔</span><span class="sxs-lookup"><span data-stu-id="ec96b-146">Boolean</span></span>|<span data-ttu-id="ec96b-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="ec96b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="ec96b-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="ec96b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="ec96b-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="ec96b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="ec96b-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="ec96b-150">This property is read-only.</span></span> <span data-ttu-id="ec96b-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ec96b-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="ec96b-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="ec96b-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="ec96b-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="ec96b-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="ec96b-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ec96b-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="ec96b-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="ec96b-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="ec96b-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ec96b-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="ec96b-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ec96b-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="ec96b-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="ec96b-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="ec96b-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="ec96b-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="ec96b-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ec96b-164">createdDateTime</span></span>|<span data-ttu-id="ec96b-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ec96b-165">DateTimeOffset</span></span>|<span data-ttu-id="ec96b-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ec96b-166">DateTime the object was created.</span></span> <span data-ttu-id="ec96b-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-168">说明</span><span class="sxs-lookup"><span data-stu-id="ec96b-168">description</span></span>|<span data-ttu-id="ec96b-169">String</span><span class="sxs-lookup"><span data-stu-id="ec96b-169">String</span></span>|<span data-ttu-id="ec96b-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ec96b-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ec96b-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-172">displayName</span><span class="sxs-lookup"><span data-stu-id="ec96b-172">displayName</span></span>|<span data-ttu-id="ec96b-173">String</span><span class="sxs-lookup"><span data-stu-id="ec96b-173">String</span></span>|<span data-ttu-id="ec96b-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ec96b-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ec96b-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-176">version</span><span class="sxs-lookup"><span data-stu-id="ec96b-176">version</span></span>|<span data-ttu-id="ec96b-177">Int32</span><span class="sxs-lookup"><span data-stu-id="ec96b-177">Int32</span></span>|<span data-ttu-id="ec96b-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ec96b-178">Version of the device configuration.</span></span> <span data-ttu-id="ec96b-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ec96b-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ec96b-180">authenticationMethod</span></span>|[<span data-ttu-id="ec96b-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="ec96b-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="ec96b-182">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="ec96b-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="ec96b-183">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ec96b-183">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ec96b-184">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="ec96b-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="ec96b-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="ec96b-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="ec96b-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="ec96b-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="ec96b-187">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="ec96b-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="ec96b-188">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ec96b-188">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ec96b-189">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="ec96b-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="ec96b-190">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="ec96b-190">emailAddressSource</span></span>|[<span data-ttu-id="ec96b-191">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="ec96b-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="ec96b-192">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="ec96b-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ec96b-193">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ec96b-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ec96b-194">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="ec96b-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="ec96b-195">hostName</span><span class="sxs-lookup"><span data-stu-id="ec96b-195">hostName</span></span>|<span data-ttu-id="ec96b-196">String</span><span class="sxs-lookup"><span data-stu-id="ec96b-196">String</span></span>|<span data-ttu-id="ec96b-197">邮件应用程序连接到的 Exchange 位置 (URL) 。</span><span class="sxs-lookup"><span data-stu-id="ec96b-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="ec96b-198">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-198">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="ec96b-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="ec96b-199">requireSsl</span></span>|<span data-ttu-id="ec96b-200">布尔</span><span class="sxs-lookup"><span data-stu-id="ec96b-200">Boolean</span></span>|<span data-ttu-id="ec96b-201">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="ec96b-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="ec96b-202">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="ec96b-202">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="ec96b-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="ec96b-203">usernameSource</span></span>|[<span data-ttu-id="ec96b-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="ec96b-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="ec96b-205">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="ec96b-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="ec96b-206">继承自 [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="ec96b-206">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="ec96b-207">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="ec96b-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="ec96b-208">响应</span><span class="sxs-lookup"><span data-stu-id="ec96b-208">Response</span></span>
<span data-ttu-id="ec96b-209">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ec96b-209">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec96b-210">示例</span><span class="sxs-lookup"><span data-stu-id="ec96b-210">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec96b-211">请求</span><span class="sxs-lookup"><span data-stu-id="ec96b-211">Request</span></span>
<span data-ttu-id="ec96b-212">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec96b-212">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1264

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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
  "usernameSource": "userPrincipalName"
}
```

### <a name="response"></a><span data-ttu-id="ec96b-213">响应</span><span class="sxs-lookup"><span data-stu-id="ec96b-213">Response</span></span>
<span data-ttu-id="ec96b-p119">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec96b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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
  "usernameSource": "userPrincipalName"
}
```





