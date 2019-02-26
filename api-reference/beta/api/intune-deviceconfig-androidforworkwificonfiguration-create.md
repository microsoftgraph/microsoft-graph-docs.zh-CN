---
title: 创建 androidForWorkWiFiConfiguration
description: 创建新的 androidForWorkWiFiConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f66b1efd63baec06ca94a88a3d12f77d76190077
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30162571"
---
# <a name="create-androidforworkwificonfiguration"></a><span data-ttu-id="9e7be-103">创建 androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="9e7be-103">Create androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="9e7be-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e7be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e7be-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e7be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e7be-106">创建新的[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9e7be-106">Create a new [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9e7be-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9e7be-107">Prerequisites</span></span>
<span data-ttu-id="9e7be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="9e7be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9e7be-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9e7be-110">Permission type</span></span>|<span data-ttu-id="9e7be-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9e7be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e7be-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9e7be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9e7be-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9e7be-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9e7be-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9e7be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e7be-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e7be-115">Not supported.</span></span>|
|<span data-ttu-id="9e7be-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9e7be-116">Application</span></span>|<span data-ttu-id="9e7be-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9e7be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e7be-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9e7be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="9e7be-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9e7be-119">Request headers</span></span>
|<span data-ttu-id="9e7be-120">标头</span><span class="sxs-lookup"><span data-stu-id="9e7be-120">Header</span></span>|<span data-ttu-id="9e7be-121">值</span><span class="sxs-lookup"><span data-stu-id="9e7be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e7be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e7be-122">Authorization</span></span>|<span data-ttu-id="9e7be-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9e7be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e7be-124">Accept</span><span class="sxs-lookup"><span data-stu-id="9e7be-124">Accept</span></span>|<span data-ttu-id="9e7be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9e7be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e7be-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9e7be-126">Request body</span></span>
<span data-ttu-id="9e7be-127">在请求正文中, 提供 androidForWorkWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e7be-127">In the request body, supply a JSON representation for the androidForWorkWiFiConfiguration object.</span></span>

<span data-ttu-id="9e7be-128">下表显示创建 androidForWorkWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9e7be-128">The following table shows the properties that are required when you create the androidForWorkWiFiConfiguration.</span></span>

