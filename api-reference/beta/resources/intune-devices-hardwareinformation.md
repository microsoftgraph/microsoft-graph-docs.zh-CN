---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 0e17df5baad3df0237218f314cdb1c5ee99f03c6
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868174"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="ab5c8-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="ab5c8-103">hardwareInformation resource type</span></span>

<span data-ttu-id="ab5c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ab5c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ab5c8-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ab5c8-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ab5c8-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="ab5c8-108">属性</span><span class="sxs-lookup"><span data-stu-id="ab5c8-108">Properties</span></span>
|<span data-ttu-id="ab5c8-109">属性</span><span class="sxs-lookup"><span data-stu-id="ab5c8-109">Property</span></span>|<span data-ttu-id="ab5c8-110">类型</span><span class="sxs-lookup"><span data-stu-id="ab5c8-110">Type</span></span>|<span data-ttu-id="ab5c8-111">说明</span><span class="sxs-lookup"><span data-stu-id="ab5c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab5c8-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="ab5c8-112">serialNumber</span></span>|<span data-ttu-id="ab5c8-113">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-113">String</span></span>|<span data-ttu-id="ab5c8-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-114">Serial number.</span></span>|
|<span data-ttu-id="ab5c8-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="ab5c8-115">totalStorageSpace</span></span>|<span data-ttu-id="ab5c8-116">Int64</span><span class="sxs-lookup"><span data-stu-id="ab5c8-116">Int64</span></span>|<span data-ttu-id="ab5c8-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="ab5c8-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="ab5c8-118">freeStorageSpace</span></span>|<span data-ttu-id="ab5c8-119">Int64</span><span class="sxs-lookup"><span data-stu-id="ab5c8-119">Int64</span></span>|<span data-ttu-id="ab5c8-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="ab5c8-121">imei</span><span class="sxs-lookup"><span data-stu-id="ab5c8-121">imei</span></span>|<span data-ttu-id="ab5c8-122">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-122">String</span></span>|<span data-ttu-id="ab5c8-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="ab5c8-123">IMEI</span></span>|
|<span data-ttu-id="ab5c8-124">meid</span><span class="sxs-lookup"><span data-stu-id="ab5c8-124">meid</span></span>|<span data-ttu-id="ab5c8-125">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-125">String</span></span>|<span data-ttu-id="ab5c8-126">MEID</span><span class="sxs-lookup"><span data-stu-id="ab5c8-126">MEID</span></span>|
|<span data-ttu-id="ab5c8-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ab5c8-127">manufacturer</span></span>|<span data-ttu-id="ab5c8-128">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-128">String</span></span>|<span data-ttu-id="ab5c8-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="ab5c8-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="ab5c8-130">model</span><span class="sxs-lookup"><span data-stu-id="ab5c8-130">model</span></span>|<span data-ttu-id="ab5c8-131">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-131">String</span></span>|<span data-ttu-id="ab5c8-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="ab5c8-132">Model of the device</span></span>|
|<span data-ttu-id="ab5c8-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ab5c8-133">phoneNumber</span></span>|<span data-ttu-id="ab5c8-134">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-134">String</span></span>|<span data-ttu-id="ab5c8-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="ab5c8-135">Phone number of the device</span></span>|
|<span data-ttu-id="ab5c8-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="ab5c8-136">subscriberCarrier</span></span>|<span data-ttu-id="ab5c8-137">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-137">String</span></span>|<span data-ttu-id="ab5c8-138">设备的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="ab5c8-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="ab5c8-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="ab5c8-139">cellularTechnology</span></span>|<span data-ttu-id="ab5c8-140">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-140">String</span></span>|<span data-ttu-id="ab5c8-141">设备的手机网络技术</span><span class="sxs-lookup"><span data-stu-id="ab5c8-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="ab5c8-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="ab5c8-142">wifiMac</span></span>|<span data-ttu-id="ab5c8-143">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-143">String</span></span>|<span data-ttu-id="ab5c8-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="ab5c8-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="ab5c8-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="ab5c8-145">operatingSystemLanguage</span></span>|<span data-ttu-id="ab5c8-146">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-146">String</span></span>|<span data-ttu-id="ab5c8-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="ab5c8-147">Operating system language of the device</span></span>|
|<span data-ttu-id="ab5c8-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="ab5c8-148">isSupervised</span></span>|<span data-ttu-id="ab5c8-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab5c8-149">Boolean</span></span>|<span data-ttu-id="ab5c8-150">设备的监督模式</span><span class="sxs-lookup"><span data-stu-id="ab5c8-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="ab5c8-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="ab5c8-151">isEncrypted</span></span>|<span data-ttu-id="ab5c8-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab5c8-152">Boolean</span></span>|<span data-ttu-id="ab5c8-153">设备的加密状态</span><span class="sxs-lookup"><span data-stu-id="ab5c8-153">Encryption status of the device</span></span>|
|<span data-ttu-id="ab5c8-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="ab5c8-154">batterySerialNumber</span></span>|<span data-ttu-id="ab5c8-155">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-155">String</span></span>|<span data-ttu-id="ab5c8-156">设备当前电池的序列号</span><span class="sxs-lookup"><span data-stu-id="ab5c8-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="ab5c8-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="ab5c8-157">batteryHealthPercentage</span></span>|<span data-ttu-id="ab5c8-158">Int32</span><span class="sxs-lookup"><span data-stu-id="ab5c8-158">Int32</span></span>|<span data-ttu-id="ab5c8-159">设备的当前电池运行状况百分比。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="ab5c8-160">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="ab5c8-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="ab5c8-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="ab5c8-161">batteryChargeCycles</span></span>|<span data-ttu-id="ab5c8-162">Int32</span><span class="sxs-lookup"><span data-stu-id="ab5c8-162">Int32</span></span>|<span data-ttu-id="ab5c8-163">设备当前电池经过的充电周期数。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="ab5c8-164">有效值为 0 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="ab5c8-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="ab5c8-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="ab5c8-165">isSharedDevice</span></span>|<span data-ttu-id="ab5c8-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="ab5c8-166">Boolean</span></span>|<span data-ttu-id="ab5c8-167">共享 iPad</span><span class="sxs-lookup"><span data-stu-id="ab5c8-167">Shared iPad</span></span>|
|<span data-ttu-id="ab5c8-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="ab5c8-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="ab5c8-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ab5c8-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="ab5c8-170">共享 Apple 设备的所有用户</span><span class="sxs-lookup"><span data-stu-id="ab5c8-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="ab5c8-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="ab5c8-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="ab5c8-172">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-172">String</span></span>|<span data-ttu-id="ab5c8-173">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="ab5c8-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="ab5c8-174">operatingSystemEdition</span></span>|<span data-ttu-id="ab5c8-175">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-175">String</span></span>|<span data-ttu-id="ab5c8-176">指定操作系统版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="ab5c8-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="ab5c8-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="ab5c8-178">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-178">String</span></span>|<span data-ttu-id="ab5c8-179">返回设备名称的完全限定 (（如果有) ）。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="ab5c8-180">如果设备未加入域，它将返回空字符串。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="ab5c8-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="ab5c8-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="ab5c8-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="ab5c8-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="ab5c8-183">基于虚拟化的安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="ab5c8-184">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="ab5c8-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="ab5c8-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="ab5c8-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="ab5c8-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="ab5c8-187">基于虚拟化的安全状态。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-187">Virtualization-based security status.</span></span> <span data-ttu-id="ab5c8-188">.</span><span class="sxs-lookup"><span data-stu-id="ab5c8-188">.</span></span> <span data-ttu-id="ab5c8-189">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="ab5c8-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="ab5c8-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="ab5c8-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="ab5c8-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="ab5c8-192">本地系统颁发 (LSA) 凭据保护状态。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="ab5c8-193">.</span><span class="sxs-lookup"><span data-stu-id="ab5c8-193">.</span></span> <span data-ttu-id="ab5c8-194">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="ab5c8-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="ab5c8-195">osBuildNumber</span></span>|<span data-ttu-id="ab5c8-196">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-196">String</span></span>|<span data-ttu-id="ab5c8-197">Android 设备上的操作系统内部版本号</span><span class="sxs-lookup"><span data-stu-id="ab5c8-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="ab5c8-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="ab5c8-198">operatingSystemProductType</span></span>|<span data-ttu-id="ab5c8-199">Int32</span><span class="sxs-lookup"><span data-stu-id="ab5c8-199">Int32</span></span>|<span data-ttu-id="ab5c8-200">指定 Windows 操作系统 ProductType 的 Int。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="ab5c8-201">此处的更多详细信息 https://go.microsoft.com/fwlink/?linkid=2126950 。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="ab5c8-202">有效值为 0 到 2147483647</span><span class="sxs-lookup"><span data-stu-id="ab5c8-202">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="ab5c8-203">ipAddressV4</span><span class="sxs-lookup"><span data-stu-id="ab5c8-203">ipAddressV4</span></span>|<span data-ttu-id="ab5c8-204">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-204">String</span></span>|<span data-ttu-id="ab5c8-205">IPAddressV4</span><span class="sxs-lookup"><span data-stu-id="ab5c8-205">IPAddressV4</span></span>|
|<span data-ttu-id="ab5c8-206">subnetAddress</span><span class="sxs-lookup"><span data-stu-id="ab5c8-206">subnetAddress</span></span>|<span data-ttu-id="ab5c8-207">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-207">String</span></span>|<span data-ttu-id="ab5c8-208">SubnetAddress</span><span class="sxs-lookup"><span data-stu-id="ab5c8-208">SubnetAddress</span></span>|
|<span data-ttu-id="ab5c8-209">esimIdentifier</span><span class="sxs-lookup"><span data-stu-id="ab5c8-209">esimIdentifier</span></span>|<span data-ttu-id="ab5c8-210">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-210">String</span></span>|<span data-ttu-id="ab5c8-211">eSIM 标识符</span><span class="sxs-lookup"><span data-stu-id="ab5c8-211">eSIM identifier</span></span>|
|<span data-ttu-id="ab5c8-212">systemManagementBIOSVersion</span><span class="sxs-lookup"><span data-stu-id="ab5c8-212">systemManagementBIOSVersion</span></span>|<span data-ttu-id="ab5c8-213">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-213">String</span></span>|<span data-ttu-id="ab5c8-214">SMBIOS 报告的 BIOS 版本</span><span class="sxs-lookup"><span data-stu-id="ab5c8-214">BIOS version as reported by SMBIOS</span></span>|
|<span data-ttu-id="ab5c8-215">tpmManufacturer</span><span class="sxs-lookup"><span data-stu-id="ab5c8-215">tpmManufacturer</span></span>|<span data-ttu-id="ab5c8-216">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-216">String</span></span>|<span data-ttu-id="ab5c8-217">唯一命名 TPM 制造商的标识信息</span><span class="sxs-lookup"><span data-stu-id="ab5c8-217">The identifying information that uniquely names the TPM manufacturer</span></span>|
|<span data-ttu-id="ab5c8-218">tpmVersion</span><span class="sxs-lookup"><span data-stu-id="ab5c8-218">tpmVersion</span></span>|<span data-ttu-id="ab5c8-219">String</span><span class="sxs-lookup"><span data-stu-id="ab5c8-219">String</span></span>|<span data-ttu-id="ab5c8-220">制造商指定的 TPM 版本</span><span class="sxs-lookup"><span data-stu-id="ab5c8-220">The version of the TPM, as specified by the manufacturer</span></span>|

