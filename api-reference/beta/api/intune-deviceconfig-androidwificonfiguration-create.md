---
title: 创建 androidWiFiConfiguration
description: 创建新的 androidWiFiConfiguration 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 32db8da5f399ead83c8cc47e38d33f875b2379b1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33928814"
---
# <a name="create-androidwificonfiguration"></a><span data-ttu-id="3b945-103">创建 androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="3b945-103">Create androidWiFiConfiguration</span></span>

> <span data-ttu-id="3b945-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3b945-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3b945-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3b945-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b945-106">创建新的[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3b945-106">Create a new [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b945-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3b945-107">Prerequisites</span></span>
<span data-ttu-id="3b945-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3b945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3b945-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3b945-110">Permission type</span></span>|<span data-ttu-id="3b945-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3b945-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b945-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3b945-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b945-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b945-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3b945-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3b945-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b945-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b945-115">Not supported.</span></span>|
|<span data-ttu-id="3b945-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3b945-116">Application</span></span>|<span data-ttu-id="3b945-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3b945-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b945-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3b945-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3b945-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3b945-119">Request headers</span></span>
|<span data-ttu-id="3b945-120">标头</span><span class="sxs-lookup"><span data-stu-id="3b945-120">Header</span></span>|<span data-ttu-id="3b945-121">值</span><span class="sxs-lookup"><span data-stu-id="3b945-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b945-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3b945-122">Authorization</span></span>|<span data-ttu-id="3b945-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3b945-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b945-124">接受</span><span class="sxs-lookup"><span data-stu-id="3b945-124">Accept</span></span>|<span data-ttu-id="3b945-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b945-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b945-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3b945-126">Request body</span></span>
<span data-ttu-id="3b945-127">在请求正文中, 提供 androidWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3b945-127">In the request body, supply a JSON representation for the androidWiFiConfiguration object.</span></span>

<span data-ttu-id="3b945-128">下表显示创建 androidWiFiConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3b945-128">The following table shows the properties that are required when you create the androidWiFiConfiguration.</span></span>

|<span data-ttu-id="3b945-129">属性</span><span class="sxs-lookup"><span data-stu-id="3b945-129">Property</span></span>|<span data-ttu-id="3b945-130">类型</span><span class="sxs-lookup"><span data-stu-id="3b945-130">Type</span></span>|<span data-ttu-id="3b945-131">说明</span><span class="sxs-lookup"><span data-stu-id="3b945-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b945-132">id</span><span class="sxs-lookup"><span data-stu-id="3b945-132">id</span></span>|<span data-ttu-id="3b945-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3b945-133">String</span></span>|<span data-ttu-id="3b945-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3b945-134">Key of the entity.</span></span> <span data-ttu-id="3b945-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b945-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b945-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b945-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3b945-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b945-137">DateTimeOffset</span></span>|<span data-ttu-id="3b945-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3b945-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3b945-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b945-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b945-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="3b945-140">roleScopeTagIds</span></span>|<span data-ttu-id="3b945-141">String collection</span><span class="sxs-lookup"><span data-stu-id="3b945-141">String collection</span></span>|<span data-ttu-id="3b945-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="3b945-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="3b945-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b945-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b945-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="3b945-144">supportsScopeTags</span></span>|<span data-ttu-id="3b945-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b945-145">Boolean</span></span>|<span data-ttu-id="3b945-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="3b945-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="3b945-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="3b945-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="3b945-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="3b945-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="3b945-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="3b945-149">This property is read-only.</span></span> <span data-ttu-id="3b945-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b945-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b945-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b945-151">createdDateTime</span></span>|<span data-ttu-id="3b945-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b945-152">DateTimeOffset</span></span>|<span data-ttu-id="3b945-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3b945-153">DateTime the object was created.</span></span> <span data-ttu-id="3b945-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b945-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b945-155">说明</span><span class="sxs-lookup"><span data-stu-id="3b945-155">description</span></span>|<span data-ttu-id="3b945-156">String</span><span class="sxs-lookup"><span data-stu-id="3b945-156">String</span></span>|<span data-ttu-id="3b945-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3b945-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3b945-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b945-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b945-159">displayName</span><span class="sxs-lookup"><span data-stu-id="3b945-159">displayName</span></span>|<span data-ttu-id="3b945-160">String</span><span class="sxs-lookup"><span data-stu-id="3b945-160">String</span></span>|<span data-ttu-id="3b945-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3b945-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3b945-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b945-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b945-163">version</span><span class="sxs-lookup"><span data-stu-id="3b945-163">version</span></span>|<span data-ttu-id="3b945-164">Int32</span><span class="sxs-lookup"><span data-stu-id="3b945-164">Int32</span></span>|<span data-ttu-id="3b945-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3b945-165">Version of the device configuration.</span></span> <span data-ttu-id="3b945-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3b945-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3b945-167">networkName</span><span class="sxs-lookup"><span data-stu-id="3b945-167">networkName</span></span>|<span data-ttu-id="3b945-168">String</span><span class="sxs-lookup"><span data-stu-id="3b945-168">String</span></span>|<span data-ttu-id="3b945-169">网络名称</span><span class="sxs-lookup"><span data-stu-id="3b945-169">Network Name</span></span>|
|<span data-ttu-id="3b945-170">ssid</span><span class="sxs-lookup"><span data-stu-id="3b945-170">ssid</span></span>|<span data-ttu-id="3b945-171">String</span><span class="sxs-lookup"><span data-stu-id="3b945-171">String</span></span>|<span data-ttu-id="3b945-172">这是广播到所有设备的 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="3b945-172">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="3b945-173">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="3b945-173">connectAutomatically</span></span>|<span data-ttu-id="3b945-174">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b945-174">Boolean</span></span>|<span data-ttu-id="3b945-175">当此网络在范围内时自动连接。</span><span class="sxs-lookup"><span data-stu-id="3b945-175">Connect automatically when this network is in range.</span></span> <span data-ttu-id="3b945-176">将此设置为 true 将跳过用户提示, 并自动将设备连接到 Wlan 网络。</span><span class="sxs-lookup"><span data-stu-id="3b945-176">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="3b945-177">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="3b945-177">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="3b945-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b945-178">Boolean</span></span>|<span data-ttu-id="3b945-179">当设置为 true 时, 此配置文件将强制设备连接到不会将其 SSID 广播给所有设备的网络。</span><span class="sxs-lookup"><span data-stu-id="3b945-179">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="3b945-180">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3b945-180">wiFiSecurityType</span></span>|[<span data-ttu-id="3b945-181">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="3b945-181">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="3b945-182">指示 Wi-fi 终结点是否使用基于 EAP 的安全类型。</span><span class="sxs-lookup"><span data-stu-id="3b945-182">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="3b945-183">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="3b945-183">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="3b945-184">响应</span><span class="sxs-lookup"><span data-stu-id="3b945-184">Response</span></span>
<span data-ttu-id="3b945-185">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3b945-185">If successful, this method returns a `201 Created` response code and a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b945-186">示例</span><span class="sxs-lookup"><span data-stu-id="3b945-186">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b945-187">请求</span><span class="sxs-lookup"><span data-stu-id="3b945-187">Request</span></span>
<span data-ttu-id="3b945-188">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3b945-188">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 435

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="3b945-189">响应</span><span class="sxs-lookup"><span data-stu-id="3b945-189">Response</span></span>
<span data-ttu-id="3b945-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3b945-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 607

{
  "@odata.type": "#microsoft.graph.androidWiFiConfiguration",
  "id": "51cfd26f-d26f-51cf-6fd2-cf516fd2cf51",
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