|<span data-ttu-id="9e7be-129">属性</span><span class="sxs-lookup"><span data-stu-id="9e7be-129">Property</span></span>|<span data-ttu-id="9e7be-130">类型</span><span class="sxs-lookup"><span data-stu-id="9e7be-130">Type</span></span>|<span data-ttu-id="9e7be-131">说明</span><span class="sxs-lookup"><span data-stu-id="9e7be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e7be-132">id</span><span class="sxs-lookup"><span data-stu-id="9e7be-132">id</span></span>|<span data-ttu-id="9e7be-133">String</span><span class="sxs-lookup"><span data-stu-id="9e7be-133">String</span></span>|<span data-ttu-id="9e7be-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9e7be-134">Key of the entity.</span></span> <span data-ttu-id="9e7be-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e7be-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e7be-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9e7be-136">lastModifiedDateTime</span></span>|<span data-ttu-id="9e7be-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e7be-137">DateTimeOffset</span></span>|<span data-ttu-id="9e7be-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9e7be-138">DateTime the object was last modified.</span></span> <span data-ttu-id="9e7be-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e7be-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e7be-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="9e7be-140">roleScopeTagIds</span></span>|<span data-ttu-id="9e7be-141">String collection</span><span class="sxs-lookup"><span data-stu-id="9e7be-141">String collection</span></span>|<span data-ttu-id="9e7be-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="9e7be-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="9e7be-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e7be-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e7be-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="9e7be-144">supportsScopeTags</span></span>|<span data-ttu-id="9e7be-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e7be-145">Boolean</span></span>|<span data-ttu-id="9e7be-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="9e7be-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="9e7be-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="9e7be-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="9e7be-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="9e7be-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="9e7be-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="9e7be-149">This property is read-only.</span></span> <span data-ttu-id="9e7be-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e7be-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e7be-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="9e7be-151">createdDateTime</span></span>|<span data-ttu-id="9e7be-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9e7be-152">DateTimeOffset</span></span>|<span data-ttu-id="9e7be-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="9e7be-153">DateTime the object was created.</span></span> <span data-ttu-id="9e7be-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e7be-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e7be-155">description</span><span class="sxs-lookup"><span data-stu-id="9e7be-155">description</span></span>|<span data-ttu-id="9e7be-156">String</span><span class="sxs-lookup"><span data-stu-id="9e7be-156">String</span></span>|<span data-ttu-id="9e7be-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="9e7be-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="9e7be-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e7be-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e7be-159">displayName</span><span class="sxs-lookup"><span data-stu-id="9e7be-159">displayName</span></span>|<span data-ttu-id="9e7be-160">String</span><span class="sxs-lookup"><span data-stu-id="9e7be-160">String</span></span>|<span data-ttu-id="9e7be-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="9e7be-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="9e7be-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e7be-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e7be-163">version</span><span class="sxs-lookup"><span data-stu-id="9e7be-163">version</span></span>|<span data-ttu-id="9e7be-164">Int32</span><span class="sxs-lookup"><span data-stu-id="9e7be-164">Int32</span></span>|<span data-ttu-id="9e7be-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="9e7be-165">Version of the device configuration.</span></span> <span data-ttu-id="9e7be-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="9e7be-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="9e7be-167">networkName</span><span class="sxs-lookup"><span data-stu-id="9e7be-167">networkName</span></span>|<span data-ttu-id="9e7be-168">String</span><span class="sxs-lookup"><span data-stu-id="9e7be-168">String</span></span>|<span data-ttu-id="9e7be-169">网络名称</span><span class="sxs-lookup"><span data-stu-id="9e7be-169">Network Name</span></span>|
|<span data-ttu-id="9e7be-170">ssid</span><span class="sxs-lookup"><span data-stu-id="9e7be-170">ssid</span></span>|<span data-ttu-id="9e7be-171">String</span><span class="sxs-lookup"><span data-stu-id="9e7be-171">String</span></span>|<span data-ttu-id="9e7be-172">这是广播到所有设备的 wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="9e7be-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="9e7be-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="9e7be-173">connectAutomatically</span></span>|<span data-ttu-id="9e7be-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e7be-174">Boolean</span></span>|<span data-ttu-id="9e7be-175">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="9e7be-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="9e7be-176">将此设置为 true 将跳过用户提示, 并自动将设备连接到 wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="9e7be-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="9e7be-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="9e7be-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="9e7be-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e7be-178">Boolean</span></span>|<span data-ttu-id="9e7be-179">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="9e7be-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="9e7be-180">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9e7be-180">wiFiSecurityType</span></span>|[<span data-ttu-id="9e7be-181">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="9e7be-181">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="9e7be-182">指示 wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="9e7be-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="9e7be-183">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="9e7be-183">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="9e7be-184">响应</span><span class="sxs-lookup"><span data-stu-id="9e7be-184">Response</span></span>
<span data-ttu-id="9e7be-185">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9e7be-185">If successful, this method returns a `201 Created` response code and a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e7be-186">示例</span><span class="sxs-lookup"><span data-stu-id="9e7be-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="9e7be-187">请求</span><span class="sxs-lookup"><span data-stu-id="9e7be-187">Request</span></span>
<span data-ttu-id="9e7be-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9e7be-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 442

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="9e7be-189">响应</span><span class="sxs-lookup"><span data-stu-id="9e7be-189">Response</span></span>
<span data-ttu-id="9e7be-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9e7be-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 614

{
  "@odata.type": "#microsoft.graph.androidForWorkWiFiConfiguration",
  "id": "58bcfe05-fe05-58bc-05fe-bc5805febc58",
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
  "wiFiSecurityType": "wpaEnterprise"
}
```




