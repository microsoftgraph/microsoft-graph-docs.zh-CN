---
title: 创建 androidWiFiConfiguration
description: 创建新的 androidWiFiConfiguration 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 69ba72acd57454ecd70e6ee0de4cc5a1f8f4f213
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413029"
---
# <a name="create-androidwificonfiguration"></a><span data-ttu-id="10cbd-103">创建 androidWiFiConfiguration</span><span class="sxs-lookup"><span data-stu-id="10cbd-103">Create androidWiFiConfiguration</span></span>

> <span data-ttu-id="10cbd-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="10cbd-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="10cbd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="10cbd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10cbd-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="10cbd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="10cbd-107">创建新的[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10cbd-107">Create a new [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="10cbd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="10cbd-108">Prerequisites</span></span>
<span data-ttu-id="10cbd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="10cbd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="10cbd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="10cbd-111">Permission type</span></span>|<span data-ttu-id="10cbd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10cbd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10cbd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10cbd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10cbd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="10cbd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="10cbd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10cbd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10cbd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10cbd-116">Not supported.</span></span>|
|<span data-ttu-id="10cbd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="10cbd-117">Application</span></span>|<span data-ttu-id="10cbd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="10cbd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10cbd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10cbd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="10cbd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="10cbd-120">Request headers</span></span>
|<span data-ttu-id="10cbd-121">标头</span><span class="sxs-lookup"><span data-stu-id="10cbd-121">Header</span></span>|<span data-ttu-id="10cbd-122">值</span><span class="sxs-lookup"><span data-stu-id="10cbd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10cbd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10cbd-123">Authorization</span></span>|<span data-ttu-id="10cbd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10cbd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10cbd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10cbd-125">Accept</span></span>|<span data-ttu-id="10cbd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10cbd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10cbd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="10cbd-127">Request body</span></span>
<span data-ttu-id="10cbd-128">在请求正文中，提供 androidWiFiConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="10cbd-128">In the request body, supply a JSON representation for the androidWiFiConfiguration object.</span></span>

<span data-ttu-id="10cbd-129">下表显示时创建 androidWiFiConfiguration 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="10cbd-129">The following table shows the properties that are required when you create the androidWiFiConfiguration.</span></span>

|<span data-ttu-id="10cbd-130">属性</span><span class="sxs-lookup"><span data-stu-id="10cbd-130">Property</span></span>|<span data-ttu-id="10cbd-131">类型</span><span class="sxs-lookup"><span data-stu-id="10cbd-131">Type</span></span>|<span data-ttu-id="10cbd-132">说明</span><span class="sxs-lookup"><span data-stu-id="10cbd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="10cbd-133">id</span><span class="sxs-lookup"><span data-stu-id="10cbd-133">id</span></span>|<span data-ttu-id="10cbd-134">String</span><span class="sxs-lookup"><span data-stu-id="10cbd-134">String</span></span>|<span data-ttu-id="10cbd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="10cbd-135">Key of the entity.</span></span> <span data-ttu-id="10cbd-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10cbd-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10cbd-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="10cbd-137">lastModifiedDateTime</span></span>|<span data-ttu-id="10cbd-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10cbd-138">DateTimeOffset</span></span>|<span data-ttu-id="10cbd-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="10cbd-139">DateTime the object was last modified.</span></span> <span data-ttu-id="10cbd-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10cbd-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10cbd-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="10cbd-141">roleScopeTagIds</span></span>|<span data-ttu-id="10cbd-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="10cbd-142">String collection</span></span>|<span data-ttu-id="10cbd-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="10cbd-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="10cbd-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10cbd-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10cbd-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="10cbd-145">supportsScopeTags</span></span>|<span data-ttu-id="10cbd-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="10cbd-146">Boolean</span></span>|<span data-ttu-id="10cbd-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="10cbd-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="10cbd-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="10cbd-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="10cbd-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="10cbd-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="10cbd-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="10cbd-150">This property is read-only.</span></span> <span data-ttu-id="10cbd-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10cbd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10cbd-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="10cbd-152">createdDateTime</span></span>|<span data-ttu-id="10cbd-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="10cbd-153">DateTimeOffset</span></span>|<span data-ttu-id="10cbd-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="10cbd-154">DateTime the object was created.</span></span> <span data-ttu-id="10cbd-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10cbd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10cbd-156">description</span><span class="sxs-lookup"><span data-stu-id="10cbd-156">description</span></span>|<span data-ttu-id="10cbd-157">String</span><span class="sxs-lookup"><span data-stu-id="10cbd-157">String</span></span>|<span data-ttu-id="10cbd-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="10cbd-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="10cbd-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10cbd-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10cbd-160">displayName</span><span class="sxs-lookup"><span data-stu-id="10cbd-160">displayName</span></span>|<span data-ttu-id="10cbd-161">String</span><span class="sxs-lookup"><span data-stu-id="10cbd-161">String</span></span>|<span data-ttu-id="10cbd-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="10cbd-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="10cbd-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10cbd-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10cbd-164">version</span><span class="sxs-lookup"><span data-stu-id="10cbd-164">version</span></span>|<span data-ttu-id="10cbd-165">Int32</span><span class="sxs-lookup"><span data-stu-id="10cbd-165">Int32</span></span>|<span data-ttu-id="10cbd-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="10cbd-166">Version of the device configuration.</span></span> <span data-ttu-id="10cbd-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="10cbd-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="10cbd-168">networkName</span><span class="sxs-lookup"><span data-stu-id="10cbd-168">networkName</span></span>|<span data-ttu-id="10cbd-169">String</span><span class="sxs-lookup"><span data-stu-id="10cbd-169">String</span></span>|<span data-ttu-id="10cbd-170">网络名称</span><span class="sxs-lookup"><span data-stu-id="10cbd-170">Network Name</span></span>|
|<span data-ttu-id="10cbd-171">ssid</span><span class="sxs-lookup"><span data-stu-id="10cbd-171">ssid</span></span>|<span data-ttu-id="10cbd-172">String</span><span class="sxs-lookup"><span data-stu-id="10cbd-172">String</span></span>|<span data-ttu-id="10cbd-173">这是广播到所有设备 Wi-fi 网络的名称。</span><span class="sxs-lookup"><span data-stu-id="10cbd-173">This is the name of the Wi-Fi network that is broadcast to all devices.</span></span>|
|<span data-ttu-id="10cbd-174">connectAutomatically</span><span class="sxs-lookup"><span data-stu-id="10cbd-174">connectAutomatically</span></span>|<span data-ttu-id="10cbd-175">Boolean</span><span class="sxs-lookup"><span data-stu-id="10cbd-175">Boolean</span></span>|<span data-ttu-id="10cbd-176">自动连接此网络何时范围中。</span><span class="sxs-lookup"><span data-stu-id="10cbd-176">Connect automatically when this network is in range.</span></span> <span data-ttu-id="10cbd-177">将此值设置为 true 将跳过的用户提示并自动将设备连接到 Wi-fi 网络。</span><span class="sxs-lookup"><span data-stu-id="10cbd-177">Setting this to true will skip the user prompt and automatically connect the device to Wi-Fi network.</span></span>|
|<span data-ttu-id="10cbd-178">connectWhenNetworkNameIsHidden</span><span class="sxs-lookup"><span data-stu-id="10cbd-178">connectWhenNetworkNameIsHidden</span></span>|<span data-ttu-id="10cbd-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="10cbd-179">Boolean</span></span>|<span data-ttu-id="10cbd-180">当设置为 true，该配置文件强制设备连接到不广播到所有设备其 SSID 网络。</span><span class="sxs-lookup"><span data-stu-id="10cbd-180">When set to true, this profile forces the device to connect to a network that doesn't broadcast its SSID to all devices.</span></span>|
|<span data-ttu-id="10cbd-181">wiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="10cbd-181">wiFiSecurityType</span></span>|[<span data-ttu-id="10cbd-182">androidWiFiSecurityType</span><span class="sxs-lookup"><span data-stu-id="10cbd-182">androidWiFiSecurityType</span></span>](../resources/intune-deviceconfig-androidwifisecuritytype.md)|<span data-ttu-id="10cbd-183">指示是否 Wi-fi 终结点使用 EAP 基于安全类型。</span><span class="sxs-lookup"><span data-stu-id="10cbd-183">Indicates whether Wi-Fi endpoint uses an EAP based security type.</span></span> <span data-ttu-id="10cbd-184">可取值为：`open`、`wpaEnterprise`。</span><span class="sxs-lookup"><span data-stu-id="10cbd-184">Possible values are: `open`, `wpaEnterprise`.</span></span>|



## <a name="response"></a><span data-ttu-id="10cbd-185">响应</span><span class="sxs-lookup"><span data-stu-id="10cbd-185">Response</span></span>
<span data-ttu-id="10cbd-186">如果成功，此方法返回`201 Created`响应代码和响应正文中的[androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="10cbd-186">If successful, this method returns a `201 Created` response code and a [androidWiFiConfiguration](../resources/intune-deviceconfig-androidwificonfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10cbd-187">示例</span><span class="sxs-lookup"><span data-stu-id="10cbd-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="10cbd-188">请求</span><span class="sxs-lookup"><span data-stu-id="10cbd-188">Request</span></span>
<span data-ttu-id="10cbd-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10cbd-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="10cbd-190">响应</span><span class="sxs-lookup"><span data-stu-id="10cbd-190">Response</span></span>
<span data-ttu-id="10cbd-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10cbd-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




