---
title: 创建 macOSDeviceFeaturesConfiguration
description: 创建新的 macOSDeviceFeaturesConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8d19dc422c59231aad723effb5ce25ada57631f2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924956"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="d6bb3-103">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6bb3-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="d6bb3-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d6bb3-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d6bb3-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d6bb3-107">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-107">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d6bb3-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6bb3-108">Prerequisites</span></span>
<span data-ttu-id="d6bb3-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d6bb3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6bb3-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6bb3-111">Permission type</span></span>|<span data-ttu-id="d6bb3-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d6bb3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6bb3-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6bb3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d6bb3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6bb3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6bb3-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6bb3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6bb3-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-116">Not supported.</span></span>|
|<span data-ttu-id="d6bb3-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6bb3-117">Application</span></span>|<span data-ttu-id="d6bb3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6bb3-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6bb3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6bb3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6bb3-120">Request headers</span></span>
|<span data-ttu-id="d6bb3-121">标头</span><span class="sxs-lookup"><span data-stu-id="d6bb3-121">Header</span></span>|<span data-ttu-id="d6bb3-122">值</span><span class="sxs-lookup"><span data-stu-id="d6bb3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6bb3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6bb3-123">Authorization</span></span>|<span data-ttu-id="d6bb3-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6bb3-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d6bb3-125">Accept</span></span>|<span data-ttu-id="d6bb3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d6bb3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6bb3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6bb3-127">Request body</span></span>
<span data-ttu-id="d6bb3-128">在请求正文中，提供 macOSDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-128">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="d6bb3-129">下表显示创建 macOSDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-129">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="d6bb3-130">属性</span><span class="sxs-lookup"><span data-stu-id="d6bb3-130">Property</span></span>|<span data-ttu-id="d6bb3-131">类型</span><span class="sxs-lookup"><span data-stu-id="d6bb3-131">Type</span></span>|<span data-ttu-id="d6bb3-132">说明</span><span class="sxs-lookup"><span data-stu-id="d6bb3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6bb3-133">id</span><span class="sxs-lookup"><span data-stu-id="d6bb3-133">id</span></span>|<span data-ttu-id="d6bb3-134">String</span><span class="sxs-lookup"><span data-stu-id="d6bb3-134">String</span></span>|<span data-ttu-id="d6bb3-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-135">Key of the entity.</span></span> <span data-ttu-id="d6bb3-136">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6bb3-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6bb3-137">lastModifiedDateTime</span></span>|<span data-ttu-id="d6bb3-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6bb3-138">DateTimeOffset</span></span>|<span data-ttu-id="d6bb3-139">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-139">DateTime the object was last modified.</span></span> <span data-ttu-id="d6bb3-140">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6bb3-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="d6bb3-141">roleScopeTagIds</span></span>|<span data-ttu-id="d6bb3-142">String 集合</span><span class="sxs-lookup"><span data-stu-id="d6bb3-142">String collection</span></span>|<span data-ttu-id="d6bb3-143">此实体实例范围标记的列表。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="d6bb3-144">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6bb3-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="d6bb3-145">supportsScopeTags</span></span>|<span data-ttu-id="d6bb3-146">布尔</span><span class="sxs-lookup"><span data-stu-id="d6bb3-146">Boolean</span></span>|<span data-ttu-id="d6bb3-147">指示基础的设备配置支持分配的范围标记。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="d6bb3-148">此值为 false，并且实体将不会对作用域的用户可见时，不允许将分配给 ScopeTags 属性。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="d6bb3-149">这将发生在 Silverlight 中创建的旧策略，并可以解析通过删除并重新创建 Azure 门户中的策略。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="d6bb3-150">此属性是只读的。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-150">This property is read-only.</span></span> <span data-ttu-id="d6bb3-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6bb3-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6bb3-152">createdDateTime</span></span>|<span data-ttu-id="d6bb3-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6bb3-153">DateTimeOffset</span></span>|<span data-ttu-id="d6bb3-154">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-154">DateTime the object was created.</span></span> <span data-ttu-id="d6bb3-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6bb3-156">description</span><span class="sxs-lookup"><span data-stu-id="d6bb3-156">description</span></span>|<span data-ttu-id="d6bb3-157">String</span><span class="sxs-lookup"><span data-stu-id="d6bb3-157">String</span></span>|<span data-ttu-id="d6bb3-158">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6bb3-159">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6bb3-160">displayName</span><span class="sxs-lookup"><span data-stu-id="d6bb3-160">displayName</span></span>|<span data-ttu-id="d6bb3-161">String</span><span class="sxs-lookup"><span data-stu-id="d6bb3-161">String</span></span>|<span data-ttu-id="d6bb3-162">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6bb3-163">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6bb3-164">version</span><span class="sxs-lookup"><span data-stu-id="d6bb3-164">version</span></span>|<span data-ttu-id="d6bb3-165">Int32</span><span class="sxs-lookup"><span data-stu-id="d6bb3-165">Int32</span></span>|<span data-ttu-id="d6bb3-166">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-166">Version of the device configuration.</span></span> <span data-ttu-id="d6bb3-167">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6bb3-168">airPrintDestinations</span><span class="sxs-lookup"><span data-stu-id="d6bb3-168">airPrintDestinations</span></span>|<span data-ttu-id="d6bb3-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md)集合</span><span class="sxs-lookup"><span data-stu-id="d6bb3-169">[airPrintDestination](../resources/intune-deviceconfig-airprintdestination.md) collection</span></span>|<span data-ttu-id="d6bb3-170">应始终显示的 AirPrint 打印机的数组。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-170">An array of AirPrint printers that should always be shown.</span></span> <span data-ttu-id="d6bb3-171">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-171">This collection can contain a maximum of 500 elements.</span></span> <span data-ttu-id="d6bb3-172">继承自[appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span><span class="sxs-lookup"><span data-stu-id="d6bb3-172">Inherited from [appleDeviceFeaturesConfigurationBase](../resources/intune-deviceconfig-appledevicefeaturesconfigurationbase.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d6bb3-173">响应</span><span class="sxs-lookup"><span data-stu-id="d6bb3-173">Response</span></span>
<span data-ttu-id="d6bb3-174">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-174">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6bb3-175">示例</span><span class="sxs-lookup"><span data-stu-id="d6bb3-175">Example</span></span>
### <a name="request"></a><span data-ttu-id="d6bb3-176">请求</span><span class="sxs-lookup"><span data-stu-id="d6bb3-176">Request</span></span>
<span data-ttu-id="d6bb3-177">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-177">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 564

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="d6bb3-178">响应</span><span class="sxs-lookup"><span data-stu-id="d6bb3-178">Response</span></span>
<span data-ttu-id="d6bb3-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6bb3-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





