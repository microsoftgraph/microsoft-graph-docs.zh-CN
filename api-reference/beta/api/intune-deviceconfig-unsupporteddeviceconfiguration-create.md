---
title: 创建 unsupportedDeviceConfiguration
description: 创建新的 unsupportedDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e6012a286a98f676986fb8cb4aa6bb45948f50c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32517783"
---
# <a name="create-unsupporteddeviceconfiguration"></a><span data-ttu-id="b0472-103">创建 unsupportedDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0472-103">Create unsupportedDeviceConfiguration</span></span>

> <span data-ttu-id="b0472-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b0472-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0472-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0472-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0472-106">创建新的[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0472-106">Create a new [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0472-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0472-107">Prerequisites</span></span>
<span data-ttu-id="b0472-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b0472-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b0472-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0472-110">Permission type</span></span>|<span data-ttu-id="b0472-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0472-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0472-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0472-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b0472-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0472-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0472-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0472-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0472-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0472-115">Not supported.</span></span>|
|<span data-ttu-id="b0472-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0472-116">Application</span></span>|<span data-ttu-id="b0472-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0472-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0472-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0472-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b0472-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0472-119">Request headers</span></span>
|<span data-ttu-id="b0472-120">标头</span><span class="sxs-lookup"><span data-stu-id="b0472-120">Header</span></span>|<span data-ttu-id="b0472-121">值</span><span class="sxs-lookup"><span data-stu-id="b0472-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0472-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0472-122">Authorization</span></span>|<span data-ttu-id="b0472-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0472-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0472-124">接受</span><span class="sxs-lookup"><span data-stu-id="b0472-124">Accept</span></span>|<span data-ttu-id="b0472-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b0472-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0472-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0472-126">Request body</span></span>
<span data-ttu-id="b0472-127">在请求正文中, 提供 unsupportedDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0472-127">In the request body, supply a JSON representation for the unsupportedDeviceConfiguration object.</span></span>

<span data-ttu-id="b0472-128">下表显示创建 unsupportedDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b0472-128">The following table shows the properties that are required when you create the unsupportedDeviceConfiguration.</span></span>

|<span data-ttu-id="b0472-129">属性</span><span class="sxs-lookup"><span data-stu-id="b0472-129">Property</span></span>|<span data-ttu-id="b0472-130">类型</span><span class="sxs-lookup"><span data-stu-id="b0472-130">Type</span></span>|<span data-ttu-id="b0472-131">说明</span><span class="sxs-lookup"><span data-stu-id="b0472-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0472-132">id</span><span class="sxs-lookup"><span data-stu-id="b0472-132">id</span></span>|<span data-ttu-id="b0472-133">String</span><span class="sxs-lookup"><span data-stu-id="b0472-133">String</span></span>|<span data-ttu-id="b0472-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b0472-134">Key of the entity.</span></span> <span data-ttu-id="b0472-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0472-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0472-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0472-136">lastModifiedDateTime</span></span>|<span data-ttu-id="b0472-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0472-137">DateTimeOffset</span></span>|<span data-ttu-id="b0472-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b0472-138">DateTime the object was last modified.</span></span> <span data-ttu-id="b0472-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0472-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0472-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0472-140">roleScopeTagIds</span></span>|<span data-ttu-id="b0472-141">String collection</span><span class="sxs-lookup"><span data-stu-id="b0472-141">String collection</span></span>|<span data-ttu-id="b0472-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="b0472-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b0472-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0472-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0472-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="b0472-144">supportsScopeTags</span></span>|<span data-ttu-id="b0472-145">布尔</span><span class="sxs-lookup"><span data-stu-id="b0472-145">Boolean</span></span>|<span data-ttu-id="b0472-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="b0472-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="b0472-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="b0472-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="b0472-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="b0472-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="b0472-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="b0472-149">This property is read-only.</span></span> <span data-ttu-id="b0472-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0472-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0472-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0472-151">createdDateTime</span></span>|<span data-ttu-id="b0472-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0472-152">DateTimeOffset</span></span>|<span data-ttu-id="b0472-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b0472-153">DateTime the object was created.</span></span> <span data-ttu-id="b0472-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0472-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0472-155">description</span><span class="sxs-lookup"><span data-stu-id="b0472-155">description</span></span>|<span data-ttu-id="b0472-156">字符串</span><span class="sxs-lookup"><span data-stu-id="b0472-156">String</span></span>|<span data-ttu-id="b0472-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="b0472-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="b0472-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0472-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0472-159">displayName</span><span class="sxs-lookup"><span data-stu-id="b0472-159">displayName</span></span>|<span data-ttu-id="b0472-160">String</span><span class="sxs-lookup"><span data-stu-id="b0472-160">String</span></span>|<span data-ttu-id="b0472-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b0472-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="b0472-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0472-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0472-163">version</span><span class="sxs-lookup"><span data-stu-id="b0472-163">version</span></span>|<span data-ttu-id="b0472-164">Int32</span><span class="sxs-lookup"><span data-stu-id="b0472-164">Int32</span></span>|<span data-ttu-id="b0472-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="b0472-165">Version of the device configuration.</span></span> <span data-ttu-id="b0472-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="b0472-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="b0472-167">originalEntityTypeName</span><span class="sxs-lookup"><span data-stu-id="b0472-167">originalEntityTypeName</span></span>|<span data-ttu-id="b0472-168">字符串</span><span class="sxs-lookup"><span data-stu-id="b0472-168">String</span></span>|<span data-ttu-id="b0472-169">将以其他方式返回的实体的类型。</span><span class="sxs-lookup"><span data-stu-id="b0472-169">The type of entity that would be returned otherwise.</span></span>|
|<span data-ttu-id="b0472-170">详细信息</span><span class="sxs-lookup"><span data-stu-id="b0472-170">details</span></span>|<span data-ttu-id="b0472-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0472-171">[unsupportedDeviceConfigurationDetail](../resources/intune-deviceconfig-unsupporteddeviceconfigurationdetail.md) collection</span></span>|<span data-ttu-id="b0472-172">描述实体不受支持的原因的详细信息。</span><span class="sxs-lookup"><span data-stu-id="b0472-172">Details describing why the entity is unsupported.</span></span> <span data-ttu-id="b0472-173">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="b0472-173">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="b0472-174">响应</span><span class="sxs-lookup"><span data-stu-id="b0472-174">Response</span></span>
<span data-ttu-id="b0472-175">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0472-175">If successful, this method returns a `201 Created` response code and a [unsupportedDeviceConfiguration](../resources/intune-deviceconfig-unsupporteddeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0472-176">示例</span><span class="sxs-lookup"><span data-stu-id="b0472-176">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0472-177">请求</span><span class="sxs-lookup"><span data-stu-id="b0472-177">Request</span></span>
<span data-ttu-id="b0472-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0472-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="b0472-179">响应</span><span class="sxs-lookup"><span data-stu-id="b0472-179">Response</span></span>
<span data-ttu-id="b0472-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0472-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





