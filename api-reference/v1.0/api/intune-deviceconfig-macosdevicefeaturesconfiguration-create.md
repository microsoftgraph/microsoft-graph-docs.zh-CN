---
title: 创建 macOSDeviceFeaturesConfiguration
description: 创建新的 macOSDeviceFeaturesConfiguration 对象。
ms.openlocfilehash: e8d6d16ce66e512d44cbae63ec41122b526ac471
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007700"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="24085-103">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="24085-103">Create macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="24085-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="24085-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="24085-105">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24085-105">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="24085-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="24085-106">Prerequisites</span></span>
<span data-ttu-id="24085-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="24085-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24085-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24085-109">Permission type</span></span>|<span data-ttu-id="24085-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="24085-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24085-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24085-111">Delegated (work or school account)</span></span>|<span data-ttu-id="24085-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24085-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24085-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24085-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24085-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24085-114">Not supported.</span></span>|
|<span data-ttu-id="24085-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="24085-115">Application</span></span>|<span data-ttu-id="24085-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="24085-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="24085-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24085-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="24085-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="24085-118">Request headers</span></span>
|<span data-ttu-id="24085-119">标头</span><span class="sxs-lookup"><span data-stu-id="24085-119">Header</span></span>|<span data-ttu-id="24085-120">值</span><span class="sxs-lookup"><span data-stu-id="24085-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24085-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="24085-121">Authorization</span></span>|<span data-ttu-id="24085-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24085-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24085-123">Accept</span><span class="sxs-lookup"><span data-stu-id="24085-123">Accept</span></span>|<span data-ttu-id="24085-124">application/json</span><span class="sxs-lookup"><span data-stu-id="24085-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24085-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="24085-125">Request body</span></span>
<span data-ttu-id="24085-126">在请求正文中，提供 macOSDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="24085-126">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="24085-127">下表显示创建 macOSDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="24085-127">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="24085-128">属性</span><span class="sxs-lookup"><span data-stu-id="24085-128">Property</span></span>|<span data-ttu-id="24085-129">类型</span><span class="sxs-lookup"><span data-stu-id="24085-129">Type</span></span>|<span data-ttu-id="24085-130">说明</span><span class="sxs-lookup"><span data-stu-id="24085-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="24085-131">id</span><span class="sxs-lookup"><span data-stu-id="24085-131">id</span></span>|<span data-ttu-id="24085-132">String</span><span class="sxs-lookup"><span data-stu-id="24085-132">String</span></span>|<span data-ttu-id="24085-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="24085-133">Key of the entity.</span></span> <span data-ttu-id="24085-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24085-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24085-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="24085-135">lastModifiedDateTime</span></span>|<span data-ttu-id="24085-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24085-136">DateTimeOffset</span></span>|<span data-ttu-id="24085-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="24085-137">DateTime the object was last modified.</span></span> <span data-ttu-id="24085-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24085-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24085-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="24085-139">createdDateTime</span></span>|<span data-ttu-id="24085-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24085-140">DateTimeOffset</span></span>|<span data-ttu-id="24085-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="24085-141">DateTime the object was created.</span></span> <span data-ttu-id="24085-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24085-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24085-143">description</span><span class="sxs-lookup"><span data-stu-id="24085-143">description</span></span>|<span data-ttu-id="24085-144">String</span><span class="sxs-lookup"><span data-stu-id="24085-144">String</span></span>|<span data-ttu-id="24085-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="24085-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="24085-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24085-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24085-147">displayName</span><span class="sxs-lookup"><span data-stu-id="24085-147">displayName</span></span>|<span data-ttu-id="24085-148">String</span><span class="sxs-lookup"><span data-stu-id="24085-148">String</span></span>|<span data-ttu-id="24085-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="24085-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="24085-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24085-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="24085-151">version</span><span class="sxs-lookup"><span data-stu-id="24085-151">version</span></span>|<span data-ttu-id="24085-152">Int32</span><span class="sxs-lookup"><span data-stu-id="24085-152">Int32</span></span>|<span data-ttu-id="24085-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="24085-153">Version of the device configuration.</span></span> <span data-ttu-id="24085-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="24085-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="24085-155">响应</span><span class="sxs-lookup"><span data-stu-id="24085-155">Response</span></span>
<span data-ttu-id="24085-156">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="24085-156">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24085-157">示例</span><span class="sxs-lookup"><span data-stu-id="24085-157">Example</span></span>
### <a name="request"></a><span data-ttu-id="24085-158">请求</span><span class="sxs-lookup"><span data-stu-id="24085-158">Request</span></span>
<span data-ttu-id="24085-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24085-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="24085-160">响应</span><span class="sxs-lookup"><span data-stu-id="24085-160">Response</span></span>
<span data-ttu-id="24085-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24085-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 342

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "id": "49fa957d-957d-49fa-7d95-fa497d95fa49",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```



