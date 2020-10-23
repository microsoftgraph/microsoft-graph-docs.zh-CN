---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: aba75cb97b15253932eda90dbd252fde640f8461
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697656"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="d1dba-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="d1dba-103">hardwareInformation resource type</span></span>

<span data-ttu-id="d1dba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d1dba-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d1dba-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d1dba-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d1dba-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d1dba-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d1dba-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="d1dba-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="d1dba-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1dba-108">Properties</span></span>
|<span data-ttu-id="d1dba-109">属性</span><span class="sxs-lookup"><span data-stu-id="d1dba-109">Property</span></span>|<span data-ttu-id="d1dba-110">类型</span><span class="sxs-lookup"><span data-stu-id="d1dba-110">Type</span></span>|<span data-ttu-id="d1dba-111">说明</span><span class="sxs-lookup"><span data-stu-id="d1dba-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d1dba-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="d1dba-112">serialNumber</span></span>|<span data-ttu-id="d1dba-113">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-113">String</span></span>|<span data-ttu-id="d1dba-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="d1dba-114">Serial number.</span></span>|
|<span data-ttu-id="d1dba-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="d1dba-115">totalStorageSpace</span></span>|<span data-ttu-id="d1dba-116">Int64</span><span class="sxs-lookup"><span data-stu-id="d1dba-116">Int64</span></span>|<span data-ttu-id="d1dba-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="d1dba-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="d1dba-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="d1dba-118">freeStorageSpace</span></span>|<span data-ttu-id="d1dba-119">Int64</span><span class="sxs-lookup"><span data-stu-id="d1dba-119">Int64</span></span>|<span data-ttu-id="d1dba-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="d1dba-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="d1dba-121">imei</span><span class="sxs-lookup"><span data-stu-id="d1dba-121">imei</span></span>|<span data-ttu-id="d1dba-122">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-122">String</span></span>|<span data-ttu-id="d1dba-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="d1dba-123">IMEI</span></span>|
|<span data-ttu-id="d1dba-124">meid</span><span class="sxs-lookup"><span data-stu-id="d1dba-124">meid</span></span>|<span data-ttu-id="d1dba-125">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-125">String</span></span>|<span data-ttu-id="d1dba-126">MEID</span><span class="sxs-lookup"><span data-stu-id="d1dba-126">MEID</span></span>|
|<span data-ttu-id="d1dba-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="d1dba-127">manufacturer</span></span>|<span data-ttu-id="d1dba-128">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-128">String</span></span>|<span data-ttu-id="d1dba-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="d1dba-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="d1dba-130">model</span><span class="sxs-lookup"><span data-stu-id="d1dba-130">model</span></span>|<span data-ttu-id="d1dba-131">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-131">String</span></span>|<span data-ttu-id="d1dba-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="d1dba-132">Model of the device</span></span>|
|<span data-ttu-id="d1dba-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="d1dba-133">phoneNumber</span></span>|<span data-ttu-id="d1dba-134">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-134">String</span></span>|<span data-ttu-id="d1dba-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="d1dba-135">Phone number of the device</span></span>|
|<span data-ttu-id="d1dba-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="d1dba-136">subscriberCarrier</span></span>|<span data-ttu-id="d1dba-137">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-137">String</span></span>|<span data-ttu-id="d1dba-138">设备的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="d1dba-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="d1dba-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="d1dba-139">cellularTechnology</span></span>|<span data-ttu-id="d1dba-140">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-140">String</span></span>|<span data-ttu-id="d1dba-141">设备的手机网络技术</span><span class="sxs-lookup"><span data-stu-id="d1dba-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="d1dba-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="d1dba-142">wifiMac</span></span>|<span data-ttu-id="d1dba-143">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-143">String</span></span>|<span data-ttu-id="d1dba-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="d1dba-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="d1dba-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="d1dba-145">operatingSystemLanguage</span></span>|<span data-ttu-id="d1dba-146">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-146">String</span></span>|<span data-ttu-id="d1dba-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="d1dba-147">Operating system language of the device</span></span>|
|<span data-ttu-id="d1dba-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="d1dba-148">isSupervised</span></span>|<span data-ttu-id="d1dba-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1dba-149">Boolean</span></span>|<span data-ttu-id="d1dba-150">受监督的设备模式</span><span class="sxs-lookup"><span data-stu-id="d1dba-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="d1dba-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="d1dba-151">isEncrypted</span></span>|<span data-ttu-id="d1dba-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="d1dba-152">Boolean</span></span>|<span data-ttu-id="d1dba-153">设备的加密状态</span><span class="sxs-lookup"><span data-stu-id="d1dba-153">Encryption status of the device</span></span>|
|<span data-ttu-id="d1dba-154">batterySerialNumber</span><span class="sxs-lookup"><span data-stu-id="d1dba-154">batterySerialNumber</span></span>|<span data-ttu-id="d1dba-155">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-155">String</span></span>|<span data-ttu-id="d1dba-156">设备的当前电池的序列号</span><span class="sxs-lookup"><span data-stu-id="d1dba-156">The serial number of the device’s current battery</span></span>|
|<span data-ttu-id="d1dba-157">batteryHealthPercentage</span><span class="sxs-lookup"><span data-stu-id="d1dba-157">batteryHealthPercentage</span></span>|<span data-ttu-id="d1dba-158">Int32</span><span class="sxs-lookup"><span data-stu-id="d1dba-158">Int32</span></span>|<span data-ttu-id="d1dba-159">设备的当前电池的运行状况百分比。</span><span class="sxs-lookup"><span data-stu-id="d1dba-159">The device’s current battery’s health percentage.</span></span> <span data-ttu-id="d1dba-160">有效值为 0 至 100</span><span class="sxs-lookup"><span data-stu-id="d1dba-160">Valid values 0 to 100</span></span>|
|<span data-ttu-id="d1dba-161">batteryChargeCycles</span><span class="sxs-lookup"><span data-stu-id="d1dba-161">batteryChargeCycles</span></span>|<span data-ttu-id="d1dba-162">Int32</span><span class="sxs-lookup"><span data-stu-id="d1dba-162">Int32</span></span>|<span data-ttu-id="d1dba-163">设备的当前电池已过期的充电周期数。</span><span class="sxs-lookup"><span data-stu-id="d1dba-163">The number of charge cycles the device’s current battery has gone through.</span></span> <span data-ttu-id="d1dba-164">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="d1dba-164">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="d1dba-165">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="d1dba-165">isSharedDevice</span></span>|<span data-ttu-id="d1dba-166">布尔</span><span class="sxs-lookup"><span data-stu-id="d1dba-166">Boolean</span></span>|<span data-ttu-id="d1dba-167">共享 iPad</span><span class="sxs-lookup"><span data-stu-id="d1dba-167">Shared iPad</span></span>|
|<span data-ttu-id="d1dba-168">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="d1dba-168">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="d1dba-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d1dba-169">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="d1dba-170">共享 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="d1dba-170">All users on the shared Apple device</span></span>|
|<span data-ttu-id="d1dba-171">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="d1dba-171">tpmSpecificationVersion</span></span>|<span data-ttu-id="d1dba-172">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-172">String</span></span>|<span data-ttu-id="d1dba-173">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="d1dba-173">String that specifies the specification version.</span></span>|
|<span data-ttu-id="d1dba-174">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="d1dba-174">operatingSystemEdition</span></span>|<span data-ttu-id="d1dba-175">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-175">String</span></span>|<span data-ttu-id="d1dba-176">指定 OS 版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="d1dba-176">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="d1dba-177">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="d1dba-177">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="d1dba-178">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-178">String</span></span>|<span data-ttu-id="d1dba-179">如果任何) ，则返回设备 (的完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="d1dba-179">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="d1dba-180">如果设备未加入域，则返回一个空字符串。</span><span class="sxs-lookup"><span data-stu-id="d1dba-180">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="d1dba-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="d1dba-181">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="d1dba-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="d1dba-182">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="d1dba-183">基于虚拟化的安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="d1dba-183">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="d1dba-184">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="d1dba-184">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="d1dba-185">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="d1dba-185">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="d1dba-186">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="d1dba-186">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="d1dba-187">基于虚拟化的安全状态。</span><span class="sxs-lookup"><span data-stu-id="d1dba-187">Virtualization-based security status.</span></span> <span data-ttu-id="d1dba-188">.</span><span class="sxs-lookup"><span data-stu-id="d1dba-188">.</span></span> <span data-ttu-id="d1dba-189">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="d1dba-189">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="d1dba-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="d1dba-190">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="d1dba-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="d1dba-191">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="d1dba-192">本地系统颁发机构 (LSA) credential guard 状态。</span><span class="sxs-lookup"><span data-stu-id="d1dba-192">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="d1dba-193">.</span><span class="sxs-lookup"><span data-stu-id="d1dba-193">.</span></span> <span data-ttu-id="d1dba-194">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="d1dba-194">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="d1dba-195">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="d1dba-195">osBuildNumber</span></span>|<span data-ttu-id="d1dba-196">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-196">String</span></span>|<span data-ttu-id="d1dba-197">Android 设备上的操作系统内部版本号</span><span class="sxs-lookup"><span data-stu-id="d1dba-197">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="d1dba-198">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="d1dba-198">operatingSystemProductType</span></span>|<span data-ttu-id="d1dba-199">Int32</span><span class="sxs-lookup"><span data-stu-id="d1dba-199">Int32</span></span>|<span data-ttu-id="d1dba-200">指定 Windows 操作系统 ProductType 的 Int。</span><span class="sxs-lookup"><span data-stu-id="d1dba-200">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="d1dba-201">此处提供了更多详细信息 https://go.microsoft.com/fwlink/?linkid=2126950 。</span><span class="sxs-lookup"><span data-stu-id="d1dba-201">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="d1dba-202">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="d1dba-202">Valid values 0 to 2147483647</span></span>|
|<span data-ttu-id="d1dba-203">ipAddressV4</span><span class="sxs-lookup"><span data-stu-id="d1dba-203">ipAddressV4</span></span>|<span data-ttu-id="d1dba-204">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-204">String</span></span>|<span data-ttu-id="d1dba-205">IPAddressV4</span><span class="sxs-lookup"><span data-stu-id="d1dba-205">IPAddressV4</span></span>|
|<span data-ttu-id="d1dba-206">subnetAddress</span><span class="sxs-lookup"><span data-stu-id="d1dba-206">subnetAddress</span></span>|<span data-ttu-id="d1dba-207">String</span><span class="sxs-lookup"><span data-stu-id="d1dba-207">String</span></span>|<span data-ttu-id="d1dba-208">SubnetAddress</span><span class="sxs-lookup"><span data-stu-id="d1dba-208">SubnetAddress</span></span>|

## <a name="relationships"></a><span data-ttu-id="d1dba-209">关系</span><span class="sxs-lookup"><span data-stu-id="d1dba-209">Relationships</span></span>
<span data-ttu-id="d1dba-210">无</span><span class="sxs-lookup"><span data-stu-id="d1dba-210">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d1dba-211">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d1dba-211">JSON Representation</span></span>
<span data-ttu-id="d1dba-212">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d1dba-212">Here is a JSON representation of the resource.</span></span>
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
  "subnetAddress": "String"
}
```





