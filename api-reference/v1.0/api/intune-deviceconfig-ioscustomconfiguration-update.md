---
title: 更新 iosCustomConfiguration
description: 更新 iosCustomConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fbd8c85281930c1f8d646425bcac47322802ccbb
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259015"
---
# <a name="update-ioscustomconfiguration"></a><span data-ttu-id="51e31-103">更新 iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="51e31-103">Update iosCustomConfiguration</span></span>

> <span data-ttu-id="51e31-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51e31-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51e31-105">更新 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="51e31-105">Update the properties of a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51e31-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="51e31-106">Prerequisites</span></span>
<span data-ttu-id="51e31-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="51e31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="51e31-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="51e31-109">Permission type</span></span>|<span data-ttu-id="51e31-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="51e31-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51e31-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51e31-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51e31-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51e31-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51e31-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51e31-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51e31-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="51e31-114">Not supported.</span></span>|
|<span data-ttu-id="51e31-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="51e31-115">Application</span></span>|<span data-ttu-id="51e31-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="51e31-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51e31-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51e31-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="51e31-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="51e31-118">Request headers</span></span>
|<span data-ttu-id="51e31-119">标头</span><span class="sxs-lookup"><span data-stu-id="51e31-119">Header</span></span>|<span data-ttu-id="51e31-120">值</span><span class="sxs-lookup"><span data-stu-id="51e31-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51e31-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51e31-121">Authorization</span></span>|<span data-ttu-id="51e31-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="51e31-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51e31-123">Accept</span><span class="sxs-lookup"><span data-stu-id="51e31-123">Accept</span></span>|<span data-ttu-id="51e31-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51e31-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51e31-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="51e31-125">Request body</span></span>
<span data-ttu-id="51e31-126">在请求正文中，提供 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="51e31-126">In the request body, supply a JSON representation for the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>

<span data-ttu-id="51e31-127">下表显示创建 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="51e31-127">The following table shows the properties that are required when you create the [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md).</span></span>

|<span data-ttu-id="51e31-128">属性</span><span class="sxs-lookup"><span data-stu-id="51e31-128">Property</span></span>|<span data-ttu-id="51e31-129">类型</span><span class="sxs-lookup"><span data-stu-id="51e31-129">Type</span></span>|<span data-ttu-id="51e31-130">说明</span><span class="sxs-lookup"><span data-stu-id="51e31-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51e31-131">id</span><span class="sxs-lookup"><span data-stu-id="51e31-131">id</span></span>|<span data-ttu-id="51e31-132">字符串</span><span class="sxs-lookup"><span data-stu-id="51e31-132">String</span></span>|<span data-ttu-id="51e31-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="51e31-133">Key of the entity.</span></span> <span data-ttu-id="51e31-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51e31-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e31-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51e31-135">lastModifiedDateTime</span></span>|<span data-ttu-id="51e31-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51e31-136">DateTimeOffset</span></span>|<span data-ttu-id="51e31-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="51e31-137">DateTime the object was last modified.</span></span> <span data-ttu-id="51e31-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51e31-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e31-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51e31-139">createdDateTime</span></span>|<span data-ttu-id="51e31-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51e31-140">DateTimeOffset</span></span>|<span data-ttu-id="51e31-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="51e31-141">DateTime the object was created.</span></span> <span data-ttu-id="51e31-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51e31-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e31-143">description</span><span class="sxs-lookup"><span data-stu-id="51e31-143">description</span></span>|<span data-ttu-id="51e31-144">字符串</span><span class="sxs-lookup"><span data-stu-id="51e31-144">String</span></span>|<span data-ttu-id="51e31-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="51e31-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51e31-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51e31-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e31-147">displayName</span><span class="sxs-lookup"><span data-stu-id="51e31-147">displayName</span></span>|<span data-ttu-id="51e31-148">String</span><span class="sxs-lookup"><span data-stu-id="51e31-148">String</span></span>|<span data-ttu-id="51e31-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="51e31-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51e31-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51e31-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e31-151">version</span><span class="sxs-lookup"><span data-stu-id="51e31-151">version</span></span>|<span data-ttu-id="51e31-152">Int32</span><span class="sxs-lookup"><span data-stu-id="51e31-152">Int32</span></span>|<span data-ttu-id="51e31-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="51e31-153">Version of the device configuration.</span></span> <span data-ttu-id="51e31-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51e31-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51e31-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="51e31-155">payloadName</span></span>|<span data-ttu-id="51e31-156">String</span><span class="sxs-lookup"><span data-stu-id="51e31-156">String</span></span>|<span data-ttu-id="51e31-157">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="51e31-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="51e31-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="51e31-158">payloadFileName</span></span>|<span data-ttu-id="51e31-159">String</span><span class="sxs-lookup"><span data-stu-id="51e31-159">String</span></span>|<span data-ttu-id="51e31-160">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="51e31-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="51e31-161">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="51e31-161">\*.xml).</span></span>|
|<span data-ttu-id="51e31-162">payload</span><span class="sxs-lookup"><span data-stu-id="51e31-162">payload</span></span>|<span data-ttu-id="51e31-163">Binary</span><span class="sxs-lookup"><span data-stu-id="51e31-163">Binary</span></span>|<span data-ttu-id="51e31-164">有效负载。</span><span class="sxs-lookup"><span data-stu-id="51e31-164">Payload.</span></span> <span data-ttu-id="51e31-165">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="51e31-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="51e31-166">响应</span><span class="sxs-lookup"><span data-stu-id="51e31-166">Response</span></span>
<span data-ttu-id="51e31-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="51e31-167">If successful, this method returns a `200 OK` response code and an updated [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51e31-168">示例</span><span class="sxs-lookup"><span data-stu-id="51e31-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="51e31-169">请求</span><span class="sxs-lookup"><span data-stu-id="51e31-169">Request</span></span>
<span data-ttu-id="51e31-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="51e31-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51e31-171">响应</span><span class="sxs-lookup"><span data-stu-id="51e31-171">Response</span></span>
<span data-ttu-id="51e31-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51e31-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



