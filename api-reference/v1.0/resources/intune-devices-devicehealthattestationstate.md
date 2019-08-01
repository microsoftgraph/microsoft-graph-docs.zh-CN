---
title: deviceHealthAttestationState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: d2a4ab6f846b5172ca91f191f32392b915df116e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36030805"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="b6250-103">deviceHealthAttestationState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6250-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="b6250-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6250-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6250-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b6250-105">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="b6250-106">属性</span><span class="sxs-lookup"><span data-stu-id="b6250-106">Properties</span></span>
|<span data-ttu-id="b6250-107">属性</span><span class="sxs-lookup"><span data-stu-id="b6250-107">Property</span></span>|<span data-ttu-id="b6250-108">类型</span><span class="sxs-lookup"><span data-stu-id="b6250-108">Type</span></span>|<span data-ttu-id="b6250-109">说明</span><span class="sxs-lookup"><span data-stu-id="b6250-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6250-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="b6250-110">lastUpdateDateTime</span></span>|<span data-ttu-id="b6250-111">String</span><span class="sxs-lookup"><span data-stu-id="b6250-111">String</span></span>|<span data-ttu-id="b6250-112">上次更新时间戳。</span><span class="sxs-lookup"><span data-stu-id="b6250-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="b6250-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="b6250-113">contentNamespaceUrl</span></span>|<span data-ttu-id="b6250-114">String</span><span class="sxs-lookup"><span data-stu-id="b6250-114">String</span></span>|<span data-ttu-id="b6250-115">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="b6250-115">The DHA report version.</span></span> <span data-ttu-id="b6250-116">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="b6250-116">(Namespace version)</span></span>|
|<span data-ttu-id="b6250-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="b6250-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="b6250-118">String</span><span class="sxs-lookup"><span data-stu-id="b6250-118">String</span></span>|<span data-ttu-id="b6250-119">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="b6250-119">The DHA report version.</span></span> <span data-ttu-id="b6250-120">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="b6250-120">(Namespace version)</span></span>|
|<span data-ttu-id="b6250-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="b6250-121">contentVersion</span></span>|<span data-ttu-id="b6250-122">String</span><span class="sxs-lookup"><span data-stu-id="b6250-122">String</span></span>|<span data-ttu-id="b6250-123">HealthAttestation 状态架构版本</span><span class="sxs-lookup"><span data-stu-id="b6250-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="b6250-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6250-124">issuedDateTime</span></span>|<span data-ttu-id="b6250-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6250-125">DateTimeOffset</span></span>|<span data-ttu-id="b6250-126">评估设备或颁发给 MDM 的日期/时间</span><span class="sxs-lookup"><span data-stu-id="b6250-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="b6250-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="b6250-127">attestationIdentityKey</span></span>|<span data-ttu-id="b6250-128">String</span><span class="sxs-lookup"><span data-stu-id="b6250-128">String</span></span>|<span data-ttu-id="b6250-129">当设备上存在证明标识密钥 (AIK) 时，它表示设备具有认可密钥 (EK) 证书。</span><span class="sxs-lookup"><span data-stu-id="b6250-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="b6250-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="b6250-130">resetCount</span></span>|<span data-ttu-id="b6250-131">Int64</span><span class="sxs-lookup"><span data-stu-id="b6250-131">Int64</span></span>|<span data-ttu-id="b6250-132">电脑设备已休眠或恢复的次数</span><span class="sxs-lookup"><span data-stu-id="b6250-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="b6250-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="b6250-133">restartCount</span></span>|<span data-ttu-id="b6250-134">Int64</span><span class="sxs-lookup"><span data-stu-id="b6250-134">Int64</span></span>|<span data-ttu-id="b6250-135">电脑设备已重新启动的次数</span><span class="sxs-lookup"><span data-stu-id="b6250-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="b6250-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="b6250-136">dataExcutionPolicy</span></span>|<span data-ttu-id="b6250-137">String</span><span class="sxs-lookup"><span data-stu-id="b6250-137">String</span></span>|<span data-ttu-id="b6250-138">DEP 策略定义一组对内存执行额外检查的硬件和软件技术</span><span class="sxs-lookup"><span data-stu-id="b6250-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="b6250-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="b6250-139">bitLockerStatus</span></span>|<span data-ttu-id="b6250-140">String</span><span class="sxs-lookup"><span data-stu-id="b6250-140">String</span></span>|<span data-ttu-id="b6250-141">BitLocker 驱动器加密开启或关闭</span><span class="sxs-lookup"><span data-stu-id="b6250-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="b6250-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="b6250-142">bootManagerVersion</span></span>|<span data-ttu-id="b6250-143">String</span><span class="sxs-lookup"><span data-stu-id="b6250-143">String</span></span>|<span data-ttu-id="b6250-144">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="b6250-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="b6250-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="b6250-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="b6250-146">String</span><span class="sxs-lookup"><span data-stu-id="b6250-146">String</span></span>|<span data-ttu-id="b6250-147">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="b6250-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="b6250-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="b6250-148">secureBoot</span></span>|<span data-ttu-id="b6250-149">String</span><span class="sxs-lookup"><span data-stu-id="b6250-149">String</span></span>|<span data-ttu-id="b6250-150">启用安全启动后，核心组件必须具有正确的加密签名</span><span class="sxs-lookup"><span data-stu-id="b6250-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="b6250-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="b6250-151">bootDebugging</span></span>|<span data-ttu-id="b6250-152">String</span><span class="sxs-lookup"><span data-stu-id="b6250-152">String</span></span>|<span data-ttu-id="b6250-153">启用 bootDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="b6250-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="b6250-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="b6250-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="b6250-155">String</span><span class="sxs-lookup"><span data-stu-id="b6250-155">String</span></span>|<span data-ttu-id="b6250-156">启用 operatingSystemKernelDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="b6250-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="b6250-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="b6250-157">codeIntegrity</span></span>|<span data-ttu-id="b6250-158">String</span><span class="sxs-lookup"><span data-stu-id="b6250-158">String</span></span>| <span data-ttu-id="b6250-159">启用代码完整性后，代码执行限于完整性已验证的代码</span><span class="sxs-lookup"><span data-stu-id="b6250-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="b6250-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="b6250-160">testSigning</span></span>|<span data-ttu-id="b6250-161">String</span><span class="sxs-lookup"><span data-stu-id="b6250-161">String</span></span>|<span data-ttu-id="b6250-162">当允许测试签名时，设备不会在引导期间强制执行签名验证</span><span class="sxs-lookup"><span data-stu-id="b6250-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="b6250-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="b6250-163">safeMode</span></span>|<span data-ttu-id="b6250-164">String</span><span class="sxs-lookup"><span data-stu-id="b6250-164">String</span></span>|<span data-ttu-id="b6250-165">安全模式是 Windows 的一种故障排除选项，用于在受限状态下启动计算机</span><span class="sxs-lookup"><span data-stu-id="b6250-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="b6250-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="b6250-166">windowsPE</span></span>|<span data-ttu-id="b6250-167">String</span><span class="sxs-lookup"><span data-stu-id="b6250-167">String</span></span>|<span data-ttu-id="b6250-168">运行受限服务的操作系统，用于为 Windows 准备计算机</span><span class="sxs-lookup"><span data-stu-id="b6250-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="b6250-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="b6250-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="b6250-170">String</span><span class="sxs-lookup"><span data-stu-id="b6250-170">String</span></span>|<span data-ttu-id="b6250-171">ELAM 为网络中的计算机启动时提供保护</span><span class="sxs-lookup"><span data-stu-id="b6250-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="b6250-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="b6250-172">virtualSecureMode</span></span>|<span data-ttu-id="b6250-173">String</span><span class="sxs-lookup"><span data-stu-id="b6250-173">String</span></span>|<span data-ttu-id="b6250-174">VSM 是一个容器，可以保护高价值资产免受已损坏内核的威胁</span><span class="sxs-lookup"><span data-stu-id="b6250-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="b6250-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="b6250-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="b6250-176">String</span><span class="sxs-lookup"><span data-stu-id="b6250-176">String</span></span>|<span data-ttu-id="b6250-177">标识 TPM 使用的 HASH 算法的信息属性</span><span class="sxs-lookup"><span data-stu-id="b6250-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="b6250-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="b6250-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="b6250-179">String</span><span class="sxs-lookup"><span data-stu-id="b6250-179">String</span></span>|<span data-ttu-id="b6250-180">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="b6250-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="b6250-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="b6250-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="b6250-182">String</span><span class="sxs-lookup"><span data-stu-id="b6250-182">String</span></span>|<span data-ttu-id="b6250-183">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="b6250-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="b6250-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="b6250-184">tpmVersion</span></span>|<span data-ttu-id="b6250-185">String</span><span class="sxs-lookup"><span data-stu-id="b6250-185">String</span></span>|<span data-ttu-id="b6250-186">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="b6250-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="b6250-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="b6250-187">pcr0</span></span>|<span data-ttu-id="b6250-188">String</span><span class="sxs-lookup"><span data-stu-id="b6250-188">String</span></span>|<span data-ttu-id="b6250-189">在 PCR\[0\] 中捕获的度量</span><span class="sxs-lookup"><span data-stu-id="b6250-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="b6250-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="b6250-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="b6250-191">String</span><span class="sxs-lookup"><span data-stu-id="b6250-191">String</span></span>|<span data-ttu-id="b6250-192">自定义安全启动配置策略的指纹</span><span class="sxs-lookup"><span data-stu-id="b6250-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="b6250-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="b6250-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="b6250-194">String</span><span class="sxs-lookup"><span data-stu-id="b6250-194">String</span></span>|<span data-ttu-id="b6250-195">控制启动环境安全性的代码完整性策略</span><span class="sxs-lookup"><span data-stu-id="b6250-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="b6250-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="b6250-196">bootRevisionListInfo</span></span>|<span data-ttu-id="b6250-197">String</span><span class="sxs-lookup"><span data-stu-id="b6250-197">String</span></span>|<span data-ttu-id="b6250-198">在已证明的设备上进行初始启动期间加载的启动修订列表</span><span class="sxs-lookup"><span data-stu-id="b6250-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="b6250-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="b6250-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="b6250-200">String</span><span class="sxs-lookup"><span data-stu-id="b6250-200">String</span></span>|<span data-ttu-id="b6250-201">在已证明的设备上进行初始启动期间加载的操作系统修订列表</span><span class="sxs-lookup"><span data-stu-id="b6250-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="b6250-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="b6250-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="b6250-203">String</span><span class="sxs-lookup"><span data-stu-id="b6250-203">String</span></span>|<span data-ttu-id="b6250-204">如果 DHA 服务检测到完整性问题，则此属性会出现</span><span class="sxs-lookup"><span data-stu-id="b6250-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="b6250-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="b6250-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="b6250-206">String</span><span class="sxs-lookup"><span data-stu-id="b6250-206">String</span></span>|<span data-ttu-id="b6250-207">此属性指示设备是否支持 DHA</span><span class="sxs-lookup"><span data-stu-id="b6250-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6250-208">关系</span><span class="sxs-lookup"><span data-stu-id="b6250-208">Relationships</span></span>
<span data-ttu-id="b6250-209">无</span><span class="sxs-lookup"><span data-stu-id="b6250-209">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6250-210">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6250-210">JSON Representation</span></span>
<span data-ttu-id="b6250-211">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6250-211">Here is a JSON representation of the resource.</span></span>
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



