---
title: 更新 androidForWorkGmailEasConfiguration
description: 更新 androidForWorkGmailEasConfiguration 对象的属性。
author: tfitzmac
ms.openlocfilehash: 9da99cb4ecb0d466a8367e2d7b5ad3902956e1c7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27317792"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="cabb0-103">更新 androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="cabb0-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="cabb0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cabb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cabb0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cabb0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cabb0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cabb0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cabb0-107">更新[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cabb0-107">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cabb0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cabb0-108">Prerequisites</span></span>
<span data-ttu-id="cabb0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cabb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cabb0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cabb0-111">Permission type</span></span>|<span data-ttu-id="cabb0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cabb0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cabb0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cabb0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cabb0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cabb0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cabb0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cabb0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cabb0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cabb0-116">Not supported.</span></span>|
|<span data-ttu-id="cabb0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cabb0-117">Application</span></span>|<span data-ttu-id="cabb0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cabb0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cabb0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cabb0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cabb0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cabb0-120">Request headers</span></span>
|<span data-ttu-id="cabb0-121">标头</span><span class="sxs-lookup"><span data-stu-id="cabb0-121">Header</span></span>|<span data-ttu-id="cabb0-122">值</span><span class="sxs-lookup"><span data-stu-id="cabb0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cabb0-123">授权</span><span class="sxs-lookup"><span data-stu-id="cabb0-123">Authorization</span></span>|<span data-ttu-id="cabb0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cabb0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cabb0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cabb0-125">Accept</span></span>|<span data-ttu-id="cabb0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cabb0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cabb0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cabb0-127">Request body</span></span>
<span data-ttu-id="cabb0-128">在请求正文中，提供[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cabb0-128">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="cabb0-129">下表显示时创建[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cabb0-129">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="cabb0-130">属性</span><span class="sxs-lookup"><span data-stu-id="cabb0-130">Property</span></span>|<span data-ttu-id="cabb0-131">类型</span><span class="sxs-lookup"><span data-stu-id="cabb0-131">Type</span></span>|<span data-ttu-id="cabb0-132">说明</span><span class="sxs-lookup"><span data-stu-id="cabb0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cabb0-133">id</span><span class="sxs-lookup"><span data-stu-id="cabb0-133">id</span></span>|<span data-ttu-id="cabb0-134">String</span><span class="sxs-lookup"><span data-stu-id="cabb0-134">String</span></span>|<span data-ttu-id="cabb0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cabb0-135">Key of the entity.</span></span> <span data-ttu-id="cabb0-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cabb0-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="cabb0-137">lastModifiedDateTime</span></span>|<span data-ttu-id="cabb0-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cabb0-138">DateTimeOffset</span></span>|<span data-ttu-id="cabb0-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cabb0-139">DateTime the object was last modified.</span></span> <span data-ttu-id="cabb0-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cabb0-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="cabb0-141">roleScopeTagIds</span></span>|<span data-ttu-id="cabb0-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="cabb0-142">String collection</span></span>|<span data-ttu-id="cabb0-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="cabb0-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="cabb0-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cabb0-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="cabb0-145">supportsScopeTags</span></span>|<span data-ttu-id="cabb0-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="cabb0-146">Boolean</span></span>|<span data-ttu-id="cabb0-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="cabb0-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="cabb0-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="cabb0-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="cabb0-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="cabb0-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="cabb0-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="cabb0-150">This property is read-only.</span></span> <span data-ttu-id="cabb0-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cabb0-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="cabb0-152">createdDateTime</span></span>|<span data-ttu-id="cabb0-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="cabb0-153">DateTimeOffset</span></span>|<span data-ttu-id="cabb0-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="cabb0-154">DateTime the object was created.</span></span> <span data-ttu-id="cabb0-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cabb0-156">description</span><span class="sxs-lookup"><span data-stu-id="cabb0-156">description</span></span>|<span data-ttu-id="cabb0-157">String</span><span class="sxs-lookup"><span data-stu-id="cabb0-157">String</span></span>|<span data-ttu-id="cabb0-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="cabb0-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="cabb0-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cabb0-160">displayName</span><span class="sxs-lookup"><span data-stu-id="cabb0-160">displayName</span></span>|<span data-ttu-id="cabb0-161">String</span><span class="sxs-lookup"><span data-stu-id="cabb0-161">String</span></span>|<span data-ttu-id="cabb0-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="cabb0-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="cabb0-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cabb0-164">version</span><span class="sxs-lookup"><span data-stu-id="cabb0-164">version</span></span>|<span data-ttu-id="cabb0-165">Int32</span><span class="sxs-lookup"><span data-stu-id="cabb0-165">Int32</span></span>|<span data-ttu-id="cabb0-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="cabb0-166">Version of the device configuration.</span></span> <span data-ttu-id="cabb0-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="cabb0-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cabb0-168">authenticationMethod</span></span>|[<span data-ttu-id="cabb0-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="cabb0-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="cabb0-170">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="cabb0-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="cabb0-171">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="cabb0-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="cabb0-172">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="cabb0-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="cabb0-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="cabb0-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="cabb0-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="cabb0-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="cabb0-175">应为同步的时间电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="cabb0-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="cabb0-176">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="cabb0-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="cabb0-177">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。</span><span class="sxs-lookup"><span data-stu-id="cabb0-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="cabb0-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="cabb0-178">emailAddressSource</span></span>|[<span data-ttu-id="cabb0-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="cabb0-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="cabb0-180">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="cabb0-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="cabb0-181">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="cabb0-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="cabb0-182">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="cabb0-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="cabb0-183">hostName</span><span class="sxs-lookup"><span data-stu-id="cabb0-183">hostName</span></span>|<span data-ttu-id="cabb0-184">String</span><span class="sxs-lookup"><span data-stu-id="cabb0-184">String</span></span>|<span data-ttu-id="cabb0-185">Exchange 位置 (URL) 的邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="cabb0-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="cabb0-186">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="cabb0-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="cabb0-187">requireSsl</span></span>|<span data-ttu-id="cabb0-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="cabb0-188">Boolean</span></span>|<span data-ttu-id="cabb0-189">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="cabb0-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="cabb0-190">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="cabb0-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="cabb0-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="cabb0-191">usernameSource</span></span>|[<span data-ttu-id="cabb0-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="cabb0-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="cabb0-193">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="cabb0-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="cabb0-194">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="cabb0-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="cabb0-195">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="cabb0-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="cabb0-196">响应</span><span class="sxs-lookup"><span data-stu-id="cabb0-196">Response</span></span>
<span data-ttu-id="cabb0-197">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cabb0-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cabb0-198">示例</span><span class="sxs-lookup"><span data-stu-id="cabb0-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="cabb0-199">请求</span><span class="sxs-lookup"><span data-stu-id="cabb0-199">Request</span></span>
<span data-ttu-id="cabb0-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cabb0-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 481

{
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

### <a name="response"></a><span data-ttu-id="cabb0-201">响应</span><span class="sxs-lookup"><span data-stu-id="cabb0-201">Response</span></span>
<span data-ttu-id="cabb0-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cabb0-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





