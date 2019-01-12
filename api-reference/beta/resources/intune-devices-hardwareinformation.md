---
title: hardwareInformation 资源类型
description: 硬件的给定设备的信息。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0665152e3cc483f2303f458b79c891658651d91f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930311"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="68f6f-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="68f6f-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="68f6f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="68f6f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68f6f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="68f6f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="68f6f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="68f6f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="68f6f-107">硬件的给定设备的信息。</span><span class="sxs-lookup"><span data-stu-id="68f6f-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="68f6f-108">属性</span><span class="sxs-lookup"><span data-stu-id="68f6f-108">Properties</span></span>
|<span data-ttu-id="68f6f-109">属性</span><span class="sxs-lookup"><span data-stu-id="68f6f-109">Property</span></span>|<span data-ttu-id="68f6f-110">类型</span><span class="sxs-lookup"><span data-stu-id="68f6f-110">Type</span></span>|<span data-ttu-id="68f6f-111">说明</span><span class="sxs-lookup"><span data-stu-id="68f6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68f6f-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="68f6f-112">serialNumber</span></span>|<span data-ttu-id="68f6f-113">字符串</span><span class="sxs-lookup"><span data-stu-id="68f6f-113">String</span></span>|<span data-ttu-id="68f6f-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="68f6f-114">Serial number.</span></span>|
|<span data-ttu-id="68f6f-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="68f6f-115">totalStorageSpace</span></span>|<span data-ttu-id="68f6f-116">Int64</span><span class="sxs-lookup"><span data-stu-id="68f6f-116">Int64</span></span>|<span data-ttu-id="68f6f-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="68f6f-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="68f6f-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="68f6f-118">freeStorageSpace</span></span>|<span data-ttu-id="68f6f-119">Int64</span><span class="sxs-lookup"><span data-stu-id="68f6f-119">Int64</span></span>|<span data-ttu-id="68f6f-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="68f6f-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="68f6f-121">imei</span><span class="sxs-lookup"><span data-stu-id="68f6f-121">imei</span></span>|<span data-ttu-id="68f6f-122">String</span><span class="sxs-lookup"><span data-stu-id="68f6f-122">String</span></span>|<span data-ttu-id="68f6f-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="68f6f-123">IMEI</span></span>|
|<span data-ttu-id="68f6f-124">meid</span><span class="sxs-lookup"><span data-stu-id="68f6f-124">meid</span></span>|<span data-ttu-id="68f6f-125">String</span><span class="sxs-lookup"><span data-stu-id="68f6f-125">String</span></span>|<span data-ttu-id="68f6f-126">MEID</span><span class="sxs-lookup"><span data-stu-id="68f6f-126">MEID</span></span>|
|<span data-ttu-id="68f6f-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="68f6f-127">manufacturer</span></span>|<span data-ttu-id="68f6f-128">String</span><span class="sxs-lookup"><span data-stu-id="68f6f-128">String</span></span>|<span data-ttu-id="68f6f-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="68f6f-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="68f6f-130">model</span><span class="sxs-lookup"><span data-stu-id="68f6f-130">model</span></span>|<span data-ttu-id="68f6f-131">String</span><span class="sxs-lookup"><span data-stu-id="68f6f-131">String</span></span>|<span data-ttu-id="68f6f-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="68f6f-132">Model of the device</span></span>|
|<span data-ttu-id="68f6f-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="68f6f-133">phoneNumber</span></span>|<span data-ttu-id="68f6f-134">String</span><span class="sxs-lookup"><span data-stu-id="68f6f-134">String</span></span>|<span data-ttu-id="68f6f-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="68f6f-135">Phone number of the device</span></span>|
|<span data-ttu-id="68f6f-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="68f6f-136">subscriberCarrier</span></span>|<span data-ttu-id="68f6f-137">String</span><span class="sxs-lookup"><span data-stu-id="68f6f-137">String</span></span>|<span data-ttu-id="68f6f-138">订阅者运营商的设备</span><span class="sxs-lookup"><span data-stu-id="68f6f-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="68f6f-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="68f6f-139">cellularTechnology</span></span>|<span data-ttu-id="68f6f-140">字符串</span><span class="sxs-lookup"><span data-stu-id="68f6f-140">String</span></span>|<span data-ttu-id="68f6f-141">移动电话的设备的技术</span><span class="sxs-lookup"><span data-stu-id="68f6f-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="68f6f-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="68f6f-142">wifiMac</span></span>|<span data-ttu-id="68f6f-143">字符串</span><span class="sxs-lookup"><span data-stu-id="68f6f-143">String</span></span>|<span data-ttu-id="68f6f-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="68f6f-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="68f6f-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="68f6f-145">operatingSystemLanguage</span></span>|<span data-ttu-id="68f6f-146">字符串</span><span class="sxs-lookup"><span data-stu-id="68f6f-146">String</span></span>|<span data-ttu-id="68f6f-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="68f6f-147">Operating system language of the device</span></span>|
|<span data-ttu-id="68f6f-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="68f6f-148">isSupervised</span></span>|<span data-ttu-id="68f6f-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="68f6f-149">Boolean</span></span>|<span data-ttu-id="68f6f-150">设备监管的模式</span><span class="sxs-lookup"><span data-stu-id="68f6f-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="68f6f-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="68f6f-151">isEncrypted</span></span>|<span data-ttu-id="68f6f-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="68f6f-152">Boolean</span></span>|<span data-ttu-id="68f6f-153">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="68f6f-153">Encryption status of the device</span></span>|
|<span data-ttu-id="68f6f-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="68f6f-154">isSharedDevice</span></span>|<span data-ttu-id="68f6f-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="68f6f-155">Boolean</span></span>|<span data-ttu-id="68f6f-156">共享的 iPad</span><span class="sxs-lookup"><span data-stu-id="68f6f-156">Shared iPad</span></span>|
|<span data-ttu-id="68f6f-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="68f6f-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="68f6f-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="68f6f-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="68f6f-159">共享的 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="68f6f-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="68f6f-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="68f6f-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="68f6f-161">字符串</span><span class="sxs-lookup"><span data-stu-id="68f6f-161">String</span></span>|<span data-ttu-id="68f6f-162">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="68f6f-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="68f6f-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="68f6f-163">operatingSystemEdition</span></span>|<span data-ttu-id="68f6f-164">字符串</span><span class="sxs-lookup"><span data-stu-id="68f6f-164">String</span></span>|<span data-ttu-id="68f6f-165">指定的操作系统版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="68f6f-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="68f6f-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="68f6f-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="68f6f-167">字符串</span><span class="sxs-lookup"><span data-stu-id="68f6f-167">String</span></span>|<span data-ttu-id="68f6f-168">（如果有），则返回设备的完全限定的的域名。</span><span class="sxs-lookup"><span data-stu-id="68f6f-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="68f6f-169">如果设备不加入域的它将返回空字符串。</span><span class="sxs-lookup"><span data-stu-id="68f6f-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="68f6f-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="68f6f-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="68f6f-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="68f6f-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="68f6f-172">虚拟化基于安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="68f6f-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="68f6f-173">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="68f6f-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="68f6f-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="68f6f-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="68f6f-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="68f6f-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="68f6f-176">虚拟化基于安全状态。</span><span class="sxs-lookup"><span data-stu-id="68f6f-176">Virtualization-based security status.</span></span> <span data-ttu-id="68f6f-177">.</span><span class="sxs-lookup"><span data-stu-id="68f6f-177"></span></span> <span data-ttu-id="68f6f-178">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other`。</span><span class="sxs-lookup"><span data-stu-id="68f6f-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="68f6f-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="68f6f-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="68f6f-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="68f6f-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="68f6f-181">本地系统证书颁发机构 (LSA) 凭据 guard 状态。</span><span class="sxs-lookup"><span data-stu-id="68f6f-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="68f6f-182">.</span><span class="sxs-lookup"><span data-stu-id="68f6f-182"></span></span> <span data-ttu-id="68f6f-183">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="68f6f-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="68f6f-184">Relationships</span><span class="sxs-lookup"><span data-stu-id="68f6f-184">Relationships</span></span>
<span data-ttu-id="68f6f-185">无</span><span class="sxs-lookup"><span data-stu-id="68f6f-185">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="68f6f-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68f6f-186">JSON Representation</span></span>
<span data-ttu-id="68f6f-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68f6f-187">Here is a JSON representation of the resource.</span></span>
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





