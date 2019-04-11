---
title: 创建 androidWorkProfileGmailEasConfiguration
description: 创建新的 androidWorkProfileGmailEasConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c2948e8942dbc14c9810669120921ffae13a941e
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31774419"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="04315-103">创建 androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="04315-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="04315-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04315-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04315-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04315-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04315-106">创建新的[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04315-106">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04315-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="04315-107">Prerequisites</span></span>
<span data-ttu-id="04315-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04315-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04315-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="04315-110">Permission type</span></span>|<span data-ttu-id="04315-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04315-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04315-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04315-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04315-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04315-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04315-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04315-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04315-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="04315-115">Not supported.</span></span>|
|<span data-ttu-id="04315-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="04315-116">Application</span></span>|<span data-ttu-id="04315-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="04315-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04315-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04315-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="04315-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="04315-119">Request headers</span></span>
|<span data-ttu-id="04315-120">标头</span><span class="sxs-lookup"><span data-stu-id="04315-120">Header</span></span>|<span data-ttu-id="04315-121">值</span><span class="sxs-lookup"><span data-stu-id="04315-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04315-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04315-122">Authorization</span></span>|<span data-ttu-id="04315-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04315-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04315-124">接受</span><span class="sxs-lookup"><span data-stu-id="04315-124">Accept</span></span>|<span data-ttu-id="04315-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04315-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04315-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="04315-126">Request body</span></span>
<span data-ttu-id="04315-127">在请求正文中, 提供 androidWorkProfileGmailEasConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04315-127">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="04315-128">下表显示创建 androidWorkProfileGmailEasConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="04315-128">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="04315-129">属性</span><span class="sxs-lookup"><span data-stu-id="04315-129">Property</span></span>|<span data-ttu-id="04315-130">类型</span><span class="sxs-lookup"><span data-stu-id="04315-130">Type</span></span>|<span data-ttu-id="04315-131">说明</span><span class="sxs-lookup"><span data-stu-id="04315-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04315-132">id</span><span class="sxs-lookup"><span data-stu-id="04315-132">id</span></span>|<span data-ttu-id="04315-133">String</span><span class="sxs-lookup"><span data-stu-id="04315-133">String</span></span>|<span data-ttu-id="04315-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="04315-134">Key of the entity.</span></span> <span data-ttu-id="04315-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04315-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04315-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04315-136">lastModifiedDateTime</span></span>|<span data-ttu-id="04315-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04315-137">DateTimeOffset</span></span>|<span data-ttu-id="04315-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="04315-138">DateTime the object was last modified.</span></span> <span data-ttu-id="04315-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04315-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04315-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="04315-140">roleScopeTagIds</span></span>|<span data-ttu-id="04315-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="04315-141">String collection</span></span>|<span data-ttu-id="04315-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="04315-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="04315-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04315-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04315-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="04315-144">supportsScopeTags</span></span>|<span data-ttu-id="04315-145">布尔值</span><span class="sxs-lookup"><span data-stu-id="04315-145">Boolean</span></span>|<span data-ttu-id="04315-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="04315-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="04315-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="04315-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="04315-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="04315-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="04315-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="04315-149">This property is read-only.</span></span> <span data-ttu-id="04315-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04315-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04315-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="04315-151">createdDateTime</span></span>|<span data-ttu-id="04315-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04315-152">DateTimeOffset</span></span>|<span data-ttu-id="04315-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="04315-153">DateTime the object was created.</span></span> <span data-ttu-id="04315-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04315-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04315-155">description</span><span class="sxs-lookup"><span data-stu-id="04315-155">description</span></span>|<span data-ttu-id="04315-156">String</span><span class="sxs-lookup"><span data-stu-id="04315-156">String</span></span>|<span data-ttu-id="04315-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="04315-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="04315-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04315-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04315-159">displayName</span><span class="sxs-lookup"><span data-stu-id="04315-159">displayName</span></span>|<span data-ttu-id="04315-160">String</span><span class="sxs-lookup"><span data-stu-id="04315-160">String</span></span>|<span data-ttu-id="04315-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="04315-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="04315-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04315-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04315-163">version</span><span class="sxs-lookup"><span data-stu-id="04315-163">version</span></span>|<span data-ttu-id="04315-164">Int32</span><span class="sxs-lookup"><span data-stu-id="04315-164">Int32</span></span>|<span data-ttu-id="04315-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="04315-165">Version of the device configuration.</span></span> <span data-ttu-id="04315-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="04315-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="04315-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="04315-167">authenticationMethod</span></span>|[<span data-ttu-id="04315-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="04315-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="04315-169">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="04315-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="04315-170">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="04315-170">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="04315-171">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="04315-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="04315-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="04315-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="04315-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="04315-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="04315-174">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="04315-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="04315-175">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="04315-175">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="04315-176">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="04315-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="04315-177">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="04315-177">emailAddressSource</span></span>|[<span data-ttu-id="04315-178">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="04315-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="04315-179">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="04315-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="04315-180">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="04315-180">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="04315-181">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="04315-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="04315-182">hostName</span><span class="sxs-lookup"><span data-stu-id="04315-182">hostName</span></span>|<span data-ttu-id="04315-183">String</span><span class="sxs-lookup"><span data-stu-id="04315-183">String</span></span>|<span data-ttu-id="04315-184">邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="04315-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="04315-185">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="04315-185">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="04315-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="04315-186">requireSsl</span></span>|<span data-ttu-id="04315-187">布尔值</span><span class="sxs-lookup"><span data-stu-id="04315-187">Boolean</span></span>|<span data-ttu-id="04315-188">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="04315-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="04315-189">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="04315-189">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="04315-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="04315-190">usernameSource</span></span>|[<span data-ttu-id="04315-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="04315-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="04315-192">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="04315-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="04315-193">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="04315-193">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="04315-194">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="04315-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="04315-195">响应</span><span class="sxs-lookup"><span data-stu-id="04315-195">Response</span></span>
<span data-ttu-id="04315-196">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04315-196">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04315-197">示例</span><span class="sxs-lookup"><span data-stu-id="04315-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="04315-198">请求</span><span class="sxs-lookup"><span data-stu-id="04315-198">Request</span></span>
<span data-ttu-id="04315-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04315-199">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 495

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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

### <a name="response"></a><span data-ttu-id="04315-200">响应</span><span class="sxs-lookup"><span data-stu-id="04315-200">Response</span></span>
<span data-ttu-id="04315-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04315-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 667

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGmailEasConfiguration",
  "id": "a4a44bb5-4bb5-a4a4-b54b-a4a4b54ba4a4",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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





