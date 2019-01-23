---
title: hardwareInformation 资源类型
description: 硬件的给定设备的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 32b6d0e637c477265a6d23f39e531ca89c7e490c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394822"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="e6070-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="e6070-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="e6070-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e6070-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e6070-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e6070-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e6070-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e6070-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e6070-107">硬件的给定设备的信息。</span><span class="sxs-lookup"><span data-stu-id="e6070-107">Hardware information of a given device.</span></span>

## <a name="properties"></a><span data-ttu-id="e6070-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6070-108">Properties</span></span>
|<span data-ttu-id="e6070-109">属性</span><span class="sxs-lookup"><span data-stu-id="e6070-109">Property</span></span>|<span data-ttu-id="e6070-110">类型</span><span class="sxs-lookup"><span data-stu-id="e6070-110">Type</span></span>|<span data-ttu-id="e6070-111">说明</span><span class="sxs-lookup"><span data-stu-id="e6070-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e6070-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="e6070-112">serialNumber</span></span>|<span data-ttu-id="e6070-113">String</span><span class="sxs-lookup"><span data-stu-id="e6070-113">String</span></span>|<span data-ttu-id="e6070-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="e6070-114">Serial number.</span></span>|
|<span data-ttu-id="e6070-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="e6070-115">totalStorageSpace</span></span>|<span data-ttu-id="e6070-116">Int64</span><span class="sxs-lookup"><span data-stu-id="e6070-116">Int64</span></span>|<span data-ttu-id="e6070-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="e6070-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="e6070-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="e6070-118">freeStorageSpace</span></span>|<span data-ttu-id="e6070-119">Int64</span><span class="sxs-lookup"><span data-stu-id="e6070-119">Int64</span></span>|<span data-ttu-id="e6070-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="e6070-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="e6070-121">imei</span><span class="sxs-lookup"><span data-stu-id="e6070-121">imei</span></span>|<span data-ttu-id="e6070-122">String</span><span class="sxs-lookup"><span data-stu-id="e6070-122">String</span></span>|<span data-ttu-id="e6070-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="e6070-123">IMEI</span></span>|
|<span data-ttu-id="e6070-124">meid</span><span class="sxs-lookup"><span data-stu-id="e6070-124">meid</span></span>|<span data-ttu-id="e6070-125">String</span><span class="sxs-lookup"><span data-stu-id="e6070-125">String</span></span>|<span data-ttu-id="e6070-126">MEID</span><span class="sxs-lookup"><span data-stu-id="e6070-126">MEID</span></span>|
|<span data-ttu-id="e6070-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="e6070-127">manufacturer</span></span>|<span data-ttu-id="e6070-128">String</span><span class="sxs-lookup"><span data-stu-id="e6070-128">String</span></span>|<span data-ttu-id="e6070-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="e6070-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="e6070-130">model</span><span class="sxs-lookup"><span data-stu-id="e6070-130">model</span></span>|<span data-ttu-id="e6070-131">String</span><span class="sxs-lookup"><span data-stu-id="e6070-131">String</span></span>|<span data-ttu-id="e6070-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="e6070-132">Model of the device</span></span>|
|<span data-ttu-id="e6070-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="e6070-133">phoneNumber</span></span>|<span data-ttu-id="e6070-134">String</span><span class="sxs-lookup"><span data-stu-id="e6070-134">String</span></span>|<span data-ttu-id="e6070-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="e6070-135">Phone number of the device</span></span>|
|<span data-ttu-id="e6070-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="e6070-136">subscriberCarrier</span></span>|<span data-ttu-id="e6070-137">String</span><span class="sxs-lookup"><span data-stu-id="e6070-137">String</span></span>|<span data-ttu-id="e6070-138">订阅者运营商的设备</span><span class="sxs-lookup"><span data-stu-id="e6070-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="e6070-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="e6070-139">cellularTechnology</span></span>|<span data-ttu-id="e6070-140">String</span><span class="sxs-lookup"><span data-stu-id="e6070-140">String</span></span>|<span data-ttu-id="e6070-141">移动电话的设备的技术</span><span class="sxs-lookup"><span data-stu-id="e6070-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="e6070-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="e6070-142">wifiMac</span></span>|<span data-ttu-id="e6070-143">String</span><span class="sxs-lookup"><span data-stu-id="e6070-143">String</span></span>|<span data-ttu-id="e6070-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="e6070-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="e6070-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="e6070-145">operatingSystemLanguage</span></span>|<span data-ttu-id="e6070-146">String</span><span class="sxs-lookup"><span data-stu-id="e6070-146">String</span></span>|<span data-ttu-id="e6070-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="e6070-147">Operating system language of the device</span></span>|
|<span data-ttu-id="e6070-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="e6070-148">isSupervised</span></span>|<span data-ttu-id="e6070-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6070-149">Boolean</span></span>|<span data-ttu-id="e6070-150">设备监管的模式</span><span class="sxs-lookup"><span data-stu-id="e6070-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="e6070-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="e6070-151">isEncrypted</span></span>|<span data-ttu-id="e6070-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6070-152">Boolean</span></span>|<span data-ttu-id="e6070-153">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="e6070-153">Encryption status of the device</span></span>|
|<span data-ttu-id="e6070-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="e6070-154">isSharedDevice</span></span>|<span data-ttu-id="e6070-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="e6070-155">Boolean</span></span>|<span data-ttu-id="e6070-156">共享的 iPad</span><span class="sxs-lookup"><span data-stu-id="e6070-156">Shared iPad</span></span>|
|<span data-ttu-id="e6070-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="e6070-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="e6070-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="e6070-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="e6070-159">共享的 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="e6070-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="e6070-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="e6070-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="e6070-161">String</span><span class="sxs-lookup"><span data-stu-id="e6070-161">String</span></span>|<span data-ttu-id="e6070-162">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="e6070-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="e6070-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="e6070-163">operatingSystemEdition</span></span>|<span data-ttu-id="e6070-164">String</span><span class="sxs-lookup"><span data-stu-id="e6070-164">String</span></span>|<span data-ttu-id="e6070-165">指定的操作系统版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="e6070-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="e6070-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="e6070-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="e6070-167">String</span><span class="sxs-lookup"><span data-stu-id="e6070-167">String</span></span>|<span data-ttu-id="e6070-168">（如果有），则返回设备的完全限定的的域名。</span><span class="sxs-lookup"><span data-stu-id="e6070-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="e6070-169">如果设备不加入域的它将返回空字符串。</span><span class="sxs-lookup"><span data-stu-id="e6070-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="e6070-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="e6070-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="e6070-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="e6070-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="e6070-172">虚拟化基于安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="e6070-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="e6070-173">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="e6070-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="e6070-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="e6070-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="e6070-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="e6070-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="e6070-176">虚拟化基于安全状态。</span><span class="sxs-lookup"><span data-stu-id="e6070-176">Virtualization-based security status.</span></span> <span data-ttu-id="e6070-177">.</span><span class="sxs-lookup"><span data-stu-id="e6070-177"></span></span> <span data-ttu-id="e6070-178">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other`。</span><span class="sxs-lookup"><span data-stu-id="e6070-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="e6070-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="e6070-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="e6070-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="e6070-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="e6070-181">本地系统证书颁发机构 (LSA) 凭据 guard 状态。</span><span class="sxs-lookup"><span data-stu-id="e6070-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="e6070-182">.</span><span class="sxs-lookup"><span data-stu-id="e6070-182"></span></span> <span data-ttu-id="e6070-183">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="e6070-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6070-184">关系</span><span class="sxs-lookup"><span data-stu-id="e6070-184">Relationships</span></span>
<span data-ttu-id="e6070-185">无</span><span class="sxs-lookup"><span data-stu-id="e6070-185">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e6070-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e6070-186">JSON Representation</span></span>
<span data-ttu-id="e6070-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e6070-187">Here is a JSON representation of the resource.</span></span>
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




