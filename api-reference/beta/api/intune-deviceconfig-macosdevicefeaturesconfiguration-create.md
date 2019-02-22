---
title: 创建 macOSDeviceFeaturesConfiguration
description: 创建新的 macOSDeviceFeaturesConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5bccd64c5fc4b102340407ba1967a3b101c0b43e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148970"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="8f467-103">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="8f467-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="8f467-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8f467-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f467-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8f467-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f467-106">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f467-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8f467-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8f467-107">Prerequisites</span></span>
<span data-ttu-id="8f467-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="8f467-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="8f467-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8f467-110">Permission type</span></span>|<span data-ttu-id="8f467-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8f467-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f467-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8f467-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8f467-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8f467-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8f467-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8f467-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f467-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f467-115">Not supported.</span></span>|
|<span data-ttu-id="8f467-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8f467-116">Application</span></span>|<span data-ttu-id="8f467-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8f467-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f467-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8f467-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8f467-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8f467-119">Request headers</span></span>
|<span data-ttu-id="8f467-120">标头</span><span class="sxs-lookup"><span data-stu-id="8f467-120">Header</span></span>|<span data-ttu-id="8f467-121">值</span><span class="sxs-lookup"><span data-stu-id="8f467-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f467-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f467-122">Authorization</span></span>|<span data-ttu-id="8f467-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8f467-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f467-124">Accept</span><span class="sxs-lookup"><span data-stu-id="8f467-124">Accept</span></span>|<span data-ttu-id="8f467-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8f467-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f467-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8f467-126">Request body</span></span>
<span data-ttu-id="8f467-127">在请求正文中，提供 macOSDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8f467-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="8f467-128">下表显示创建 macOSDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8f467-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="8f467-129">属性</span><span class="sxs-lookup"><span data-stu-id="8f467-129">Property</span></span>|<span data-ttu-id="8f467-130">类型</span><span class="sxs-lookup"><span data-stu-id="8f467-130">Type</span></span>|<span data-ttu-id="8f467-131">说明</span><span class="sxs-lookup"><span data-stu-id="8f467-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f467-132">id</span><span class="sxs-lookup"><span data-stu-id="8f467-132">id</span></span>|<span data-ttu-id="8f467-133">String</span><span class="sxs-lookup"><span data-stu-id="8f467-133">String</span></span>|<span data-ttu-id="8f467-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8f467-134">Key of the entity.</span></span> <span data-ttu-id="8f467-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f467-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f467-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8f467-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f467-137">DateTimeOffset</span></span>|<span data-ttu-id="8f467-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8f467-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8f467-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f467-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="8f467-140">roleScopeTagIds</span></span>|<span data-ttu-id="8f467-141">String collection</span><span class="sxs-lookup"><span data-stu-id="8f467-141">String collection</span></span>|<span data-ttu-id="8f467-142">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="8f467-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="8f467-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f467-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="8f467-144">supportsScopeTags</span></span>|<span data-ttu-id="8f467-145">布尔</span><span class="sxs-lookup"><span data-stu-id="8f467-145">Boolean</span></span>|<span data-ttu-id="8f467-146">指示基础设备配置是否支持作用域标记的分配。</span><span class="sxs-lookup"><span data-stu-id="8f467-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="8f467-147">如果此值为 false, 则不允许分配给 ScopeTags 属性, 并且实体将对作用域用户不可见。</span><span class="sxs-lookup"><span data-stu-id="8f467-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="8f467-148">这适用于在 Silverlight 中创建的旧版策略, 可以通过在 Azure 门户中删除并重新创建策略来解决此事件。</span><span class="sxs-lookup"><span data-stu-id="8f467-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="8f467-149">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="8f467-149">This property is read-only.</span></span> <span data-ttu-id="8f467-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f467-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8f467-151">createdDateTime</span></span>|<span data-ttu-id="8f467-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f467-152">DateTimeOffset</span></span>|<span data-ttu-id="8f467-153">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8f467-153">DateTime the object was created.</span></span> <span data-ttu-id="8f467-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f467-155">description</span><span class="sxs-lookup"><span data-stu-id="8f467-155">description</span></span>|<span data-ttu-id="8f467-156">String</span><span class="sxs-lookup"><span data-stu-id="8f467-156">String</span></span>|<span data-ttu-id="8f467-157">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8f467-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8f467-158">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f467-159">displayName</span><span class="sxs-lookup"><span data-stu-id="8f467-159">displayName</span></span>|<span data-ttu-id="8f467-160">String</span><span class="sxs-lookup"><span data-stu-id="8f467-160">String</span></span>|<span data-ttu-id="8f467-161">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8f467-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8f467-162">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f467-163">version</span><span class="sxs-lookup"><span data-stu-id="8f467-163">version</span></span>|<span data-ttu-id="8f467-164">Int32</span><span class="sxs-lookup"><span data-stu-id="8f467-164">Int32</span></span>|<span data-ttu-id="8f467-165">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8f467-165">Version of the device configuration.</span></span> <span data-ttu-id="8f467-166">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8f467-167">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="8f467-167">airPrintDestinations</span></span>|<span data-ttu-id="8f467-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="8f467-168">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="8f467-169">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="8f467-169">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="8f467-170">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="8f467-170">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="8f467-171">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="8f467-171">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8f467-172">响应</span><span class="sxs-lookup"><span data-stu-id="8f467-172">Response</span></span>
<span data-ttu-id="8f467-173">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8f467-173">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f467-174">示例</span><span class="sxs-lookup"><span data-stu-id="8f467-174">Example</span></span>

### <a name="request"></a><span data-ttu-id="8f467-175">请求</span><span class="sxs-lookup"><span data-stu-id="8f467-175">Request</span></span>
<span data-ttu-id="8f467-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8f467-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 500

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="8f467-177">响应</span><span class="sxs-lookup"><span data-stu-id="8f467-177">Response</span></span>
<span data-ttu-id="8f467-p111">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8f467-p111">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 672

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "airPrintDestinations": [
    {
      "@odata.type": "microsoft.graph.airPrintDestination",
      "ipAddress": "Ip Address value",
      "resourcePath": "Resource Path value",
      "port": 4,
      "forceTls": true
    }
  ]
}
```




