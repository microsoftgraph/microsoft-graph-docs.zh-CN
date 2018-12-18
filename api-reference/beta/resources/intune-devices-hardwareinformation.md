---
title: hardwareInformation 资源类型
description: 硬件的给定设备的信息。
author: tfitzmac
ms.openlocfilehash: c483aa800d920a50392d21c326cd20dea7b72e18
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334522"
---
# <a name="hardwareinformation-resource-type"></a><span data-ttu-id="b58e4-103">hardwareInformation 资源类型</span><span class="sxs-lookup"><span data-stu-id="b58e4-103">hardwareInformation resource type</span></span>

> <span data-ttu-id="b58e4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b58e4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b58e4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b58e4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b58e4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b58e4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b58e4-107">硬件的给定设备的信息。</span><span class="sxs-lookup"><span data-stu-id="b58e4-107">Hardware information of a given device.</span></span>
## <a name="properties"></a><span data-ttu-id="b58e4-108">属性</span><span class="sxs-lookup"><span data-stu-id="b58e4-108">Properties</span></span>
|<span data-ttu-id="b58e4-109">属性</span><span class="sxs-lookup"><span data-stu-id="b58e4-109">Property</span></span>|<span data-ttu-id="b58e4-110">类型</span><span class="sxs-lookup"><span data-stu-id="b58e4-110">Type</span></span>|<span data-ttu-id="b58e4-111">说明</span><span class="sxs-lookup"><span data-stu-id="b58e4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b58e4-112">serialNumber</span><span class="sxs-lookup"><span data-stu-id="b58e4-112">serialNumber</span></span>|<span data-ttu-id="b58e4-113">字符串</span><span class="sxs-lookup"><span data-stu-id="b58e4-113">String</span></span>|<span data-ttu-id="b58e4-114">序列号。</span><span class="sxs-lookup"><span data-stu-id="b58e4-114">Serial number.</span></span>|
|<span data-ttu-id="b58e4-115">totalStorageSpace</span><span class="sxs-lookup"><span data-stu-id="b58e4-115">totalStorageSpace</span></span>|<span data-ttu-id="b58e4-116">Int64</span><span class="sxs-lookup"><span data-stu-id="b58e4-116">Int64</span></span>|<span data-ttu-id="b58e4-117">设备的总存储空间。</span><span class="sxs-lookup"><span data-stu-id="b58e4-117">Total storage space of the device.</span></span>|
|<span data-ttu-id="b58e4-118">freeStorageSpace</span><span class="sxs-lookup"><span data-stu-id="b58e4-118">freeStorageSpace</span></span>|<span data-ttu-id="b58e4-119">Int64</span><span class="sxs-lookup"><span data-stu-id="b58e4-119">Int64</span></span>|<span data-ttu-id="b58e4-120">设备的可用存储空间。</span><span class="sxs-lookup"><span data-stu-id="b58e4-120">Free storage space of the device.</span></span>|
|<span data-ttu-id="b58e4-121">imei</span><span class="sxs-lookup"><span data-stu-id="b58e4-121">imei</span></span>|<span data-ttu-id="b58e4-122">String</span><span class="sxs-lookup"><span data-stu-id="b58e4-122">String</span></span>|<span data-ttu-id="b58e4-123">IMEI</span><span class="sxs-lookup"><span data-stu-id="b58e4-123">IMEI</span></span>|
|<span data-ttu-id="b58e4-124">meid</span><span class="sxs-lookup"><span data-stu-id="b58e4-124">meid</span></span>|<span data-ttu-id="b58e4-125">String</span><span class="sxs-lookup"><span data-stu-id="b58e4-125">String</span></span>|<span data-ttu-id="b58e4-126">MEID</span><span class="sxs-lookup"><span data-stu-id="b58e4-126">MEID</span></span>|
|<span data-ttu-id="b58e4-127">manufacturer</span><span class="sxs-lookup"><span data-stu-id="b58e4-127">manufacturer</span></span>|<span data-ttu-id="b58e4-128">String</span><span class="sxs-lookup"><span data-stu-id="b58e4-128">String</span></span>|<span data-ttu-id="b58e4-129">设备的制造商</span><span class="sxs-lookup"><span data-stu-id="b58e4-129">Manufacturer of the device</span></span>|
|<span data-ttu-id="b58e4-130">model</span><span class="sxs-lookup"><span data-stu-id="b58e4-130">model</span></span>|<span data-ttu-id="b58e4-131">String</span><span class="sxs-lookup"><span data-stu-id="b58e4-131">String</span></span>|<span data-ttu-id="b58e4-132">设备的型号</span><span class="sxs-lookup"><span data-stu-id="b58e4-132">Model of the device</span></span>|
|<span data-ttu-id="b58e4-133">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="b58e4-133">phoneNumber</span></span>|<span data-ttu-id="b58e4-134">String</span><span class="sxs-lookup"><span data-stu-id="b58e4-134">String</span></span>|<span data-ttu-id="b58e4-135">设备的电话号码</span><span class="sxs-lookup"><span data-stu-id="b58e4-135">Phone number of the device</span></span>|
|<span data-ttu-id="b58e4-136">subscriberCarrier</span><span class="sxs-lookup"><span data-stu-id="b58e4-136">subscriberCarrier</span></span>|<span data-ttu-id="b58e4-137">String</span><span class="sxs-lookup"><span data-stu-id="b58e4-137">String</span></span>|<span data-ttu-id="b58e4-138">订阅者运营商的设备</span><span class="sxs-lookup"><span data-stu-id="b58e4-138">Subscriber carrier of the device</span></span>|
|<span data-ttu-id="b58e4-139">cellularTechnology</span><span class="sxs-lookup"><span data-stu-id="b58e4-139">cellularTechnology</span></span>|<span data-ttu-id="b58e4-140">字符串</span><span class="sxs-lookup"><span data-stu-id="b58e4-140">String</span></span>|<span data-ttu-id="b58e4-141">移动电话的设备的技术</span><span class="sxs-lookup"><span data-stu-id="b58e4-141">Cellular technology of the device</span></span>|
|<span data-ttu-id="b58e4-142">wifiMac</span><span class="sxs-lookup"><span data-stu-id="b58e4-142">wifiMac</span></span>|<span data-ttu-id="b58e4-143">字符串</span><span class="sxs-lookup"><span data-stu-id="b58e4-143">String</span></span>|<span data-ttu-id="b58e4-144">设备的 WiFi MAC 地址</span><span class="sxs-lookup"><span data-stu-id="b58e4-144">WiFi MAC address of the device</span></span>|
|<span data-ttu-id="b58e4-145">operatingSystemLanguage</span><span class="sxs-lookup"><span data-stu-id="b58e4-145">operatingSystemLanguage</span></span>|<span data-ttu-id="b58e4-146">字符串</span><span class="sxs-lookup"><span data-stu-id="b58e4-146">String</span></span>|<span data-ttu-id="b58e4-147">设备的操作系统语言</span><span class="sxs-lookup"><span data-stu-id="b58e4-147">Operating system language of the device</span></span>|
|<span data-ttu-id="b58e4-148">isSupervised</span><span class="sxs-lookup"><span data-stu-id="b58e4-148">isSupervised</span></span>|<span data-ttu-id="b58e4-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="b58e4-149">Boolean</span></span>|<span data-ttu-id="b58e4-150">设备监管的模式</span><span class="sxs-lookup"><span data-stu-id="b58e4-150">Supervised mode of the device</span></span>|
|<span data-ttu-id="b58e4-151">isEncrypted</span><span class="sxs-lookup"><span data-stu-id="b58e4-151">isEncrypted</span></span>|<span data-ttu-id="b58e4-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="b58e4-152">Boolean</span></span>|<span data-ttu-id="b58e4-153">设备加密状态</span><span class="sxs-lookup"><span data-stu-id="b58e4-153">Encryption status of the device</span></span>|
|<span data-ttu-id="b58e4-154">isSharedDevice</span><span class="sxs-lookup"><span data-stu-id="b58e4-154">isSharedDevice</span></span>|<span data-ttu-id="b58e4-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="b58e4-155">Boolean</span></span>|<span data-ttu-id="b58e4-156">共享的 iPad</span><span class="sxs-lookup"><span data-stu-id="b58e4-156">Shared iPad</span></span>|
|<span data-ttu-id="b58e4-157">sharedDeviceCachedUsers</span><span class="sxs-lookup"><span data-stu-id="b58e4-157">sharedDeviceCachedUsers</span></span>|<span data-ttu-id="b58e4-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md)集合</span><span class="sxs-lookup"><span data-stu-id="b58e4-158">[sharedAppleDeviceUser](../resources/intune-devices-sharedappledeviceuser.md) collection</span></span>|<span data-ttu-id="b58e4-159">共享的 Apple 设备上的所有用户</span><span class="sxs-lookup"><span data-stu-id="b58e4-159">All users on the shared Apple device</span></span>|
|<span data-ttu-id="b58e4-160">tpmSpecificationVersion</span><span class="sxs-lookup"><span data-stu-id="b58e4-160">tpmSpecificationVersion</span></span>|<span data-ttu-id="b58e4-161">字符串</span><span class="sxs-lookup"><span data-stu-id="b58e4-161">String</span></span>|<span data-ttu-id="b58e4-162">指定规范版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="b58e4-162">String that specifies the specification version.</span></span>|
|<span data-ttu-id="b58e4-163">operatingSystemEdition</span><span class="sxs-lookup"><span data-stu-id="b58e4-163">operatingSystemEdition</span></span>|<span data-ttu-id="b58e4-164">字符串</span><span class="sxs-lookup"><span data-stu-id="b58e4-164">String</span></span>|<span data-ttu-id="b58e4-165">指定的操作系统版本的字符串。</span><span class="sxs-lookup"><span data-stu-id="b58e4-165">String that specifies the OS edition.</span></span>|
|<span data-ttu-id="b58e4-166">deviceFullQualifiedDomainName</span><span class="sxs-lookup"><span data-stu-id="b58e4-166">deviceFullQualifiedDomainName</span></span>|<span data-ttu-id="b58e4-167">字符串</span><span class="sxs-lookup"><span data-stu-id="b58e4-167">String</span></span>|<span data-ttu-id="b58e4-168">（如果有），则返回设备的完全限定的的域名。</span><span class="sxs-lookup"><span data-stu-id="b58e4-168">Returns the fully qualified domain name of the device (if any).</span></span> <span data-ttu-id="b58e4-169">如果设备不加入域的它将返回空字符串。</span><span class="sxs-lookup"><span data-stu-id="b58e4-169">If the device is not domain-joined, it returns an empty string.</span></span> |
|<span data-ttu-id="b58e4-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="b58e4-170">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>|[<span data-ttu-id="b58e4-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span><span class="sxs-lookup"><span data-stu-id="b58e4-171">deviceGuardVirtualizationBasedSecurityHardwareRequirementState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecurityhardwarerequirementstate.md)|<span data-ttu-id="b58e4-172">虚拟化基于安全硬件要求状态。</span><span class="sxs-lookup"><span data-stu-id="b58e4-172">Virtualization-based security hardware requirement status.</span></span> <span data-ttu-id="b58e4-173">可取值为：`meetHardwareRequirements`、`secureBootRequired`、`dmaProtectionRequired`、`hyperVNotSupportedForGuestVM`、`hyperVNotAvailable`。</span><span class="sxs-lookup"><span data-stu-id="b58e4-173">Possible values are: `meetHardwareRequirements`, `secureBootRequired`, `dmaProtectionRequired`, `hyperVNotSupportedForGuestVM`, `hyperVNotAvailable`.</span></span>|
|<span data-ttu-id="b58e4-174">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="b58e4-174">deviceGuardVirtualizationBasedSecurityState</span></span>|[<span data-ttu-id="b58e4-175">deviceGuardVirtualizationBasedSecurityState</span><span class="sxs-lookup"><span data-stu-id="b58e4-175">deviceGuardVirtualizationBasedSecurityState</span></span>](../resources/intune-devices-deviceguardvirtualizationbasedsecuritystate.md)|<span data-ttu-id="b58e4-176">虚拟化基于安全状态。</span><span class="sxs-lookup"><span data-stu-id="b58e4-176">Virtualization-based security status.</span></span> <span data-ttu-id="b58e4-177">.</span><span class="sxs-lookup"><span data-stu-id="b58e4-177"></span></span> <span data-ttu-id="b58e4-178">可取值为：`running`、`rebootRequired`、`require64BitArchitecture`、`notLicensed`、`notConfigured`、`doesNotMeetHardwareRequirements`、`other`。</span><span class="sxs-lookup"><span data-stu-id="b58e4-178">Possible values are: `running`, `rebootRequired`, `require64BitArchitecture`, `notLicensed`, `notConfigured`, `doesNotMeetHardwareRequirements`, `other`.</span></span>|
|<span data-ttu-id="b58e4-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="b58e4-179">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>|[<span data-ttu-id="b58e4-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span><span class="sxs-lookup"><span data-stu-id="b58e4-180">deviceGuardLocalSystemAuthorityCredentialGuardState</span></span>](../resources/intune-devices-deviceguardlocalsystemauthoritycredentialguardstate.md)|<span data-ttu-id="b58e4-181">本地系统证书颁发机构 (LSA) 凭据 guard 状态。</span><span class="sxs-lookup"><span data-stu-id="b58e4-181">Local System Authority (LSA) credential guard status.</span></span> <span data-ttu-id="b58e4-182">.</span><span class="sxs-lookup"><span data-stu-id="b58e4-182"></span></span> <span data-ttu-id="b58e4-183">可取值为：`running`、`rebootRequired`、`notLicensed`、`notConfigured`、`virtualizationBasedSecurityNotRunning`。</span><span class="sxs-lookup"><span data-stu-id="b58e4-183">Possible values are: `running`, `rebootRequired`, `notLicensed`, `notConfigured`, `virtualizationBasedSecurityNotRunning`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b58e4-184">Relationships</span><span class="sxs-lookup"><span data-stu-id="b58e4-184">Relationships</span></span>
<span data-ttu-id="b58e4-185">无</span><span class="sxs-lookup"><span data-stu-id="b58e4-185">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b58e4-186">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b58e4-186">JSON Representation</span></span>
<span data-ttu-id="b58e4-187">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b58e4-187">Here is a JSON representation of the resource.</span></span>
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





