---
title: 创建 androidWorkProfileWiFiConfiguration
description: 创建新的 androidWorkProfileWiFiConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5723c9ba230805856563999c92146fbc9a248ad2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817371"
---
# <a name="create-androidworkprofilewificonfiguration"></a><span data-ttu-id="7d581-103">创建 androidWorkProfileWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="7d581-103">Create androidWorkProfileWiFiConfiguration</span></span>

> <span data-ttu-id="7d581-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7d581-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7d581-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7d581-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7d581-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7d581-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7d581-107">创建新的[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7d581-107">Create a new [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7d581-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7d581-108">Prerequisites</span></span>
<span data-ttu-id="7d581-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7d581-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d581-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d581-111">Permission type</span></span>|<span data-ttu-id="7d581-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7d581-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d581-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d581-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7d581-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d581-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7d581-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d581-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d581-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d581-116">Not supported.</span></span>|
|<span data-ttu-id="7d581-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d581-117">Application</span></span>|<span data-ttu-id="7d581-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d581-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d581-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d581-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7d581-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d581-120">Request headers</span></span>
|<span data-ttu-id="7d581-121">标头</span><span class="sxs-lookup"><span data-stu-id="7d581-121">Header</span></span>|<span data-ttu-id="7d581-122">值</span><span class="sxs-lookup"><span data-stu-id="7d581-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d581-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d581-123">Authorization</span></span>|<span data-ttu-id="7d581-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7d581-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d581-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7d581-125">Accept</span></span>|<span data-ttu-id="7d581-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7d581-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d581-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d581-127">Request body</span></span>
<span data-ttu-id="7d581-128">在请求正文中，提供 androidWorkProfileWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d581-128">In the request body, supply a JSON representation for the androidWorkProfileWiFiConfiguration object.</span></span>

<span data-ttu-id="7d581-129">下表显示时创建 androidWorkProfileWiFiConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7d581-129">The following table shows the properties that are required when you create the androidWorkProfileWiFiConfiguration.</span></span>

|<span data-ttu-id="7d581-130">属性</span><span class="sxs-lookup"><span data-stu-id="7d581-130">Property</span></span>|<span data-ttu-id="7d581-131">类型</span><span class="sxs-lookup"><span data-stu-id="7d581-131">Type</span></span>|<span data-ttu-id="7d581-132">说明</span><span class="sxs-lookup"><span data-stu-id="7d581-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d581-133">id</span><span class="sxs-lookup"><span data-stu-id="7d581-133">id</span></span>|<span data-ttu-id="7d581-134">String</span><span class="sxs-lookup"><span data-stu-id="7d581-134">String</span></span>|<span data-ttu-id="7d581-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7d581-135">Key of the entity.</span></span> <span data-ttu-id="7d581-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d581-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d581-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7d581-137">lastModifiedDateTime</span></span>|<span data-ttu-id="7d581-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d581-138">DateTimeOffset</span></span>|<span data-ttu-id="7d581-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7d581-139">DateTime the object was last modified.</span></span> <span data-ttu-id="7d581-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d581-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d581-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="7d581-141">roleScopeTagIds</span></span>|<span data-ttu-id="7d581-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="7d581-142">String collection</span></span>|<span data-ttu-id="7d581-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="7d581-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="7d581-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d581-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d581-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="7d581-145">supportsScopeTags</span></span>|<span data-ttu-id="7d581-146">布尔</span><span class="sxs-lookup"><span data-stu-id="7d581-146">Boolean</span></span>|<span data-ttu-id="7d581-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="7d581-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="7d581-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="7d581-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="7d581-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="7d581-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="7d581-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="7d581-150">This property is read-only.</span></span> <span data-ttu-id="7d581-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d581-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d581-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7d581-152">createdDateTime</span></span>|<span data-ttu-id="7d581-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7d581-153">DateTimeOffset</span></span>|<span data-ttu-id="7d581-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7d581-154">DateTime the object was created.</span></span> <span data-ttu-id="7d581-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d581-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d581-156">description</span><span class="sxs-lookup"><span data-stu-id="7d581-156">description</span></span>|<span data-ttu-id="7d581-157">String</span><span class="sxs-lookup"><span data-stu-id="7d581-157">String</span></span>|<span data-ttu-id="7d581-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7d581-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7d581-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d581-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d581-160">displayName</span><span class="sxs-lookup"><span data-stu-id="7d581-160">displayName</span></span>|<span data-ttu-id="7d581-161">String</span><span class="sxs-lookup"><span data-stu-id="7d581-161">String</span></span>|<span data-ttu-id="7d581-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7d581-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7d581-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d581-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d581-164">version</span><span class="sxs-lookup"><span data-stu-id="7d581-164">version</span></span>|<span data-ttu-id="7d581-165">Int32</span><span class="sxs-lookup"><span data-stu-id="7d581-165">Int32</span></span>|<span data-ttu-id="7d581-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7d581-166">Version of the device configuration.</span></span> <span data-ttu-id="7d581-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7d581-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7d581-168">networkName</span><span class="sxs-lookup"><span data-stu-id="7d581-168">networkName</span></span>|<span data-ttu-id="7d581-169">字符串</span><span class="sxs-lookup"><span data-stu-id="7d581-169">String</span></span>|<span data-ttu-id="7d581-170">网络名称</span><span class="sxs-lookup"><span data-stu-id="7d581-170">Network Name</span></span>|
|<span data-ttu-id="7d581-171">ssid</span><span class="sxs-lookup"><span data-stu-id="7d581-171">ssid</span></span>|<span data-ttu-id="7d581-172">字符串</span><span class="sxs-lookup"><span data-stu-id="7d581-172">String</span></span>|<span data-ttu-id="7d581-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="7d581-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="7d581-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="7d581-174">connectAutomatically</span></span>|<span data-ttu-id="7d581-175">布尔</span><span class="sxs-lookup"><span data-stu-id="7d581-175">Boolean</span></span>|<span data-ttu-id="7d581-176">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="7d581-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="7d581-177">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="7d581-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="7d581-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="7d581-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="7d581-179">布尔</span><span class="sxs-lookup"><span data-stu-id="7d581-179">Boolean</span></span>|<span data-ttu-id="7d581-180">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="7d581-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="7d581-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="7d581-181">wiFiSecurityType</span></span>|[<span data-ttu-id="7d581-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="7d581-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="7d581-183">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="7d581-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="7d581-184">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="7d581-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="7d581-185">响应</span><span class="sxs-lookup"><span data-stu-id="7d581-185">Response</span></span>
<span data-ttu-id="7d581-186">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7d581-186">If successful, this method returns a `201 Created` response code and a [androidWorkProfileWiFiConfiguration](../resources/intune-deviceconfig-androidworkprofilewificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7d581-187">示例</span><span class="sxs-lookup"><span data-stu-id="7d581-187">Example</span></span>
### <a name="request"></a><span data-ttu-id="7d581-188">请求</span><span class="sxs-lookup"><span data-stu-id="7d581-188">Request</span></span>
<span data-ttu-id="7d581-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d581-189">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 510

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
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

### <a name="response"></a><span data-ttu-id="7d581-190">响应</span><span class="sxs-lookup"><span data-stu-id="7d581-190">Response</span></span>
<span data-ttu-id="7d581-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7d581-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 618

{
  "@odata.type": "#microsoft.graph.androidWorkProfileWiFiConfiguration",
  "id": "8400d131-d131-8400-31d1-008431d10084",
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





