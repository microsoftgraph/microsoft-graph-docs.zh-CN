---
title: 更新 androidWorkProfileNineWorkEasConfiguration
description: 更新 androidWorkProfileNineWorkEasConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c368a33221a4fc38099db08999635e65b54cb0c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022706"
---
# <a name="update-androidworkprofilenineworkeasconfiguration"></a><span data-ttu-id="e3b63-103">更新 androidWorkProfileNineWorkEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="e3b63-103">Update androidWorkProfileNineWorkEasConfiguration</span></span>

<span data-ttu-id="e3b63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3b63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3b63-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e3b63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e3b63-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3b63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3b63-107">更新 [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e3b63-107">Update the properties of a [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3b63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e3b63-108">Prerequisites</span></span>
<span data-ttu-id="e3b63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e3b63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3b63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e3b63-111">Permission type</span></span>|<span data-ttu-id="e3b63-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e3b63-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3b63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3b63-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3b63-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e3b63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e3b63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3b63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e3b63-116">Not supported.</span></span>|
|<span data-ttu-id="e3b63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e3b63-117">Application</span></span>|<span data-ttu-id="e3b63-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3b63-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3b63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e3b63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="e3b63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e3b63-120">Request headers</span></span>
|<span data-ttu-id="e3b63-121">标头</span><span class="sxs-lookup"><span data-stu-id="e3b63-121">Header</span></span>|<span data-ttu-id="e3b63-122">值</span><span class="sxs-lookup"><span data-stu-id="e3b63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3b63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3b63-123">Authorization</span></span>|<span data-ttu-id="e3b63-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e3b63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3b63-125">接受</span><span class="sxs-lookup"><span data-stu-id="e3b63-125">Accept</span></span>|<span data-ttu-id="e3b63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3b63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3b63-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e3b63-127">Request body</span></span>
<span data-ttu-id="e3b63-128">在请求正文中，提供 [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3b63-128">In the request body, supply a JSON representation for the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object.</span></span>

<span data-ttu-id="e3b63-129">下表显示创建 [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e3b63-129">The following table shows the properties that are required when you create the [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md).</span></span>

|<span data-ttu-id="e3b63-130">属性</span><span class="sxs-lookup"><span data-stu-id="e3b63-130">Property</span></span>|<span data-ttu-id="e3b63-131">类型</span><span class="sxs-lookup"><span data-stu-id="e3b63-131">Type</span></span>|<span data-ttu-id="e3b63-132">说明</span><span class="sxs-lookup"><span data-stu-id="e3b63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3b63-133">id</span><span class="sxs-lookup"><span data-stu-id="e3b63-133">id</span></span>|<span data-ttu-id="e3b63-134">String</span><span class="sxs-lookup"><span data-stu-id="e3b63-134">String</span></span>|<span data-ttu-id="e3b63-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e3b63-135">Key of the entity.</span></span> <span data-ttu-id="e3b63-136">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e3b63-137">lastModifiedDateTime</span></span>|<span data-ttu-id="e3b63-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3b63-138">DateTimeOffset</span></span>|<span data-ttu-id="e3b63-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e3b63-139">DateTime the object was last modified.</span></span> <span data-ttu-id="e3b63-140">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e3b63-141">roleScopeTagIds</span></span>|<span data-ttu-id="e3b63-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="e3b63-142">String collection</span></span>|<span data-ttu-id="e3b63-143">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="e3b63-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e3b63-144">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="e3b63-145">supportsScopeTags</span></span>|<span data-ttu-id="e3b63-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3b63-146">Boolean</span></span>|<span data-ttu-id="e3b63-147">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="e3b63-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="e3b63-148">如果此值为 false，则不允许分配给 ScopeTags 属性，并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="e3b63-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="e3b63-149">这适用于在 Silverlight 中创建的旧版策略，可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="e3b63-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="e3b63-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="e3b63-150">This property is read-only.</span></span> <span data-ttu-id="e3b63-151">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e3b63-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="e3b63-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="e3b63-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="e3b63-154">适用于此策略的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="e3b63-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="e3b63-155">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e3b63-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="e3b63-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="e3b63-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="e3b63-158">此策略的操作系统版本适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e3b63-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="e3b63-159">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e3b63-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="e3b63-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="e3b63-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="e3b63-162">此策略的设备模式适用性规则。</span><span class="sxs-lookup"><span data-stu-id="e3b63-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="e3b63-163">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e3b63-164">createdDateTime</span></span>|<span data-ttu-id="e3b63-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e3b63-165">DateTimeOffset</span></span>|<span data-ttu-id="e3b63-166">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e3b63-166">DateTime the object was created.</span></span> <span data-ttu-id="e3b63-167">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-168">description</span><span class="sxs-lookup"><span data-stu-id="e3b63-168">description</span></span>|<span data-ttu-id="e3b63-169">String</span><span class="sxs-lookup"><span data-stu-id="e3b63-169">String</span></span>|<span data-ttu-id="e3b63-170">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e3b63-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e3b63-171">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-172">displayName</span><span class="sxs-lookup"><span data-stu-id="e3b63-172">displayName</span></span>|<span data-ttu-id="e3b63-173">String</span><span class="sxs-lookup"><span data-stu-id="e3b63-173">String</span></span>|<span data-ttu-id="e3b63-174">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e3b63-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e3b63-175">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-176">version</span><span class="sxs-lookup"><span data-stu-id="e3b63-176">version</span></span>|<span data-ttu-id="e3b63-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e3b63-177">Int32</span></span>|<span data-ttu-id="e3b63-178">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e3b63-178">Version of the device configuration.</span></span> <span data-ttu-id="e3b63-179">继承自 [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e3b63-180">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e3b63-180">authenticationMethod</span></span>|[<span data-ttu-id="e3b63-181">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="e3b63-181">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="e3b63-182">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="e3b63-182">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="e3b63-183">继承自 [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="e3b63-183">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="e3b63-184">可取值为：`usernameAndPassword`、`certificate`、`derivedCredential`。</span><span class="sxs-lookup"><span data-stu-id="e3b63-184">Possible values are: `usernameAndPassword`, `certificate`, `derivedCredential`.</span></span>|
|<span data-ttu-id="e3b63-185">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="e3b63-185">durationOfEmailToSync</span></span>|[<span data-ttu-id="e3b63-186">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="e3b63-186">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="e3b63-187">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="e3b63-187">Duration of time email should be synced to.</span></span> <span data-ttu-id="e3b63-188">继承自 [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="e3b63-188">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="e3b63-189">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="e3b63-189">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="e3b63-190">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="e3b63-190">emailAddressSource</span></span>|[<span data-ttu-id="e3b63-191">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="e3b63-191">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="e3b63-192">在设备上安装之前，从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="e3b63-192">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e3b63-193">继承自 [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="e3b63-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="e3b63-194">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="e3b63-194">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e3b63-195">hostName</span><span class="sxs-lookup"><span data-stu-id="e3b63-195">hostName</span></span>|<span data-ttu-id="e3b63-196">String</span><span class="sxs-lookup"><span data-stu-id="e3b63-196">String</span></span>|<span data-ttu-id="e3b63-197">邮件应用程序连接到的 Exchange 位置 (URL) 。</span><span class="sxs-lookup"><span data-stu-id="e3b63-197">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="e3b63-198">继承自 [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-198">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="e3b63-199">requireSsl</span><span class="sxs-lookup"><span data-stu-id="e3b63-199">requireSsl</span></span>|<span data-ttu-id="e3b63-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3b63-200">Boolean</span></span>|<span data-ttu-id="e3b63-201">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="e3b63-201">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="e3b63-202">继承自 [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="e3b63-202">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="e3b63-203">usernameSource</span><span class="sxs-lookup"><span data-stu-id="e3b63-203">usernameSource</span></span>|[<span data-ttu-id="e3b63-204">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="e3b63-204">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="e3b63-205">在设备上安装之前，从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="e3b63-205">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="e3b63-206">继承自 [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="e3b63-206">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="e3b63-207">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="e3b63-207">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="e3b63-208">syncCalendar</span><span class="sxs-lookup"><span data-stu-id="e3b63-208">syncCalendar</span></span>|<span data-ttu-id="e3b63-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3b63-209">Boolean</span></span>|<span data-ttu-id="e3b63-210">切换同步日历。</span><span class="sxs-lookup"><span data-stu-id="e3b63-210">Toggles syncing the calendar.</span></span> <span data-ttu-id="e3b63-211">如果设置为 false，则表示设备上的日历处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="e3b63-211">If set to false the calendar is turned off on the device.</span></span>|
|<span data-ttu-id="e3b63-212">syncContacts</span><span class="sxs-lookup"><span data-stu-id="e3b63-212">syncContacts</span></span>|<span data-ttu-id="e3b63-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3b63-213">Boolean</span></span>|<span data-ttu-id="e3b63-214">切换同步联系人。</span><span class="sxs-lookup"><span data-stu-id="e3b63-214">Toggles syncing contacts.</span></span> <span data-ttu-id="e3b63-215">如果设置为 false，则设备上的联系人处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="e3b63-215">If set to false contacts are turned off on the device.</span></span>|
|<span data-ttu-id="e3b63-216">syncTasks</span><span class="sxs-lookup"><span data-stu-id="e3b63-216">syncTasks</span></span>|<span data-ttu-id="e3b63-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3b63-217">Boolean</span></span>|<span data-ttu-id="e3b63-218">切换同步任务。</span><span class="sxs-lookup"><span data-stu-id="e3b63-218">Toggles syncing tasks.</span></span> <span data-ttu-id="e3b63-219">如果设备上的 "设置为 false 任务" 处于关闭状态。</span><span class="sxs-lookup"><span data-stu-id="e3b63-219">If set to false tasks are turned off on the device.</span></span>|



## <a name="response"></a><span data-ttu-id="e3b63-220">响应</span><span class="sxs-lookup"><span data-stu-id="e3b63-220">Response</span></span>
<span data-ttu-id="e3b63-221">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e3b63-221">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileNineWorkEasConfiguration](../resources/intune-deviceconfig-androidworkprofilenineworkeasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3b63-222">示例</span><span class="sxs-lookup"><span data-stu-id="e3b63-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3b63-223">请求</span><span class="sxs-lookup"><span data-stu-id="e3b63-223">Request</span></span>
<span data-ttu-id="e3b63-224">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e3b63-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="e3b63-225">响应</span><span class="sxs-lookup"><span data-stu-id="e3b63-225">Response</span></span>
<span data-ttu-id="e3b63-p122">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e3b63-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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






