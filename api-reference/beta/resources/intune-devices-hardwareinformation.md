---
title: hardwareInformation 资源类型
description: 给定设备的硬件信息。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7cbbd95c495a970dfddbc3b6c78e5e784b43d297
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34995194"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="4cf0c-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="4cf0c-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="4cf0c-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4cf0c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4cf0c-106">给定设备的硬件信息。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-106">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="4cf0c-107">属性</span><span class="sxs-lookup"><span data-stu-id="4cf0c-107">Properties</span></span>
|<span data-ttu-id="4cf0c-108">属性</span><span class="sxs-lookup"><span data-stu-id="4cf0c-108">Property</span></span>|<span data-ttu-id="4cf0c-109">类型</span><span class="sxs-lookup"><span data-stu-id="4cf0c-109">Type</span></span>|<span data-ttu-id="4cf0c-110">说明</span><span class="sxs-lookup"><span data-stu-id="4cf0c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cf0c-111">serialNumber</span><span class="sxs-lookup"><span data-stu-id="4cf0c-111">serialNumber</span></span>|<span data-ttu-id="4cf0c-112">字符串</span><span class="sxs-lookup"><span data-stu-id="4cf0c-112">String</span></span>|<span data-ttu-id="4cf0c-113">序列号。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-113">Serial number.</span></span>|
|<span data-ttu-id="4cf0c-114">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="4cf0c-114">totalStorageSpace</span></span>|<span data-ttu-id="4cf0c-115">Int64</span><span class="sxs-lookup"><span data-stu-id="4cf0c-115">Int64</span></span>|<span data-ttu-id="4cf0c-116">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-116">Total storage space of the device.</span></span>|
|<span data-ttu-id="4cf0c-117">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="4cf0c-117">freeStorageSpace</span></span>|<span data-ttu-id="4cf0c-118">Int64</span><span class="sxs-lookup"><span data-stu-id="4cf0c-118">Int64</span></span>|<span data-ttu-id="4cf0c-119">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-119">Free storage space of the device.</span></span>|
|<span data-ttu-id="4cf0c-120">imei</span><span class="sxs-lookup"><span data-stu-id="4cf0c-120">imei</span></span>|<span data-ttu-id="4cf0c-121">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-121">String</span></span>|<span data-ttu-id="4cf0c-122">IMEI</span><span class="sxs-lookup"><span data-stu-id="4cf0c-122">IMEI</span></span>|
|<span data-ttu-id="4cf0c-123">meid</span><span class="sxs-lookup"><span data-stu-id="4cf0c-123">meid</span></span>|<span data-ttu-id="4cf0c-124">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-124">String</span></span>|<span data-ttu-id="4cf0c-125">MEID</span><span class="sxs-lookup"><span data-stu-id="4cf0c-125">MEID</span></span>|
|<span data-ttu-id="4cf0c-126">manufacturer</span><span class="sxs-lookup"><span data-stu-id="4cf0c-126">manufacturer</span></span>|<span data-ttu-id="4cf0c-127">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-127">String</span></span>|<span data-ttu-id="4cf0c-128">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="4cf0c-128">Manufacturer of the device</span></span>|
|<span data-ttu-id="4cf0c-129">model</span><span class="sxs-lookup"><span data-stu-id="4cf0c-129">model</span></span>|<span data-ttu-id="4cf0c-130">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-130">String</span></span>|<span data-ttu-id="4cf0c-131">设备的型号</span><span class="sxs-lookup"><span data-stu-id="4cf0c-131">Model of the device</span></span>|
|<span data-ttu-id="4cf0c-132">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="4cf0c-132">phoneNumber</span></span>|<span data-ttu-id="4cf0c-133">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-133">String</span></span>|<span data-ttu-id="4cf0c-134">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="4cf0c-134">Phone number of the device</span></span>|
|<span data-ttu-id="4cf0c-135">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="4cf0c-135">subscriberCarrier</span></span>|<span data-ttu-id="4cf0c-136">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-136">String</span></span>|<span data-ttu-id="4cf0c-137">设备的订阅者运营商</span><span class="sxs-lookup"><span data-stu-id="4cf0c-137">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="4cf0c-138">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="4cf0c-138">cellularTechnology</span></span>|<span data-ttu-id="4cf0c-139">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-139">String</span></span>|<span data-ttu-id="4cf0c-140">设备的手机网络技术</span><span class="sxs-lookup"><span data-stu-id="4cf0c-140">Cellular technology of the device</span></span>|
|<span data-ttu-id="4cf0c-141">wifiMac</span><span class="sxs-lookup"><span data-stu-id="4cf0c-141">wifiMac</span></span>|<span data-ttu-id="4cf0c-142">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-142">String</span></span>|<span data-ttu-id="4cf0c-143">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="4cf0c-143">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="4cf0c-144">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="4cf0c-144">operatingSystemLanguage</span></span>|<span data-ttu-id="4cf0c-145">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-145">String</span></span>|<span data-ttu-id="4cf0c-146">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="4cf0c-146">Operating system language of the device</span></span>|
|<span data-ttu-id="4cf0c-147">isSupervised</span><span class="sxs-lookup"><span data-stu-id="4cf0c-147">isSupervised</span></span>|<span data-ttu-id="4cf0c-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cf0c-148">Boolean</span></span>|<span data-ttu-id="4cf0c-149">受监督的设备模式</span><span class="sxs-lookup"><span data-stu-id="4cf0c-149">Supervised mode of the device</span></span>|
|<span data-ttu-id="4cf0c-150">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="4cf0c-150">isEncrypted</span></span>|<span data-ttu-id="4cf0c-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cf0c-151">Boolean</span></span>|<span data-ttu-id="4cf0c-152">设备的加密状态</span><span class="sxs-lookup"><span data-stu-id="4cf0c-152">Encryption status of the device</span></span>|
|<span data-ttu-id="4cf0c-153">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="4cf0c-153">isSharedDevice</span></span>|<span data-ttu-id="4cf0c-154">Boolean</span><span class="sxs-lookup"><span data-stu-id="4cf0c-154">Boolean</span></span>|<span data-ttu-id="4cf0c-155">共享 iPad</span><span class="sxs-lookup"><span data-stu-id="4cf0c-155">Shared iPad</span></span>|
|<span data-ttu-id="4cf0c-156">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="4cf0c-156">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="4cf0c-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="4cf0c-157">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="4cf0c-158">共享 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="4cf0c-158">All users on the shared Apple device</span></span>|
|<span data-ttu-id="4cf0c-159">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="4cf0c-159">tpmSpecificationVersion</span></span>|<span data-ttu-id="4cf0c-160">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-160">String</span></span>|<span data-ttu-id="4cf0c-161">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-161">String that specifies the specification version.</span></span>|
|<span data-ttu-id="4cf0c-162">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="4cf0c-162">operatingSystemEdition</span></span>|<span data-ttu-id="4cf0c-163">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-163">String</span></span>|<span data-ttu-id="4cf0c-164">指定 OS 版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-164">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="4cf0c-165">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="4cf0c-165">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="4cf0c-166">String</span><span class="sxs-lookup"><span data-stu-id="4cf0c-166">String</span></span>|<span data-ttu-id="4cf0c-167">返回设备的完全限定的域名 (如果有)。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-167">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="4cf0c-168">如果设备未加入域, 则返回一个空字符串。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-168">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="4cf0c-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="4cf0c-169">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="4cf0c-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="4cf0c-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="4cf0c-171">基于虚拟化的安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-171">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="4cf0c-172">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-172">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="4cf0c-173">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="4cf0c-173">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="4cf0c-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="4cf0c-174">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="4cf0c-175">基于虚拟化的安全状态。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-175">Virtualization-based security status.</span></span> <span data-ttu-id="4cf0c-176">.</span><span class="sxs-lookup"><span data-stu-id="4cf0c-176"></span></span> <span data-ttu-id="4cf0c-177">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements` 或 `other`。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-177">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="4cf0c-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="4cf0c-178">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="4cf0c-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="4cf0c-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="4cf0c-180">本地系统颁发机构 (LSA) credential guard 状态。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-180">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="4cf0c-181">.</span><span class="sxs-lookup"><span data-stu-id="4cf0c-181"></span></span> <span data-ttu-id="4cf0c-182">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-182">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cf0c-183">关系</span><span class="sxs-lookup"><span data-stu-id="4cf0c-183">Relationships</span></span>
<span data-ttu-id="4cf0c-184">无</span><span class="sxs-lookup"><span data-stu-id="4cf0c-184">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4cf0c-185">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4cf0c-185">JSON Representation</span></span>
<span data-ttu-id="4cf0c-186">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cf0c-186">Here is a JSON representation of the resource.</span></span>
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
  "deviceGuardLocalSystemAuthorityCredentialGuardState": "String"
}
```





