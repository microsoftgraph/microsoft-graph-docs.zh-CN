---
title: 更新 unsupportedDeviceConfiguration
description: 更新 unsupportedDeviceConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a52781f6a018da8780ee052fdcae781ef9bc5480
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858014"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="16242-103">更新 unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="16242-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="16242-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="16242-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16242-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="16242-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16242-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="16242-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16242-107">更新[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="16242-107">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16242-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="16242-108">Prerequisites</span></span>
<span data-ttu-id="16242-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="16242-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16242-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="16242-111">Permission type</span></span>|<span data-ttu-id="16242-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="16242-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16242-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16242-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16242-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16242-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="16242-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16242-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16242-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="16242-116">Not supported.</span></span>|
|<span data-ttu-id="16242-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="16242-117">Application</span></span>|<span data-ttu-id="16242-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="16242-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16242-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16242-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="16242-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="16242-120">Request headers</span></span>
|<span data-ttu-id="16242-121">标头</span><span class="sxs-lookup"><span data-stu-id="16242-121">Header</span></span>|<span data-ttu-id="16242-122">值</span><span class="sxs-lookup"><span data-stu-id="16242-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16242-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16242-123">Authorization</span></span>|<span data-ttu-id="16242-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="16242-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16242-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16242-125">Accept</span></span>|<span data-ttu-id="16242-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16242-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16242-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="16242-127">Request body</span></span>
<span data-ttu-id="16242-128">在请求正文中，提供[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16242-128">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="16242-129">下表显示时创建[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="16242-129">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="16242-130">属性</span><span class="sxs-lookup"><span data-stu-id="16242-130">Property</span></span>|<span data-ttu-id="16242-131">类型</span><span class="sxs-lookup"><span data-stu-id="16242-131">Type</span></span>|<span data-ttu-id="16242-132">说明</span><span class="sxs-lookup"><span data-stu-id="16242-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16242-133">id</span><span class="sxs-lookup"><span data-stu-id="16242-133">id</span></span>|<span data-ttu-id="16242-134">String</span><span class="sxs-lookup"><span data-stu-id="16242-134">String</span></span>|<span data-ttu-id="16242-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="16242-135">Key of the entity.</span></span> <span data-ttu-id="16242-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16242-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16242-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="16242-137">lastModifiedDateTime</span></span>|<span data-ttu-id="16242-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16242-138">DateTimeOffset</span></span>|<span data-ttu-id="16242-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="16242-139">DateTime the object was last modified.</span></span> <span data-ttu-id="16242-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16242-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16242-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="16242-141">roleScopeTagIds</span></span>|<span data-ttu-id="16242-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="16242-142">String collection</span></span>|<span data-ttu-id="16242-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="16242-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="16242-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16242-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16242-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="16242-145">supportsScopeTags</span></span>|<span data-ttu-id="16242-146">布尔</span><span class="sxs-lookup"><span data-stu-id="16242-146">Boolean</span></span>|<span data-ttu-id="16242-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="16242-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="16242-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="16242-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="16242-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="16242-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="16242-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="16242-150">This property is read-only.</span></span> <span data-ttu-id="16242-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16242-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16242-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="16242-152">createdDateTime</span></span>|<span data-ttu-id="16242-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16242-153">DateTimeOffset</span></span>|<span data-ttu-id="16242-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="16242-154">DateTime the object was created.</span></span> <span data-ttu-id="16242-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16242-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16242-156">description</span><span class="sxs-lookup"><span data-stu-id="16242-156">description</span></span>|<span data-ttu-id="16242-157">String</span><span class="sxs-lookup"><span data-stu-id="16242-157">String</span></span>|<span data-ttu-id="16242-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="16242-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="16242-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16242-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16242-160">displayName</span><span class="sxs-lookup"><span data-stu-id="16242-160">displayName</span></span>|<span data-ttu-id="16242-161">String</span><span class="sxs-lookup"><span data-stu-id="16242-161">String</span></span>|<span data-ttu-id="16242-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="16242-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="16242-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16242-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16242-164">version</span><span class="sxs-lookup"><span data-stu-id="16242-164">version</span></span>|<span data-ttu-id="16242-165">Int32</span><span class="sxs-lookup"><span data-stu-id="16242-165">Int32</span></span>|<span data-ttu-id="16242-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="16242-166">Version of the device configuration.</span></span> <span data-ttu-id="16242-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="16242-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="16242-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="16242-168">originalEntityTypeName</span></span>|<span data-ttu-id="16242-169">字符串</span><span class="sxs-lookup"><span data-stu-id="16242-169">String</span></span>|<span data-ttu-id="16242-170">否则将返回的实体的类型。</span><span class="sxs-lookup"><span data-stu-id="16242-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="16242-171">详细信息</span><span class="sxs-lookup"><span data-stu-id="16242-171">details</span></span>|<span data-ttu-id="16242-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="16242-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="16242-173">说明为什么实体不受支持的详细信息。</span><span class="sxs-lookup"><span data-stu-id="16242-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="16242-174">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="16242-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="16242-175">响应</span><span class="sxs-lookup"><span data-stu-id="16242-175">Response</span></span>
<span data-ttu-id="16242-176">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="16242-176">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16242-177">示例</span><span class="sxs-lookup"><span data-stu-id="16242-177">Example</span></span>
### <a name="request"></a><span data-ttu-id="16242-178">请求</span><span class="sxs-lookup"><span data-stu-id="16242-178">Request</span></span>
<span data-ttu-id="16242-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16242-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 513

{
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="16242-180">响应</span><span class="sxs-lookup"><span data-stu-id="16242-180">Response</span></span>
<span data-ttu-id="16242-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16242-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 690

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
  "id": "f80d6fc8-6fc8-f80d-c86f-0df8c86f0df8",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "originalEntityTypeName": "Original Entity Type Name value",
  "details": [
    {
      "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail",
      "message": "Message value",
      "propertyName": "Property Name value"
    }
  ]
}
```





