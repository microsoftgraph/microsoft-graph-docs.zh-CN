---
title: 更新 unsupportedDeviceConfiguration
description: 更新 unsupportedDeviceConfiguration 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: cf4dc0e52b577682ea88a93abaabb561dbb444b7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29395018"
---
# <a name="update-unsupporteddeviceconfiguration"></a><span data-ttu-id="0cb40-103">更新 unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="0cb40-103">Update unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="0cb40-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="0cb40-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0cb40-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0cb40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0cb40-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0cb40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cb40-107">更新[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0cb40-107">Update the properties of a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cb40-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0cb40-108">Prerequisites</span></span>
<span data-ttu-id="0cb40-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0cb40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="0cb40-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cb40-111">Permission type</span></span>|<span data-ttu-id="0cb40-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0cb40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cb40-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cb40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0cb40-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cb40-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cb40-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cb40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cb40-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cb40-116">Not supported.</span></span>|
|<span data-ttu-id="0cb40-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cb40-117">Application</span></span>|<span data-ttu-id="0cb40-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cb40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cb40-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cb40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="0cb40-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cb40-120">Request headers</span></span>
|<span data-ttu-id="0cb40-121">标头</span><span class="sxs-lookup"><span data-stu-id="0cb40-121">Header</span></span>|<span data-ttu-id="0cb40-122">值</span><span class="sxs-lookup"><span data-stu-id="0cb40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cb40-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cb40-123">Authorization</span></span>|<span data-ttu-id="0cb40-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0cb40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cb40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0cb40-125">Accept</span></span>|<span data-ttu-id="0cb40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0cb40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cb40-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cb40-127">Request body</span></span>
<span data-ttu-id="0cb40-128">在请求正文中，提供[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cb40-128">In the request body, supply a JSON representation for the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

<span data-ttu-id="0cb40-129">下表显示时创建[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0cb40-129">The following table shows the properties that are required when you create the [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md).</span></span>

|<span data-ttu-id="0cb40-130">属性</span><span class="sxs-lookup"><span data-stu-id="0cb40-130">Property</span></span>|<span data-ttu-id="0cb40-131">类型</span><span class="sxs-lookup"><span data-stu-id="0cb40-131">Type</span></span>|<span data-ttu-id="0cb40-132">说明</span><span class="sxs-lookup"><span data-stu-id="0cb40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cb40-133">id</span><span class="sxs-lookup"><span data-stu-id="0cb40-133">id</span></span>|<span data-ttu-id="0cb40-134">String</span><span class="sxs-lookup"><span data-stu-id="0cb40-134">String</span></span>|<span data-ttu-id="0cb40-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0cb40-135">Key of the entity.</span></span> <span data-ttu-id="0cb40-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cb40-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cb40-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0cb40-137">lastModifiedDateTime</span></span>|<span data-ttu-id="0cb40-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cb40-138">DateTimeOffset</span></span>|<span data-ttu-id="0cb40-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0cb40-139">DateTime the object was last modified.</span></span> <span data-ttu-id="0cb40-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cb40-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cb40-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0cb40-141">roleScopeTagIds</span></span>|<span data-ttu-id="0cb40-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="0cb40-142">String collection</span></span>|<span data-ttu-id="0cb40-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="0cb40-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="0cb40-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cb40-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cb40-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="0cb40-145">supportsScopeTags</span></span>|<span data-ttu-id="0cb40-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb40-146">Boolean</span></span>|<span data-ttu-id="0cb40-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="0cb40-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="0cb40-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="0cb40-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="0cb40-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="0cb40-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="0cb40-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="0cb40-150">This property is read-only.</span></span> <span data-ttu-id="0cb40-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cb40-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cb40-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0cb40-152">createdDateTime</span></span>|<span data-ttu-id="0cb40-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0cb40-153">DateTimeOffset</span></span>|<span data-ttu-id="0cb40-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="0cb40-154">DateTime the object was created.</span></span> <span data-ttu-id="0cb40-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cb40-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cb40-156">description</span><span class="sxs-lookup"><span data-stu-id="0cb40-156">description</span></span>|<span data-ttu-id="0cb40-157">String</span><span class="sxs-lookup"><span data-stu-id="0cb40-157">String</span></span>|<span data-ttu-id="0cb40-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="0cb40-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="0cb40-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cb40-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cb40-160">displayName</span><span class="sxs-lookup"><span data-stu-id="0cb40-160">displayName</span></span>|<span data-ttu-id="0cb40-161">String</span><span class="sxs-lookup"><span data-stu-id="0cb40-161">String</span></span>|<span data-ttu-id="0cb40-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="0cb40-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="0cb40-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cb40-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cb40-164">version</span><span class="sxs-lookup"><span data-stu-id="0cb40-164">version</span></span>|<span data-ttu-id="0cb40-165">Int32</span><span class="sxs-lookup"><span data-stu-id="0cb40-165">Int32</span></span>|<span data-ttu-id="0cb40-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="0cb40-166">Version of the device configuration.</span></span> <span data-ttu-id="0cb40-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="0cb40-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="0cb40-168">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="0cb40-168">originalEntityTypeName</span></span>|<span data-ttu-id="0cb40-169">String</span><span class="sxs-lookup"><span data-stu-id="0cb40-169">String</span></span>|<span data-ttu-id="0cb40-170">否则将返回的实体的类型。</span><span class="sxs-lookup"><span data-stu-id="0cb40-170">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="0cb40-171">详细信息</span><span class="sxs-lookup"><span data-stu-id="0cb40-171">details</span></span>|<span data-ttu-id="0cb40-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="0cb40-172">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="0cb40-173">说明为什么实体不受支持的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0cb40-173">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="0cb40-174">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="0cb40-174">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="0cb40-175">响应</span><span class="sxs-lookup"><span data-stu-id="0cb40-175">Response</span></span>
<span data-ttu-id="0cb40-176">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0cb40-176">If successful, this method returns a `200 OK` response code and an updated [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cb40-177">示例</span><span class="sxs-lookup"><span data-stu-id="0cb40-177">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cb40-178">请求</span><span class="sxs-lookup"><span data-stu-id="0cb40-178">Request</span></span>
<span data-ttu-id="0cb40-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0cb40-179">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 518

{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="0cb40-180">响应</span><span class="sxs-lookup"><span data-stu-id="0cb40-180">Response</span></span>
<span data-ttu-id="0cb40-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0cb40-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




