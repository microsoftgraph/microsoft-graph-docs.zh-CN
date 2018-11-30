---
title: 创建 androidForWorkGmailEasConfiguration
description: 创建新的 androidForWorkGmailEasConfiguration 对象。
ms.openlocfilehash: e1002f7e2679ab5180403b4ccd3724be81b8786d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044498"
---
# <a name="create-androidforworkgmaileasconfiguration"></a><span data-ttu-id="5b816-103">创建 androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="5b816-103">Create androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="5b816-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5b816-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5b816-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5b816-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5b816-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5b816-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b816-107">创建新的[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5b816-107">Create a new [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5b816-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5b816-108">Prerequisites</span></span>
<span data-ttu-id="5b816-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5b816-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b816-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b816-111">Permission type</span></span>|<span data-ttu-id="5b816-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5b816-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b816-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b816-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b816-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b816-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b816-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b816-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b816-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b816-116">Not supported.</span></span>|
|<span data-ttu-id="5b816-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b816-117">Application</span></span>|<span data-ttu-id="5b816-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b816-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b816-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b816-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5b816-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b816-120">Request headers</span></span>
|<span data-ttu-id="5b816-121">标头</span><span class="sxs-lookup"><span data-stu-id="5b816-121">Header</span></span>|<span data-ttu-id="5b816-122">值</span><span class="sxs-lookup"><span data-stu-id="5b816-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b816-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b816-123">Authorization</span></span>|<span data-ttu-id="5b816-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5b816-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b816-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5b816-125">Accept</span></span>|<span data-ttu-id="5b816-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b816-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b816-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b816-127">Request body</span></span>
<span data-ttu-id="5b816-128">在请求正文中，提供 androidForWorkGmailEasConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b816-128">In the request body, supply a JSON representation for the androidForWorkGmailEasConfiguration object.</span></span>

<span data-ttu-id="5b816-129">下表显示时创建 androidForWorkGmailEasConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5b816-129">The following table shows the properties that are required when you create the androidForWorkGmailEasConfiguration.</span></span>

|<span data-ttu-id="5b816-130">属性</span><span class="sxs-lookup"><span data-stu-id="5b816-130">Property</span></span>|<span data-ttu-id="5b816-131">类型</span><span class="sxs-lookup"><span data-stu-id="5b816-131">Type</span></span>|<span data-ttu-id="5b816-132">说明</span><span class="sxs-lookup"><span data-stu-id="5b816-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b816-133">id</span><span class="sxs-lookup"><span data-stu-id="5b816-133">id</span></span>|<span data-ttu-id="5b816-134">String</span><span class="sxs-lookup"><span data-stu-id="5b816-134">String</span></span>|<span data-ttu-id="5b816-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5b816-135">Key of the entity.</span></span> <span data-ttu-id="5b816-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b816-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5b816-137">lastModifiedDateTime</span></span>|<span data-ttu-id="5b816-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b816-138">DateTimeOffset</span></span>|<span data-ttu-id="5b816-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5b816-139">DateTime the object was last modified.</span></span> <span data-ttu-id="5b816-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b816-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5b816-141">roleScopeTagIds</span></span>|<span data-ttu-id="5b816-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="5b816-142">String collection</span></span>|<span data-ttu-id="5b816-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="5b816-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="5b816-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b816-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="5b816-145">supportsScopeTags</span></span>|<span data-ttu-id="5b816-146">布尔</span><span class="sxs-lookup"><span data-stu-id="5b816-146">Boolean</span></span>|<span data-ttu-id="5b816-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="5b816-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="5b816-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="5b816-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="5b816-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="5b816-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="5b816-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="5b816-150">This property is read-only.</span></span> <span data-ttu-id="5b816-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b816-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5b816-152">createdDateTime</span></span>|<span data-ttu-id="5b816-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5b816-153">DateTimeOffset</span></span>|<span data-ttu-id="5b816-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="5b816-154">DateTime the object was created.</span></span> <span data-ttu-id="5b816-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b816-156">description</span><span class="sxs-lookup"><span data-stu-id="5b816-156">description</span></span>|<span data-ttu-id="5b816-157">String</span><span class="sxs-lookup"><span data-stu-id="5b816-157">String</span></span>|<span data-ttu-id="5b816-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="5b816-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5b816-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b816-160">displayName</span><span class="sxs-lookup"><span data-stu-id="5b816-160">displayName</span></span>|<span data-ttu-id="5b816-161">String</span><span class="sxs-lookup"><span data-stu-id="5b816-161">String</span></span>|<span data-ttu-id="5b816-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="5b816-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5b816-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b816-164">version</span><span class="sxs-lookup"><span data-stu-id="5b816-164">version</span></span>|<span data-ttu-id="5b816-165">Int32</span><span class="sxs-lookup"><span data-stu-id="5b816-165">Int32</span></span>|<span data-ttu-id="5b816-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="5b816-166">Version of the device configuration.</span></span> <span data-ttu-id="5b816-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5b816-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5b816-168">authenticationMethod</span></span>|[<span data-ttu-id="5b816-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5b816-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="5b816-170">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="5b816-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="5b816-171">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="5b816-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="5b816-172">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="5b816-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="5b816-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="5b816-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="5b816-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="5b816-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="5b816-175">应为同步的时间电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="5b816-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="5b816-176">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="5b816-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="5b816-177">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。</span><span class="sxs-lookup"><span data-stu-id="5b816-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="5b816-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="5b816-178">emailAddressSource</span></span>|[<span data-ttu-id="5b816-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="5b816-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="5b816-180">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="5b816-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="5b816-181">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="5b816-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="5b816-182">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="5b816-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="5b816-183">hostName</span><span class="sxs-lookup"><span data-stu-id="5b816-183">hostName</span></span>|<span data-ttu-id="5b816-184">String</span><span class="sxs-lookup"><span data-stu-id="5b816-184">String</span></span>|<span data-ttu-id="5b816-185">Exchange 位置 (URL) 的邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="5b816-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="5b816-186">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="5b816-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="5b816-187">requireSsl</span></span>|<span data-ttu-id="5b816-188">布尔</span><span class="sxs-lookup"><span data-stu-id="5b816-188">Boolean</span></span>|<span data-ttu-id="5b816-189">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="5b816-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="5b816-190">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="5b816-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="5b816-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="5b816-191">usernameSource</span></span>|[<span data-ttu-id="5b816-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="5b816-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="5b816-193">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="5b816-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="5b816-194">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="5b816-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="5b816-195">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="5b816-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="5b816-196">响应</span><span class="sxs-lookup"><span data-stu-id="5b816-196">Response</span></span>
<span data-ttu-id="5b816-197">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5b816-197">If successful, this method returns a `201 Created` response code and a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b816-198">示例</span><span class="sxs-lookup"><span data-stu-id="5b816-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="5b816-199">请求</span><span class="sxs-lookup"><span data-stu-id="5b816-199">Request</span></span>
<span data-ttu-id="5b816-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b816-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 555

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="5b816-201">响应</span><span class="sxs-lookup"><span data-stu-id="5b816-201">Response</span></span>
<span data-ttu-id="5b816-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b816-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 663

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
  "id": "2bafc891-c891-2baf-91c8-af2b91c8af2b",
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





