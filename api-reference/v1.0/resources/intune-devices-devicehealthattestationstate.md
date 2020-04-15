---
title: deviceHealthAttestationState 资源类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 41c9fd4f09749857c9aeb588086ef23ce5775d48
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454002"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="2d8a9-103">deviceHealthAttestationState 资源类型</span><span class="sxs-lookup"><span data-stu-id="2d8a9-103">deviceHealthAttestationState resource type</span></span>

<span data-ttu-id="2d8a9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d8a9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d8a9-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d8a9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d8a9-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="2d8a9-106">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="2d8a9-107">属性</span><span class="sxs-lookup"><span data-stu-id="2d8a9-107">Properties</span></span>
|<span data-ttu-id="2d8a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="2d8a9-108">Property</span></span>|<span data-ttu-id="2d8a9-109">类型</span><span class="sxs-lookup"><span data-stu-id="2d8a9-109">Type</span></span>|<span data-ttu-id="2d8a9-110">说明</span><span class="sxs-lookup"><span data-stu-id="2d8a9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d8a9-111">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="2d8a9-111">lastUpdateDateTime</span></span>|<span data-ttu-id="2d8a9-112">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-112">String</span></span>|<span data-ttu-id="2d8a9-113">上次更新时间戳。</span><span class="sxs-lookup"><span data-stu-id="2d8a9-113">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="2d8a9-114">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="2d8a9-114">contentNamespaceUrl</span></span>|<span data-ttu-id="2d8a9-115">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-115">String</span></span>|<span data-ttu-id="2d8a9-116">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="2d8a9-116">The DHA report version.</span></span> <span data-ttu-id="2d8a9-117">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="2d8a9-117">(Namespace version)</span></span>|
|<span data-ttu-id="2d8a9-118">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="2d8a9-118">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="2d8a9-119">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-119">String</span></span>|<span data-ttu-id="2d8a9-120">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="2d8a9-120">The DHA report version.</span></span> <span data-ttu-id="2d8a9-121">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="2d8a9-121">(Namespace version)</span></span>|
|<span data-ttu-id="2d8a9-122">contentVersion</span><span class="sxs-lookup"><span data-stu-id="2d8a9-122">contentVersion</span></span>|<span data-ttu-id="2d8a9-123">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-123">String</span></span>|<span data-ttu-id="2d8a9-124">HealthAttestation 状态架构版本</span><span class="sxs-lookup"><span data-stu-id="2d8a9-124">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="2d8a9-125">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d8a9-125">issuedDateTime</span></span>|<span data-ttu-id="2d8a9-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d8a9-126">DateTimeOffset</span></span>|<span data-ttu-id="2d8a9-127">评估设备或颁发给 MDM 的日期/时间</span><span class="sxs-lookup"><span data-stu-id="2d8a9-127">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="2d8a9-128">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="2d8a9-128">attestationIdentityKey</span></span>|<span data-ttu-id="2d8a9-129">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-129">String</span></span>|<span data-ttu-id="2d8a9-130">当设备上存在证明标识密钥 (AIK) 时，它表示设备具有认可密钥 (EK) 证书。</span><span class="sxs-lookup"><span data-stu-id="2d8a9-130">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="2d8a9-131">resetCount</span><span class="sxs-lookup"><span data-stu-id="2d8a9-131">resetCount</span></span>|<span data-ttu-id="2d8a9-132">Int64</span><span class="sxs-lookup"><span data-stu-id="2d8a9-132">Int64</span></span>|<span data-ttu-id="2d8a9-133">电脑设备已休眠或恢复的次数</span><span class="sxs-lookup"><span data-stu-id="2d8a9-133">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="2d8a9-134">restartCount</span><span class="sxs-lookup"><span data-stu-id="2d8a9-134">restartCount</span></span>|<span data-ttu-id="2d8a9-135">Int64</span><span class="sxs-lookup"><span data-stu-id="2d8a9-135">Int64</span></span>|<span data-ttu-id="2d8a9-136">电脑设备已重新启动的次数</span><span class="sxs-lookup"><span data-stu-id="2d8a9-136">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="2d8a9-137">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="2d8a9-137">dataExcutionPolicy</span></span>|<span data-ttu-id="2d8a9-138">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-138">String</span></span>|<span data-ttu-id="2d8a9-139">DEP 策略定义一组对内存执行额外检查的硬件和软件技术</span><span class="sxs-lookup"><span data-stu-id="2d8a9-139">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="2d8a9-140">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="2d8a9-140">bitLockerStatus</span></span>|<span data-ttu-id="2d8a9-141">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-141">String</span></span>|<span data-ttu-id="2d8a9-142">BitLocker 驱动器加密开启或关闭</span><span class="sxs-lookup"><span data-stu-id="2d8a9-142">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="2d8a9-143">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="2d8a9-143">bootManagerVersion</span></span>|<span data-ttu-id="2d8a9-144">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-144">String</span></span>|<span data-ttu-id="2d8a9-145">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="2d8a9-145">The version of the Boot Manager</span></span>|
|<span data-ttu-id="2d8a9-146">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="2d8a9-146">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="2d8a9-147">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-147">String</span></span>|<span data-ttu-id="2d8a9-148">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="2d8a9-148">The version of the Boot Manager</span></span>|
|<span data-ttu-id="2d8a9-149">secureBoot</span><span class="sxs-lookup"><span data-stu-id="2d8a9-149">secureBoot</span></span>|<span data-ttu-id="2d8a9-150">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-150">String</span></span>|<span data-ttu-id="2d8a9-151">启用安全启动后，核心组件必须具有正确的加密签名</span><span class="sxs-lookup"><span data-stu-id="2d8a9-151">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="2d8a9-152">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="2d8a9-152">bootDebugging</span></span>|<span data-ttu-id="2d8a9-153">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-153">String</span></span>|<span data-ttu-id="2d8a9-154">启用 bootDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="2d8a9-154">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="2d8a9-155">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="2d8a9-155">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="2d8a9-156">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-156">String</span></span>|<span data-ttu-id="2d8a9-157">启用 operatingSystemKernelDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="2d8a9-157">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="2d8a9-158">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="2d8a9-158">codeIntegrity</span></span>|<span data-ttu-id="2d8a9-159">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-159">String</span></span>| <span data-ttu-id="2d8a9-160">启用代码完整性后，代码执行限于完整性已验证的代码</span><span class="sxs-lookup"><span data-stu-id="2d8a9-160">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="2d8a9-161">testSigning</span><span class="sxs-lookup"><span data-stu-id="2d8a9-161">testSigning</span></span>|<span data-ttu-id="2d8a9-162">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-162">String</span></span>|<span data-ttu-id="2d8a9-163">当允许测试签名时，设备不会在引导期间强制执行签名验证</span><span class="sxs-lookup"><span data-stu-id="2d8a9-163">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="2d8a9-164">safeMode</span><span class="sxs-lookup"><span data-stu-id="2d8a9-164">safeMode</span></span>|<span data-ttu-id="2d8a9-165">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-165">String</span></span>|<span data-ttu-id="2d8a9-166">安全模式是 Windows 的一种故障排除选项，用于在受限状态下启动计算机</span><span class="sxs-lookup"><span data-stu-id="2d8a9-166">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="2d8a9-167">windowsPE</span><span class="sxs-lookup"><span data-stu-id="2d8a9-167">windowsPE</span></span>|<span data-ttu-id="2d8a9-168">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-168">String</span></span>|<span data-ttu-id="2d8a9-169">运行受限服务的操作系统，用于为 Windows 准备计算机</span><span class="sxs-lookup"><span data-stu-id="2d8a9-169">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="2d8a9-170">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="2d8a9-170">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="2d8a9-171">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-171">String</span></span>|<span data-ttu-id="2d8a9-172">ELAM 为网络中的计算机启动时提供保护</span><span class="sxs-lookup"><span data-stu-id="2d8a9-172">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="2d8a9-173">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="2d8a9-173">virtualSecureMode</span></span>|<span data-ttu-id="2d8a9-174">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-174">String</span></span>|<span data-ttu-id="2d8a9-175">VSM 是一个容器，可以保护高价值资产免受已损坏内核的威胁</span><span class="sxs-lookup"><span data-stu-id="2d8a9-175">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="2d8a9-176">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="2d8a9-176">pcrHashAlgorithm</span></span>|<span data-ttu-id="2d8a9-177">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-177">String</span></span>|<span data-ttu-id="2d8a9-178">标识 TPM 使用的 HASH 算法的信息属性</span><span class="sxs-lookup"><span data-stu-id="2d8a9-178">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="2d8a9-179">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="2d8a9-179">bootAppSecurityVersion</span></span>|<span data-ttu-id="2d8a9-180">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-180">String</span></span>|<span data-ttu-id="2d8a9-181">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="2d8a9-181">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="2d8a9-182">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="2d8a9-182">bootManagerSecurityVersion</span></span>|<span data-ttu-id="2d8a9-183">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-183">String</span></span>|<span data-ttu-id="2d8a9-184">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="2d8a9-184">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="2d8a9-185">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="2d8a9-185">tpmVersion</span></span>|<span data-ttu-id="2d8a9-186">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-186">String</span></span>|<span data-ttu-id="2d8a9-187">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="2d8a9-187">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="2d8a9-188">pcr0</span><span class="sxs-lookup"><span data-stu-id="2d8a9-188">pcr0</span></span>|<span data-ttu-id="2d8a9-189">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-189">String</span></span>|<span data-ttu-id="2d8a9-190">在 PCR\[0\] 中捕获的度量</span><span class="sxs-lookup"><span data-stu-id="2d8a9-190">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="2d8a9-191">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="2d8a9-191">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="2d8a9-192">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-192">String</span></span>|<span data-ttu-id="2d8a9-193">自定义安全启动配置策略的指纹</span><span class="sxs-lookup"><span data-stu-id="2d8a9-193">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="2d8a9-194">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="2d8a9-194">codeIntegrityPolicy</span></span>|<span data-ttu-id="2d8a9-195">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-195">String</span></span>|<span data-ttu-id="2d8a9-196">控制启动环境安全性的代码完整性策略</span><span class="sxs-lookup"><span data-stu-id="2d8a9-196">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="2d8a9-197">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="2d8a9-197">bootRevisionListInfo</span></span>|<span data-ttu-id="2d8a9-198">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-198">String</span></span>|<span data-ttu-id="2d8a9-199">在已证明的设备上进行初始启动期间加载的启动修订列表</span><span class="sxs-lookup"><span data-stu-id="2d8a9-199">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="2d8a9-200">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="2d8a9-200">operatingSystemRevListInfo</span></span>|<span data-ttu-id="2d8a9-201">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-201">String</span></span>|<span data-ttu-id="2d8a9-202">在已证明的设备上进行初始启动期间加载的操作系统修订列表</span><span class="sxs-lookup"><span data-stu-id="2d8a9-202">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="2d8a9-203">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="2d8a9-203">healthStatusMismatchInfo</span></span>|<span data-ttu-id="2d8a9-204">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-204">String</span></span>|<span data-ttu-id="2d8a9-205">如果 DHA 服务检测到完整性问题，则此属性会出现</span><span class="sxs-lookup"><span data-stu-id="2d8a9-205">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="2d8a9-206">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="2d8a9-206">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="2d8a9-207">String</span><span class="sxs-lookup"><span data-stu-id="2d8a9-207">String</span></span>|<span data-ttu-id="2d8a9-208">此属性指示设备是否支持 DHA</span><span class="sxs-lookup"><span data-stu-id="2d8a9-208">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="2d8a9-209">关系</span><span class="sxs-lookup"><span data-stu-id="2d8a9-209">Relationships</span></span>
<span data-ttu-id="2d8a9-210">无</span><span class="sxs-lookup"><span data-stu-id="2d8a9-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2d8a9-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2d8a9-211">JSON Representation</span></span>
<span data-ttu-id="2d8a9-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d8a9-212">Here is a JSON representation of the resource.</span></span>
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







