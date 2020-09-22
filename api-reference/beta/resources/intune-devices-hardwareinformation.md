---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2875ea3a4f8ba7bd00b2a1095ecaf496c36e5ef6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081389"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="25e17-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="25e17-103">hardwareInformation resource type</span></span>

<span data-ttu-id="25e17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="25e17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="25e17-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25e17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25e17-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25e17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25e17-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="25e17-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="25e17-108">属性</span><span class="sxs-lookup"><span data-stu-id="25e17-108">Properties</span></span>
|<span data-ttu-id="25e17-109">属性</span><span class="sxs-lookup"><span data-stu-id="25e17-109">Property</span></span>|<span data-ttu-id="25e17-110">类型</span><span class="sxs-lookup"><span data-stu-id="25e17-110">Type</span></span>|<span data-ttu-id="25e17-111">说明</span><span class="sxs-lookup"><span data-stu-id="25e17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25e17-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="25e17-112">serialNumber</span></span>|<span data-ttu-id="25e17-113">String</span><span class="sxs-lookup"><span data-stu-id="25e17-113">String</span></span>|<span data-ttu-id="25e17-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="25e17-114">Serial number.</span></span>|
|<span data-ttu-id="25e17-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="25e17-115">totalStorageSpace</span></span>|<span data-ttu-id="25e17-116">Int64</span><span class="sxs-lookup"><span data-stu-id="25e17-116">Int64</span></span>|<span data-ttu-id="25e17-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="25e17-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="25e17-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="25e17-118">freeStorageSpace</span></span>|<span data-ttu-id="25e17-119">Int64</span><span class="sxs-lookup"><span data-stu-id="25e17-119">Int64</span></span>|<span data-ttu-id="25e17-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="25e17-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="25e17-121">imei</span><span class="sxs-lookup"><span data-stu-id="25e17-121">imei</span></span>|<span data-ttu-id="25e17-122">String</span><span class="sxs-lookup"><span data-stu-id="25e17-122">String</span></span>|<span data-ttu-id="25e17-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="25e17-123">IMEI</span></span>|
|<span data-ttu-id="25e17-124">meid</span><span class="sxs-lookup"><span data-stu-id="25e17-124">meid</span></span>|<span data-ttu-id="25e17-125">String</span><span class="sxs-lookup"><span data-stu-id="25e17-125">String</span></span>|<span data-ttu-id="25e17-126">MEID</span><span class="sxs-lookup"><span data-stu-id="25e17-126">MEID</span></span>|
|<span data-ttu-id="25e17-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="25e17-127">manufacturer</span></span>|<span data-ttu-id="25e17-128">String</span><span class="sxs-lookup"><span data-stu-id="25e17-128">String</span></span>|<span data-ttu-id="25e17-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="25e17-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="25e17-130">model</span><span class="sxs-lookup"><span data-stu-id="25e17-130">model</span></span>|<span data-ttu-id="25e17-131">String</span><span class="sxs-lookup"><span data-stu-id="25e17-131">String</span></span>|<span data-ttu-id="25e17-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="25e17-132">Model of the device</span></span>|
|<span data-ttu-id="25e17-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="25e17-133">phoneNumber</span></span>|<span data-ttu-id="25e17-134">String</span><span class="sxs-lookup"><span data-stu-id="25e17-134">String</span></span>|<span data-ttu-id="25e17-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="25e17-135">Phone number of the device</span></span>|
|<span data-ttu-id="25e17-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="25e17-136">subscriberCarrier</span></span>|<span data-ttu-id="25e17-137">String</span><span class="sxs-lookup"><span data-stu-id="25e17-137">String</span></span>|<span data-ttu-id="25e17-138">设备的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="25e17-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="25e17-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="25e17-139">cellularTechnology</span></span>|<span data-ttu-id="25e17-140">字符串</span><span class="sxs-lookup"><span data-stu-id="25e17-140">String</span></span>|<span data-ttu-id="25e17-141">设备的手机网络技术</span><span class="sxs-lookup"><span data-stu-id="25e17-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="25e17-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="25e17-142">wifiMac</span></span>|<span data-ttu-id="25e17-143">字符串</span><span class="sxs-lookup"><span data-stu-id="25e17-143">String</span></span>|<span data-ttu-id="25e17-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="25e17-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="25e17-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="25e17-145">operatingSystemLanguage</span></span>|<span data-ttu-id="25e17-146">字符串</span><span class="sxs-lookup"><span data-stu-id="25e17-146">String</span></span>|<span data-ttu-id="25e17-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="25e17-147">Operating system language of the device</span></span>|
|<span data-ttu-id="25e17-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="25e17-148">isSupervised</span></span>|<span data-ttu-id="25e17-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="25e17-149">Boolean</span></span>|<span data-ttu-id="25e17-150">受监督的设备模式</span><span class="sxs-lookup"><span data-stu-id="25e17-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="25e17-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="25e17-151">isEncrypted</span></span>|<span data-ttu-id="25e17-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="25e17-152">Boolean</span></span>|<span data-ttu-id="25e17-153">设备的加密状态</span><span class="sxs-lookup"><span data-stu-id="25e17-153">Encryption status of the device</span></span>|
|<span data-ttu-id="25e17-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="25e17-154">batterySerialNumber</span></span>|<span data-ttu-id="25e17-155">字符串</span><span class="sxs-lookup"><span data-stu-id="25e17-155">String</span></span>|<span data-ttu-id="25e17-156">设备的当前电池的序列号</span><span class="sxs-lookup"><span data-stu-id="25e17-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="25e17-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="25e17-157">batteryHealthPercentage</span></span>|<span data-ttu-id="25e17-158">Int32</span><span class="sxs-lookup"><span data-stu-id="25e17-158">Int32</span></span>|<span data-ttu-id="25e17-159">设备的当前电池的运行状况百分比。</span><span class="sxs-lookup"><span data-stu-id="25e17-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="25e17-160">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="25e17-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="25e17-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="25e17-161">batteryChargeCycles</span></span>|<span data-ttu-id="25e17-162">Int32</span><span class="sxs-lookup"><span data-stu-id="25e17-162">Int32</span></span>|<span data-ttu-id="25e17-163">设备的当前电池已过期的充电周期数。</span><span class="sxs-lookup"><span data-stu-id="25e17-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="25e17-164">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="25e17-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="25e17-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="25e17-165">isSharedDevice</span></span>|<span data-ttu-id="25e17-166">布尔</span><span class="sxs-lookup"><span data-stu-id="25e17-166">Boolean</span></span>|<span data-ttu-id="25e17-167">共享 iPad</span><span class="sxs-lookup"><span data-stu-id="25e17-167">Shared iPad</span></span>|
|<span data-ttu-id="25e17-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="25e17-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="25e17-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="25e17-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="25e17-170">共享 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="25e17-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="25e17-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="25e17-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="25e17-172">字符串</span><span class="sxs-lookup"><span data-stu-id="25e17-172">String</span></span>|<span data-ttu-id="25e17-173">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="25e17-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="25e17-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="25e17-174">operatingSystemEdition</span></span>|<span data-ttu-id="25e17-175">字符串</span><span class="sxs-lookup"><span data-stu-id="25e17-175">String</span></span>|<span data-ttu-id="25e17-176">指定 OS 版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="25e17-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="25e17-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="25e17-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="25e17-178">字符串</span><span class="sxs-lookup"><span data-stu-id="25e17-178">String</span></span>|<span data-ttu-id="25e17-179">如果任何) ，则返回设备 (的完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="25e17-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="25e17-180">如果设备未加入域，则返回一个空字符串。</span><span class="sxs-lookup"><span data-stu-id="25e17-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="25e17-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="25e17-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="25e17-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="25e17-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="25e17-183">基于虚拟化的安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="25e17-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="25e17-184">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="25e17-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="25e17-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="25e17-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="25e17-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="25e17-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="25e17-187">基于虚拟化的安全状态。</span><span class="sxs-lookup"><span data-stu-id="25e17-187">Virtualization-based security status.</span></span> <span data-ttu-id="25e17-188">.</span><span class="sxs-lookup"><span data-stu-id="25e17-188">.</span></span> <span data-ttu-id="25e17-189">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="25e17-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="25e17-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="25e17-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="25e17-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="25e17-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="25e17-192">本地系统颁发机构 (LSA) credential guard 状态。</span><span class="sxs-lookup"><span data-stu-id="25e17-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="25e17-193">.</span><span class="sxs-lookup"><span data-stu-id="25e17-193">.</span></span> <span data-ttu-id="25e17-194">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="25e17-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="25e17-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="25e17-195">osBuildNumber</span></span>|<span data-ttu-id="25e17-196">字符串</span><span class="sxs-lookup"><span data-stu-id="25e17-196">String</span></span>|<span data-ttu-id="25e17-197">Android 设备上的操作系统内部版本号</span><span class="sxs-lookup"><span data-stu-id="25e17-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="25e17-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="25e17-198">operatingSystemProductType</span></span>|<span data-ttu-id="25e17-199">Int32</span><span class="sxs-lookup"><span data-stu-id="25e17-199">Int32</span></span>|<span data-ttu-id="25e17-200">指定 Windows 操作系统 ProductType 的 Int。</span><span class="sxs-lookup"><span data-stu-id="25e17-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="25e17-201">此处提供了更多详细信息 https://go.microsoft.com/fwlink/?linkid=2126950 。</span><span class="sxs-lookup"><span data-stu-id="25e17-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="25e17-202">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="25e17-202">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="25e17-203">关系</span><span class="sxs-lookup"><span data-stu-id="25e17-203">Relationships</span></span>
<span data-ttu-id="25e17-204">无</span><span class="sxs-lookup"><span data-stu-id="25e17-204">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="25e17-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="25e17-205">JSON Representation</span></span>
<span data-ttu-id="25e17-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25e17-206">Here is a JSON representation of the resource.</span></span>
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
  "operatingSystemProductType": 1024
}
```