## <a name="relationships"></a><span data-ttu-id="ab5c8-221">关系</span><span class="sxs-lookup"><span data-stu-id="ab5c8-221">Relationships</span></span>
<span data-ttu-id="ab5c8-222">无</span><span class="sxs-lookup"><span data-stu-id="ab5c8-222">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ab5c8-223">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ab5c8-223">JSON Representation</span></span>
<span data-ttu-id="ab5c8-224">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab5c8-224">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.hardwareInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.hardwareInformation",
  "serialNumber": "String",
  "totalStorageSpace": 1024,
  "freeStorageSpace": 1024,
  "imei": "String",
  "meid": "String",
  "manufacturer": "String",
  "model": "String",
  "phoneNumber": "String",
  "subscriberCarrier": "String",
  "cellularTechnology": "String",
  "wifiMac": "String",
  "operatingSystemLanguage": "String",
  "isSupervised": true,
  "isEncrypted": true,
  "batterySerialNumber": "String",
  "batteryHealthPercentage": 1024,
  "batteryChargeCycles": 1024,
  "isSharedDevice": true,
  "sharedDeviceCachedUsers": [
    {
      "@odata.type": "microsoft.graph.sharedAppleDeviceUser",
      "userPrincipalName": "String",
      "dataToSync": true,
      "dataQuota": 1024,
      "dataUsed": 1024
    }
  ],
  "tpmSpecificationVersion": "String",
  "operatingSystemEdition": "String",
  "deviceFullQualifiedDomainName": "String",
  "deviceGuardVirtualizationBasedSecurityHardwareRequirementState": "String",
  "deviceGuardVirtualizationBasedSecurityState": "String",
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String",
  "osBuildNumber": "String",
  "operatingSystemProductType": 1024,
  "ipAddressV4": "String",
  "subnetAddress": "String",
  "esimIdentifier": "String",
  "systemManagementBIOSVersion": "String",
  "tpmManufacturer": "String",
  "tpmVersion": "String"
}
```




