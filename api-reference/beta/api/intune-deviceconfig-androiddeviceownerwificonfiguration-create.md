---
title: 创建 androidDeviceOwnerWiFiConfiguration
description: 创建新的 androidDeviceOwnerWiFiConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: aa815b191a13937a411faf209155028a488b72d0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32480448"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="affdf-103">创建 androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="affdf-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="affdf-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="affdf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="affdf-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="affdf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="affdf-106">创建新的[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="affdf-106">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="affdf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="affdf-107">Prerequisites</span></span>
<span data-ttu-id="affdf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="affdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="affdf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="affdf-110">Permission type</span></span>|<span data-ttu-id="affdf-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="affdf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="affdf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="affdf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="affdf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="affdf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="affdf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="affdf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="affdf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="affdf-115">Not supported.</span></span>|
|<span data-ttu-id="affdf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="affdf-116">Application</span></span>|<span data-ttu-id="affdf-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="affdf-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="affdf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="affdf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="affdf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="affdf-119">Request headers</span></span>
|<span data-ttu-id="affdf-120">标头</span><span class="sxs-lookup"><span data-stu-id="affdf-120">Header</span></span>|<span data-ttu-id="affdf-121">值</span><span class="sxs-lookup"><span data-stu-id="affdf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="affdf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="affdf-122">Authorization</span></span>|<span data-ttu-id="affdf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="affdf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="affdf-124">接受</span><span class="sxs-lookup"><span data-stu-id="affdf-124">Accept</span></span>|<span data-ttu-id="affdf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="affdf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="affdf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="affdf-126">Request body</span></span>
<span data-ttu-id="affdf-127">在请求正文中, 提供 androidDeviceOwnerWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="affdf-127">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="affdf-128">下表显示创建 androidDeviceOwnerWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="affdf-128">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="affdf-129">属性</span><span class="sxs-lookup"><span data-stu-id="affdf-129">Property</span></span>|<span data-ttu-id="affdf-130">类型</span><span class="sxs-lookup"><span data-stu-id="affdf-130">Type</span></span>|<span data-ttu-id="affdf-131">说明</span><span class="sxs-lookup"><span data-stu-id="affdf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="affdf-132">id</span><span class="sxs-lookup"><span data-stu-id="affdf-132">id</span></span>|<span data-ttu-id="affdf-133">String</span><span class="sxs-lookup"><span data-stu-id="affdf-133">String</span></span>|<span data-ttu-id="affdf-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="affdf-134">Key of the entity.</span></span> <span data-ttu-id="affdf-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="affdf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="affdf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="affdf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="affdf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="affdf-137">DateTimeOffset</span></span>|<span data-ttu-id="affdf-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="affdf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="affdf-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="affdf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="affdf-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="affdf-140">roleScopeTagIds</span></span>|<span data-ttu-id="affdf-141">String collection</span><span class="sxs-lookup"><span data-stu-id="affdf-141">String collection</span></span>|<span data-ttu-id="affdf-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="affdf-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="affdf-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="affdf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="affdf-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="affdf-144">supportsScopeTags</span></span>|<span data-ttu-id="affdf-145">布尔</span><span class="sxs-lookup"><span data-stu-id="affdf-145">Boolean</span></span>|<span data-ttu-id="affdf-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="affdf-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="affdf-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="affdf-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="affdf-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="affdf-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="affdf-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="affdf-149">This property is read-only.</span></span> <span data-ttu-id="affdf-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="affdf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="affdf-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="affdf-151">createdDateTime</span></span>|<span data-ttu-id="affdf-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="affdf-152">DateTimeOffset</span></span>|<span data-ttu-id="affdf-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="affdf-153">DateTime the object was created.</span></span> <span data-ttu-id="affdf-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="affdf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="affdf-155">description</span><span class="sxs-lookup"><span data-stu-id="affdf-155">description</span></span>|<span data-ttu-id="affdf-156">字符串</span><span class="sxs-lookup"><span data-stu-id="affdf-156">String</span></span>|<span data-ttu-id="affdf-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="affdf-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="affdf-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="affdf-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="affdf-159">displayName</span><span class="sxs-lookup"><span data-stu-id="affdf-159">displayName</span></span>|<span data-ttu-id="affdf-160">String</span><span class="sxs-lookup"><span data-stu-id="affdf-160">String</span></span>|<span data-ttu-id="affdf-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="affdf-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="affdf-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="affdf-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="affdf-163">version</span><span class="sxs-lookup"><span data-stu-id="affdf-163">version</span></span>|<span data-ttu-id="affdf-164">Int32</span><span class="sxs-lookup"><span data-stu-id="affdf-164">Int32</span></span>|<span data-ttu-id="affdf-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="affdf-165">Version of the device configuration.</span></span> <span data-ttu-id="affdf-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="affdf-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="affdf-167">networkName</span><span class="sxs-lookup"><span data-stu-id="affdf-167">networkName</span></span>|<span data-ttu-id="affdf-168">字符串</span><span class="sxs-lookup"><span data-stu-id="affdf-168">String</span></span>|<span data-ttu-id="affdf-169">网络名称</span><span class="sxs-lookup"><span data-stu-id="affdf-169">Network Name</span></span>|
|<span data-ttu-id="affdf-170">ssid</span><span class="sxs-lookup"><span data-stu-id="affdf-170">ssid</span></span>|<span data-ttu-id="affdf-171">字符串</span><span class="sxs-lookup"><span data-stu-id="affdf-171">String</span></span>|<span data-ttu-id="affdf-172">这是广播到所有设备的 wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="affdf-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="affdf-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="affdf-173">connectAutomatically</span></span>|<span data-ttu-id="affdf-174">布尔</span><span class="sxs-lookup"><span data-stu-id="affdf-174">Boolean</span></span>|<span data-ttu-id="affdf-175">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="affdf-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="affdf-176">将此设置为 true 将跳过用户提示, 并自动将设备连接到 wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="affdf-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="affdf-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="affdf-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="affdf-178">布尔</span><span class="sxs-lookup"><span data-stu-id="affdf-178">Boolean</span></span>|<span data-ttu-id="affdf-179">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="affdf-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="affdf-180">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="affdf-180">wiFiSecurityType</span></span>|[<span data-ttu-id="affdf-181">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="affdf-181">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="affdf-182">指示 wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="affdf-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="affdf-183">可取值为：`open`、`wep`、`wpaPersonal`。</span><span class="sxs-lookup"><span data-stu-id="affdf-183">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="affdf-184">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="affdf-184">preSharedKey</span></span>|<span data-ttu-id="affdf-185">字符串</span><span class="sxs-lookup"><span data-stu-id="affdf-185">String</span></span>|<span data-ttu-id="affdf-186">这是 WPA 个人 wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="affdf-186">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="affdf-187">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="affdf-187">preSharedKeyIsSet</span></span>|<span data-ttu-id="affdf-188">布尔</span><span class="sxs-lookup"><span data-stu-id="affdf-188">Boolean</span></span>|<span data-ttu-id="affdf-189">这是 WPA 个人 wi-fi 网络的预共享密钥。</span><span class="sxs-lookup"><span data-stu-id="affdf-189">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="affdf-190">响应</span><span class="sxs-lookup"><span data-stu-id="affdf-190">Response</span></span>
<span data-ttu-id="affdf-191">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="affdf-191">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="affdf-192">示例</span><span class="sxs-lookup"><span data-stu-id="affdf-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="affdf-193">请求</span><span class="sxs-lookup"><span data-stu-id="affdf-193">Request</span></span>
<span data-ttu-id="affdf-194">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="affdf-194">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 509

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```

### <a name="response"></a><span data-ttu-id="affdf-195">响应</span><span class="sxs-lookup"><span data-stu-id="affdf-195">Response</span></span>
<span data-ttu-id="affdf-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="affdf-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 681

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "id": "8d25beba-beba-8d25-babe-258dbabe258d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "networkName": "Network Name value",
  "ssid": "Ssid value",
  "connectAutomatically": true,
  "connectWhenNetworkNameIsHidden": true,
  "wiFiSecurityType": "wep",
  "preSharedKey": "Pre Shared Key value",
  "preSharedKeyIsSet": true
}
```





