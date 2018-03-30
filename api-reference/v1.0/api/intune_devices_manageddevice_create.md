# <a name="create-manageddevice"></a><span data-ttu-id="24da5-101">创建 managedDevice</span><span class="sxs-lookup"><span data-stu-id="24da5-101">Create managedDevice</span></span>

> <span data-ttu-id="24da5-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="24da5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24da5-103">创建新的 [managedDevice](../resources/intune_devices_manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24da5-103">Create a new [plannerBucket](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24da5-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="24da5-104">Prerequisites</span></span>
<span data-ttu-id="24da5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="24da5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="24da5-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="24da5-107">Permission type</span></span>|<span data-ttu-id="24da5-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24da5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24da5-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24da5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="24da5-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24da5-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="24da5-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24da5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24da5-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="24da5-112">Not supported.</span></span>|
|<span data-ttu-id="24da5-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="24da5-113">Application</span></span>|<span data-ttu-id="24da5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24da5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24da5-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24da5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="24da5-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="24da5-116">Request headers</span></span>
|<span data-ttu-id="24da5-117">标头</span><span class="sxs-lookup"><span data-stu-id="24da5-117">Header</span></span>|<span data-ttu-id="24da5-118">值</span><span class="sxs-lookup"><span data-stu-id="24da5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24da5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="24da5-119">Authorization</span></span>|<span data-ttu-id="24da5-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24da5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="24da5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="24da5-121">Accept</span></span>|<span data-ttu-id="24da5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="24da5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24da5-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="24da5-123">Request body</span></span>
<span data-ttu-id="24da5-124">在请求正文中，提供 managedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24da5-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="24da5-125">下表显示创建 managedDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="24da5-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="24da5-126">属性</span><span class="sxs-lookup"><span data-stu-id="24da5-126">Property</span></span>|<span data-ttu-id="24da5-127">类型</span><span class="sxs-lookup"><span data-stu-id="24da5-127">Type</span></span>|<span data-ttu-id="24da5-128">说明</span><span class="sxs-lookup"><span data-stu-id="24da5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24da5-129">id</span><span class="sxs-lookup"><span data-stu-id="24da5-129">id</span></span>|<span data-ttu-id="24da5-130">String</span><span class="sxs-lookup"><span data-stu-id="24da5-130">String</span></span>|<span data-ttu-id="24da5-131">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="24da5-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="24da5-132">userId</span><span class="sxs-lookup"><span data-stu-id="24da5-132">userID</span></span>|<span data-ttu-id="24da5-133">String</span><span class="sxs-lookup"><span data-stu-id="24da5-133">String</span></span>|<span data-ttu-id="24da5-134">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="24da5-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="24da5-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="24da5-135">deviceName</span></span>|<span data-ttu-id="24da5-136">String</span><span class="sxs-lookup"><span data-stu-id="24da5-136">String</span></span>|<span data-ttu-id="24da5-137">设备的名称</span><span class="sxs-lookup"><span data-stu-id="24da5-137">Name of the device</span></span>|
|<span data-ttu-id="24da5-138">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="24da5-138">deviceActionResults</span></span>|<span data-ttu-id="24da5-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="24da5-139">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="24da5-140">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="24da5-140">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="24da5-141">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="24da5-141">enrolledDateTime</span></span>|<span data-ttu-id="24da5-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24da5-142">DateTimeOffset</span></span>|<span data-ttu-id="24da5-143">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="24da5-143">Enrollment time of the device.</span></span>|
|<span data-ttu-id="24da5-144">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="24da5-144">lastSyncDateTime</span></span>|<span data-ttu-id="24da5-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24da5-145">DateTimeOffset</span></span>|<span data-ttu-id="24da5-146">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="24da5-146">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="24da5-147">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="24da5-147">operatingSystem</span></span>|<span data-ttu-id="24da5-148">String</span><span class="sxs-lookup"><span data-stu-id="24da5-148">String</span></span>|<span data-ttu-id="24da5-149">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="24da5-149">Operating system of the device.</span></span> <span data-ttu-id="24da5-150">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="24da5-150">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="24da5-151">complianceState</span><span class="sxs-lookup"><span data-stu-id="24da5-151">complianceState</span></span>|<span data-ttu-id="24da5-152">String</span><span class="sxs-lookup"><span data-stu-id="24da5-152">String</span></span>|<span data-ttu-id="24da5-153">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="24da5-153">Compliance state of the device.</span></span> <span data-ttu-id="24da5-154">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="24da5-154">Possible values are: `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`.</span></span>|
|<span data-ttu-id="24da5-155">jailBroken</span><span class="sxs-lookup"><span data-stu-id="24da5-155">jailBroken</span></span>|<span data-ttu-id="24da5-156">String</span><span class="sxs-lookup"><span data-stu-id="24da5-156">String</span></span>|<span data-ttu-id="24da5-157">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="24da5-157">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="24da5-158">managementAgent</span><span class="sxs-lookup"><span data-stu-id="24da5-158">managementAgent</span></span>|<span data-ttu-id="24da5-159">String</span><span class="sxs-lookup"><span data-stu-id="24da5-159">String</span></span>|<span data-ttu-id="24da5-160">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="24da5-160">Management channel of the device.</span></span> <span data-ttu-id="24da5-161">Intune、EAS 等。可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。</span><span class="sxs-lookup"><span data-stu-id="24da5-161">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="24da5-162">osVersion</span><span class="sxs-lookup"><span data-stu-id="24da5-162">osVersion</span></span>|<span data-ttu-id="24da5-163">String</span><span class="sxs-lookup"><span data-stu-id="24da5-163">String</span></span>|<span data-ttu-id="24da5-164">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="24da5-164">Operating system version of the device.</span></span>|
|<span data-ttu-id="24da5-165">easActivated</span><span class="sxs-lookup"><span data-stu-id="24da5-165">easActivated</span></span>|<span data-ttu-id="24da5-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="24da5-166">Boolean</span></span>|<span data-ttu-id="24da5-167">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="24da5-167">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="24da5-168">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="24da5-168">easDeviceId</span></span>|<span data-ttu-id="24da5-169">String</span><span class="sxs-lookup"><span data-stu-id="24da5-169">String</span></span>|<span data-ttu-id="24da5-170">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="24da5-170">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="24da5-171">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="24da5-171">easActivationDateTime</span></span>|<span data-ttu-id="24da5-172">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24da5-172">DateTimeOffset</span></span>|<span data-ttu-id="24da5-173">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="24da5-173">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="24da5-174">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="24da5-174">azureADRegistered</span></span>|<span data-ttu-id="24da5-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="24da5-175">Boolean</span></span>|<span data-ttu-id="24da5-176">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="24da5-176">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="24da5-177">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="24da5-177">deviceEnrollmentType</span></span>|<span data-ttu-id="24da5-178">String</span><span class="sxs-lookup"><span data-stu-id="24da5-178">String</span></span>|<span data-ttu-id="24da5-179">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="24da5-179">Enrollment type of the device.</span></span> <span data-ttu-id="24da5-180">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="24da5-180">Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.</span></span>|
|<span data-ttu-id="24da5-181">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="24da5-181">activationLockBypassCode</span></span>|<span data-ttu-id="24da5-182">String</span><span class="sxs-lookup"><span data-stu-id="24da5-182">String</span></span>|<span data-ttu-id="24da5-183">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="24da5-183">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="24da5-184">emailAddress</span><span class="sxs-lookup"><span data-stu-id="24da5-184">emailAddress</span></span>|<span data-ttu-id="24da5-185">String</span><span class="sxs-lookup"><span data-stu-id="24da5-185">String</span></span>|<span data-ttu-id="24da5-186">与设备关联的用户的电子邮件</span><span class="sxs-lookup"><span data-stu-id="24da5-186">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="24da5-187">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="24da5-187">azureADDeviceId</span></span>|<span data-ttu-id="24da5-188">String</span><span class="sxs-lookup"><span data-stu-id="24da5-188">String</span></span>|<span data-ttu-id="24da5-189">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="24da5-189">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="24da5-190">只读。</span><span class="sxs-lookup"><span data-stu-id="24da5-190">Read only.</span></span>|
|<span data-ttu-id="24da5-191">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="24da5-191">deviceRegistrationState</span></span>|<span data-ttu-id="24da5-192">String</span><span class="sxs-lookup"><span data-stu-id="24da5-192">String</span></span>|<span data-ttu-id="24da5-193">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="24da5-193">Device registration state.</span></span> <span data-ttu-id="24da5-194">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="24da5-194">Possible values are: `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`.</span></span>|
|<span data-ttu-id="24da5-195">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="24da5-195">deviceCategoryDisplayName</span></span>|<span data-ttu-id="24da5-196">String</span><span class="sxs-lookup"><span data-stu-id="24da5-196">String</span></span>|<span data-ttu-id="24da5-197">设备类别显示名称</span><span class="sxs-lookup"><span data-stu-id="24da5-197">Device category display name</span></span>|
|<span data-ttu-id="24da5-198">isSupervised</span><span class="sxs-lookup"><span data-stu-id="24da5-198">isSupervised</span></span>|<span data-ttu-id="24da5-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="24da5-199">Boolean</span></span>|<span data-ttu-id="24da5-200">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="24da5-200">Device supervised status</span></span>|
|<span data-ttu-id="24da5-201">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="24da5-201">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="24da5-202">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24da5-202">DateTimeOffset</span></span>|<span data-ttu-id="24da5-203">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="24da5-203">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="24da5-204">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="24da5-204">exchangeAccessState</span></span>|<span data-ttu-id="24da5-205">String</span><span class="sxs-lookup"><span data-stu-id="24da5-205">String</span></span>|<span data-ttu-id="24da5-206">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="24da5-206">The Access State of the device in Exchange.</span></span> <span data-ttu-id="24da5-207">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="24da5-207">Possible values are: `none`, `unknown`, `allowed`, `blocked`, `quarantined`.</span></span>|
|<span data-ttu-id="24da5-208">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="24da5-208">exchangeAccessStateReason</span></span>|<span data-ttu-id="24da5-209">String</span><span class="sxs-lookup"><span data-stu-id="24da5-209">String</span></span>|<span data-ttu-id="24da5-210">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="24da5-210">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="24da5-211">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="24da5-211">Possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="24da5-212">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="24da5-212">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="24da5-213">String</span><span class="sxs-lookup"><span data-stu-id="24da5-213">String</span></span>|<span data-ttu-id="24da5-214">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="24da5-214">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="24da5-215">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="24da5-215">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="24da5-216">String</span><span class="sxs-lookup"><span data-stu-id="24da5-216">String</span></span>|<span data-ttu-id="24da5-217">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="24da5-217">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="24da5-218">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="24da5-218">isEncrypted</span></span>|<span data-ttu-id="24da5-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="24da5-219">Boolean</span></span>|<span data-ttu-id="24da5-220">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="24da5-220">Device encryption status</span></span>|
|<span data-ttu-id="24da5-221">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="24da5-221">userPrincipalName</span></span>|<span data-ttu-id="24da5-222">String</span><span class="sxs-lookup"><span data-stu-id="24da5-222">String</span></span>|<span data-ttu-id="24da5-223">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="24da5-223">Device user principal name</span></span>|
|<span data-ttu-id="24da5-224">model</span><span class="sxs-lookup"><span data-stu-id="24da5-224">model</span></span>|<span data-ttu-id="24da5-225">String</span><span class="sxs-lookup"><span data-stu-id="24da5-225">String</span></span>|<span data-ttu-id="24da5-226">设备的型号</span><span class="sxs-lookup"><span data-stu-id="24da5-226">Model of the device</span></span>|
|<span data-ttu-id="24da5-227">manufacturer</span><span class="sxs-lookup"><span data-stu-id="24da5-227">Camera manufacturer.</span></span>|<span data-ttu-id="24da5-228">String</span><span class="sxs-lookup"><span data-stu-id="24da5-228">String</span></span>|<span data-ttu-id="24da5-229">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="24da5-229">Manufacturer of the device</span></span>|
|<span data-ttu-id="24da5-230">imei</span><span class="sxs-lookup"><span data-stu-id="24da5-230">imei</span></span>|<span data-ttu-id="24da5-231">String</span><span class="sxs-lookup"><span data-stu-id="24da5-231">String</span></span>|<span data-ttu-id="24da5-232">IMEI</span><span class="sxs-lookup"><span data-stu-id="24da5-232">IMEI</span></span>|
|<span data-ttu-id="24da5-233">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="24da5-233">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="24da5-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24da5-234">DateTimeOffset</span></span>|<span data-ttu-id="24da5-235">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="24da5-235">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="24da5-236">serialNumber</span><span class="sxs-lookup"><span data-stu-id="24da5-236">serialNumber</span></span>|<span data-ttu-id="24da5-237">String</span><span class="sxs-lookup"><span data-stu-id="24da5-237">String</span></span>|<span data-ttu-id="24da5-238">序列号</span><span class="sxs-lookup"><span data-stu-id="24da5-238">SerialNumber Property</span></span>|
|<span data-ttu-id="24da5-239">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="24da5-239">PhoneNumber</span></span>|<span data-ttu-id="24da5-240">String</span><span class="sxs-lookup"><span data-stu-id="24da5-240">String</span></span>|<span data-ttu-id="24da5-241">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="24da5-241">Phone number of the device</span></span>|
|<span data-ttu-id="24da5-242">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="24da5-242">androidSecurityPatchLevel</span></span>|<span data-ttu-id="24da5-243">String</span><span class="sxs-lookup"><span data-stu-id="24da5-243">String</span></span>|<span data-ttu-id="24da5-244">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="24da5-244">Android security patch level</span></span>|
|<span data-ttu-id="24da5-245">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="24da5-245">userDisplayName</span></span>|<span data-ttu-id="24da5-246">String</span><span class="sxs-lookup"><span data-stu-id="24da5-246">String</span></span>|<span data-ttu-id="24da5-247">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="24da5-247">user display name</span></span>|
|<span data-ttu-id="24da5-248">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="24da5-248">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="24da5-249">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="24da5-249">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="24da5-250">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="24da5-250">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="24da5-251">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="24da5-251">wiFiMacAddress</span></span>|<span data-ttu-id="24da5-252">String</span><span class="sxs-lookup"><span data-stu-id="24da5-252">String</span></span>|<span data-ttu-id="24da5-253">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="24da5-253">Wi-Fi MAC</span></span>|
|<span data-ttu-id="24da5-254">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="24da5-254">deviceHealthAttestationState</span></span>|[<span data-ttu-id="24da5-255">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="24da5-255">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="24da5-256">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="24da5-256">The device health attestation state.</span></span>|
|<span data-ttu-id="24da5-257">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="24da5-257">subscriberCarrier</span></span>|<span data-ttu-id="24da5-258">String</span><span class="sxs-lookup"><span data-stu-id="24da5-258">String</span></span>|<span data-ttu-id="24da5-259">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="24da5-259">Subscriber Carrier</span></span>|
|<span data-ttu-id="24da5-260">meid</span><span class="sxs-lookup"><span data-stu-id="24da5-260">meid</span></span>|<span data-ttu-id="24da5-261">String</span><span class="sxs-lookup"><span data-stu-id="24da5-261">String</span></span>|<span data-ttu-id="24da5-262">MEID</span><span class="sxs-lookup"><span data-stu-id="24da5-262">MEID</span></span>|
|<span data-ttu-id="24da5-263">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="24da5-263">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="24da5-264">Int64</span><span class="sxs-lookup"><span data-stu-id="24da5-264">Int64</span></span>|<span data-ttu-id="24da5-265">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="24da5-265">Total Storage in Bytes</span></span>|
|<span data-ttu-id="24da5-266">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="24da5-266">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="24da5-267">Int64</span><span class="sxs-lookup"><span data-stu-id="24da5-267">Int64</span></span>|<span data-ttu-id="24da5-268">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="24da5-268">Free Storage in Bytes</span></span>|
|<span data-ttu-id="24da5-269">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="24da5-269">managedDeviceName</span></span>|<span data-ttu-id="24da5-270">String</span><span class="sxs-lookup"><span data-stu-id="24da5-270">String</span></span>|<span data-ttu-id="24da5-271">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="24da5-271">Automatically generated name to identify a device.</span></span> <span data-ttu-id="24da5-272">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="24da5-272">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="24da5-273">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="24da5-273">partnerReportedThreatState</span></span>|<span data-ttu-id="24da5-274">String</span><span class="sxs-lookup"><span data-stu-id="24da5-274">String</span></span>|<span data-ttu-id="24da5-275">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="24da5-275">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="24da5-276">只读。</span><span class="sxs-lookup"><span data-stu-id="24da5-276">Read Only</span></span> <span data-ttu-id="24da5-277">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="24da5-277">Possible values are: `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`.</span></span>|



## <a name="response"></a><span data-ttu-id="24da5-278">响应</span><span class="sxs-lookup"><span data-stu-id="24da5-278">Response</span></span>
<span data-ttu-id="24da5-279">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedDevice](../resources/intune_devices_manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24da5-279">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24da5-280">示例</span><span class="sxs-lookup"><span data-stu-id="24da5-280">Example</span></span>
### <a name="request"></a><span data-ttu-id="24da5-281">请求</span><span class="sxs-lookup"><span data-stu-id="24da5-281">Request</span></span>
<span data-ttu-id="24da5-282">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24da5-282">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4616

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```

### <a name="response"></a><span data-ttu-id="24da5-283">响应</span><span class="sxs-lookup"><span data-stu-id="24da5-283">Response</span></span>
<span data-ttu-id="24da5-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24da5-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4665

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "deviceActionResults": [
    {
      "@odata.type": "microsoft.graph.deviceActionResult",
      "actionName": "Action Name value",
      "actionState": "pending",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
    }
  ],
  "enrolledDateTime": "2016-12-31T23:59:43.797191-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "operatingSystem": "Operating System value",
  "complianceState": "compliant",
  "jailBroken": "Jail Broken value",
  "managementAgent": "mdm",
  "osVersion": "Os Version value",
  "easActivated": true,
  "easDeviceId": "Eas Device Id value",
  "easActivationDateTime": "2016-12-31T23:59:43.4878784-08:00",
  "azureADRegistered": true,
  "deviceEnrollmentType": "userEnrollment",
  "activationLockBypassCode": "Activation Lock Bypass Code value",
  "emailAddress": "Email Address value",
  "azureADDeviceId": "Azure ADDevice Id value",
  "deviceRegistrationState": "registered",
  "deviceCategoryDisplayName": "Device Category Display Name value",
  "isSupervised": true,
  "exchangeLastSuccessfulSyncDateTime": "2017-01-01T00:00:45.8803083-08:00",
  "exchangeAccessState": "unknown",
  "exchangeAccessStateReason": "unknown",
  "remoteAssistanceSessionUrl": "https://example.com/remoteAssistanceSessionUrl/",
  "remoteAssistanceSessionErrorDetails": "Remote Assistance Session Error Details value",
  "isEncrypted": true,
  "userPrincipalName": "User Principal Name value",
  "model": "Model value",
  "manufacturer": "Manufacturer value",
  "imei": "Imei value",
  "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
  "serialNumber": "Serial Number value",
  "phoneNumber": "Phone Number value",
  "androidSecurityPatchLevel": "Android Security Patch Level value",
  "userDisplayName": "User Display Name value",
  "configurationManagerClientEnabledFeatures": {
    "@odata.type": "microsoft.graph.configurationManagerClientEnabledFeatures",
    "inventory": true,
    "modernApps": true,
    "resourceAccess": true,
    "deviceConfiguration": true,
    "compliancePolicy": true,
    "windowsUpdateForBusiness": true
  },
  "wiFiMacAddress": "Wi Fi Mac Address value",
  "deviceHealthAttestationState": {
    "@odata.type": "microsoft.graph.deviceHealthAttestationState",
    "lastUpdateDateTime": "Last Update Date Time value",
    "contentNamespaceUrl": "https://example.com/contentNamespaceUrl/",
    "deviceHealthAttestationStatus": "Device Health Attestation Status value",
    "contentVersion": "Content Version value",
    "issuedDateTime": "2016-12-31T23:58:22.1231038-08:00",
    "attestationIdentityKey": "Attestation Identity Key value",
    "resetCount": 10,
    "restartCount": 12,
    "dataExcutionPolicy": "Data Excution Policy value",
    "bitLockerStatus": "Bit Locker Status value",
    "bootManagerVersion": "Boot Manager Version value",
    "codeIntegrityCheckVersion": "Code Integrity Check Version value",
    "secureBoot": "Secure Boot value",
    "bootDebugging": "Boot Debugging value",
    "operatingSystemKernelDebugging": "Operating System Kernel Debugging value",
    "codeIntegrity": "Code Integrity value",
    "testSigning": "Test Signing value",
    "safeMode": "Safe Mode value",
    "windowsPE": "Windows PE value",
    "earlyLaunchAntiMalwareDriverProtection": "Early Launch Anti Malware Driver Protection value",
    "virtualSecureMode": "Virtual Secure Mode value",
    "pcrHashAlgorithm": "Pcr Hash Algorithm value",
    "bootAppSecurityVersion": "Boot App Security Version value",
    "bootManagerSecurityVersion": "Boot Manager Security Version value",
    "tpmVersion": "Tpm Version value",
    "pcr0": "Pcr0 value",
    "secureBootConfigurationPolicyFingerPrint": "Secure Boot Configuration Policy Finger Print value",
    "codeIntegrityPolicy": "Code Integrity Policy value",
    "bootRevisionListInfo": "Boot Revision List Info value",
    "operatingSystemRevListInfo": "Operating System Rev List Info value",
    "healthStatusMismatchInfo": "Health Status Mismatch Info value",
    "healthAttestationSupportedStatus": "Health Attestation Supported Status value"
  },
  "subscriberCarrier": "Subscriber Carrier value",
  "meid": "Meid value",
  "totalStorageSpaceInBytes": 8,
  "freeStorageSpaceInBytes": 7,
  "managedDeviceName": "Managed Device Name value",
  "partnerReportedThreatState": "activated"
}
```



