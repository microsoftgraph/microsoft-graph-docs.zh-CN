---
title: 更新 iosCustomConfiguration
description: 更新 iosCustomConfiguration 对象的属性。
ms.openlocfilehash: 6151c93e83bd35db70d6c5428d55bde92e8027de
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009705"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="eca25-103">更新 iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="eca25-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="eca25-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="eca25-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="eca25-105">更新 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="eca25-105">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eca25-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="eca25-106">Prerequisites</span></span>
<span data-ttu-id="eca25-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="eca25-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eca25-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="eca25-109">Permission type</span></span>|<span data-ttu-id="eca25-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eca25-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eca25-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eca25-111">Delegated (work or school account)</span></span>|<span data-ttu-id="eca25-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eca25-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eca25-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eca25-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eca25-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="eca25-114">Not supported.</span></span>|
|<span data-ttu-id="eca25-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="eca25-115">Application</span></span>|<span data-ttu-id="eca25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eca25-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eca25-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eca25-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="eca25-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="eca25-118">Request headers</span></span>
|<span data-ttu-id="eca25-119">标头</span><span class="sxs-lookup"><span data-stu-id="eca25-119">Header</span></span>|<span data-ttu-id="eca25-120">值</span><span class="sxs-lookup"><span data-stu-id="eca25-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eca25-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="eca25-121">Authorization</span></span>|<span data-ttu-id="eca25-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eca25-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eca25-123">Accept</span><span class="sxs-lookup"><span data-stu-id="eca25-123">Accept</span></span>|<span data-ttu-id="eca25-124">application/json</span><span class="sxs-lookup"><span data-stu-id="eca25-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eca25-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="eca25-125">Request body</span></span>
<span data-ttu-id="eca25-126">在请求正文中，提供 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eca25-126">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="eca25-127">下表显示创建 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eca25-127">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="eca25-128">属性</span><span class="sxs-lookup"><span data-stu-id="eca25-128">Property</span></span>|<span data-ttu-id="eca25-129">类型</span><span class="sxs-lookup"><span data-stu-id="eca25-129">Type</span></span>|<span data-ttu-id="eca25-130">说明</span><span class="sxs-lookup"><span data-stu-id="eca25-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eca25-131">id</span><span class="sxs-lookup"><span data-stu-id="eca25-131">id</span></span>|<span data-ttu-id="eca25-132">String</span><span class="sxs-lookup"><span data-stu-id="eca25-132">String</span></span>|<span data-ttu-id="eca25-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="eca25-133">Key of the entity.</span></span> <span data-ttu-id="eca25-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eca25-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca25-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eca25-135">lastModifiedDateTime</span></span>|<span data-ttu-id="eca25-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eca25-136">DateTimeOffset</span></span>|<span data-ttu-id="eca25-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eca25-137">DateTime the object was last modified.</span></span> <span data-ttu-id="eca25-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eca25-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca25-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eca25-139">createdDateTime</span></span>|<span data-ttu-id="eca25-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eca25-140">DateTimeOffset</span></span>|<span data-ttu-id="eca25-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="eca25-141">DateTime the object was created.</span></span> <span data-ttu-id="eca25-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eca25-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca25-143">description</span><span class="sxs-lookup"><span data-stu-id="eca25-143">description</span></span>|<span data-ttu-id="eca25-144">String</span><span class="sxs-lookup"><span data-stu-id="eca25-144">String</span></span>|<span data-ttu-id="eca25-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="eca25-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="eca25-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eca25-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca25-147">displayName</span><span class="sxs-lookup"><span data-stu-id="eca25-147">displayName</span></span>|<span data-ttu-id="eca25-148">String</span><span class="sxs-lookup"><span data-stu-id="eca25-148">String</span></span>|<span data-ttu-id="eca25-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="eca25-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="eca25-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eca25-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca25-151">version</span><span class="sxs-lookup"><span data-stu-id="eca25-151">version</span></span>|<span data-ttu-id="eca25-152">Int32</span><span class="sxs-lookup"><span data-stu-id="eca25-152">Int32</span></span>|<span data-ttu-id="eca25-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="eca25-153">Version of the device configuration.</span></span> <span data-ttu-id="eca25-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="eca25-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="eca25-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="eca25-155">payloadName</span></span>|<span data-ttu-id="eca25-156">String</span><span class="sxs-lookup"><span data-stu-id="eca25-156">String</span></span>|<span data-ttu-id="eca25-157">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="eca25-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="eca25-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="eca25-158">payloadFileName</span></span>|<span data-ttu-id="eca25-159">String</span><span class="sxs-lookup"><span data-stu-id="eca25-159">String</span></span>|<span data-ttu-id="eca25-160">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="eca25-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="eca25-161">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="eca25-161">\*.xml).</span></span>|
|<span data-ttu-id="eca25-162">payload</span><span class="sxs-lookup"><span data-stu-id="eca25-162">payload</span></span>|<span data-ttu-id="eca25-163">Binary</span><span class="sxs-lookup"><span data-stu-id="eca25-163">Binary</span></span>|<span data-ttu-id="eca25-164">有效负载。</span><span class="sxs-lookup"><span data-stu-id="eca25-164">Payload.</span></span> <span data-ttu-id="eca25-165">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="eca25-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="eca25-166">响应</span><span class="sxs-lookup"><span data-stu-id="eca25-166">Response</span></span>
<span data-ttu-id="eca25-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="eca25-167">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eca25-168">示例</span><span class="sxs-lookup"><span data-stu-id="eca25-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="eca25-169">请求</span><span class="sxs-lookup"><span data-stu-id="eca25-169">Request</span></span>
<span data-ttu-id="eca25-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eca25-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 279

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="eca25-171">响应</span><span class="sxs-lookup"><span data-stu-id="eca25-171">Response</span></span>
<span data-ttu-id="eca25-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eca25-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 451

{
  "@odata.type": "#microsoft.graph.iosCustomConfiguration",
  "id": "f34428e3-28e3-f344-e328-44f3e32844f3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```



