---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 369631fc29203c54ef3c63c2cd32df67254c76bf
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46791776"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="39ad1-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="39ad1-103">hardwareInformation resource type</span></span>

<span data-ttu-id="39ad1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39ad1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="39ad1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="39ad1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39ad1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="39ad1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39ad1-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="39ad1-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="39ad1-108">属性</span><span class="sxs-lookup"><span data-stu-id="39ad1-108">Properties</span></span>
|<span data-ttu-id="39ad1-109">属性</span><span class="sxs-lookup"><span data-stu-id="39ad1-109">Property</span></span>|<span data-ttu-id="39ad1-110">类型</span><span class="sxs-lookup"><span data-stu-id="39ad1-110">Type</span></span>|<span data-ttu-id="39ad1-111">说明</span><span class="sxs-lookup"><span data-stu-id="39ad1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39ad1-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="39ad1-112">serialNumber</span></span>|<span data-ttu-id="39ad1-113">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-113">String</span></span>|<span data-ttu-id="39ad1-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="39ad1-114">Serial number.</span></span>|
|<span data-ttu-id="39ad1-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="39ad1-115">totalStorageSpace</span></span>|<span data-ttu-id="39ad1-116">Int64</span><span class="sxs-lookup"><span data-stu-id="39ad1-116">Int64</span></span>|<span data-ttu-id="39ad1-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="39ad1-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="39ad1-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="39ad1-118">freeStorageSpace</span></span>|<span data-ttu-id="39ad1-119">Int64</span><span class="sxs-lookup"><span data-stu-id="39ad1-119">Int64</span></span>|<span data-ttu-id="39ad1-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="39ad1-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="39ad1-121">imei</span><span class="sxs-lookup"><span data-stu-id="39ad1-121">imei</span></span>|<span data-ttu-id="39ad1-122">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-122">String</span></span>|<span data-ttu-id="39ad1-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="39ad1-123">IMEI</span></span>|
|<span data-ttu-id="39ad1-124">meid</span><span class="sxs-lookup"><span data-stu-id="39ad1-124">meid</span></span>|<span data-ttu-id="39ad1-125">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-125">String</span></span>|<span data-ttu-id="39ad1-126">MEID</span><span class="sxs-lookup"><span data-stu-id="39ad1-126">MEID</span></span>|
|<span data-ttu-id="39ad1-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="39ad1-127">manufacturer</span></span>|<span data-ttu-id="39ad1-128">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-128">String</span></span>|<span data-ttu-id="39ad1-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="39ad1-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="39ad1-130">model</span><span class="sxs-lookup"><span data-stu-id="39ad1-130">model</span></span>|<span data-ttu-id="39ad1-131">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-131">String</span></span>|<span data-ttu-id="39ad1-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="39ad1-132">Model of the device</span></span>|
|<span data-ttu-id="39ad1-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="39ad1-133">phoneNumber</span></span>|<span data-ttu-id="39ad1-134">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-134">String</span></span>|<span data-ttu-id="39ad1-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="39ad1-135">Phone number of the device</span></span>|
|<span data-ttu-id="39ad1-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="39ad1-136">subscriberCarrier</span></span>|<span data-ttu-id="39ad1-137">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-137">String</span></span>|<span data-ttu-id="39ad1-138">设备的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="39ad1-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="39ad1-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="39ad1-139">cellularTechnology</span></span>|<span data-ttu-id="39ad1-140">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-140">String</span></span>|<span data-ttu-id="39ad1-141">设备的手机网络技术</span><span class="sxs-lookup"><span data-stu-id="39ad1-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="39ad1-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="39ad1-142">wifiMac</span></span>|<span data-ttu-id="39ad1-143">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-143">String</span></span>|<span data-ttu-id="39ad1-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="39ad1-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="39ad1-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="39ad1-145">operatingSystemLanguage</span></span>|<span data-ttu-id="39ad1-146">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-146">String</span></span>|<span data-ttu-id="39ad1-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="39ad1-147">Operating system language of the device</span></span>|
|<span data-ttu-id="39ad1-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="39ad1-148">isSupervised</span></span>|<span data-ttu-id="39ad1-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ad1-149">Boolean</span></span>|<span data-ttu-id="39ad1-150">受监督的设备模式</span><span class="sxs-lookup"><span data-stu-id="39ad1-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="39ad1-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="39ad1-151">isEncrypted</span></span>|<span data-ttu-id="39ad1-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="39ad1-152">Boolean</span></span>|<span data-ttu-id="39ad1-153">设备的加密状态</span><span class="sxs-lookup"><span data-stu-id="39ad1-153">Encryption status of the device</span></span>|
|<span data-ttu-id="39ad1-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="39ad1-154">batterySerialNumber</span></span>|<span data-ttu-id="39ad1-155">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-155">String</span></span>|<span data-ttu-id="39ad1-156">设备的当前电池的序列号</span><span class="sxs-lookup"><span data-stu-id="39ad1-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="39ad1-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="39ad1-157">batteryHealthPercentage</span></span>|<span data-ttu-id="39ad1-158">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad1-158">Int32</span></span>|<span data-ttu-id="39ad1-159">设备的当前电池的运行状况百分比。</span><span class="sxs-lookup"><span data-stu-id="39ad1-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="39ad1-160">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="39ad1-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="39ad1-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="39ad1-161">batteryChargeCycles</span></span>|<span data-ttu-id="39ad1-162">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad1-162">Int32</span></span>|<span data-ttu-id="39ad1-163">设备的当前电池已过期的充电周期数。</span><span class="sxs-lookup"><span data-stu-id="39ad1-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="39ad1-164">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="39ad1-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="39ad1-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="39ad1-165">isSharedDevice</span></span>|<span data-ttu-id="39ad1-166">布尔值</span><span class="sxs-lookup"><span data-stu-id="39ad1-166">Boolean</span></span>|<span data-ttu-id="39ad1-167">共享 iPad</span><span class="sxs-lookup"><span data-stu-id="39ad1-167">Shared iPad</span></span>|
|<span data-ttu-id="39ad1-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="39ad1-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="39ad1-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="39ad1-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="39ad1-170">共享 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="39ad1-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="39ad1-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="39ad1-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="39ad1-172">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-172">String</span></span>|<span data-ttu-id="39ad1-173">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="39ad1-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="39ad1-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="39ad1-174">operatingSystemEdition</span></span>|<span data-ttu-id="39ad1-175">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-175">String</span></span>|<span data-ttu-id="39ad1-176">指定 OS 版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="39ad1-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="39ad1-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="39ad1-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="39ad1-178">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-178">String</span></span>|<span data-ttu-id="39ad1-179">如果任何) ，则返回设备 (的完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="39ad1-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="39ad1-180">如果设备未加入域，则返回一个空字符串。</span><span class="sxs-lookup"><span data-stu-id="39ad1-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="39ad1-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="39ad1-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="39ad1-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="39ad1-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="39ad1-183">基于虚拟化的安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="39ad1-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="39ad1-184">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="39ad1-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="39ad1-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="39ad1-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="39ad1-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="39ad1-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="39ad1-187">基于虚拟化的安全状态。</span><span class="sxs-lookup"><span data-stu-id="39ad1-187">Virtualization-based security status.</span></span> <span data-ttu-id="39ad1-188">.</span><span class="sxs-lookup"><span data-stu-id="39ad1-188">.</span></span> <span data-ttu-id="39ad1-189">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="39ad1-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="39ad1-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="39ad1-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="39ad1-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="39ad1-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="39ad1-192">本地系统颁发机构 (LSA) credential guard 状态。</span><span class="sxs-lookup"><span data-stu-id="39ad1-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="39ad1-193">.</span><span class="sxs-lookup"><span data-stu-id="39ad1-193">.</span></span> <span data-ttu-id="39ad1-194">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="39ad1-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="39ad1-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="39ad1-195">osBuildNumber</span></span>|<span data-ttu-id="39ad1-196">String</span><span class="sxs-lookup"><span data-stu-id="39ad1-196">String</span></span>|<span data-ttu-id="39ad1-197">Android 设备上的操作系统内部版本号</span><span class="sxs-lookup"><span data-stu-id="39ad1-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="39ad1-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="39ad1-198">operatingSystemProductType</span></span>|<span data-ttu-id="39ad1-199">Int32</span><span class="sxs-lookup"><span data-stu-id="39ad1-199">Int32</span></span>|<span data-ttu-id="39ad1-200">指定 Windows 操作系统 ProductType 的 Int。</span><span class="sxs-lookup"><span data-stu-id="39ad1-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="39ad1-201">此处提供了更多详细信息 https://go.microsoft.com/fwlink/?linkid=2126950 。</span><span class="sxs-lookup"><span data-stu-id="39ad1-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="39ad1-202">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="39ad1-202">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="39ad1-203">关系</span><span class="sxs-lookup"><span data-stu-id="39ad1-203">Relationships</span></span>
<span data-ttu-id="39ad1-204">无</span><span class="sxs-lookup"><span data-stu-id="39ad1-204">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="39ad1-205">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39ad1-205">JSON Representation</span></span>
<span data-ttu-id="39ad1-206">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39ad1-206">Here is a JSON representation of the resource.</span></span>
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



