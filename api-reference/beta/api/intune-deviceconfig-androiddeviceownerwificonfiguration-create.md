---
title: 创建 androidDeviceOwnerWiFiConfiguration
description: 创建新的 androidDeviceOwnerWiFiConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 41a1a73a789053a16302ed15e1430eddd8119499
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983329"
---
# <a name="create-androiddeviceownerwificonfiguration"></a><span data-ttu-id="2b29a-103">创建 androidDeviceOwnerWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="2b29a-103">Create androidDeviceOwnerWiFiConfiguration</span></span>

> <span data-ttu-id="2b29a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2b29a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b29a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2b29a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b29a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2b29a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b29a-107">创建新的[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b29a-107">Create a new [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b29a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2b29a-108">Prerequisites</span></span>
<span data-ttu-id="2b29a-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2b29a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b29a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b29a-111">Permission type</span></span>|<span data-ttu-id="2b29a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2b29a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b29a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b29a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2b29a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b29a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b29a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b29a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b29a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b29a-116">Not supported.</span></span>|
|<span data-ttu-id="2b29a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b29a-117">Application</span></span>|<span data-ttu-id="2b29a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b29a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b29a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b29a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2b29a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b29a-120">Request headers</span></span>
|<span data-ttu-id="2b29a-121">标头</span><span class="sxs-lookup"><span data-stu-id="2b29a-121">Header</span></span>|<span data-ttu-id="2b29a-122">值</span><span class="sxs-lookup"><span data-stu-id="2b29a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b29a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b29a-123">Authorization</span></span>|<span data-ttu-id="2b29a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2b29a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b29a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2b29a-125">Accept</span></span>|<span data-ttu-id="2b29a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2b29a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b29a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b29a-127">Request body</span></span>
<span data-ttu-id="2b29a-128">在请求正文中，提供 androidDeviceOwnerWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b29a-128">In the request body, supply a JSON representation for the androidDeviceOwnerWiFiConfiguration object.</span></span>

<span data-ttu-id="2b29a-129">下表显示时创建 androidDeviceOwnerWiFiConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2b29a-129">The following table shows the properties that are required when you create the androidDeviceOwnerWiFiConfiguration.</span></span>

|<span data-ttu-id="2b29a-130">属性</span><span class="sxs-lookup"><span data-stu-id="2b29a-130">Property</span></span>|<span data-ttu-id="2b29a-131">类型</span><span class="sxs-lookup"><span data-stu-id="2b29a-131">Type</span></span>|<span data-ttu-id="2b29a-132">说明</span><span class="sxs-lookup"><span data-stu-id="2b29a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b29a-133">id</span><span class="sxs-lookup"><span data-stu-id="2b29a-133">id</span></span>|<span data-ttu-id="2b29a-134">String</span><span class="sxs-lookup"><span data-stu-id="2b29a-134">String</span></span>|<span data-ttu-id="2b29a-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2b29a-135">Key of the entity.</span></span> <span data-ttu-id="2b29a-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b29a-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b29a-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b29a-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2b29a-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b29a-138">DateTimeOffset</span></span>|<span data-ttu-id="2b29a-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2b29a-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2b29a-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b29a-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b29a-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2b29a-141">roleScopeTagIds</span></span>|<span data-ttu-id="2b29a-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="2b29a-142">String collection</span></span>|<span data-ttu-id="2b29a-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="2b29a-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2b29a-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b29a-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b29a-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2b29a-145">supportsScopeTags</span></span>|<span data-ttu-id="2b29a-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b29a-146">Boolean</span></span>|<span data-ttu-id="2b29a-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="2b29a-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2b29a-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="2b29a-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2b29a-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="2b29a-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2b29a-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2b29a-150">This property is read-only.</span></span> <span data-ttu-id="2b29a-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b29a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b29a-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2b29a-152">createdDateTime</span></span>|<span data-ttu-id="2b29a-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b29a-153">DateTimeOffset</span></span>|<span data-ttu-id="2b29a-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2b29a-154">DateTime the object was created.</span></span> <span data-ttu-id="2b29a-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b29a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b29a-156">description</span><span class="sxs-lookup"><span data-stu-id="2b29a-156">description</span></span>|<span data-ttu-id="2b29a-157">String</span><span class="sxs-lookup"><span data-stu-id="2b29a-157">String</span></span>|<span data-ttu-id="2b29a-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2b29a-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2b29a-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b29a-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b29a-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2b29a-160">displayName</span></span>|<span data-ttu-id="2b29a-161">String</span><span class="sxs-lookup"><span data-stu-id="2b29a-161">String</span></span>|<span data-ttu-id="2b29a-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2b29a-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2b29a-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b29a-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b29a-164">version</span><span class="sxs-lookup"><span data-stu-id="2b29a-164">version</span></span>|<span data-ttu-id="2b29a-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2b29a-165">Int32</span></span>|<span data-ttu-id="2b29a-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2b29a-166">Version of the device configuration.</span></span> <span data-ttu-id="2b29a-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2b29a-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2b29a-168">networkName</span><span class="sxs-lookup"><span data-stu-id="2b29a-168">networkName</span></span>|<span data-ttu-id="2b29a-169">字符串</span><span class="sxs-lookup"><span data-stu-id="2b29a-169">String</span></span>|<span data-ttu-id="2b29a-170">网络名称</span><span class="sxs-lookup"><span data-stu-id="2b29a-170">Network Name</span></span>|
|<span data-ttu-id="2b29a-171">ssid</span><span class="sxs-lookup"><span data-stu-id="2b29a-171">ssid</span></span>|<span data-ttu-id="2b29a-172">字符串</span><span class="sxs-lookup"><span data-stu-id="2b29a-172">String</span></span>|<span data-ttu-id="2b29a-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="2b29a-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="2b29a-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="2b29a-174">connectAutomatically</span></span>|<span data-ttu-id="2b29a-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b29a-175">Boolean</span></span>|<span data-ttu-id="2b29a-176">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="2b29a-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="2b29a-177">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="2b29a-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="2b29a-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="2b29a-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="2b29a-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b29a-179">Boolean</span></span>|<span data-ttu-id="2b29a-180">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="2b29a-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="2b29a-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="2b29a-181">wiFiSecurityType</span></span>|[<span data-ttu-id="2b29a-182">androidDeviceOwnerWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="2b29a-182">androidDeviceOwnerWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androiddeviceownerwifisecuritytype.md)|<span data-ttu-id="2b29a-183">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="2b29a-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="2b29a-184">可取值为：`open`、`wep`、`wpaPersonal`。</span><span class="sxs-lookup"><span data-stu-id="2b29a-184">Possible values are: `open`, `wep`, `wpaPersonal`.</span></span>|
|<span data-ttu-id="2b29a-185">preSharedKey</span><span class="sxs-lookup"><span data-stu-id="2b29a-185">preSharedKey</span></span>|<span data-ttu-id="2b29a-186">字符串</span><span class="sxs-lookup"><span data-stu-id="2b29a-186">String</span></span>|<span data-ttu-id="2b29a-187">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="2b29a-187">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|
|<span data-ttu-id="2b29a-188">preSharedKeyIsSet</span><span class="sxs-lookup"><span data-stu-id="2b29a-188">preSharedKeyIsSet</span></span>|<span data-ttu-id="2b29a-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b29a-189">Boolean</span></span>|<span data-ttu-id="2b29a-190">这是预共享的 WPA 个人 Wi-fi 网络密钥。</span><span class="sxs-lookup"><span data-stu-id="2b29a-190">This is the pre-shared key for WPA Personal Wi-Fi network.</span></span>|



## <a name="response"></a><span data-ttu-id="2b29a-191">响应</span><span class="sxs-lookup"><span data-stu-id="2b29a-191">Response</span></span>
<span data-ttu-id="2b29a-192">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b29a-192">If successful, this method returns a `201 Created` response code and a [androidDeviceOwnerWiFiConfiguration](../resources/intune-deviceconfig-androiddeviceownerwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b29a-193">示例</span><span class="sxs-lookup"><span data-stu-id="2b29a-193">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b29a-194">请求</span><span class="sxs-lookup"><span data-stu-id="2b29a-194">Request</span></span>
<span data-ttu-id="2b29a-195">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b29a-195">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 573

{
  "@odata.type": "#microsoft.graph.androidDeviceOwnerWiFiConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="2b29a-196">响应</span><span class="sxs-lookup"><span data-stu-id="2b29a-196">Response</span></span>
<span data-ttu-id="2b29a-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b29a-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





