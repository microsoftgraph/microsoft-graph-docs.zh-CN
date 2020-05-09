---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bc09cbb5f1c3664d0f9a2bcb0cc0aceac7f85bf3
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44178841"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="b3a80-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b3a80-103">hardwareInformation resource type</span></span>

<span data-ttu-id="b3a80-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3a80-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3a80-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3a80-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3a80-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3a80-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3a80-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="b3a80-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="b3a80-108">属性</span><span class="sxs-lookup"><span data-stu-id="b3a80-108">Properties</span></span>
|<span data-ttu-id="b3a80-109">属性</span><span class="sxs-lookup"><span data-stu-id="b3a80-109">Property</span></span>|<span data-ttu-id="b3a80-110">类型</span><span class="sxs-lookup"><span data-stu-id="b3a80-110">Type</span></span>|<span data-ttu-id="b3a80-111">说明</span><span class="sxs-lookup"><span data-stu-id="b3a80-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3a80-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b3a80-112">serialNumber</span></span>|<span data-ttu-id="b3a80-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-113">String</span></span>|<span data-ttu-id="b3a80-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="b3a80-114">Serial number.</span></span>|
|<span data-ttu-id="b3a80-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="b3a80-115">totalStorageSpace</span></span>|<span data-ttu-id="b3a80-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b3a80-116">Int64</span></span>|<span data-ttu-id="b3a80-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="b3a80-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="b3a80-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="b3a80-118">freeStorageSpace</span></span>|<span data-ttu-id="b3a80-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b3a80-119">Int64</span></span>|<span data-ttu-id="b3a80-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="b3a80-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="b3a80-121">imei</span><span class="sxs-lookup"><span data-stu-id="b3a80-121">imei</span></span>|<span data-ttu-id="b3a80-122">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-122">String</span></span>|<span data-ttu-id="b3a80-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="b3a80-123">IMEI</span></span>|
|<span data-ttu-id="b3a80-124">meid</span><span class="sxs-lookup"><span data-stu-id="b3a80-124">meid</span></span>|<span data-ttu-id="b3a80-125">String</span><span class="sxs-lookup"><span data-stu-id="b3a80-125">String</span></span>|<span data-ttu-id="b3a80-126">MEID</span><span class="sxs-lookup"><span data-stu-id="b3a80-126">MEID</span></span>|
|<span data-ttu-id="b3a80-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b3a80-127">manufacturer</span></span>|<span data-ttu-id="b3a80-128">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-128">String</span></span>|<span data-ttu-id="b3a80-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="b3a80-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="b3a80-130">model</span><span class="sxs-lookup"><span data-stu-id="b3a80-130">model</span></span>|<span data-ttu-id="b3a80-131">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-131">String</span></span>|<span data-ttu-id="b3a80-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="b3a80-132">Model of the device</span></span>|
|<span data-ttu-id="b3a80-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b3a80-133">phoneNumber</span></span>|<span data-ttu-id="b3a80-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-134">String</span></span>|<span data-ttu-id="b3a80-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="b3a80-135">Phone number of the device</span></span>|
|<span data-ttu-id="b3a80-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="b3a80-136">subscriberCarrier</span></span>|<span data-ttu-id="b3a80-137">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-137">String</span></span>|<span data-ttu-id="b3a80-138">设备的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="b3a80-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="b3a80-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="b3a80-139">cellularTechnology</span></span>|<span data-ttu-id="b3a80-140">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-140">String</span></span>|<span data-ttu-id="b3a80-141">设备的手机网络技术</span><span class="sxs-lookup"><span data-stu-id="b3a80-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="b3a80-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="b3a80-142">wifiMac</span></span>|<span data-ttu-id="b3a80-143">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-143">String</span></span>|<span data-ttu-id="b3a80-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="b3a80-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="b3a80-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="b3a80-145">operatingSystemLanguage</span></span>|<span data-ttu-id="b3a80-146">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-146">String</span></span>|<span data-ttu-id="b3a80-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="b3a80-147">Operating system language of the device</span></span>|
|<span data-ttu-id="b3a80-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="b3a80-148">isSupervised</span></span>|<span data-ttu-id="b3a80-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3a80-149">Boolean</span></span>|<span data-ttu-id="b3a80-150">受监督的设备模式</span><span class="sxs-lookup"><span data-stu-id="b3a80-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="b3a80-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="b3a80-151">isEncrypted</span></span>|<span data-ttu-id="b3a80-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3a80-152">Boolean</span></span>|<span data-ttu-id="b3a80-153">设备的加密状态</span><span class="sxs-lookup"><span data-stu-id="b3a80-153">Encryption status of the device</span></span>|
|<span data-ttu-id="b3a80-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="b3a80-154">isSharedDevice</span></span>|<span data-ttu-id="b3a80-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3a80-155">Boolean</span></span>|<span data-ttu-id="b3a80-156">共享 iPad</span><span class="sxs-lookup"><span data-stu-id="b3a80-156">Shared iPad</span></span>|
|<span data-ttu-id="b3a80-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="b3a80-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="b3a80-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="b3a80-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="b3a80-159">共享 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="b3a80-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="b3a80-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="b3a80-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="b3a80-161">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-161">String</span></span>|<span data-ttu-id="b3a80-162">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="b3a80-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="b3a80-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="b3a80-163">operatingSystemEdition</span></span>|<span data-ttu-id="b3a80-164">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-164">String</span></span>|<span data-ttu-id="b3a80-165">指定 OS 版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="b3a80-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="b3a80-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="b3a80-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="b3a80-167">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-167">String</span></span>|<span data-ttu-id="b3a80-168">返回设备的完全限定的域名（如果有）。</span><span class="sxs-lookup"><span data-stu-id="b3a80-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="b3a80-169">如果设备未加入域，则返回一个空字符串。</span><span class="sxs-lookup"><span data-stu-id="b3a80-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="b3a80-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="b3a80-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="b3a80-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="b3a80-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="b3a80-172">基于虚拟化的安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="b3a80-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="b3a80-173">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="b3a80-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="b3a80-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="b3a80-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="b3a80-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="b3a80-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="b3a80-176">基于虚拟化的安全状态。</span><span class="sxs-lookup"><span data-stu-id="b3a80-176">Virtualization-based security status.</span></span> <span data-ttu-id="b3a80-177">.</span><span class="sxs-lookup"><span data-stu-id="b3a80-177">.</span></span> <span data-ttu-id="b3a80-178">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="b3a80-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="b3a80-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="b3a80-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="b3a80-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="b3a80-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="b3a80-181">本地系统颁发机构（LSA） credential guard 状态。</span><span class="sxs-lookup"><span data-stu-id="b3a80-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="b3a80-182">.</span><span class="sxs-lookup"><span data-stu-id="b3a80-182">.</span></span> <span data-ttu-id="b3a80-183">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="b3a80-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="b3a80-184">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="b3a80-184">osBuildNumber</span></span>|<span data-ttu-id="b3a80-185">字符串</span><span class="sxs-lookup"><span data-stu-id="b3a80-185">String</span></span>|<span data-ttu-id="b3a80-186">Android 设备上的操作系统内部版本号</span><span class="sxs-lookup"><span data-stu-id="b3a80-186">Operating System Build Number on Android device</span></span>|
|<span data-ttu-id="b3a80-187">operatingSystemProductType</span><span class="sxs-lookup"><span data-stu-id="b3a80-187">operatingSystemProductType</span></span>|<span data-ttu-id="b3a80-188">Int32</span><span class="sxs-lookup"><span data-stu-id="b3a80-188">Int32</span></span>|<span data-ttu-id="b3a80-189">指定 Windows 操作系统 ProductType 的 Int。</span><span class="sxs-lookup"><span data-stu-id="b3a80-189">Int that specifies the Windows Operating System ProductType.</span></span> <span data-ttu-id="b3a80-190">此处https://go.microsoft.com/fwlink/?linkid=2126950提供了更多详细信息。</span><span class="sxs-lookup"><span data-stu-id="b3a80-190">More details here https://go.microsoft.com/fwlink/?linkid=2126950.</span></span> <span data-ttu-id="b3a80-191">有效值为0至2147483647</span><span class="sxs-lookup"><span data-stu-id="b3a80-191">Valid values 0 to 2147483647</span></span>|

## <a name="relationships"></a><span data-ttu-id="b3a80-192">关系</span><span class="sxs-lookup"><span data-stu-id="b3a80-192">Relationships</span></span>
<span data-ttu-id="b3a80-193">无</span><span class="sxs-lookup"><span data-stu-id="b3a80-193">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b3a80-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b3a80-194">JSON Representation</span></span>
<span data-ttu-id="b3a80-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3a80-195">Here is a JSON representation of the resource.</span></span>
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



