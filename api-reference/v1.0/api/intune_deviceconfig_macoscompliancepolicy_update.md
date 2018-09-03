# <a name="update-macoscompliancepolicy"></a><span data-ttu-id="3f0d4-101">更新 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="3f0d4-101">Update macOSCompliancePolicy</span></span>

> <span data-ttu-id="3f0d4-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3f0d4-103">更新 [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-103">Update the properties of a [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3f0d4-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="3f0d4-104">Prerequisites</span></span>
<span data-ttu-id="3f0d4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="3f0d4-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="3f0d4-107">Permission type</span></span>|<span data-ttu-id="3f0d4-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3f0d4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3f0d4-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3f0d4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="3f0d4-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3f0d4-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3f0d4-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3f0d4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3f0d4-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-112">Not supported.</span></span>|
|<span data-ttu-id="3f0d4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="3f0d4-113">Application</span></span>|<span data-ttu-id="3f0d4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3f0d4-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3f0d4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="3f0d4-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="3f0d4-116">Request headers</span></span>
|<span data-ttu-id="3f0d4-117">标头</span><span class="sxs-lookup"><span data-stu-id="3f0d4-117">Header</span></span>|<span data-ttu-id="3f0d4-118">值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3f0d4-119">授权</span><span class="sxs-lookup"><span data-stu-id="3f0d4-119">Authorization</span></span>|<span data-ttu-id="3f0d4-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3f0d4-121">接受</span><span class="sxs-lookup"><span data-stu-id="3f0d4-121">Accept</span></span>|<span data-ttu-id="3f0d4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="3f0d4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3f0d4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="3f0d4-123">Request body</span></span>
<span data-ttu-id="3f0d4-124">在请求正文中，提供 [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-124">In the request body, supply a JSON representation for the [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>

<span data-ttu-id="3f0d4-125">下表显示创建 [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-125">The following table shows the properties that are required when you create the [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md).</span></span>

|<span data-ttu-id="3f0d4-126">属性</span><span class="sxs-lookup"><span data-stu-id="3f0d4-126">Property</span></span>|<span data-ttu-id="3f0d4-127">类型</span><span class="sxs-lookup"><span data-stu-id="3f0d4-127">Type</span></span>|<span data-ttu-id="3f0d4-128">说明</span><span class="sxs-lookup"><span data-stu-id="3f0d4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f0d4-129">ID</span><span class="sxs-lookup"><span data-stu-id="3f0d4-129">id</span></span>|<span data-ttu-id="3f0d4-130">字符串</span><span class="sxs-lookup"><span data-stu-id="3f0d4-130">String</span></span>|<span data-ttu-id="3f0d4-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-131">Key of the entity.</span></span> <span data-ttu-id="3f0d4-132">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3f0d4-132">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f0d4-133">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3f0d4-133">createdDateTime</span></span>|<span data-ttu-id="3f0d4-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f0d4-134">DateTimeOffset</span></span>|<span data-ttu-id="3f0d4-135">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-135">DateTime the object was created.</span></span> <span data-ttu-id="3f0d4-136">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3f0d4-136">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f0d4-137">说明</span><span class="sxs-lookup"><span data-stu-id="3f0d4-137">description</span></span>|<span data-ttu-id="3f0d4-138">字符串</span><span class="sxs-lookup"><span data-stu-id="3f0d4-138">String</span></span>|<span data-ttu-id="3f0d4-139">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-139">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3f0d4-140">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3f0d4-140">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f0d4-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3f0d4-141">lastModifiedDateTime</span></span>|<span data-ttu-id="3f0d4-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f0d4-142">DateTimeOffset</span></span>|<span data-ttu-id="3f0d4-143">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-143">DateTime the object was last modified.</span></span> <span data-ttu-id="3f0d4-144">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3f0d4-144">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f0d4-145">displayName</span><span class="sxs-lookup"><span data-stu-id="3f0d4-145">displayName</span></span>|<span data-ttu-id="3f0d4-146">字符串</span><span class="sxs-lookup"><span data-stu-id="3f0d4-146">String</span></span>|<span data-ttu-id="3f0d4-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3f0d4-148">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3f0d4-148">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f0d4-149">版本</span><span class="sxs-lookup"><span data-stu-id="3f0d4-149">version</span></span>|<span data-ttu-id="3f0d4-150">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d4-150">Int32</span></span>|<span data-ttu-id="3f0d4-151">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-151">Version of the device configuration.</span></span> <span data-ttu-id="3f0d4-152">继承自 [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span><span class="sxs-lookup"><span data-stu-id="3f0d4-152">Inherited from [deviceCompliancePolicy](../resources/intune_deviceconfig_devicecompliancepolicy.md)</span></span>|
|<span data-ttu-id="3f0d4-153">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="3f0d4-153">passwordRequired</span></span>|<span data-ttu-id="3f0d4-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-154">Boolean</span></span>|<span data-ttu-id="3f0d4-155">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-155">Whether or not to require a password.</span></span>|
|<span data-ttu-id="3f0d4-156">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="3f0d4-156">passwordBlockSimple</span></span>|<span data-ttu-id="3f0d4-157">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-157">Boolean</span></span>|<span data-ttu-id="3f0d4-158">指示是否阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-158">Indicates whether or not to block simple passwords.</span></span>|
|<span data-ttu-id="3f0d4-159">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="3f0d4-159">passwordExpirationDays</span></span>|<span data-ttu-id="3f0d4-160">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d4-160">Int32</span></span>|<span data-ttu-id="3f0d4-161">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-161">Number of days before the password expires.</span></span> <span data-ttu-id="3f0d4-162">有效值为 1 至 65535</span><span class="sxs-lookup"><span data-stu-id="3f0d4-162">Valid values 1 to 65535</span></span>|
|<span data-ttu-id="3f0d4-163">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="3f0d4-163">passwordMinimumLength</span></span>|<span data-ttu-id="3f0d4-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d4-164">Int32</span></span>|<span data-ttu-id="3f0d4-165">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-165">Minimum length of password.</span></span> <span data-ttu-id="3f0d4-166">有效值为 4 至 14</span><span class="sxs-lookup"><span data-stu-id="3f0d4-166">Valid values 4 to 14</span></span>|
|<span data-ttu-id="3f0d4-167">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="3f0d4-167">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="3f0d4-168">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d4-168">Int32</span></span>|<span data-ttu-id="3f0d4-169">在需要密码之前不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-169">Minutes of inactivity before a password is required.</span></span>|
|<span data-ttu-id="3f0d4-170">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="3f0d4-170">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="3f0d4-171">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d4-171">Int32</span></span>|<span data-ttu-id="3f0d4-172">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-172">Number of previous passwords to block.</span></span> <span data-ttu-id="3f0d4-173">有效值为 1 至 24</span><span class="sxs-lookup"><span data-stu-id="3f0d4-173">Valid values 1 to 24</span></span>|
|<span data-ttu-id="3f0d4-174">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="3f0d4-174">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="3f0d4-175">Int32</span><span class="sxs-lookup"><span data-stu-id="3f0d4-175">Int32</span></span>|<span data-ttu-id="3f0d4-176">密码中必需的字符集数。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-176">The number of character sets required in the password.</span></span>|
|<span data-ttu-id="3f0d4-177">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="3f0d4-177">passwordRequiredType</span></span>|[<span data-ttu-id="3f0d4-178">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="3f0d4-178">requiredPasswordType</span></span>](../resources/intune_deviceconfig_requiredpasswordtype.md)|<span data-ttu-id="3f0d4-179">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-179">The required password type.</span></span> <span data-ttu-id="3f0d4-180">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-180">The possible values are `deviceDefault`, `alphanumeric`, `numeric`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="3f0d4-181">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="3f0d4-181">osMinimumVersion</span></span>|<span data-ttu-id="3f0d4-182">字符串</span><span class="sxs-lookup"><span data-stu-id="3f0d4-182">String</span></span>|<span data-ttu-id="3f0d4-183">最低 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-183">Minimum IOS version.</span></span>|
|<span data-ttu-id="3f0d4-184">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="3f0d4-184">osMaximumVersion</span></span>|<span data-ttu-id="3f0d4-185">字符串</span><span class="sxs-lookup"><span data-stu-id="3f0d4-185">String</span></span>|<span data-ttu-id="3f0d4-186">最高 IOS 版本。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-186">Maximum IOS version.</span></span>|
|<span data-ttu-id="3f0d4-187">systemIntegrityProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3f0d4-187">systemIntegrityProtectionEnabled</span></span>|<span data-ttu-id="3f0d4-188">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-188">Boolean</span></span>|<span data-ttu-id="3f0d4-189">要求设备已启用系统完整性保护。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-189">Require that devices have enabled system integrity protection.</span></span>|
|<span data-ttu-id="3f0d4-190">deviceThreatProtectionEnabled</span><span class="sxs-lookup"><span data-stu-id="3f0d4-190">deviceThreatProtectionEnabled</span></span>|<span data-ttu-id="3f0d4-191">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-191">Boolean</span></span>|<span data-ttu-id="3f0d4-192">要求设备已启用设备威胁防护。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-192">Require that devices have enabled device threat protection .</span></span>|
|<span data-ttu-id="3f0d4-193">deviceThreatProtectionRequiredSecurityLevel</span><span class="sxs-lookup"><span data-stu-id="3f0d4-193">deviceThreatProtectionRequiredSecurityLevel</span></span>|[<span data-ttu-id="3f0d4-194">deviceThreatProtectionLevel</span><span class="sxs-lookup"><span data-stu-id="3f0d4-194">deviceThreatProtectionLevel</span></span>](../resources/intune_deviceconfig_devicethreatprotectionlevel.md)|<span data-ttu-id="3f0d4-195">要求按移动威胁防护最低风险级别报告不符合情况。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-195">Require Mobile Threat Protection minimum risk level to report noncompliance.</span></span> <span data-ttu-id="3f0d4-196">可取值为：`unavailable`、`secured`、`low`、`medium`、`high`、`notSet`。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-196">The possible values are `unavailable`, `secured`, `low`, `medium`, `high`, `notSet`, , , , , , or .</span></span>|
|<span data-ttu-id="3f0d4-197">storageRequireEncryption</span><span class="sxs-lookup"><span data-stu-id="3f0d4-197">storageRequireEncryption</span></span>|<span data-ttu-id="3f0d4-198">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-198">Boolean</span></span>|<span data-ttu-id="3f0d4-199">要求对 Mac OS 设备加密。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-199">Require encryption on Mac OS devices.</span></span>|
|<span data-ttu-id="3f0d4-200">firewallEnabled</span><span class="sxs-lookup"><span data-stu-id="3f0d4-200">firewallEnabled</span></span>|<span data-ttu-id="3f0d4-201">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-201">Boolean</span></span>|<span data-ttu-id="3f0d4-202">是否应启用防火墙。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-202">Whether the firewall should be enabled or not.</span></span>|
|<span data-ttu-id="3f0d4-203">firewallBlockAllIncoming</span><span class="sxs-lookup"><span data-stu-id="3f0d4-203">firewallBlockAllIncoming</span></span>|<span data-ttu-id="3f0d4-204">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-204">Boolean</span></span>|<span data-ttu-id="3f0d4-205">对应于"阻止所有传入连接"选项。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-205">Corresponds to the “Block all incoming connections” option.</span></span>|
|<span data-ttu-id="3f0d4-206">firewallEnableStealthMode</span><span class="sxs-lookup"><span data-stu-id="3f0d4-206">firewallEnableStealthMode</span></span>|<span data-ttu-id="3f0d4-207">布尔值</span><span class="sxs-lookup"><span data-stu-id="3f0d4-207">Boolean</span></span>|<span data-ttu-id="3f0d4-208">对应于"启用隐藏模式"。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-208">Corresponds to “Enable stealth mode.”</span></span>|



## <a name="response"></a><span data-ttu-id="3f0d4-209">响应</span><span class="sxs-lookup"><span data-stu-id="3f0d4-209">Response</span></span>
<span data-ttu-id="3f0d4-210">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-210">If successful, this method returns a `200 OK` response code and an updated [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3f0d4-211">示例</span><span class="sxs-lookup"><span data-stu-id="3f0d4-211">Example</span></span>
### <a name="request"></a><span data-ttu-id="3f0d4-212">请求</span><span class="sxs-lookup"><span data-stu-id="3f0d4-212">Request</span></span>
<span data-ttu-id="3f0d4-213">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-213">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
Content-type: application/json
Content-length: 853

{
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```

### <a name="response"></a><span data-ttu-id="3f0d4-214">响应</span><span class="sxs-lookup"><span data-stu-id="3f0d4-214">Response</span></span>
<span data-ttu-id="3f0d4-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3f0d4-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1021

{
  "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
  "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "version": 7,
  "passwordRequired": true,
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordMinimumCharacterSetCount": 0,
  "passwordRequiredType": "alphanumeric",
  "osMinimumVersion": "Os Minimum Version value",
  "osMaximumVersion": "Os Maximum Version value",
  "systemIntegrityProtectionEnabled": true,
  "deviceThreatProtectionEnabled": true,
  "deviceThreatProtectionRequiredSecurityLevel": "secured",
  "storageRequireEncryption": true,
  "firewallEnabled": true,
  "firewallBlockAllIncoming": true,
  "firewallEnableStealthMode": true
}
```



