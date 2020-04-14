---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 15369ff988d13e7d083358dceb874da2a0ffa6a4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470640"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="9e330-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e330-103">hardwareInformation resource type</span></span>

<span data-ttu-id="9e330-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e330-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e330-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e330-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e330-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e330-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e330-107">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="9e330-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="9e330-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e330-108">Properties</span></span>
|<span data-ttu-id="9e330-109">属性</span><span class="sxs-lookup"><span data-stu-id="9e330-109">Property</span></span>|<span data-ttu-id="9e330-110">类型</span><span class="sxs-lookup"><span data-stu-id="9e330-110">Type</span></span>|<span data-ttu-id="9e330-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e330-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e330-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="9e330-112">serialNumber</span></span>|<span data-ttu-id="9e330-113">字符串</span><span class="sxs-lookup"><span data-stu-id="9e330-113">String</span></span>|<span data-ttu-id="9e330-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="9e330-114">Serial number.</span></span>|
|<span data-ttu-id="9e330-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="9e330-115">totalStorageSpace</span></span>|<span data-ttu-id="9e330-116">Int64</span><span class="sxs-lookup"><span data-stu-id="9e330-116">Int64</span></span>|<span data-ttu-id="9e330-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="9e330-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="9e330-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="9e330-118">freeStorageSpace</span></span>|<span data-ttu-id="9e330-119">Int64</span><span class="sxs-lookup"><span data-stu-id="9e330-119">Int64</span></span>|<span data-ttu-id="9e330-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="9e330-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="9e330-121">imei</span><span class="sxs-lookup"><span data-stu-id="9e330-121">imei</span></span>|<span data-ttu-id="9e330-122">String</span><span class="sxs-lookup"><span data-stu-id="9e330-122">String</span></span>|<span data-ttu-id="9e330-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="9e330-123">IMEI</span></span>|
|<span data-ttu-id="9e330-124">meid</span><span class="sxs-lookup"><span data-stu-id="9e330-124">meid</span></span>|<span data-ttu-id="9e330-125">String</span><span class="sxs-lookup"><span data-stu-id="9e330-125">String</span></span>|<span data-ttu-id="9e330-126">MEID</span><span class="sxs-lookup"><span data-stu-id="9e330-126">MEID</span></span>|
|<span data-ttu-id="9e330-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="9e330-127">manufacturer</span></span>|<span data-ttu-id="9e330-128">String</span><span class="sxs-lookup"><span data-stu-id="9e330-128">String</span></span>|<span data-ttu-id="9e330-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="9e330-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="9e330-130">model</span><span class="sxs-lookup"><span data-stu-id="9e330-130">model</span></span>|<span data-ttu-id="9e330-131">String</span><span class="sxs-lookup"><span data-stu-id="9e330-131">String</span></span>|<span data-ttu-id="9e330-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="9e330-132">Model of the device</span></span>|
|<span data-ttu-id="9e330-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="9e330-133">phoneNumber</span></span>|<span data-ttu-id="9e330-134">String</span><span class="sxs-lookup"><span data-stu-id="9e330-134">String</span></span>|<span data-ttu-id="9e330-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="9e330-135">Phone number of the device</span></span>|
|<span data-ttu-id="9e330-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="9e330-136">subscriberCarrier</span></span>|<span data-ttu-id="9e330-137">String</span><span class="sxs-lookup"><span data-stu-id="9e330-137">String</span></span>|<span data-ttu-id="9e330-138">设备的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="9e330-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="9e330-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="9e330-139">cellularTechnology</span></span>|<span data-ttu-id="9e330-140">String</span><span class="sxs-lookup"><span data-stu-id="9e330-140">String</span></span>|<span data-ttu-id="9e330-141">设备的手机网络技术</span><span class="sxs-lookup"><span data-stu-id="9e330-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="9e330-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="9e330-142">wifiMac</span></span>|<span data-ttu-id="9e330-143">String</span><span class="sxs-lookup"><span data-stu-id="9e330-143">String</span></span>|<span data-ttu-id="9e330-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="9e330-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="9e330-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="9e330-145">operatingSystemLanguage</span></span>|<span data-ttu-id="9e330-146">String</span><span class="sxs-lookup"><span data-stu-id="9e330-146">String</span></span>|<span data-ttu-id="9e330-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="9e330-147">Operating system language of the device</span></span>|
|<span data-ttu-id="9e330-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="9e330-148">isSupervised</span></span>|<span data-ttu-id="9e330-149">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e330-149">Boolean</span></span>|<span data-ttu-id="9e330-150">受监督的设备模式</span><span class="sxs-lookup"><span data-stu-id="9e330-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="9e330-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="9e330-151">isEncrypted</span></span>|<span data-ttu-id="9e330-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e330-152">Boolean</span></span>|<span data-ttu-id="9e330-153">设备的加密状态</span><span class="sxs-lookup"><span data-stu-id="9e330-153">Encryption status of the device</span></span>|
|<span data-ttu-id="9e330-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="9e330-154">isSharedDevice</span></span>|<span data-ttu-id="9e330-155">布尔值</span><span class="sxs-lookup"><span data-stu-id="9e330-155">Boolean</span></span>|<span data-ttu-id="9e330-156">共享 iPad</span><span class="sxs-lookup"><span data-stu-id="9e330-156">Shared iPad</span></span>|
|<span data-ttu-id="9e330-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="9e330-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="9e330-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="9e330-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="9e330-159">共享 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="9e330-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="9e330-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="9e330-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="9e330-161">String</span><span class="sxs-lookup"><span data-stu-id="9e330-161">String</span></span>|<span data-ttu-id="9e330-162">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="9e330-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="9e330-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="9e330-163">operatingSystemEdition</span></span>|<span data-ttu-id="9e330-164">String</span><span class="sxs-lookup"><span data-stu-id="9e330-164">String</span></span>|<span data-ttu-id="9e330-165">指定 OS 版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="9e330-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="9e330-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="9e330-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="9e330-167">String</span><span class="sxs-lookup"><span data-stu-id="9e330-167">String</span></span>|<span data-ttu-id="9e330-168">返回设备的完全限定的域名（如果有）。</span><span class="sxs-lookup"><span data-stu-id="9e330-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="9e330-169">如果设备未加入域，则返回一个空字符串。</span><span class="sxs-lookup"><span data-stu-id="9e330-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="9e330-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="9e330-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="9e330-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="9e330-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="9e330-172">基于虚拟化的安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="9e330-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="9e330-173">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="9e330-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="9e330-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="9e330-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="9e330-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="9e330-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="9e330-176">基于虚拟化的安全状态。</span><span class="sxs-lookup"><span data-stu-id="9e330-176">Virtualization-based security status.</span></span> <span data-ttu-id="9e330-177">.</span><span class="sxs-lookup"><span data-stu-id="9e330-177">.</span></span> <span data-ttu-id="9e330-178">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="9e330-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="9e330-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="9e330-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="9e330-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="9e330-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="9e330-181">本地系统颁发机构（LSA） credential guard 状态。</span><span class="sxs-lookup"><span data-stu-id="9e330-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="9e330-182">.</span><span class="sxs-lookup"><span data-stu-id="9e330-182">.</span></span> <span data-ttu-id="9e330-183">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="9e330-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|
|<span data-ttu-id="9e330-184">osBuildNumber</span><span class="sxs-lookup"><span data-stu-id="9e330-184">osBuildNumber</span></span>|<span data-ttu-id="9e330-185">String</span><span class="sxs-lookup"><span data-stu-id="9e330-185">String</span></span>|<span data-ttu-id="9e330-186">Android 设备上的操作系统内部版本号</span><span class="sxs-lookup"><span data-stu-id="9e330-186">Operating System Build Number on Android device</span></span>|

## <a name="relationships"></a><span data-ttu-id="9e330-187">关系</span><span class="sxs-lookup"><span data-stu-id="9e330-187">Relationships</span></span>
<span data-ttu-id="9e330-188">无</span><span class="sxs-lookup"><span data-stu-id="9e330-188">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9e330-189">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e330-189">JSON Representation</span></span>
<span data-ttu-id="9e330-190">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e330-190">Here is a JSON representation of the resource.</span></span>
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
  "osBuildNumber": "String"
}
```



