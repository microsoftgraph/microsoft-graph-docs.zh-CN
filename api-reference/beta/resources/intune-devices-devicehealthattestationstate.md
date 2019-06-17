---
title: deviceHealthAttestationState 资源类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6804fe21403c53472a3da4cb521d54da3dbb9d6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983041"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="20f9c-103">deviceHealthAttestationState 资源类型</span><span class="sxs-lookup"><span data-stu-id="20f9c-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="20f9c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="20f9c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20f9c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="20f9c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20f9c-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="20f9c-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="20f9c-107">属性</span><span class="sxs-lookup"><span data-stu-id="20f9c-107">Properties</span></span>
|<span data-ttu-id="20f9c-108">属性</span><span class="sxs-lookup"><span data-stu-id="20f9c-108">Property</span></span>|<span data-ttu-id="20f9c-109">类型</span><span class="sxs-lookup"><span data-stu-id="20f9c-109">Type</span></span>|<span data-ttu-id="20f9c-110">说明</span><span class="sxs-lookup"><span data-stu-id="20f9c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20f9c-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="20f9c-111">lastUpdateDateTime</span></span>|<span data-ttu-id="20f9c-112">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-112">String</span></span>|<span data-ttu-id="20f9c-113">上次更新时间戳。</span><span class="sxs-lookup"><span data-stu-id="20f9c-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="20f9c-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="20f9c-114">contentNamespaceUrl</span></span>|<span data-ttu-id="20f9c-115">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-115">String</span></span>|<span data-ttu-id="20f9c-116">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="20f9c-116">The DHA report version.</span></span> <span data-ttu-id="20f9c-117">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="20f9c-117">(Namespace version)</span></span>|
|<span data-ttu-id="20f9c-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="20f9c-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="20f9c-119">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-119">String</span></span>|<span data-ttu-id="20f9c-120">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="20f9c-120">The DHA report version.</span></span> <span data-ttu-id="20f9c-121">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="20f9c-121">(Namespace version)</span></span>|
|<span data-ttu-id="20f9c-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="20f9c-122">contentVersion</span></span>|<span data-ttu-id="20f9c-123">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-123">String</span></span>|<span data-ttu-id="20f9c-124">HealthAttestation 状态架构版本</span><span class="sxs-lookup"><span data-stu-id="20f9c-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="20f9c-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="20f9c-125">issuedDateTime</span></span>|<span data-ttu-id="20f9c-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="20f9c-126">DateTimeOffset</span></span>|<span data-ttu-id="20f9c-127">评估设备或颁发给 MDM 的日期/时间</span><span class="sxs-lookup"><span data-stu-id="20f9c-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="20f9c-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="20f9c-128">attestationIdentityKey</span></span>|<span data-ttu-id="20f9c-129">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-129">String</span></span>|<span data-ttu-id="20f9c-130">当设备上存在证明标识密钥 (AIK) 时，它表示设备具有认可密钥 (EK) 证书。</span><span class="sxs-lookup"><span data-stu-id="20f9c-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="20f9c-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="20f9c-131">resetCount</span></span>|<span data-ttu-id="20f9c-132">Int64</span><span class="sxs-lookup"><span data-stu-id="20f9c-132">Int64</span></span>|<span data-ttu-id="20f9c-133">电脑设备已休眠或恢复的次数</span><span class="sxs-lookup"><span data-stu-id="20f9c-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="20f9c-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="20f9c-134">restartCount</span></span>|<span data-ttu-id="20f9c-135">Int64</span><span class="sxs-lookup"><span data-stu-id="20f9c-135">Int64</span></span>|<span data-ttu-id="20f9c-136">电脑设备已重新启动的次数</span><span class="sxs-lookup"><span data-stu-id="20f9c-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="20f9c-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="20f9c-137">dataExcutionPolicy</span></span>|<span data-ttu-id="20f9c-138">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-138">String</span></span>|<span data-ttu-id="20f9c-139">DEP 策略定义一组对内存执行额外检查的硬件和软件技术</span><span class="sxs-lookup"><span data-stu-id="20f9c-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="20f9c-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="20f9c-140">bitLockerStatus</span></span>|<span data-ttu-id="20f9c-141">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-141">String</span></span>|<span data-ttu-id="20f9c-142">BitLocker 驱动器加密开启或关闭</span><span class="sxs-lookup"><span data-stu-id="20f9c-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="20f9c-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="20f9c-143">bootManagerVersion</span></span>|<span data-ttu-id="20f9c-144">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-144">String</span></span>|<span data-ttu-id="20f9c-145">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="20f9c-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="20f9c-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="20f9c-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="20f9c-147">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-147">String</span></span>|<span data-ttu-id="20f9c-148">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="20f9c-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="20f9c-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="20f9c-149">secureBoot</span></span>|<span data-ttu-id="20f9c-150">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-150">String</span></span>|<span data-ttu-id="20f9c-151">启用安全启动后，核心组件必须具有正确的加密签名</span><span class="sxs-lookup"><span data-stu-id="20f9c-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="20f9c-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="20f9c-152">bootDebugging</span></span>|<span data-ttu-id="20f9c-153">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-153">String</span></span>|<span data-ttu-id="20f9c-154">启用 bootDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="20f9c-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="20f9c-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="20f9c-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="20f9c-156">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-156">String</span></span>|<span data-ttu-id="20f9c-157">启用 operatingSystemKernelDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="20f9c-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="20f9c-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="20f9c-158">codeIntegrity</span></span>|<span data-ttu-id="20f9c-159">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-159">String</span></span>| <span data-ttu-id="20f9c-160">启用代码完整性后，代码执行限于完整性已验证的代码</span><span class="sxs-lookup"><span data-stu-id="20f9c-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="20f9c-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="20f9c-161">testSigning</span></span>|<span data-ttu-id="20f9c-162">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-162">String</span></span>|<span data-ttu-id="20f9c-163">当允许测试签名时，设备不会在引导期间强制执行签名验证</span><span class="sxs-lookup"><span data-stu-id="20f9c-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="20f9c-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="20f9c-164">safeMode</span></span>|<span data-ttu-id="20f9c-165">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-165">String</span></span>|<span data-ttu-id="20f9c-166">安全模式是 Windows 的一种故障排除选项，用于在受限状态下启动计算机</span><span class="sxs-lookup"><span data-stu-id="20f9c-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="20f9c-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="20f9c-167">windowsPE</span></span>|<span data-ttu-id="20f9c-168">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-168">String</span></span>|<span data-ttu-id="20f9c-169">运行受限服务的操作系统，用于为 Windows 准备计算机</span><span class="sxs-lookup"><span data-stu-id="20f9c-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="20f9c-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="20f9c-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="20f9c-171">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-171">String</span></span>|<span data-ttu-id="20f9c-172">ELAM 为网络中的计算机启动时提供保护</span><span class="sxs-lookup"><span data-stu-id="20f9c-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="20f9c-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="20f9c-173">virtualSecureMode</span></span>|<span data-ttu-id="20f9c-174">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-174">String</span></span>|<span data-ttu-id="20f9c-175">VSM 是一个容器，可以保护高价值资产免受已损坏内核的威胁</span><span class="sxs-lookup"><span data-stu-id="20f9c-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="20f9c-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="20f9c-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="20f9c-177">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-177">String</span></span>|<span data-ttu-id="20f9c-178">标识 TPM 使用的 HASH 算法的信息属性</span><span class="sxs-lookup"><span data-stu-id="20f9c-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="20f9c-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="20f9c-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="20f9c-180">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-180">String</span></span>|<span data-ttu-id="20f9c-181">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="20f9c-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="20f9c-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="20f9c-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="20f9c-183">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-183">String</span></span>|<span data-ttu-id="20f9c-184">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="20f9c-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="20f9c-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="20f9c-185">tpmVersion</span></span>|<span data-ttu-id="20f9c-186">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-186">String</span></span>|<span data-ttu-id="20f9c-187">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="20f9c-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="20f9c-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="20f9c-188">pcr0</span></span>|<span data-ttu-id="20f9c-189">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-189">String</span></span>|<span data-ttu-id="20f9c-190">在 PCR\[0\] 中捕获的度量</span><span class="sxs-lookup"><span data-stu-id="20f9c-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="20f9c-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="20f9c-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="20f9c-192">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-192">String</span></span>|<span data-ttu-id="20f9c-193">自定义安全启动配置策略的指纹</span><span class="sxs-lookup"><span data-stu-id="20f9c-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="20f9c-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="20f9c-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="20f9c-195">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-195">String</span></span>|<span data-ttu-id="20f9c-196">控制启动环境安全性的代码完整性策略</span><span class="sxs-lookup"><span data-stu-id="20f9c-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="20f9c-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="20f9c-197">bootRevisionListInfo</span></span>|<span data-ttu-id="20f9c-198">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-198">String</span></span>|<span data-ttu-id="20f9c-199">在已证明的设备上进行初始启动期间加载的启动修订列表</span><span class="sxs-lookup"><span data-stu-id="20f9c-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="20f9c-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="20f9c-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="20f9c-201">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-201">String</span></span>|<span data-ttu-id="20f9c-202">在已证明的设备上进行初始启动期间加载的操作系统修订列表</span><span class="sxs-lookup"><span data-stu-id="20f9c-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="20f9c-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="20f9c-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="20f9c-204">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-204">String</span></span>|<span data-ttu-id="20f9c-205">如果 DHA 服务检测到完整性问题，则此属性会出现</span><span class="sxs-lookup"><span data-stu-id="20f9c-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="20f9c-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="20f9c-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="20f9c-207">String</span><span class="sxs-lookup"><span data-stu-id="20f9c-207">String</span></span>|<span data-ttu-id="20f9c-208">此属性指示设备是否支持 DHA</span><span class="sxs-lookup"><span data-stu-id="20f9c-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="20f9c-209">关系</span><span class="sxs-lookup"><span data-stu-id="20f9c-209">Relationships</span></span>
<span data-ttu-id="20f9c-210">无</span><span class="sxs-lookup"><span data-stu-id="20f9c-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20f9c-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="20f9c-211">JSON Representation</span></span>
<span data-ttu-id="20f9c-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20f9c-212">Here is a JSON representation of the resource.</span></span>
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





