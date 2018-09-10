# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="22548-101">deviceHealthAttestationState 资源类型</span><span class="sxs-lookup"><span data-stu-id="22548-101">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="22548-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="22548-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22548-103">尚未记录</span><span class="sxs-lookup"><span data-stu-id="22548-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="22548-104">属性</span><span class="sxs-lookup"><span data-stu-id="22548-104">Properties</span></span>
|<span data-ttu-id="22548-105">属性</span><span class="sxs-lookup"><span data-stu-id="22548-105">Property</span></span>|<span data-ttu-id="22548-106">类型</span><span class="sxs-lookup"><span data-stu-id="22548-106">Type</span></span>|<span data-ttu-id="22548-107">说明</span><span class="sxs-lookup"><span data-stu-id="22548-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22548-108">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="22548-108">lastUpdateDateTime</span></span>|<span data-ttu-id="22548-109">String</span><span class="sxs-lookup"><span data-stu-id="22548-109">String</span></span>|<span data-ttu-id="22548-110">上次更新时间戳。</span><span class="sxs-lookup"><span data-stu-id="22548-110">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="22548-111">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="22548-111">contentNamespaceUrl</span></span>|<span data-ttu-id="22548-112">String</span><span class="sxs-lookup"><span data-stu-id="22548-112">String</span></span>|<span data-ttu-id="22548-113">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="22548-113">The DHA report version.</span></span> <span data-ttu-id="22548-114">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="22548-114">(Namespace version)</span></span>|
|<span data-ttu-id="22548-115">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="22548-115">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="22548-116">String</span><span class="sxs-lookup"><span data-stu-id="22548-116">String</span></span>|<span data-ttu-id="22548-117">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="22548-117">The DHA report version.</span></span> <span data-ttu-id="22548-118">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="22548-118">(Namespace version)</span></span>|
|<span data-ttu-id="22548-119">contentVersion</span><span class="sxs-lookup"><span data-stu-id="22548-119">contentVersion</span></span>|<span data-ttu-id="22548-120">String</span><span class="sxs-lookup"><span data-stu-id="22548-120">String</span></span>|<span data-ttu-id="22548-121">HealthAttestation 状态架构版本</span><span class="sxs-lookup"><span data-stu-id="22548-121">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="22548-122">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="22548-122">issuedDateTime</span></span>|<span data-ttu-id="22548-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="22548-123">DateTimeOffset</span></span>|<span data-ttu-id="22548-124">评估设备或颁发给 MDM 的日期/时间</span><span class="sxs-lookup"><span data-stu-id="22548-124">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="22548-125">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="22548-125">attestationIdentityKey</span></span>|<span data-ttu-id="22548-126">String</span><span class="sxs-lookup"><span data-stu-id="22548-126">String</span></span>|<span data-ttu-id="22548-127">当设备上存在证明标识密钥 (AIK) 时，它表示设备具有认可密钥 (EK) 证书。</span><span class="sxs-lookup"><span data-stu-id="22548-127">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="22548-128">resetCount</span><span class="sxs-lookup"><span data-stu-id="22548-128">resetCount</span></span>|<span data-ttu-id="22548-129">Int64</span><span class="sxs-lookup"><span data-stu-id="22548-129">Int64</span></span>|<span data-ttu-id="22548-130">电脑设备已休眠或恢复的次数</span><span class="sxs-lookup"><span data-stu-id="22548-130">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="22548-131">restartCount</span><span class="sxs-lookup"><span data-stu-id="22548-131">restartCount</span></span>|<span data-ttu-id="22548-132">Int64</span><span class="sxs-lookup"><span data-stu-id="22548-132">Int64</span></span>|<span data-ttu-id="22548-133">电脑设备已重新启动的次数</span><span class="sxs-lookup"><span data-stu-id="22548-133">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="22548-134">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="22548-134">dataExcutionPolicy</span></span>|<span data-ttu-id="22548-135">String</span><span class="sxs-lookup"><span data-stu-id="22548-135">String</span></span>|<span data-ttu-id="22548-136">DEP 策略定义一组对内存执行额外检查的硬件和软件技术</span><span class="sxs-lookup"><span data-stu-id="22548-136">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="22548-137">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="22548-137">bitLockerStatus</span></span>|<span data-ttu-id="22548-138">String</span><span class="sxs-lookup"><span data-stu-id="22548-138">String</span></span>|<span data-ttu-id="22548-139">BitLocker 驱动器加密开启或关闭</span><span class="sxs-lookup"><span data-stu-id="22548-139">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="22548-140">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="22548-140">bootManagerVersion</span></span>|<span data-ttu-id="22548-141">String</span><span class="sxs-lookup"><span data-stu-id="22548-141">String</span></span>|<span data-ttu-id="22548-142">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="22548-142">The version of the Boot Manager</span></span>|
|<span data-ttu-id="22548-143">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="22548-143">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="22548-144">String</span><span class="sxs-lookup"><span data-stu-id="22548-144">String</span></span>|<span data-ttu-id="22548-145">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="22548-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="22548-146">secureBoot</span><span class="sxs-lookup"><span data-stu-id="22548-146">secureBoot</span></span>|<span data-ttu-id="22548-147">String</span><span class="sxs-lookup"><span data-stu-id="22548-147">String</span></span>|<span data-ttu-id="22548-148">启用安全启动后，核心组件必须具有正确的加密签名</span><span class="sxs-lookup"><span data-stu-id="22548-148">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="22548-149">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="22548-149">bootDebugging</span></span>|<span data-ttu-id="22548-150">String</span><span class="sxs-lookup"><span data-stu-id="22548-150">String</span></span>|<span data-ttu-id="22548-151">启用 bootDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="22548-151">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="22548-152">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="22548-152">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="22548-153">String</span><span class="sxs-lookup"><span data-stu-id="22548-153">String</span></span>|<span data-ttu-id="22548-154">启用 operatingSystemKernelDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="22548-154">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="22548-155">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="22548-155">codeIntegrity</span></span>|<span data-ttu-id="22548-156">String</span><span class="sxs-lookup"><span data-stu-id="22548-156">String</span></span>| <span data-ttu-id="22548-157">启用代码完整性后，代码执行限于完整性已验证的代码</span><span class="sxs-lookup"><span data-stu-id="22548-157">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="22548-158">testSigning</span><span class="sxs-lookup"><span data-stu-id="22548-158">testSigning</span></span>|<span data-ttu-id="22548-159">String</span><span class="sxs-lookup"><span data-stu-id="22548-159">String</span></span>|<span data-ttu-id="22548-160">当允许测试签名时，设备不会在引导期间强制执行签名验证</span><span class="sxs-lookup"><span data-stu-id="22548-160">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="22548-161">safeMode</span><span class="sxs-lookup"><span data-stu-id="22548-161">safeMode</span></span>|<span data-ttu-id="22548-162">String</span><span class="sxs-lookup"><span data-stu-id="22548-162">String</span></span>|<span data-ttu-id="22548-163">安全模式是 Windows 的一种故障排除选项，用于在受限状态下启动计算机</span><span class="sxs-lookup"><span data-stu-id="22548-163">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="22548-164">windowsPE</span><span class="sxs-lookup"><span data-stu-id="22548-164">windowsPE</span></span>|<span data-ttu-id="22548-165">String</span><span class="sxs-lookup"><span data-stu-id="22548-165">String</span></span>|<span data-ttu-id="22548-166">运行受限服务的操作系统，用于为 Windows 准备计算机</span><span class="sxs-lookup"><span data-stu-id="22548-166">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="22548-167">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="22548-167">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="22548-168">String</span><span class="sxs-lookup"><span data-stu-id="22548-168">String</span></span>|<span data-ttu-id="22548-169">ELAM 为网络中的计算机启动时提供保护</span><span class="sxs-lookup"><span data-stu-id="22548-169">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="22548-170">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="22548-170">virtualSecureMode</span></span>|<span data-ttu-id="22548-171">String</span><span class="sxs-lookup"><span data-stu-id="22548-171">String</span></span>|<span data-ttu-id="22548-172">VSM 是一个容器，可以保护高价值资产免受已损坏内核的威胁</span><span class="sxs-lookup"><span data-stu-id="22548-172">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="22548-173">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="22548-173">pcrHashAlgorithm</span></span>|<span data-ttu-id="22548-174">String</span><span class="sxs-lookup"><span data-stu-id="22548-174">String</span></span>|<span data-ttu-id="22548-175">标识 TPM 使用的 HASH 算法的信息属性</span><span class="sxs-lookup"><span data-stu-id="22548-175">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="22548-176">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="22548-176">bootAppSecurityVersion</span></span>|<span data-ttu-id="22548-177">String</span><span class="sxs-lookup"><span data-stu-id="22548-177">String</span></span>|<span data-ttu-id="22548-178">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="22548-178">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="22548-179">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="22548-179">bootManagerSecurityVersion</span></span>|<span data-ttu-id="22548-180">String</span><span class="sxs-lookup"><span data-stu-id="22548-180">String</span></span>|<span data-ttu-id="22548-181">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="22548-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="22548-182">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="22548-182">tpmVersion</span></span>|<span data-ttu-id="22548-183">String</span><span class="sxs-lookup"><span data-stu-id="22548-183">String</span></span>|<span data-ttu-id="22548-184">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="22548-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="22548-185">pcr0</span><span class="sxs-lookup"><span data-stu-id="22548-185">pcr0</span></span>|<span data-ttu-id="22548-186">String</span><span class="sxs-lookup"><span data-stu-id="22548-186">String</span></span>|<span data-ttu-id="22548-187">在 PCR\[0\] 中捕获的度量</span><span class="sxs-lookup"><span data-stu-id="22548-187">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="22548-188">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="22548-188">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="22548-189">String</span><span class="sxs-lookup"><span data-stu-id="22548-189">String</span></span>|<span data-ttu-id="22548-190">自定义安全启动配置策略的指纹</span><span class="sxs-lookup"><span data-stu-id="22548-190">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="22548-191">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="22548-191">codeIntegrityPolicy</span></span>|<span data-ttu-id="22548-192">String</span><span class="sxs-lookup"><span data-stu-id="22548-192">String</span></span>|<span data-ttu-id="22548-193">控制启动环境安全性的代码完整性策略</span><span class="sxs-lookup"><span data-stu-id="22548-193">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="22548-194">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="22548-194">bootRevisionListInfo</span></span>|<span data-ttu-id="22548-195">String</span><span class="sxs-lookup"><span data-stu-id="22548-195">String</span></span>|<span data-ttu-id="22548-196">在已证明的设备上进行初始启动期间加载的启动修订列表</span><span class="sxs-lookup"><span data-stu-id="22548-196">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="22548-197">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="22548-197">operatingSystemRevListInfo</span></span>|<span data-ttu-id="22548-198">String</span><span class="sxs-lookup"><span data-stu-id="22548-198">String</span></span>|<span data-ttu-id="22548-199">在已证明的设备上进行初始启动期间加载的操作系统修订列表</span><span class="sxs-lookup"><span data-stu-id="22548-199">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="22548-200">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="22548-200">healthStatusMismatchInfo</span></span>|<span data-ttu-id="22548-201">String</span><span class="sxs-lookup"><span data-stu-id="22548-201">String</span></span>|<span data-ttu-id="22548-202">如果 DHA 服务检测到完整性问题，则此属性会出现</span><span class="sxs-lookup"><span data-stu-id="22548-202">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="22548-203">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="22548-203">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="22548-204">String</span><span class="sxs-lookup"><span data-stu-id="22548-204">String</span></span>|<span data-ttu-id="22548-205">此属性指示设备是否支持 DHA</span><span class="sxs-lookup"><span data-stu-id="22548-205">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="22548-206">关系</span><span class="sxs-lookup"><span data-stu-id="22548-206">Relationships</span></span>
<span data-ttu-id="22548-207">无</span><span class="sxs-lookup"><span data-stu-id="22548-207">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="22548-208">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="22548-208">JSON Representation</span></span>
<span data-ttu-id="22548-209">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="22548-209">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthAttestationState",
  "lastUpdateDateTime": "String",
  "contentNamespaceUrl": "String",
  "deviceHealthAttestationStatus": "String",
  "contentVersion": "String",
  "issuedDateTime": "String (timestamp)",
  "attestationIdentityKey": "String",
  "resetCount": 1024,
  "restartCount": 1024,
  "dataExcutionPolicy": "String",
  "bitLockerStatus": "String",
  "bootManagerVersion": "String",
  "codeIntegrityCheckVersion": "String",
  "secureBoot": "String",
  "bootDebugging": "String",
  "operatingSystemKernelDebugging": "String",
  "codeIntegrity": "String",
  "testSigning": "String",
  "safeMode": "String",
  "windowsPE": "String",
  "earlyLaunchAntiMalwareDriverProtection": "String",
  "virtualSecureMode": "String",
  "pcrHashAlgorithm": "String",
  "bootAppSecurityVersion": "String",
  "bootManagerSecurityVersion": "String",
  "tpmVersion": "String",
  "pcr0": "String",
  "secureBootConfigurationPolicyFingerPrint": "String",
  "codeIntegrityPolicy": "String",
  "bootRevisionListInfo": "String",
  "operatingSystemRevListInfo": "String",
  "healthStatusMismatchInfo": "String",
  "healthAttestationSupportedStatus": "String"
}
```








