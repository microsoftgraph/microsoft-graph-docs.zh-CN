---
title: deviceHealthAttestationState 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 81c695d466b124568cf17472483241789fdaefd6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469649"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="7f24e-103">deviceHealthAttestationState 资源类型</span><span class="sxs-lookup"><span data-stu-id="7f24e-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="7f24e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f24e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7f24e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f24e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f24e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f24e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f24e-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7f24e-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="7f24e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f24e-108">Properties</span></span>
|<span data-ttu-id="7f24e-109">属性</span><span class="sxs-lookup"><span data-stu-id="7f24e-109">Property</span></span>|<span data-ttu-id="7f24e-110">类型</span><span class="sxs-lookup"><span data-stu-id="7f24e-110">Type</span></span>|<span data-ttu-id="7f24e-111">说明</span><span class="sxs-lookup"><span data-stu-id="7f24e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f24e-112">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="7f24e-112">lastUpdateDateTime</span></span>|<span data-ttu-id="7f24e-113">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-113">String</span></span>|<span data-ttu-id="7f24e-114">上次更新时间戳。</span><span class="sxs-lookup"><span data-stu-id="7f24e-114">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="7f24e-115">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="7f24e-115">contentNamespaceUrl</span></span>|<span data-ttu-id="7f24e-116">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-116">String</span></span>|<span data-ttu-id="7f24e-117">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="7f24e-117">The DHA report version.</span></span> <span data-ttu-id="7f24e-118">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="7f24e-118">(Namespace version)</span></span>|
|<span data-ttu-id="7f24e-119">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="7f24e-119">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="7f24e-120">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-120">String</span></span>|<span data-ttu-id="7f24e-121">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="7f24e-121">The DHA report version.</span></span> <span data-ttu-id="7f24e-122">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="7f24e-122">(Namespace version)</span></span>|
|<span data-ttu-id="7f24e-123">contentVersion</span><span class="sxs-lookup"><span data-stu-id="7f24e-123">contentVersion</span></span>|<span data-ttu-id="7f24e-124">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-124">String</span></span>|<span data-ttu-id="7f24e-125">HealthAttestation 状态架构版本</span><span class="sxs-lookup"><span data-stu-id="7f24e-125">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="7f24e-126">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f24e-126">issuedDateTime</span></span>|<span data-ttu-id="7f24e-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f24e-127">DateTimeOffset</span></span>|<span data-ttu-id="7f24e-128">评估设备或颁发给 MDM 的日期/时间</span><span class="sxs-lookup"><span data-stu-id="7f24e-128">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="7f24e-129">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="7f24e-129">attestationIdentityKey</span></span>|<span data-ttu-id="7f24e-130">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-130">String</span></span>|<span data-ttu-id="7f24e-131">当设备上存在证明标识密钥 (AIK) 时，它表示设备具有认可密钥 (EK) 证书。</span><span class="sxs-lookup"><span data-stu-id="7f24e-131">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="7f24e-132">resetCount</span><span class="sxs-lookup"><span data-stu-id="7f24e-132">resetCount</span></span>|<span data-ttu-id="7f24e-133">Int64</span><span class="sxs-lookup"><span data-stu-id="7f24e-133">Int64</span></span>|<span data-ttu-id="7f24e-134">电脑设备已休眠或恢复的次数</span><span class="sxs-lookup"><span data-stu-id="7f24e-134">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="7f24e-135">restartCount</span><span class="sxs-lookup"><span data-stu-id="7f24e-135">restartCount</span></span>|<span data-ttu-id="7f24e-136">Int64</span><span class="sxs-lookup"><span data-stu-id="7f24e-136">Int64</span></span>|<span data-ttu-id="7f24e-137">电脑设备已重新启动的次数</span><span class="sxs-lookup"><span data-stu-id="7f24e-137">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="7f24e-138">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="7f24e-138">dataExcutionPolicy</span></span>|<span data-ttu-id="7f24e-139">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-139">String</span></span>|<span data-ttu-id="7f24e-140">DEP 策略定义一组对内存执行额外检查的硬件和软件技术</span><span class="sxs-lookup"><span data-stu-id="7f24e-140">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="7f24e-141">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="7f24e-141">bitLockerStatus</span></span>|<span data-ttu-id="7f24e-142">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-142">String</span></span>|<span data-ttu-id="7f24e-143">BitLocker 驱动器加密开启或关闭</span><span class="sxs-lookup"><span data-stu-id="7f24e-143">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="7f24e-144">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="7f24e-144">bootManagerVersion</span></span>|<span data-ttu-id="7f24e-145">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-145">String</span></span>|<span data-ttu-id="7f24e-146">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="7f24e-146">The version of the Boot Manager</span></span>|
|<span data-ttu-id="7f24e-147">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="7f24e-147">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="7f24e-148">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-148">String</span></span>|<span data-ttu-id="7f24e-149">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="7f24e-149">The version of the Boot Manager</span></span>|
|<span data-ttu-id="7f24e-150">secureBoot</span><span class="sxs-lookup"><span data-stu-id="7f24e-150">secureBoot</span></span>|<span data-ttu-id="7f24e-151">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-151">String</span></span>|<span data-ttu-id="7f24e-152">启用安全启动后，核心组件必须具有正确的加密签名</span><span class="sxs-lookup"><span data-stu-id="7f24e-152">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="7f24e-153">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="7f24e-153">bootDebugging</span></span>|<span data-ttu-id="7f24e-154">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-154">String</span></span>|<span data-ttu-id="7f24e-155">启用 bootDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="7f24e-155">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="7f24e-156">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="7f24e-156">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="7f24e-157">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-157">String</span></span>|<span data-ttu-id="7f24e-158">启用 operatingSystemKernelDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="7f24e-158">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="7f24e-159">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="7f24e-159">codeIntegrity</span></span>|<span data-ttu-id="7f24e-160">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-160">String</span></span>| <span data-ttu-id="7f24e-161">启用代码完整性后，代码执行限于完整性已验证的代码</span><span class="sxs-lookup"><span data-stu-id="7f24e-161">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="7f24e-162">testSigning</span><span class="sxs-lookup"><span data-stu-id="7f24e-162">testSigning</span></span>|<span data-ttu-id="7f24e-163">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-163">String</span></span>|<span data-ttu-id="7f24e-164">当允许测试签名时，设备不会在引导期间强制执行签名验证</span><span class="sxs-lookup"><span data-stu-id="7f24e-164">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="7f24e-165">safeMode</span><span class="sxs-lookup"><span data-stu-id="7f24e-165">safeMode</span></span>|<span data-ttu-id="7f24e-166">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-166">String</span></span>|<span data-ttu-id="7f24e-167">安全模式是 Windows 的一种故障排除选项，用于在受限状态下启动计算机</span><span class="sxs-lookup"><span data-stu-id="7f24e-167">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="7f24e-168">windowsPE</span><span class="sxs-lookup"><span data-stu-id="7f24e-168">windowsPE</span></span>|<span data-ttu-id="7f24e-169">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-169">String</span></span>|<span data-ttu-id="7f24e-170">运行受限服务的操作系统，用于为 Windows 准备计算机</span><span class="sxs-lookup"><span data-stu-id="7f24e-170">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="7f24e-171">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="7f24e-171">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="7f24e-172">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-172">String</span></span>|<span data-ttu-id="7f24e-173">ELAM 为网络中的计算机启动时提供保护</span><span class="sxs-lookup"><span data-stu-id="7f24e-173">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="7f24e-174">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="7f24e-174">virtualSecureMode</span></span>|<span data-ttu-id="7f24e-175">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-175">String</span></span>|<span data-ttu-id="7f24e-176">VSM 是一个容器，可以保护高价值资产免受已损坏内核的威胁</span><span class="sxs-lookup"><span data-stu-id="7f24e-176">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="7f24e-177">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="7f24e-177">pcrHashAlgorithm</span></span>|<span data-ttu-id="7f24e-178">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-178">String</span></span>|<span data-ttu-id="7f24e-179">标识 TPM 使用的 HASH 算法的信息属性</span><span class="sxs-lookup"><span data-stu-id="7f24e-179">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="7f24e-180">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="7f24e-180">bootAppSecurityVersion</span></span>|<span data-ttu-id="7f24e-181">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-181">String</span></span>|<span data-ttu-id="7f24e-182">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="7f24e-182">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="7f24e-183">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="7f24e-183">bootManagerSecurityVersion</span></span>|<span data-ttu-id="7f24e-184">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-184">String</span></span>|<span data-ttu-id="7f24e-185">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="7f24e-185">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="7f24e-186">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="7f24e-186">tpmVersion</span></span>|<span data-ttu-id="7f24e-187">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-187">String</span></span>|<span data-ttu-id="7f24e-188">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="7f24e-188">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="7f24e-189">pcr0</span><span class="sxs-lookup"><span data-stu-id="7f24e-189">pcr0</span></span>|<span data-ttu-id="7f24e-190">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-190">String</span></span>|<span data-ttu-id="7f24e-191">在 PCR\[0\] 中捕获的度量</span><span class="sxs-lookup"><span data-stu-id="7f24e-191">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="7f24e-192">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="7f24e-192">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="7f24e-193">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-193">String</span></span>|<span data-ttu-id="7f24e-194">自定义安全启动配置策略的指纹</span><span class="sxs-lookup"><span data-stu-id="7f24e-194">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="7f24e-195">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="7f24e-195">codeIntegrityPolicy</span></span>|<span data-ttu-id="7f24e-196">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-196">String</span></span>|<span data-ttu-id="7f24e-197">控制启动环境安全性的代码完整性策略</span><span class="sxs-lookup"><span data-stu-id="7f24e-197">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="7f24e-198">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="7f24e-198">bootRevisionListInfo</span></span>|<span data-ttu-id="7f24e-199">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-199">String</span></span>|<span data-ttu-id="7f24e-200">在已证明的设备上进行初始启动期间加载的启动修订列表</span><span class="sxs-lookup"><span data-stu-id="7f24e-200">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="7f24e-201">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="7f24e-201">operatingSystemRevListInfo</span></span>|<span data-ttu-id="7f24e-202">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-202">String</span></span>|<span data-ttu-id="7f24e-203">在已证明的设备上进行初始启动期间加载的操作系统修订列表</span><span class="sxs-lookup"><span data-stu-id="7f24e-203">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="7f24e-204">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="7f24e-204">healthStatusMismatchInfo</span></span>|<span data-ttu-id="7f24e-205">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-205">String</span></span>|<span data-ttu-id="7f24e-206">如果 DHA 服务检测到完整性问题，则此属性会出现</span><span class="sxs-lookup"><span data-stu-id="7f24e-206">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="7f24e-207">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="7f24e-207">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="7f24e-208">String</span><span class="sxs-lookup"><span data-stu-id="7f24e-208">String</span></span>|<span data-ttu-id="7f24e-209">此属性指示设备是否支持 DHA</span><span class="sxs-lookup"><span data-stu-id="7f24e-209">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f24e-210">关系</span><span class="sxs-lookup"><span data-stu-id="7f24e-210">Relationships</span></span>
<span data-ttu-id="7f24e-211">无</span><span class="sxs-lookup"><span data-stu-id="7f24e-211">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7f24e-212">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7f24e-212">JSON Representation</span></span>
<span data-ttu-id="7f24e-213">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f24e-213">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthAttestationState"
}
-->
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



