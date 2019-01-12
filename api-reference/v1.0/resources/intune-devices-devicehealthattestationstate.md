---
title: deviceHealthAttestationState 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7d246e5bd4235a3bc121d2809e95a59788bf9441
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972150"
---
# <a name="devicehealthattestationstate-resource-type"></a><span data-ttu-id="80be9-103">deviceHealthAttestationState 资源类型</span><span class="sxs-lookup"><span data-stu-id="80be9-103">deviceHealthAttestationState resource type</span></span>

> <span data-ttu-id="80be9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80be9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80be9-105">尚未记录</span><span class="sxs-lookup"><span data-stu-id="80be9-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="80be9-106">属性</span><span class="sxs-lookup"><span data-stu-id="80be9-106">Properties</span></span>
|<span data-ttu-id="80be9-107">属性</span><span class="sxs-lookup"><span data-stu-id="80be9-107">Property</span></span>|<span data-ttu-id="80be9-108">类型</span><span class="sxs-lookup"><span data-stu-id="80be9-108">Type</span></span>|<span data-ttu-id="80be9-109">说明</span><span class="sxs-lookup"><span data-stu-id="80be9-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80be9-110">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="80be9-110">lastUpdateDateTime</span></span>|<span data-ttu-id="80be9-111">String</span><span class="sxs-lookup"><span data-stu-id="80be9-111">String</span></span>|<span data-ttu-id="80be9-112">上次更新时间戳。</span><span class="sxs-lookup"><span data-stu-id="80be9-112">The Timestamp of the last update.</span></span>|
|<span data-ttu-id="80be9-113">contentNamespaceUrl</span><span class="sxs-lookup"><span data-stu-id="80be9-113">contentNamespaceUrl</span></span>|<span data-ttu-id="80be9-114">String</span><span class="sxs-lookup"><span data-stu-id="80be9-114">String</span></span>|<span data-ttu-id="80be9-115">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="80be9-115">The DHA report version.</span></span> <span data-ttu-id="80be9-116">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="80be9-116">(Namespace version)</span></span>|
|<span data-ttu-id="80be9-117">deviceHealthAttestationStatus</span><span class="sxs-lookup"><span data-stu-id="80be9-117">deviceHealthAttestationStatus</span></span>|<span data-ttu-id="80be9-118">String</span><span class="sxs-lookup"><span data-stu-id="80be9-118">String</span></span>|<span data-ttu-id="80be9-119">DHA 报告版本。</span><span class="sxs-lookup"><span data-stu-id="80be9-119">The DHA report version.</span></span> <span data-ttu-id="80be9-120">（命名空间版本）</span><span class="sxs-lookup"><span data-stu-id="80be9-120">(Namespace version)</span></span>|
|<span data-ttu-id="80be9-121">contentVersion</span><span class="sxs-lookup"><span data-stu-id="80be9-121">contentVersion</span></span>|<span data-ttu-id="80be9-122">String</span><span class="sxs-lookup"><span data-stu-id="80be9-122">String</span></span>|<span data-ttu-id="80be9-123">HealthAttestation 状态架构版本</span><span class="sxs-lookup"><span data-stu-id="80be9-123">The HealthAttestation state schema version</span></span>|
|<span data-ttu-id="80be9-124">issuedDateTime</span><span class="sxs-lookup"><span data-stu-id="80be9-124">issuedDateTime</span></span>|<span data-ttu-id="80be9-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80be9-125">DateTimeOffset</span></span>|<span data-ttu-id="80be9-126">评估设备或颁发给 MDM 的日期/时间</span><span class="sxs-lookup"><span data-stu-id="80be9-126">The DateTime when device was evaluated or issued to MDM</span></span>|
|<span data-ttu-id="80be9-127">attestationIdentityKey</span><span class="sxs-lookup"><span data-stu-id="80be9-127">attestationIdentityKey</span></span>|<span data-ttu-id="80be9-128">String</span><span class="sxs-lookup"><span data-stu-id="80be9-128">String</span></span>|<span data-ttu-id="80be9-129">当设备上存在证明标识密钥 (AIK) 时，它表示设备具有认可密钥 (EK) 证书。</span><span class="sxs-lookup"><span data-stu-id="80be9-129">TWhen an Attestation Identity Key (AIK) is present on a device, it indicates that the device has an endorsement key (EK) certificate.</span></span>|
|<span data-ttu-id="80be9-130">resetCount</span><span class="sxs-lookup"><span data-stu-id="80be9-130">resetCount</span></span>|<span data-ttu-id="80be9-131">Int64</span><span class="sxs-lookup"><span data-stu-id="80be9-131">Int64</span></span>|<span data-ttu-id="80be9-132">电脑设备已休眠或恢复的次数</span><span class="sxs-lookup"><span data-stu-id="80be9-132">The number of times a PC device has hibernated or resumed</span></span>|
|<span data-ttu-id="80be9-133">restartCount</span><span class="sxs-lookup"><span data-stu-id="80be9-133">restartCount</span></span>|<span data-ttu-id="80be9-134">Int64</span><span class="sxs-lookup"><span data-stu-id="80be9-134">Int64</span></span>|<span data-ttu-id="80be9-135">电脑设备已重新启动的次数</span><span class="sxs-lookup"><span data-stu-id="80be9-135">The number of times a PC device has rebooted</span></span>|
|<span data-ttu-id="80be9-136">dataExcutionPolicy</span><span class="sxs-lookup"><span data-stu-id="80be9-136">dataExcutionPolicy</span></span>|<span data-ttu-id="80be9-137">String</span><span class="sxs-lookup"><span data-stu-id="80be9-137">String</span></span>|<span data-ttu-id="80be9-138">DEP 策略定义一组对内存执行额外检查的硬件和软件技术</span><span class="sxs-lookup"><span data-stu-id="80be9-138">DEP Policy defines a set of hardware and software technologies that perform additional checks on memory</span></span> |
|<span data-ttu-id="80be9-139">bitLockerStatus</span><span class="sxs-lookup"><span data-stu-id="80be9-139">bitLockerStatus</span></span>|<span data-ttu-id="80be9-140">String</span><span class="sxs-lookup"><span data-stu-id="80be9-140">String</span></span>|<span data-ttu-id="80be9-141">BitLocker 驱动器加密开启或关闭</span><span class="sxs-lookup"><span data-stu-id="80be9-141">On or Off of BitLocker Drive Encryption</span></span>|
|<span data-ttu-id="80be9-142">bootManagerVersion</span><span class="sxs-lookup"><span data-stu-id="80be9-142">bootManagerVersion</span></span>|<span data-ttu-id="80be9-143">String</span><span class="sxs-lookup"><span data-stu-id="80be9-143">String</span></span>|<span data-ttu-id="80be9-144">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="80be9-144">The version of the Boot Manager</span></span>|
|<span data-ttu-id="80be9-145">codeIntegrityCheckVersion</span><span class="sxs-lookup"><span data-stu-id="80be9-145">codeIntegrityCheckVersion</span></span>|<span data-ttu-id="80be9-146">String</span><span class="sxs-lookup"><span data-stu-id="80be9-146">String</span></span>|<span data-ttu-id="80be9-147">引导管理器的版本</span><span class="sxs-lookup"><span data-stu-id="80be9-147">The version of the Boot Manager</span></span>|
|<span data-ttu-id="80be9-148">secureBoot</span><span class="sxs-lookup"><span data-stu-id="80be9-148">secureBoot</span></span>|<span data-ttu-id="80be9-149">String</span><span class="sxs-lookup"><span data-stu-id="80be9-149">String</span></span>|<span data-ttu-id="80be9-150">启用安全启动后，核心组件必须具有正确的加密签名</span><span class="sxs-lookup"><span data-stu-id="80be9-150">When Secure Boot is enabled, the core components must have the correct cryptographic signatures</span></span>|
|<span data-ttu-id="80be9-151">bootDebugging</span><span class="sxs-lookup"><span data-stu-id="80be9-151">bootDebugging</span></span>|<span data-ttu-id="80be9-152">String</span><span class="sxs-lookup"><span data-stu-id="80be9-152">String</span></span>|<span data-ttu-id="80be9-153">启用 bootDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="80be9-153">When bootDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="80be9-154">operatingSystemKernelDebugging</span><span class="sxs-lookup"><span data-stu-id="80be9-154">operatingSystemKernelDebugging</span></span>|<span data-ttu-id="80be9-155">String</span><span class="sxs-lookup"><span data-stu-id="80be9-155">String</span></span>|<span data-ttu-id="80be9-156">启用 operatingSystemKernelDebugging 后，该设备用于开发和测试</span><span class="sxs-lookup"><span data-stu-id="80be9-156">When operatingSystemKernelDebugging is enabled, the device is used in development and testing</span></span>|
|<span data-ttu-id="80be9-157">codeIntegrity</span><span class="sxs-lookup"><span data-stu-id="80be9-157">codeIntegrity</span></span>|<span data-ttu-id="80be9-158">String</span><span class="sxs-lookup"><span data-stu-id="80be9-158">String</span></span>| <span data-ttu-id="80be9-159">启用代码完整性后，代码执行限于完整性已验证的代码</span><span class="sxs-lookup"><span data-stu-id="80be9-159">When code integrity is enabled, code execution is restricted to integrity verified code</span></span>|
|<span data-ttu-id="80be9-160">testSigning</span><span class="sxs-lookup"><span data-stu-id="80be9-160">testSigning</span></span>|<span data-ttu-id="80be9-161">String</span><span class="sxs-lookup"><span data-stu-id="80be9-161">String</span></span>|<span data-ttu-id="80be9-162">当允许测试签名时，设备不会在引导期间强制执行签名验证</span><span class="sxs-lookup"><span data-stu-id="80be9-162">When test signing is allowed, the device does not enforce signature validation during boot</span></span>|
|<span data-ttu-id="80be9-163">safeMode</span><span class="sxs-lookup"><span data-stu-id="80be9-163">safeMode</span></span>|<span data-ttu-id="80be9-164">String</span><span class="sxs-lookup"><span data-stu-id="80be9-164">String</span></span>|<span data-ttu-id="80be9-165">安全模式是 Windows 的一种故障排除选项，用于在受限状态下启动计算机</span><span class="sxs-lookup"><span data-stu-id="80be9-165">Safe mode is a troubleshooting option for Windows that starts your computer in a limited state</span></span>|
|<span data-ttu-id="80be9-166">windowsPE</span><span class="sxs-lookup"><span data-stu-id="80be9-166">windowsPE</span></span>|<span data-ttu-id="80be9-167">String</span><span class="sxs-lookup"><span data-stu-id="80be9-167">String</span></span>|<span data-ttu-id="80be9-168">运行受限服务的操作系统，用于为 Windows 准备计算机</span><span class="sxs-lookup"><span data-stu-id="80be9-168">Operating system running with limited services that is used to prepare a computer for Windows</span></span>|
|<span data-ttu-id="80be9-169">earlyLaunchAntiMalwareDriverProtection</span><span class="sxs-lookup"><span data-stu-id="80be9-169">earlyLaunchAntiMalwareDriverProtection</span></span>|<span data-ttu-id="80be9-170">String</span><span class="sxs-lookup"><span data-stu-id="80be9-170">String</span></span>|<span data-ttu-id="80be9-171">ELAM 为网络中的计算机启动时提供保护</span><span class="sxs-lookup"><span data-stu-id="80be9-171">ELAM provides protection for the computers in your network when they start up</span></span>|
|<span data-ttu-id="80be9-172">virtualSecureMode</span><span class="sxs-lookup"><span data-stu-id="80be9-172">virtualSecureMode</span></span>|<span data-ttu-id="80be9-173">String</span><span class="sxs-lookup"><span data-stu-id="80be9-173">String</span></span>|<span data-ttu-id="80be9-174">VSM 是一个容器，可以保护高价值资产免受已损坏内核的威胁</span><span class="sxs-lookup"><span data-stu-id="80be9-174">VSM is a container that protects high value assets from a compromised kernel</span></span>|
|<span data-ttu-id="80be9-175">pcrHashAlgorithm</span><span class="sxs-lookup"><span data-stu-id="80be9-175">pcrHashAlgorithm</span></span>|<span data-ttu-id="80be9-176">String</span><span class="sxs-lookup"><span data-stu-id="80be9-176">String</span></span>|<span data-ttu-id="80be9-177">标识 TPM 使用的 HASH 算法的信息属性</span><span class="sxs-lookup"><span data-stu-id="80be9-177">Informational attribute that identifies the HASH algorithm that was used by TPM</span></span>|
|<span data-ttu-id="80be9-178">bootAppSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="80be9-178">bootAppSecurityVersion</span></span>|<span data-ttu-id="80be9-179">String</span><span class="sxs-lookup"><span data-stu-id="80be9-179">String</span></span>|<span data-ttu-id="80be9-180">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="80be9-180">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="80be9-181">bootManagerSecurityVersion</span><span class="sxs-lookup"><span data-stu-id="80be9-181">bootManagerSecurityVersion</span></span>|<span data-ttu-id="80be9-182">String</span><span class="sxs-lookup"><span data-stu-id="80be9-182">String</span></span>|<span data-ttu-id="80be9-183">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="80be9-183">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="80be9-184">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="80be9-184">tpmVersion</span></span>|<span data-ttu-id="80be9-185">String</span><span class="sxs-lookup"><span data-stu-id="80be9-185">String</span></span>|<span data-ttu-id="80be9-186">启动应用程序的安全版本号</span><span class="sxs-lookup"><span data-stu-id="80be9-186">The security version number of the Boot Application</span></span>|
|<span data-ttu-id="80be9-187">pcr0</span><span class="sxs-lookup"><span data-stu-id="80be9-187">pcr0</span></span>|<span data-ttu-id="80be9-188">String</span><span class="sxs-lookup"><span data-stu-id="80be9-188">String</span></span>|<span data-ttu-id="80be9-189">在 PCR\[0\] 中捕获的度量</span><span class="sxs-lookup"><span data-stu-id="80be9-189">The measurement that is captured in PCR\[0\]</span></span>|
|<span data-ttu-id="80be9-190">secureBootConfigurationPolicyFingerPrint</span><span class="sxs-lookup"><span data-stu-id="80be9-190">secureBootConfigurationPolicyFingerPrint</span></span>|<span data-ttu-id="80be9-191">String</span><span class="sxs-lookup"><span data-stu-id="80be9-191">String</span></span>|<span data-ttu-id="80be9-192">自定义安全启动配置策略的指纹</span><span class="sxs-lookup"><span data-stu-id="80be9-192">Fingerprint of the Custom Secure Boot Configuration Policy</span></span>|
|<span data-ttu-id="80be9-193">codeIntegrityPolicy</span><span class="sxs-lookup"><span data-stu-id="80be9-193">codeIntegrityPolicy</span></span>|<span data-ttu-id="80be9-194">String</span><span class="sxs-lookup"><span data-stu-id="80be9-194">String</span></span>|<span data-ttu-id="80be9-195">控制启动环境安全性的代码完整性策略</span><span class="sxs-lookup"><span data-stu-id="80be9-195">The Code Integrity policy that is controlling the security of the boot environment</span></span>|
|<span data-ttu-id="80be9-196">bootRevisionListInfo</span><span class="sxs-lookup"><span data-stu-id="80be9-196">bootRevisionListInfo</span></span>|<span data-ttu-id="80be9-197">String</span><span class="sxs-lookup"><span data-stu-id="80be9-197">String</span></span>|<span data-ttu-id="80be9-198">在已证明的设备上进行初始启动期间加载的启动修订列表</span><span class="sxs-lookup"><span data-stu-id="80be9-198">The Boot Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="80be9-199">operatingSystemRevListInfo</span><span class="sxs-lookup"><span data-stu-id="80be9-199">operatingSystemRevListInfo</span></span>|<span data-ttu-id="80be9-200">String</span><span class="sxs-lookup"><span data-stu-id="80be9-200">String</span></span>|<span data-ttu-id="80be9-201">在已证明的设备上进行初始启动期间加载的操作系统修订列表</span><span class="sxs-lookup"><span data-stu-id="80be9-201">The Operating System Revision List that was loaded during initial boot on the attested device</span></span>|
|<span data-ttu-id="80be9-202">healthStatusMismatchInfo</span><span class="sxs-lookup"><span data-stu-id="80be9-202">healthStatusMismatchInfo</span></span>|<span data-ttu-id="80be9-203">String</span><span class="sxs-lookup"><span data-stu-id="80be9-203">String</span></span>|<span data-ttu-id="80be9-204">如果 DHA 服务检测到完整性问题，则此属性会出现</span><span class="sxs-lookup"><span data-stu-id="80be9-204">This attribute appears if DHA-Service detects an integrity issue</span></span>|
|<span data-ttu-id="80be9-205">healthAttestationSupportedStatus</span><span class="sxs-lookup"><span data-stu-id="80be9-205">healthAttestationSupportedStatus</span></span>|<span data-ttu-id="80be9-206">String</span><span class="sxs-lookup"><span data-stu-id="80be9-206">String</span></span>|<span data-ttu-id="80be9-207">此属性指示设备是否支持 DHA</span><span class="sxs-lookup"><span data-stu-id="80be9-207">This attribute indicates if DHA is supported for the device</span></span>|

## <a name="relationships"></a><span data-ttu-id="80be9-208">关系</span><span class="sxs-lookup"><span data-stu-id="80be9-208">Relationships</span></span>
<span data-ttu-id="80be9-209">无</span><span class="sxs-lookup"><span data-stu-id="80be9-209">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="80be9-210">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="80be9-210">JSON Representation</span></span>
<span data-ttu-id="80be9-211">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80be9-211">Here is a JSON representation of the resource.</span></span>
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



