---
title: 更新 androidForWorkGmailEasConfiguration
description: 更新 androidForWorkGmailEasConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: abc27004134882b74d4149d70bcaff4f6c920ba3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960417"
---
# <a name="update-androidforworkgmaileasconfiguration"></a><span data-ttu-id="67e75-103">更新 androidForWorkGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="67e75-103">Update androidForWorkGmailEasConfiguration</span></span>

> <span data-ttu-id="67e75-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="67e75-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67e75-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67e75-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67e75-106">更新[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="67e75-106">Update the properties of a [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67e75-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="67e75-107">Prerequisites</span></span>
<span data-ttu-id="67e75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67e75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67e75-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="67e75-110">Permission type</span></span>|<span data-ttu-id="67e75-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="67e75-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67e75-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67e75-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67e75-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67e75-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="67e75-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67e75-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67e75-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="67e75-115">Not supported.</span></span>|
|<span data-ttu-id="67e75-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="67e75-116">Application</span></span>|<span data-ttu-id="67e75-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="67e75-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67e75-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67e75-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="67e75-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="67e75-119">Request headers</span></span>
|<span data-ttu-id="67e75-120">标头</span><span class="sxs-lookup"><span data-stu-id="67e75-120">Header</span></span>|<span data-ttu-id="67e75-121">值</span><span class="sxs-lookup"><span data-stu-id="67e75-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67e75-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67e75-122">Authorization</span></span>|<span data-ttu-id="67e75-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="67e75-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67e75-124">接受</span><span class="sxs-lookup"><span data-stu-id="67e75-124">Accept</span></span>|<span data-ttu-id="67e75-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67e75-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67e75-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="67e75-126">Request body</span></span>
<span data-ttu-id="67e75-127">在请求正文中, 提供[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67e75-127">In the request body, supply a JSON representation for the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object.</span></span>

<span data-ttu-id="67e75-128">下表显示创建[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="67e75-128">The following table shows the properties that are required when you create the [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md).</span></span>

|<span data-ttu-id="67e75-129">属性</span><span class="sxs-lookup"><span data-stu-id="67e75-129">Property</span></span>|<span data-ttu-id="67e75-130">类型</span><span class="sxs-lookup"><span data-stu-id="67e75-130">Type</span></span>|<span data-ttu-id="67e75-131">说明</span><span class="sxs-lookup"><span data-stu-id="67e75-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67e75-132">id</span><span class="sxs-lookup"><span data-stu-id="67e75-132">id</span></span>|<span data-ttu-id="67e75-133">String</span><span class="sxs-lookup"><span data-stu-id="67e75-133">String</span></span>|<span data-ttu-id="67e75-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="67e75-134">Key of the entity.</span></span> <span data-ttu-id="67e75-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67e75-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="67e75-136">lastModifiedDateTime</span></span>|<span data-ttu-id="67e75-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67e75-137">DateTimeOffset</span></span>|<span data-ttu-id="67e75-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="67e75-138">DateTime the object was last modified.</span></span> <span data-ttu-id="67e75-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67e75-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="67e75-140">roleScopeTagIds</span></span>|<span data-ttu-id="67e75-141">String 集合</span><span class="sxs-lookup"><span data-stu-id="67e75-141">String collection</span></span>|<span data-ttu-id="67e75-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="67e75-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="67e75-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67e75-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="67e75-144">supportsScopeTags</span></span>|<span data-ttu-id="67e75-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="67e75-145">Boolean</span></span>|<span data-ttu-id="67e75-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="67e75-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="67e75-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="67e75-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="67e75-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="67e75-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="67e75-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="67e75-149">This property is read-only.</span></span> <span data-ttu-id="67e75-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67e75-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="67e75-151">createdDateTime</span></span>|<span data-ttu-id="67e75-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="67e75-152">DateTimeOffset</span></span>|<span data-ttu-id="67e75-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="67e75-153">DateTime the object was created.</span></span> <span data-ttu-id="67e75-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67e75-155">description</span><span class="sxs-lookup"><span data-stu-id="67e75-155">description</span></span>|<span data-ttu-id="67e75-156">String</span><span class="sxs-lookup"><span data-stu-id="67e75-156">String</span></span>|<span data-ttu-id="67e75-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="67e75-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="67e75-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67e75-159">displayName</span><span class="sxs-lookup"><span data-stu-id="67e75-159">displayName</span></span>|<span data-ttu-id="67e75-160">String</span><span class="sxs-lookup"><span data-stu-id="67e75-160">String</span></span>|<span data-ttu-id="67e75-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="67e75-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="67e75-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67e75-163">version</span><span class="sxs-lookup"><span data-stu-id="67e75-163">version</span></span>|<span data-ttu-id="67e75-164">Int32</span><span class="sxs-lookup"><span data-stu-id="67e75-164">Int32</span></span>|<span data-ttu-id="67e75-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="67e75-165">Version of the device configuration.</span></span> <span data-ttu-id="67e75-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="67e75-167">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="67e75-167">authenticationMethod</span></span>|[<span data-ttu-id="67e75-168">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="67e75-168">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="67e75-169">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="67e75-169">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="67e75-170">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="67e75-170">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="67e75-171">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="67e75-171">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="67e75-172">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="67e75-172">durationOfEmailToSync</span></span>|[<span data-ttu-id="67e75-173">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="67e75-173">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="67e75-174">应将电子邮件同步到的时间段。</span><span class="sxs-lookup"><span data-stu-id="67e75-174">Duration of time email should be synced to.</span></span> <span data-ttu-id="67e75-175">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="67e75-175">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="67e75-176">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth` 或 `unlimited`。</span><span class="sxs-lookup"><span data-stu-id="67e75-176">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="67e75-177">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="67e75-177">emailAddressSource</span></span>|[<span data-ttu-id="67e75-178">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="67e75-178">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="67e75-179">在设备上安装之前, 从 AAD 中选出并插入到此配置文件中的电子邮件属性。</span><span class="sxs-lookup"><span data-stu-id="67e75-179">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="67e75-180">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="67e75-180">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="67e75-181">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="67e75-181">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="67e75-182">hostName</span><span class="sxs-lookup"><span data-stu-id="67e75-182">hostName</span></span>|<span data-ttu-id="67e75-183">String</span><span class="sxs-lookup"><span data-stu-id="67e75-183">String</span></span>|<span data-ttu-id="67e75-184">邮件应用程序连接到的 Exchange 位置 (URL)。</span><span class="sxs-lookup"><span data-stu-id="67e75-184">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="67e75-185">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-185">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="67e75-186">requireSsl</span><span class="sxs-lookup"><span data-stu-id="67e75-186">requireSsl</span></span>|<span data-ttu-id="67e75-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="67e75-187">Boolean</span></span>|<span data-ttu-id="67e75-188">指示是否使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="67e75-188">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="67e75-189">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="67e75-189">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="67e75-190">usernameSource</span><span class="sxs-lookup"><span data-stu-id="67e75-190">usernameSource</span></span>|[<span data-ttu-id="67e75-191">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="67e75-191">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="67e75-192">在设备上安装之前, 从 AAD 中选取并插入到此配置文件中的 Username 属性。</span><span class="sxs-lookup"><span data-stu-id="67e75-192">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="67e75-193">继承自[androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="67e75-193">Inherited from [androidForWorkEasEmailProfileBase](../resources/intune-deviceconfig-androidforworkeasemailprofilebase.md).</span></span> <span data-ttu-id="67e75-194">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="67e75-194">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="67e75-195">响应</span><span class="sxs-lookup"><span data-stu-id="67e75-195">Response</span></span>
<span data-ttu-id="67e75-196">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67e75-196">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGmailEasConfiguration](../resources/intune-deviceconfig-androidforworkgmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67e75-197">示例</span><span class="sxs-lookup"><span data-stu-id="67e75-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="67e75-198">请求</span><span class="sxs-lookup"><span data-stu-id="67e75-198">Request</span></span>
<span data-ttu-id="67e75-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67e75-199">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 491

{
  "@odata.type": "#microsoft.graph.androidForWorkGmailEasConfiguration",
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

### <a name="response"></a><span data-ttu-id="67e75-200">响应</span><span class="sxs-lookup"><span data-stu-id="67e75-200">Response</span></span>
<span data-ttu-id="67e75-p116">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67e75-p116">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




