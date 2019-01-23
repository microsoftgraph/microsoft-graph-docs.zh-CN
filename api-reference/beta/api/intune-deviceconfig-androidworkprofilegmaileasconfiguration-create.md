---
title: 创建 androidWorkProfileGmailEasConfiguration
description: 创建新的 androidWorkProfileGmailEasConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e849048f84d8fd962e25fa8af2e25712618431af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395235"
---
# <a name="create-androidworkprofilegmaileasconfiguration"></a><span data-ttu-id="38d4f-103">创建 androidWorkProfileGmailEasConfiguration</span><span class="sxs-lookup"><span data-stu-id="38d4f-103">Create androidWorkProfileGmailEasConfiguration</span></span>

> <span data-ttu-id="38d4f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="38d4f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="38d4f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="38d4f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="38d4f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="38d4f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="38d4f-107">创建新的[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38d4f-107">Create a new [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="38d4f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="38d4f-108">Prerequisites</span></span>
<span data-ttu-id="38d4f-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="38d4f-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="38d4f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="38d4f-111">Permission type</span></span>|<span data-ttu-id="38d4f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="38d4f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="38d4f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38d4f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="38d4f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="38d4f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="38d4f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38d4f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="38d4f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="38d4f-116">Not supported.</span></span>|
|<span data-ttu-id="38d4f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="38d4f-117">Application</span></span>|<span data-ttu-id="38d4f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="38d4f-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="38d4f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38d4f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="38d4f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="38d4f-120">Request headers</span></span>
|<span data-ttu-id="38d4f-121">标头</span><span class="sxs-lookup"><span data-stu-id="38d4f-121">Header</span></span>|<span data-ttu-id="38d4f-122">值</span><span class="sxs-lookup"><span data-stu-id="38d4f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="38d4f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="38d4f-123">Authorization</span></span>|<span data-ttu-id="38d4f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="38d4f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="38d4f-125">Accept</span><span class="sxs-lookup"><span data-stu-id="38d4f-125">Accept</span></span>|<span data-ttu-id="38d4f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38d4f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="38d4f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38d4f-127">Request body</span></span>
<span data-ttu-id="38d4f-128">在请求正文中，提供 androidWorkProfileGmailEasConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="38d4f-128">In the request body, supply a JSON representation for the androidWorkProfileGmailEasConfiguration object.</span></span>

<span data-ttu-id="38d4f-129">下表显示时创建 androidWorkProfileGmailEasConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="38d4f-129">The following table shows the properties that are required when you create the androidWorkProfileGmailEasConfiguration.</span></span>

|<span data-ttu-id="38d4f-130">属性</span><span class="sxs-lookup"><span data-stu-id="38d4f-130">Property</span></span>|<span data-ttu-id="38d4f-131">类型</span><span class="sxs-lookup"><span data-stu-id="38d4f-131">Type</span></span>|<span data-ttu-id="38d4f-132">说明</span><span class="sxs-lookup"><span data-stu-id="38d4f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="38d4f-133">id</span><span class="sxs-lookup"><span data-stu-id="38d4f-133">id</span></span>|<span data-ttu-id="38d4f-134">String</span><span class="sxs-lookup"><span data-stu-id="38d4f-134">String</span></span>|<span data-ttu-id="38d4f-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="38d4f-135">Key of the entity.</span></span> <span data-ttu-id="38d4f-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38d4f-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="38d4f-137">lastModifiedDateTime</span></span>|<span data-ttu-id="38d4f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38d4f-138">DateTimeOffset</span></span>|<span data-ttu-id="38d4f-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="38d4f-139">DateTime the object was last modified.</span></span> <span data-ttu-id="38d4f-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38d4f-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="38d4f-141">roleScopeTagIds</span></span>|<span data-ttu-id="38d4f-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="38d4f-142">String collection</span></span>|<span data-ttu-id="38d4f-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="38d4f-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="38d4f-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38d4f-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="38d4f-145">supportsScopeTags</span></span>|<span data-ttu-id="38d4f-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="38d4f-146">Boolean</span></span>|<span data-ttu-id="38d4f-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="38d4f-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="38d4f-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="38d4f-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="38d4f-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="38d4f-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="38d4f-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="38d4f-150">This property is read-only.</span></span> <span data-ttu-id="38d4f-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38d4f-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="38d4f-152">createdDateTime</span></span>|<span data-ttu-id="38d4f-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="38d4f-153">DateTimeOffset</span></span>|<span data-ttu-id="38d4f-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="38d4f-154">DateTime the object was created.</span></span> <span data-ttu-id="38d4f-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38d4f-156">description</span><span class="sxs-lookup"><span data-stu-id="38d4f-156">description</span></span>|<span data-ttu-id="38d4f-157">String</span><span class="sxs-lookup"><span data-stu-id="38d4f-157">String</span></span>|<span data-ttu-id="38d4f-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="38d4f-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="38d4f-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38d4f-160">displayName</span><span class="sxs-lookup"><span data-stu-id="38d4f-160">displayName</span></span>|<span data-ttu-id="38d4f-161">String</span><span class="sxs-lookup"><span data-stu-id="38d4f-161">String</span></span>|<span data-ttu-id="38d4f-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="38d4f-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="38d4f-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38d4f-164">version</span><span class="sxs-lookup"><span data-stu-id="38d4f-164">version</span></span>|<span data-ttu-id="38d4f-165">Int32</span><span class="sxs-lookup"><span data-stu-id="38d4f-165">Int32</span></span>|<span data-ttu-id="38d4f-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="38d4f-166">Version of the device configuration.</span></span> <span data-ttu-id="38d4f-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="38d4f-168">authenticationMethod</span><span class="sxs-lookup"><span data-stu-id="38d4f-168">authenticationMethod</span></span>|[<span data-ttu-id="38d4f-169">easAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="38d4f-169">easAuthenticationMethod</span></span>](../resources/intune-deviceconfig-easauthenticationmethod.md)|<span data-ttu-id="38d4f-170">Exchange ActiveSync 的身份验证方法。</span><span class="sxs-lookup"><span data-stu-id="38d4f-170">Authentication method for Exchange ActiveSync.</span></span> <span data-ttu-id="38d4f-171">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="38d4f-171">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="38d4f-172">可取值为：`usernameAndPassword`、`certificate`。</span><span class="sxs-lookup"><span data-stu-id="38d4f-172">Possible values are: `usernameAndPassword`, `certificate`.</span></span>|
|<span data-ttu-id="38d4f-173">durationOfEmailToSync</span><span class="sxs-lookup"><span data-stu-id="38d4f-173">durationOfEmailToSync</span></span>|[<span data-ttu-id="38d4f-174">emailSyncDuration</span><span class="sxs-lookup"><span data-stu-id="38d4f-174">emailSyncDuration</span></span>](../resources/intune-deviceconfig-emailsyncduration.md)|<span data-ttu-id="38d4f-175">应为同步的时间电子邮件持续时间。</span><span class="sxs-lookup"><span data-stu-id="38d4f-175">Duration of time email should be synced to.</span></span> <span data-ttu-id="38d4f-176">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="38d4f-176">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="38d4f-177">可取值为：`userDefined`、`oneDay`、`threeDays`、`oneWeek`、`twoWeeks`、`oneMonth`、`unlimited`。</span><span class="sxs-lookup"><span data-stu-id="38d4f-177">Possible values are: `userDefined`, `oneDay`, `threeDays`, `oneWeek`, `twoWeeks`, `oneMonth`, `unlimited`.</span></span>|
|<span data-ttu-id="38d4f-178">emailAddressSource</span><span class="sxs-lookup"><span data-stu-id="38d4f-178">emailAddressSource</span></span>|[<span data-ttu-id="38d4f-179">userEmailSource</span><span class="sxs-lookup"><span data-stu-id="38d4f-179">userEmailSource</span></span>](../resources/intune-deviceconfig-useremailsource.md)|<span data-ttu-id="38d4f-180">电子邮件是从 AAD 选取并在设备上安装之前将其插入此配置文件的属性。</span><span class="sxs-lookup"><span data-stu-id="38d4f-180">Email attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="38d4f-181">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="38d4f-181">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="38d4f-182">可取值为：`userPrincipalName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="38d4f-182">Possible values are: `userPrincipalName`, `primarySmtpAddress`.</span></span>|
|<span data-ttu-id="38d4f-183">hostName</span><span class="sxs-lookup"><span data-stu-id="38d4f-183">hostName</span></span>|<span data-ttu-id="38d4f-184">String</span><span class="sxs-lookup"><span data-stu-id="38d4f-184">String</span></span>|<span data-ttu-id="38d4f-185">Exchange 位置 (URL) 的邮件应用程序连接到。</span><span class="sxs-lookup"><span data-stu-id="38d4f-185">Exchange location (URL) that the mail app connects to.</span></span> <span data-ttu-id="38d4f-186">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-186">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="38d4f-187">requireSsl</span><span class="sxs-lookup"><span data-stu-id="38d4f-187">requireSsl</span></span>|<span data-ttu-id="38d4f-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="38d4f-188">Boolean</span></span>|<span data-ttu-id="38d4f-189">指示使用 SSL。</span><span class="sxs-lookup"><span data-stu-id="38d4f-189">Indicates whether or not to use SSL.</span></span> <span data-ttu-id="38d4f-190">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="38d4f-190">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)</span></span>|
|<span data-ttu-id="38d4f-191">usernameSource</span><span class="sxs-lookup"><span data-stu-id="38d4f-191">usernameSource</span></span>|[<span data-ttu-id="38d4f-192">androidUsernameSource</span><span class="sxs-lookup"><span data-stu-id="38d4f-192">androidUsernameSource</span></span>](../resources/intune-deviceconfig-androidusernamesource.md)|<span data-ttu-id="38d4f-193">Username 属性是从 AAD 选取并在设备上安装之前将其插入此配置文件。</span><span class="sxs-lookup"><span data-stu-id="38d4f-193">Username attribute that is picked from AAD and injected into this profile before installing on the device.</span></span> <span data-ttu-id="38d4f-194">继承自[androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md)。</span><span class="sxs-lookup"><span data-stu-id="38d4f-194">Inherited from [androidWorkProfileEasEmailProfileBase](../resources/intune-deviceconfig-androidworkprofileeasemailprofilebase.md).</span></span> <span data-ttu-id="38d4f-195">可取值为：`username`、`userPrincipalName`、`samAccountName`、`primarySmtpAddress`。</span><span class="sxs-lookup"><span data-stu-id="38d4f-195">Possible values are: `username`, `userPrincipalName`, `samAccountName`, `primarySmtpAddress`.</span></span>|



## <a name="response"></a><span data-ttu-id="38d4f-196">响应</span><span class="sxs-lookup"><span data-stu-id="38d4f-196">Response</span></span>
<span data-ttu-id="38d4f-197">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38d4f-197">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGmailEasConfiguration](../resources/intune-deviceconfig-androidworkprofilegmaileasconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="38d4f-198">示例</span><span class="sxs-lookup"><span data-stu-id="38d4f-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="38d4f-199">请求</span><span class="sxs-lookup"><span data-stu-id="38d4f-199">Request</span></span>
<span data-ttu-id="38d4f-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="38d4f-200">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="38d4f-201">响应</span><span class="sxs-lookup"><span data-stu-id="38d4f-201">Response</span></span>
<span data-ttu-id="38d4f-p117">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38d4f-p117">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




