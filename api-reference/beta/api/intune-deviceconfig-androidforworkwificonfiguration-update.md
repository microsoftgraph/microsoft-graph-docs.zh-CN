---
title: 更新 androidForWorkWiFiConfiguration
description: 更新 androidForWorkWiFiConfiguration 对象的属性。
ms.openlocfilehash: b12baaf0a003617798160aa9b45f6aeb937c3981
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047613"
---
# <a name="update-androidforworkwificonfiguration"></a><span data-ttu-id="2fb75-103">更新 androidForWorkWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="2fb75-103">Update androidForWorkWiFiConfiguration</span></span>

> <span data-ttu-id="2fb75-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2fb75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2fb75-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2fb75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2fb75-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2fb75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2fb75-107">更新[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2fb75-107">Update the properties of a [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2fb75-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2fb75-108">Prerequisites</span></span>
<span data-ttu-id="2fb75-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2fb75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fb75-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fb75-111">Permission type</span></span>|<span data-ttu-id="2fb75-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2fb75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fb75-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fb75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fb75-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fb75-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fb75-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fb75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fb75-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fb75-116">Not supported.</span></span>|
|<span data-ttu-id="2fb75-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fb75-117">Application</span></span>|<span data-ttu-id="2fb75-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fb75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fb75-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fb75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2fb75-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fb75-120">Request headers</span></span>
|<span data-ttu-id="2fb75-121">标头</span><span class="sxs-lookup"><span data-stu-id="2fb75-121">Header</span></span>|<span data-ttu-id="2fb75-122">值</span><span class="sxs-lookup"><span data-stu-id="2fb75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fb75-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fb75-123">Authorization</span></span>|<span data-ttu-id="2fb75-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2fb75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fb75-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2fb75-125">Accept</span></span>|<span data-ttu-id="2fb75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fb75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb75-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fb75-127">Request body</span></span>
<span data-ttu-id="2fb75-128">在请求正文中，提供[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fb75-128">In the request body, supply a JSON representation for the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object.</span></span>

<span data-ttu-id="2fb75-129">下表显示时创建[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2fb75-129">The following table shows the properties that are required when you create the [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md).</span></span>

|<span data-ttu-id="2fb75-130">属性</span><span class="sxs-lookup"><span data-stu-id="2fb75-130">Property</span></span>|<span data-ttu-id="2fb75-131">类型</span><span class="sxs-lookup"><span data-stu-id="2fb75-131">Type</span></span>|<span data-ttu-id="2fb75-132">说明</span><span class="sxs-lookup"><span data-stu-id="2fb75-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fb75-133">id</span><span class="sxs-lookup"><span data-stu-id="2fb75-133">id</span></span>|<span data-ttu-id="2fb75-134">String</span><span class="sxs-lookup"><span data-stu-id="2fb75-134">String</span></span>|<span data-ttu-id="2fb75-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2fb75-135">Key of the entity.</span></span> <span data-ttu-id="2fb75-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fb75-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb75-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2fb75-137">lastModifiedDateTime</span></span>|<span data-ttu-id="2fb75-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fb75-138">DateTimeOffset</span></span>|<span data-ttu-id="2fb75-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2fb75-139">DateTime the object was last modified.</span></span> <span data-ttu-id="2fb75-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fb75-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb75-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2fb75-141">roleScopeTagIds</span></span>|<span data-ttu-id="2fb75-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="2fb75-142">String collection</span></span>|<span data-ttu-id="2fb75-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="2fb75-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="2fb75-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fb75-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb75-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="2fb75-145">supportsScopeTags</span></span>|<span data-ttu-id="2fb75-146">布尔</span><span class="sxs-lookup"><span data-stu-id="2fb75-146">Boolean</span></span>|<span data-ttu-id="2fb75-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="2fb75-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="2fb75-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="2fb75-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="2fb75-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="2fb75-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="2fb75-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="2fb75-150">This property is read-only.</span></span> <span data-ttu-id="2fb75-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fb75-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb75-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2fb75-152">createdDateTime</span></span>|<span data-ttu-id="2fb75-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2fb75-153">DateTimeOffset</span></span>|<span data-ttu-id="2fb75-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2fb75-154">DateTime the object was created.</span></span> <span data-ttu-id="2fb75-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fb75-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb75-156">description</span><span class="sxs-lookup"><span data-stu-id="2fb75-156">description</span></span>|<span data-ttu-id="2fb75-157">String</span><span class="sxs-lookup"><span data-stu-id="2fb75-157">String</span></span>|<span data-ttu-id="2fb75-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2fb75-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2fb75-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fb75-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb75-160">displayName</span><span class="sxs-lookup"><span data-stu-id="2fb75-160">displayName</span></span>|<span data-ttu-id="2fb75-161">String</span><span class="sxs-lookup"><span data-stu-id="2fb75-161">String</span></span>|<span data-ttu-id="2fb75-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2fb75-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2fb75-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fb75-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb75-164">version</span><span class="sxs-lookup"><span data-stu-id="2fb75-164">version</span></span>|<span data-ttu-id="2fb75-165">Int32</span><span class="sxs-lookup"><span data-stu-id="2fb75-165">Int32</span></span>|<span data-ttu-id="2fb75-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2fb75-166">Version of the device configuration.</span></span> <span data-ttu-id="2fb75-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2fb75-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2fb75-168">networkName</span><span class="sxs-lookup"><span data-stu-id="2fb75-168">networkName</span></span>|<span data-ttu-id="2fb75-169">字符串</span><span class="sxs-lookup"><span data-stu-id="2fb75-169">String</span></span>|<span data-ttu-id="2fb75-170">网络名称</span><span class="sxs-lookup"><span data-stu-id="2fb75-170">Network Name</span></span>|
|<span data-ttu-id="2fb75-171">ssid</span><span class="sxs-lookup"><span data-stu-id="2fb75-171">ssid</span></span>|<span data-ttu-id="2fb75-172">字符串</span><span class="sxs-lookup"><span data-stu-id="2fb75-172">String</span></span>|<span data-ttu-id="2fb75-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="2fb75-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="2fb75-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="2fb75-174">connectAutomatically</span></span>|<span data-ttu-id="2fb75-175">布尔</span><span class="sxs-lookup"><span data-stu-id="2fb75-175">Boolean</span></span>|<span data-ttu-id="2fb75-176">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="2fb75-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="2fb75-177">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="2fb75-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="2fb75-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="2fb75-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="2fb75-179">布尔</span><span class="sxs-lookup"><span data-stu-id="2fb75-179">Boolean</span></span>|<span data-ttu-id="2fb75-180">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="2fb75-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="2fb75-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="2fb75-181">wiFiSecurityType</span></span>|[<span data-ttu-id="2fb75-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="2fb75-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="2fb75-183">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="2fb75-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="2fb75-184">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="2fb75-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="2fb75-185">响应</span><span class="sxs-lookup"><span data-stu-id="2fb75-185">Response</span></span>
<span data-ttu-id="2fb75-186">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2fb75-186">If successful, this method returns a `200 OK` response code and an updated [androidForWorkWiFiConfiguration](../resources/intune-deviceconfig-androidforworkwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fb75-187">示例</span><span class="sxs-lookup"><span data-stu-id="2fb75-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="2fb75-188">请求</span><span class="sxs-lookup"><span data-stu-id="2fb75-188">Request</span></span>
<span data-ttu-id="2fb75-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2fb75-189">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 436

{
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
  "wiFiSecurityType": "wpaEnterprise"
}
```

### <a name="response"></a><span data-ttu-id="2fb75-190">响应</span><span class="sxs-lookup"><span data-stu-id="2fb75-190">Response</span></span>
<span data-ttu-id="2fb75-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2fb75-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





