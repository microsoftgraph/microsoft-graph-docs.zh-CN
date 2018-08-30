# <a name="create-manageddevice"></a><span data-ttu-id="80a68-101">创建 managedDevice</span><span class="sxs-lookup"><span data-stu-id="80a68-101">Create managedDevice</span></span>

> <span data-ttu-id="80a68-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80a68-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80a68-103">创建新的 [managedDevice](../resources/intune_devices_manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80a68-103">Create a new [managedDevice](../resources/intune_devices_manageddevice.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80a68-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="80a68-104">Prerequisites</span></span>
<span data-ttu-id="80a68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="80a68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="80a68-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="80a68-107">Permission type</span></span>|<span data-ttu-id="80a68-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80a68-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80a68-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80a68-109">Delegated (work or school account)</span></span>|<span data-ttu-id="80a68-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80a68-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="80a68-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80a68-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80a68-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="80a68-112">Not supported.</span></span>|
|<span data-ttu-id="80a68-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="80a68-113">Application</span></span>|<span data-ttu-id="80a68-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="80a68-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80a68-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80a68-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices
POST /deviceManagement/managedDevices
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices
```

## <a name="request-headers"></a><span data-ttu-id="80a68-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="80a68-116">Request headers</span></span>
|<span data-ttu-id="80a68-117">标头</span><span class="sxs-lookup"><span data-stu-id="80a68-117">Header</span></span>|<span data-ttu-id="80a68-118">值</span><span class="sxs-lookup"><span data-stu-id="80a68-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80a68-119">授权</span><span class="sxs-lookup"><span data-stu-id="80a68-119">Authorization</span></span>|<span data-ttu-id="80a68-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80a68-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80a68-121">接受</span><span class="sxs-lookup"><span data-stu-id="80a68-121">Accept</span></span>|<span data-ttu-id="80a68-122">application/json</span><span class="sxs-lookup"><span data-stu-id="80a68-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80a68-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="80a68-123">Request body</span></span>
<span data-ttu-id="80a68-124">在请求正文中，提供 managedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80a68-124">In the request body, supply a JSON representation for the managedDevice object.</span></span>

<span data-ttu-id="80a68-125">下表显示创建 managedDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="80a68-125">The following table shows the properties that are required when you create the managedDevice.</span></span>

|<span data-ttu-id="80a68-126">属性</span><span class="sxs-lookup"><span data-stu-id="80a68-126">Property</span></span>|<span data-ttu-id="80a68-127">类型</span><span class="sxs-lookup"><span data-stu-id="80a68-127">Type</span></span>|<span data-ttu-id="80a68-128">说明</span><span class="sxs-lookup"><span data-stu-id="80a68-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80a68-129">id</span><span class="sxs-lookup"><span data-stu-id="80a68-129">id</span></span>|<span data-ttu-id="80a68-130">String</span><span class="sxs-lookup"><span data-stu-id="80a68-130">String</span></span>|<span data-ttu-id="80a68-131">设备唯一标识符</span><span class="sxs-lookup"><span data-stu-id="80a68-131">Unique Identifier for the device</span></span>|
|<span data-ttu-id="80a68-132">userId</span><span class="sxs-lookup"><span data-stu-id="80a68-132">userId</span></span>|<span data-ttu-id="80a68-133">String</span><span class="sxs-lookup"><span data-stu-id="80a68-133">String</span></span>|<span data-ttu-id="80a68-134">与设备关联的用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="80a68-134">Unique Identifier for the user associated with the device</span></span>|
|<span data-ttu-id="80a68-135">deviceName</span><span class="sxs-lookup"><span data-stu-id="80a68-135">deviceName</span></span>|<span data-ttu-id="80a68-136">String</span><span class="sxs-lookup"><span data-stu-id="80a68-136">String</span></span>|<span data-ttu-id="80a68-137">设备的名称</span><span class="sxs-lookup"><span data-stu-id="80a68-137">Name of the device</span></span>|
|<span data-ttu-id="80a68-138">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="80a68-138">managedDeviceOwnerType</span></span>|[<span data-ttu-id="80a68-139">managedDeviceOwnerType</span><span class="sxs-lookup"><span data-stu-id="80a68-139">managedDeviceOwnerType</span></span>](../resources/intune_devices_manageddeviceownertype.md)|<span data-ttu-id="80a68-140">设备的所有权。</span><span class="sxs-lookup"><span data-stu-id="80a68-140">Ownership of the device.</span></span> <span data-ttu-id="80a68-141">可以是“company”或“personal”。</span><span class="sxs-lookup"><span data-stu-id="80a68-141">Can be 'company' or 'personal'.</span></span> <span data-ttu-id="80a68-142">可取值为：`unknown`、`company`、`personal`。</span><span class="sxs-lookup"><span data-stu-id="80a68-142">The possible values are `unknown`, `company`, `personal`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="80a68-143">deviceActionResults</span><span class="sxs-lookup"><span data-stu-id="80a68-143">deviceActionResults</span></span>|<span data-ttu-id="80a68-144">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) 集合</span><span class="sxs-lookup"><span data-stu-id="80a68-144">[deviceActionResult](../resources/intune_devices_deviceactionresult.md) collection</span></span>|<span data-ttu-id="80a68-145">ComplexType deviceActionResult 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="80a68-145">List of ComplexType deviceActionResult objects.</span></span>|
|<span data-ttu-id="80a68-146">enrolledDateTime</span><span class="sxs-lookup"><span data-stu-id="80a68-146">enrolledDateTime</span></span>|<span data-ttu-id="80a68-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a68-147">DateTimeOffset</span></span>|<span data-ttu-id="80a68-148">设备的注册时间。</span><span class="sxs-lookup"><span data-stu-id="80a68-148">Enrollment time of the device.</span></span>|
|<span data-ttu-id="80a68-149">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="80a68-149">lastSyncDateTime</span></span>|<span data-ttu-id="80a68-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a68-150">DateTimeOffset</span></span>|<span data-ttu-id="80a68-151">设备上次成功完成与 Intune 同步的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="80a68-151">The date and time that the device last completed a successful sync with Intune.</span></span>|
|<span data-ttu-id="80a68-152">operatingSystem</span><span class="sxs-lookup"><span data-stu-id="80a68-152">operatingSystem</span></span>|<span data-ttu-id="80a68-153">String</span><span class="sxs-lookup"><span data-stu-id="80a68-153">String</span></span>|<span data-ttu-id="80a68-154">设备的操作系统。</span><span class="sxs-lookup"><span data-stu-id="80a68-154">Operating system of the device.</span></span> <span data-ttu-id="80a68-155">Windows、iOS 等。</span><span class="sxs-lookup"><span data-stu-id="80a68-155">Windows, iOS, etc.</span></span>|
|<span data-ttu-id="80a68-156">complianceState</span><span class="sxs-lookup"><span data-stu-id="80a68-156">complianceState</span></span>|[<span data-ttu-id="80a68-157">complianceState</span><span class="sxs-lookup"><span data-stu-id="80a68-157">complianceState</span></span>](../resources/intune_devices_compliancestate.md)|<span data-ttu-id="80a68-158">设备的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="80a68-158">Compliance state of the device.</span></span> <span data-ttu-id="80a68-159">可取值为：`unknown`、`compliant`、`noncompliant`、`conflict`、`error`、`inGracePeriod`、`configManager`。</span><span class="sxs-lookup"><span data-stu-id="80a68-159">The possible values are `unknown`, `compliant`, `noncompliant`, `conflict`, `error`, `inGracePeriod`, `configManager`, , , , , or .</span></span>|
|<span data-ttu-id="80a68-160">jailBroken</span><span class="sxs-lookup"><span data-stu-id="80a68-160">jailBroken</span></span>|<span data-ttu-id="80a68-161">String</span><span class="sxs-lookup"><span data-stu-id="80a68-161">String</span></span>|<span data-ttu-id="80a68-162">设备是否已越狱或取得 root 权限。</span><span class="sxs-lookup"><span data-stu-id="80a68-162">whether the device is jail broken or rooted.</span></span>|
|<span data-ttu-id="80a68-163">managementAgent</span><span class="sxs-lookup"><span data-stu-id="80a68-163">managementAgent</span></span>|[<span data-ttu-id="80a68-164">managementAgentType</span><span class="sxs-lookup"><span data-stu-id="80a68-164">managementAgentType</span></span>](../resources/intune_devices_managementagenttype.md)|<span data-ttu-id="80a68-165">设备的管理通道。</span><span class="sxs-lookup"><span data-stu-id="80a68-165">Management channel of the device.</span></span> <span data-ttu-id="80a68-166">Intune、EAS 等。可取值为：`eas`、`mdm`、`easMdm`、`intuneClient`、`easIntuneClient`、`configurationManagerClient`、`configurationManagerClientMdm`、`configurationManagerClientMdmEas`、`unknown`、`jamf`、`googleCloudDevicePolicyController`。</span><span class="sxs-lookup"><span data-stu-id="80a68-166">Intune, EAS, etc. Possible values are: `eas`, `mdm`, `easMdm`, `intuneClient`, `easIntuneClient`, `configurationManagerClient`, `configurationManagerClientMdm`, `configurationManagerClientMdmEas`, `unknown`, `jamf`, `googleCloudDevicePolicyController`.</span></span>|
|<span data-ttu-id="80a68-167">osVersion</span><span class="sxs-lookup"><span data-stu-id="80a68-167">osVersion</span></span>|<span data-ttu-id="80a68-168">String</span><span class="sxs-lookup"><span data-stu-id="80a68-168">String</span></span>|<span data-ttu-id="80a68-169">设备的操作系统版本。</span><span class="sxs-lookup"><span data-stu-id="80a68-169">Operating system version of the device.</span></span>|
|<span data-ttu-id="80a68-170">easActivated</span><span class="sxs-lookup"><span data-stu-id="80a68-170">easActivated</span></span>|<span data-ttu-id="80a68-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a68-171">Boolean</span></span>|<span data-ttu-id="80a68-172">设备是否已激活 Exchange ActiveSync。</span><span class="sxs-lookup"><span data-stu-id="80a68-172">Whether the device is Exchange ActiveSync activated.</span></span>|
|<span data-ttu-id="80a68-173">easDeviceId</span><span class="sxs-lookup"><span data-stu-id="80a68-173">easDeviceId</span></span>|<span data-ttu-id="80a68-174">String</span><span class="sxs-lookup"><span data-stu-id="80a68-174">String</span></span>|<span data-ttu-id="80a68-175">设备的 Exchange ActiveSync ID。</span><span class="sxs-lookup"><span data-stu-id="80a68-175">Exchange ActiveSync Id of the device.</span></span>|
|<span data-ttu-id="80a68-176">easActivationDateTime</span><span class="sxs-lookup"><span data-stu-id="80a68-176">easActivationDateTime</span></span>|<span data-ttu-id="80a68-177">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a68-177">DateTimeOffset</span></span>|<span data-ttu-id="80a68-178">设备的 Exchange ActivationSync 激活时间。</span><span class="sxs-lookup"><span data-stu-id="80a68-178">Exchange ActivationSync activation time of the device.</span></span>|
|<span data-ttu-id="80a68-179">azureADRegistered</span><span class="sxs-lookup"><span data-stu-id="80a68-179">azureADRegistered</span></span>|<span data-ttu-id="80a68-180">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a68-180">Boolean</span></span>|<span data-ttu-id="80a68-181">设备是否已注册 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="80a68-181">Whether the device is Azure Active Directory registered.</span></span>|
|<span data-ttu-id="80a68-182">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="80a68-182">deviceEnrollmentType</span></span>|[<span data-ttu-id="80a68-183">deviceEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="80a68-183">deviceEnrollmentType</span></span>](../resources/intune_shared_deviceenrollmenttype.md)|<span data-ttu-id="80a68-184">设备的注册类型。</span><span class="sxs-lookup"><span data-stu-id="80a68-184">Enrollment type of the device.</span></span> <span data-ttu-id="80a68-185">可取值为：`unknown`、`userEnrollment`、`deviceEnrollmentManager`、`appleBulkWithUser`、`appleBulkWithoutUser`、`windowsAzureADJoin`、`windowsBulkUserless`、`windowsAutoEnrollment`、`windowsBulkAzureDomainJoin`、`windowsCoManagement`。</span><span class="sxs-lookup"><span data-stu-id="80a68-185">The possible values are `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`, , or .</span></span>|
|<span data-ttu-id="80a68-186">activationLockBypassCode</span><span class="sxs-lookup"><span data-stu-id="80a68-186">activationLockBypassCode</span></span>|<span data-ttu-id="80a68-187">String</span><span class="sxs-lookup"><span data-stu-id="80a68-187">String</span></span>|<span data-ttu-id="80a68-188">允许绕过设备上的激活锁的代码。</span><span class="sxs-lookup"><span data-stu-id="80a68-188">Code that allows the Activation Lock on a device to be bypassed.</span></span>|
|<span data-ttu-id="80a68-189">emailAddress</span><span class="sxs-lookup"><span data-stu-id="80a68-189">emailAddress</span></span>|<span data-ttu-id="80a68-190">String</span><span class="sxs-lookup"><span data-stu-id="80a68-190">String</span></span>|<span data-ttu-id="80a68-191">与设备关联的用户的电子邮件。</span><span class="sxs-lookup"><span data-stu-id="80a68-191">Email(s) for the user associated with the device</span></span>|
|<span data-ttu-id="80a68-192">azureADDeviceId</span><span class="sxs-lookup"><span data-stu-id="80a68-192">azureADDeviceId</span></span>|<span data-ttu-id="80a68-193">String</span><span class="sxs-lookup"><span data-stu-id="80a68-193">String</span></span>|<span data-ttu-id="80a68-194">Azure Active Directory 设备的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="80a68-194">The unique identifier for the Azure Active Directory device.</span></span> <span data-ttu-id="80a68-195">只读。</span><span class="sxs-lookup"><span data-stu-id="80a68-195">Read only.</span></span>|
|<span data-ttu-id="80a68-196">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="80a68-196">deviceRegistrationState</span></span>|[<span data-ttu-id="80a68-197">deviceRegistrationState</span><span class="sxs-lookup"><span data-stu-id="80a68-197">deviceRegistrationState</span></span>](../resources/intune_devices_deviceregistrationstate.md)|<span data-ttu-id="80a68-198">设备注册状态。</span><span class="sxs-lookup"><span data-stu-id="80a68-198">Device registration state.</span></span> <span data-ttu-id="80a68-199">可取值为：`notRegistered`、`registered`、`revoked`、`keyConflict`、`approvalPending`、`certificateReset`、`notRegisteredPendingEnrollment`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="80a68-199">The possible values are `notRegistered`, `registered`, `revoked`, `keyConflict`, `approvalPending`, `certificateReset`, `notRegisteredPendingEnrollment`, `unknown`, , , , or .</span></span>|
|<span data-ttu-id="80a68-200">deviceCategoryDisplayName</span><span class="sxs-lookup"><span data-stu-id="80a68-200">deviceCategoryDisplayName</span></span>|<span data-ttu-id="80a68-201">String</span><span class="sxs-lookup"><span data-stu-id="80a68-201">String</span></span>|<span data-ttu-id="80a68-202">设备类别显示名称。</span><span class="sxs-lookup"><span data-stu-id="80a68-202">Device category display name</span></span>|
|<span data-ttu-id="80a68-203">isSupervised</span><span class="sxs-lookup"><span data-stu-id="80a68-203">isSupervised</span></span>|<span data-ttu-id="80a68-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a68-204">Boolean</span></span>|<span data-ttu-id="80a68-205">设备受监督状态</span><span class="sxs-lookup"><span data-stu-id="80a68-205">Device supervised status</span></span>|
|<span data-ttu-id="80a68-206">exchangeLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="80a68-206">exchangeLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="80a68-207">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a68-207">DateTimeOffset</span></span>|<span data-ttu-id="80a68-208">设备上次与 Exchange 联系的时间。</span><span class="sxs-lookup"><span data-stu-id="80a68-208">Last time the device contacted Exchange.</span></span>|
|<span data-ttu-id="80a68-209">exchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="80a68-209">exchangeAccessState</span></span>|[<span data-ttu-id="80a68-210">deviceManagementExchangeAccessState</span><span class="sxs-lookup"><span data-stu-id="80a68-210">deviceManagementExchangeAccessState</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstate.md)|<span data-ttu-id="80a68-211">Exchange 中设备的访问状态。</span><span class="sxs-lookup"><span data-stu-id="80a68-211">The Access State of the device in Exchange.</span></span> <span data-ttu-id="80a68-212">可取值为：`none`、`unknown`、`allowed`、`blocked`、`quarantined`。</span><span class="sxs-lookup"><span data-stu-id="80a68-212">The possible values are `none`, `unknown`, `allowed`, `blocked`, `quarantined`, , , , , , , or .</span></span>|
|<span data-ttu-id="80a68-213">exchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="80a68-213">exchangeAccessStateReason</span></span>|[<span data-ttu-id="80a68-214">deviceManagementExchangeAccessStateReason</span><span class="sxs-lookup"><span data-stu-id="80a68-214">deviceManagementExchangeAccessStateReason</span></span>](../resources/intune_devices_devicemanagementexchangeaccessstatereason.md)|<span data-ttu-id="80a68-215">Exchange 中设备访问状态的出现原因。</span><span class="sxs-lookup"><span data-stu-id="80a68-215">The reason for the device's access state in Exchange.</span></span> <span data-ttu-id="80a68-216">可取值为：`none`、`unknown`、`exchangeGlobalRule`、`exchangeIndividualRule`、`exchangeDeviceRule`、`exchangeUpgrade`、`exchangeMailboxPolicy`、`other`、`compliant`、`notCompliant`、`notEnrolled`、`unknownLocation`、`mfaRequired`、`azureADBlockDueToAccessPolicy`、`compromisedPassword`、`deviceNotKnownWithManagedApp`。</span><span class="sxs-lookup"><span data-stu-id="80a68-216">The possible values are: `none`, `unknown`, `exchangeGlobalRule`, `exchangeIndividualRule`, `exchangeDeviceRule`, `exchangeUpgrade`, `exchangeMailboxPolicy`, `other`, `compliant`, `notCompliant`, `notEnrolled`, `unknownLocation`, `mfaRequired`, `azureADBlockDueToAccessPolicy`, `compromisedPassword`, `deviceNotKnownWithManagedApp`.</span></span>|
|<span data-ttu-id="80a68-217">remoteAssistanceSessionUrl</span><span class="sxs-lookup"><span data-stu-id="80a68-217">remoteAssistanceSessionUrl</span></span>|<span data-ttu-id="80a68-218">String</span><span class="sxs-lookup"><span data-stu-id="80a68-218">String</span></span>|<span data-ttu-id="80a68-219">允许与设备建立远程协助会话的 URL。</span><span class="sxs-lookup"><span data-stu-id="80a68-219">Url that allows a Remote Assistance session to be established with the device.</span></span>|
|<span data-ttu-id="80a68-220">remoteAssistanceSessionErrorDetails</span><span class="sxs-lookup"><span data-stu-id="80a68-220">remoteAssistanceSessionErrorDetails</span></span>|<span data-ttu-id="80a68-221">String</span><span class="sxs-lookup"><span data-stu-id="80a68-221">String</span></span>|<span data-ttu-id="80a68-222">用于在创建远程协助会话对象时识别问题的错误字符串。</span><span class="sxs-lookup"><span data-stu-id="80a68-222">An error string that identifies issues when creating Remote Assistance session objects.</span></span>|
|<span data-ttu-id="80a68-223">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="80a68-223">isEncrypted</span></span>|<span data-ttu-id="80a68-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="80a68-224">Boolean</span></span>|<span data-ttu-id="80a68-225">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="80a68-225">Device encryption status</span></span>|
|<span data-ttu-id="80a68-226">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="80a68-226">userPrincipalName</span></span>|<span data-ttu-id="80a68-227">String</span><span class="sxs-lookup"><span data-stu-id="80a68-227">String</span></span>|<span data-ttu-id="80a68-228">设备用户主体名称</span><span class="sxs-lookup"><span data-stu-id="80a68-228">Device user principal name</span></span>|
|<span data-ttu-id="80a68-229">model</span><span class="sxs-lookup"><span data-stu-id="80a68-229">model</span></span>|<span data-ttu-id="80a68-230">String</span><span class="sxs-lookup"><span data-stu-id="80a68-230">String</span></span>|<span data-ttu-id="80a68-231">设备的型号</span><span class="sxs-lookup"><span data-stu-id="80a68-231">Model of the device</span></span>|
|<span data-ttu-id="80a68-232">manufacturer</span><span class="sxs-lookup"><span data-stu-id="80a68-232">manufacturer</span></span>|<span data-ttu-id="80a68-233">String</span><span class="sxs-lookup"><span data-stu-id="80a68-233">String</span></span>|<span data-ttu-id="80a68-234">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="80a68-234">Manufacturer of the device</span></span>|
|<span data-ttu-id="80a68-235">imei</span><span class="sxs-lookup"><span data-stu-id="80a68-235">imei</span></span>|<span data-ttu-id="80a68-236">String</span><span class="sxs-lookup"><span data-stu-id="80a68-236">String</span></span>|<span data-ttu-id="80a68-237">IMEI</span><span class="sxs-lookup"><span data-stu-id="80a68-237">IMEI</span></span>|
|<span data-ttu-id="80a68-238">complianceGracePeriodExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="80a68-238">complianceGracePeriodExpirationDateTime</span></span>|<span data-ttu-id="80a68-239">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a68-239">DateTimeOffset</span></span>|<span data-ttu-id="80a68-240">设备符合性宽限期的到期日期/时间</span><span class="sxs-lookup"><span data-stu-id="80a68-240">The DateTime when device compliance grace period expires</span></span>|
|<span data-ttu-id="80a68-241">serialNumber</span><span class="sxs-lookup"><span data-stu-id="80a68-241">serialNumber</span></span>|<span data-ttu-id="80a68-242">String</span><span class="sxs-lookup"><span data-stu-id="80a68-242">String</span></span>|<span data-ttu-id="80a68-243">序列号</span><span class="sxs-lookup"><span data-stu-id="80a68-243">SerialNumber</span></span>|
|<span data-ttu-id="80a68-244">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="80a68-244">phoneNumber</span></span>|<span data-ttu-id="80a68-245">String</span><span class="sxs-lookup"><span data-stu-id="80a68-245">String</span></span>|<span data-ttu-id="80a68-246">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="80a68-246">Phone number of the device</span></span>|
|<span data-ttu-id="80a68-247">androidSecurityPatchLevel</span><span class="sxs-lookup"><span data-stu-id="80a68-247">androidSecurityPatchLevel</span></span>|<span data-ttu-id="80a68-248">String</span><span class="sxs-lookup"><span data-stu-id="80a68-248">String</span></span>|<span data-ttu-id="80a68-249">Android 安全修补程序级别</span><span class="sxs-lookup"><span data-stu-id="80a68-249">Android security patch level</span></span>|
|<span data-ttu-id="80a68-250">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="80a68-250">userDisplayName</span></span>|<span data-ttu-id="80a68-251">String</span><span class="sxs-lookup"><span data-stu-id="80a68-251">String</span></span>|<span data-ttu-id="80a68-252">用户显示名称</span><span class="sxs-lookup"><span data-stu-id="80a68-252">User display name</span></span>|
|<span data-ttu-id="80a68-253">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="80a68-253">configurationManagerClientEnabledFeatures</span></span>|[<span data-ttu-id="80a68-254">configurationManagerClientEnabledFeatures</span><span class="sxs-lookup"><span data-stu-id="80a68-254">configurationManagerClientEnabledFeatures</span></span>](../resources/intune_devices_configurationmanagerclientenabledfeatures.md)|<span data-ttu-id="80a68-255">ConfigrMgr 客户端启用的功能</span><span class="sxs-lookup"><span data-stu-id="80a68-255">ConfigrMgr client enabled features</span></span>|
|<span data-ttu-id="80a68-256">wiFiMacAddress</span><span class="sxs-lookup"><span data-stu-id="80a68-256">wiFiMacAddress</span></span>|<span data-ttu-id="80a68-257">String</span><span class="sxs-lookup"><span data-stu-id="80a68-257">String</span></span>|<span data-ttu-id="80a68-258">Wi-Fi MAC</span><span class="sxs-lookup"><span data-stu-id="80a68-258">Wi-Fi MAC</span></span>|
|<span data-ttu-id="80a68-259">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="80a68-259">deviceHealthAttestationState</span></span>|[<span data-ttu-id="80a68-260">deviceHealthAttestationState</span><span class="sxs-lookup"><span data-stu-id="80a68-260">deviceHealthAttestationState</span></span>](../resources/intune_devices_devicehealthattestationstate.md)|<span data-ttu-id="80a68-261">设备运行状况证明状态。</span><span class="sxs-lookup"><span data-stu-id="80a68-261">The device health attestation state.</span></span>|
|<span data-ttu-id="80a68-262">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="80a68-262">subscriberCarrier</span></span>|<span data-ttu-id="80a68-263">String</span><span class="sxs-lookup"><span data-stu-id="80a68-263">String</span></span>|<span data-ttu-id="80a68-264">订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="80a68-264">Subscriber Carrier</span></span>|
|<span data-ttu-id="80a68-265">meid</span><span class="sxs-lookup"><span data-stu-id="80a68-265">meid</span></span>|<span data-ttu-id="80a68-266">String</span><span class="sxs-lookup"><span data-stu-id="80a68-266">String</span></span>|<span data-ttu-id="80a68-267">MEID</span><span class="sxs-lookup"><span data-stu-id="80a68-267">MEID</span></span>|
|<span data-ttu-id="80a68-268">totalStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="80a68-268">totalStorageSpaceInBytes</span></span>|<span data-ttu-id="80a68-269">Int64</span><span class="sxs-lookup"><span data-stu-id="80a68-269">Int64</span></span>|<span data-ttu-id="80a68-270">存储空间总字节数</span><span class="sxs-lookup"><span data-stu-id="80a68-270">Total Storage in Bytes</span></span>|
|<span data-ttu-id="80a68-271">freeStorageSpaceInBytes</span><span class="sxs-lookup"><span data-stu-id="80a68-271">freeStorageSpaceInBytes</span></span>|<span data-ttu-id="80a68-272">Int64</span><span class="sxs-lookup"><span data-stu-id="80a68-272">Int64</span></span>|<span data-ttu-id="80a68-273">可用存储空间字节数</span><span class="sxs-lookup"><span data-stu-id="80a68-273">Free Storage in Bytes</span></span>|
|<span data-ttu-id="80a68-274">managedDeviceName</span><span class="sxs-lookup"><span data-stu-id="80a68-274">managedDeviceName</span></span>|<span data-ttu-id="80a68-275">String</span><span class="sxs-lookup"><span data-stu-id="80a68-275">String</span></span>|<span data-ttu-id="80a68-276">用于识别设备的自动生成的名称。</span><span class="sxs-lookup"><span data-stu-id="80a68-276">Automatically generated name to identify a device.</span></span> <span data-ttu-id="80a68-277">可以覆盖为用户友好名称。</span><span class="sxs-lookup"><span data-stu-id="80a68-277">Can be overwritten to a user friendly name.</span></span>|
|<span data-ttu-id="80a68-278">partnerReportedThreatState</span><span class="sxs-lookup"><span data-stu-id="80a68-278">partnerReportedThreatState</span></span>|[<span data-ttu-id="80a68-279">managedDevicePartnerReportedHealthState</span><span class="sxs-lookup"><span data-stu-id="80a68-279">managedDevicePartnerReportedHealthState</span></span>](../resources/intune_devices_manageddevicepartnerreportedhealthstate.md)|<span data-ttu-id="80a68-280">指示帐户和设备正在使用移动威胁防护合作伙伴时设备的威胁状态。</span><span class="sxs-lookup"><span data-stu-id="80a68-280">Indicates the threat state of a device when a Mobile Threat Defense partner is in use by the account and device.</span></span> <span data-ttu-id="80a68-281">只读。</span><span class="sxs-lookup"><span data-stu-id="80a68-281">Read Only.</span></span> <span data-ttu-id="80a68-282">可取值为：`unknown`、`activated`、`deactivated`、`secured`、`lowSeverity`、`mediumSeverity`、`highSeverity`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="80a68-282">The possible values are `unknown`, `activated`, `deactivated`, `secured`, `lowSeverity`, `mediumSeverity`, `highSeverity`, `unresponsive`, , , , or .</span></span>|



## <a name="response"></a><span data-ttu-id="80a68-283">响应</span><span class="sxs-lookup"><span data-stu-id="80a68-283">Response</span></span>
<span data-ttu-id="80a68-284">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [managedDevice](../resources/intune_devices_manageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="80a68-284">If successful, this method returns a `201 Created` response code and a [managedDevice](../resources/intune_devices_manageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80a68-285">示例</span><span class="sxs-lookup"><span data-stu-id="80a68-285">Example</span></span>
### <a name="request"></a><span data-ttu-id="80a68-286">请求</span><span class="sxs-lookup"><span data-stu-id="80a68-286">Request</span></span>
<span data-ttu-id="80a68-287">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80a68-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices
Content-type: application/json
Content-length: 4656

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
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

### <a name="response"></a><span data-ttu-id="80a68-288">响应</span><span class="sxs-lookup"><span data-stu-id="80a68-288">Response</span></span>
<span data-ttu-id="80a68-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80a68-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 4705

{
  "@odata.type": "#microsoft.graph.managedDevice",
  "id": "705c034c-034c-705c-4c03-5c704c035c70",
  "userId": "User Id value",
  "deviceName": "Device Name value",
  "managedDeviceOwnerType": "company",
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



