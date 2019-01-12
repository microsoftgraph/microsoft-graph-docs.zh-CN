---
title: 更新 androidForWorkGmailEasConfiguration
description: 更新 androidForWorkGmailEasConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ccd2b967e80ef5635087cdf3547fca93be64c53
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983406"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="14ea6-103">更新 androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="14ea6-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="14ea6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="14ea6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="14ea6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="14ea6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14ea6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="14ea6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="14ea6-107">更新[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="14ea6-107">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="14ea6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="14ea6-108">Prerequisites</span></span>
<span data-ttu-id="14ea6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="14ea6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14ea6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="14ea6-111">Permission type</span></span>|<span data-ttu-id="14ea6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="14ea6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14ea6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14ea6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14ea6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14ea6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="14ea6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14ea6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14ea6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="14ea6-116">Not supported.</span></span>|
|<span data-ttu-id="14ea6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="14ea6-117">Application</span></span>|<span data-ttu-id="14ea6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="14ea6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14ea6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14ea6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="14ea6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="14ea6-120">Request headers</span></span>
|<span data-ttu-id="14ea6-121">标头</span><span class="sxs-lookup"><span data-stu-id="14ea6-121">Header</span></span>|<span data-ttu-id="14ea6-122">值</span><span class="sxs-lookup"><span data-stu-id="14ea6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14ea6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14ea6-123">Authorization</span></span>|<span data-ttu-id="14ea6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="14ea6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14ea6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14ea6-125">Accept</span></span>|<span data-ttu-id="14ea6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14ea6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14ea6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="14ea6-127">Request body</span></span>
<span data-ttu-id="14ea6-128">在请求正文中，提供[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14ea6-128">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="14ea6-129">下表显示时创建[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="14ea6-129">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="14ea6-130">属性</span><span class="sxs-lookup"><span data-stu-id="14ea6-130">Property</span></span>|<span data-ttu-id="14ea6-131">类型</span><span class="sxs-lookup"><span data-stu-id="14ea6-131">Type</span></span>|<span data-ttu-id="14ea6-132">说明</span><span class="sxs-lookup"><span data-stu-id="14ea6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14ea6-133">id</span><span class="sxs-lookup"><span data-stu-id="14ea6-133">id</span></span>|<span data-ttu-id="14ea6-134">String</span><span class="sxs-lookup"><span data-stu-id="14ea6-134">String</span></span>|<span data-ttu-id="14ea6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="14ea6-135">Key of the entity.</span></span> <span data-ttu-id="14ea6-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14ea6-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="14ea6-137">lastModifiedDateTime</span></span>|<span data-ttu-id="14ea6-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14ea6-138">DateTimeOffset</span></span>|<span data-ttu-id="14ea6-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="14ea6-139">DateTime the object was last modified.</span></span> <span data-ttu-id="14ea6-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14ea6-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="14ea6-141">roleScopeTagIds</span></span>|<span data-ttu-id="14ea6-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="14ea6-142">String collection</span></span>|<span data-ttu-id="14ea6-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="14ea6-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="14ea6-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14ea6-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="14ea6-145">supportsScopeTags</span></span>|<span data-ttu-id="14ea6-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="14ea6-146">Boolean</span></span>|<span data-ttu-id="14ea6-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="14ea6-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="14ea6-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="14ea6-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="14ea6-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="14ea6-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="14ea6-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="14ea6-150">This property is read-only.</span></span> <span data-ttu-id="14ea6-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14ea6-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="14ea6-152">createdDateTime</span></span>|<span data-ttu-id="14ea6-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="14ea6-153">DateTimeOffset</span></span>|<span data-ttu-id="14ea6-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="14ea6-154">DateTime the object was created.</span></span> <span data-ttu-id="14ea6-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14ea6-156">description</span><span class="sxs-lookup"><span data-stu-id="14ea6-156">description</span></span>|<span data-ttu-id="14ea6-157">String</span><span class="sxs-lookup"><span data-stu-id="14ea6-157">String</span></span>|<span data-ttu-id="14ea6-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="14ea6-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="14ea6-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14ea6-160">displayName</span><span class="sxs-lookup"><span data-stu-id="14ea6-160">displayName</span></span>|<span data-ttu-id="14ea6-161">String</span><span class="sxs-lookup"><span data-stu-id="14ea6-161">String</span></span>|<span data-ttu-id="14ea6-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="14ea6-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="14ea6-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14ea6-164">version</span><span class="sxs-lookup"><span data-stu-id="14ea6-164">version</span></span>|<span data-ttu-id="14ea6-165">Int32</span><span class="sxs-lookup"><span data-stu-id="14ea6-165">Int32</span></span>|<span data-ttu-id="14ea6-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="14ea6-166">Version of the device configuration.</span></span> <span data-ttu-id="14ea6-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="14ea6-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="14ea6-168">authenticationMethod</span></span>|[<span data-ttu-id="14ea6-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="14ea6-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="14ea6-170">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="14ea6-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="14ea6-171">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="14ea6-171">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="14ea6-172">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="14ea6-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="14ea6-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="14ea6-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="14ea6-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="14ea6-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="14ea6-175">应为同步的时间电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="14ea6-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="14ea6-176">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="14ea6-176">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="14ea6-177">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。</span><span class="sxs-lookup"><span data-stu-id="14ea6-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="14ea6-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="14ea6-178">emailAddressSource</span></span>|[<span data-ttu-id="14ea6-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="14ea6-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="14ea6-180">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="14ea6-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="14ea6-181">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="14ea6-181">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="14ea6-182">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="14ea6-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="14ea6-183">hostName</span><span class="sxs-lookup"><span data-stu-id="14ea6-183">hostName</span></span>|<span data-ttu-id="14ea6-184">String</span><span class="sxs-lookup"><span data-stu-id="14ea6-184">String</span></span>|<span data-ttu-id="14ea6-185">Exchange 位置 (URL) 的邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="14ea6-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="14ea6-186">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-186">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="14ea6-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="14ea6-187">requireSsl</span></span>|<span data-ttu-id="14ea6-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="14ea6-188">Boolean</span></span>|<span data-ttu-id="14ea6-189">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="14ea6-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="14ea6-190">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="14ea6-190">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="14ea6-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="14ea6-191">usernameSource</span></span>|[<span data-ttu-id="14ea6-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="14ea6-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="14ea6-193">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="14ea6-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="14ea6-194">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="14ea6-194">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="14ea6-195">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="14ea6-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="14ea6-196">响应</span><span class="sxs-lookup"><span data-stu-id="14ea6-196">Response</span></span>
<span data-ttu-id="14ea6-197">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="14ea6-197">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14ea6-198">示例</span><span class="sxs-lookup"><span data-stu-id="14ea6-198">Example</span></span>
### <a name="request"></a><span data-ttu-id="14ea6-199">请求</span><span class="sxs-lookup"><span data-stu-id="14ea6-199">Request</span></span>
<span data-ttu-id="14ea6-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14ea6-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="14ea6-201">响应</span><span class="sxs-lookup"><span data-stu-id="14ea6-201">Response</span></span>
<span data-ttu-id="14ea6-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14ea6-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





