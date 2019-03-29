---
title: 更新 macOSDeviceFeaturesConfiguration
description: 更新 macOSDeviceFeaturesConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3754eaa1018c92259b3b4136536151bc3850f633
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30961173"
---
# <a name="update-macosdevicefeaturesconfiguration"></a><span data-ttu-id="7dfc1-103">更新 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="7dfc1-103">Update macOSDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="7dfc1-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7dfc1-105">更新 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-105">Update the properties of a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7dfc1-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7dfc1-106">Prerequisites</span></span>
<span data-ttu-id="7dfc1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dfc1-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dfc1-109">Permission type</span></span>|<span data-ttu-id="7dfc1-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7dfc1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dfc1-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dfc1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7dfc1-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dfc1-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7dfc1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dfc1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dfc1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-114">Not supported.</span></span>|
|<span data-ttu-id="7dfc1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dfc1-115">Application</span></span>|<span data-ttu-id="7dfc1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dfc1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dfc1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="7dfc1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dfc1-118">Request headers</span></span>
|<span data-ttu-id="7dfc1-119">标头</span><span class="sxs-lookup"><span data-stu-id="7dfc1-119">Header</span></span>|<span data-ttu-id="7dfc1-120">值</span><span class="sxs-lookup"><span data-stu-id="7dfc1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dfc1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dfc1-121">Authorization</span></span>|<span data-ttu-id="7dfc1-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dfc1-123">接受</span><span class="sxs-lookup"><span data-stu-id="7dfc1-123">Accept</span></span>|<span data-ttu-id="7dfc1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7dfc1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dfc1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dfc1-125">Request body</span></span>
<span data-ttu-id="7dfc1-126">在请求正文中，提供 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-126">In the request body, supply a JSON representation for the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

<span data-ttu-id="7dfc1-127">下表显示创建 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-127">The following table shows the properties that are required when you create the [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md).</span></span>

|<span data-ttu-id="7dfc1-128">属性</span><span class="sxs-lookup"><span data-stu-id="7dfc1-128">Property</span></span>|<span data-ttu-id="7dfc1-129">类型</span><span class="sxs-lookup"><span data-stu-id="7dfc1-129">Type</span></span>|<span data-ttu-id="7dfc1-130">说明</span><span class="sxs-lookup"><span data-stu-id="7dfc1-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dfc1-131">id</span><span class="sxs-lookup"><span data-stu-id="7dfc1-131">id</span></span>|<span data-ttu-id="7dfc1-132">String</span><span class="sxs-lookup"><span data-stu-id="7dfc1-132">String</span></span>|<span data-ttu-id="7dfc1-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-133">Key of the entity.</span></span> <span data-ttu-id="7dfc1-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dfc1-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dfc1-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dfc1-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7dfc1-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dfc1-136">DateTimeOffset</span></span>|<span data-ttu-id="7dfc1-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7dfc1-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dfc1-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dfc1-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dfc1-139">createdDateTime</span></span>|<span data-ttu-id="7dfc1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dfc1-140">DateTimeOffset</span></span>|<span data-ttu-id="7dfc1-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-141">DateTime the object was created.</span></span> <span data-ttu-id="7dfc1-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dfc1-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dfc1-143">description</span><span class="sxs-lookup"><span data-stu-id="7dfc1-143">description</span></span>|<span data-ttu-id="7dfc1-144">String</span><span class="sxs-lookup"><span data-stu-id="7dfc1-144">String</span></span>|<span data-ttu-id="7dfc1-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7dfc1-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dfc1-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dfc1-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7dfc1-147">displayName</span></span>|<span data-ttu-id="7dfc1-148">String</span><span class="sxs-lookup"><span data-stu-id="7dfc1-148">String</span></span>|<span data-ttu-id="7dfc1-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7dfc1-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dfc1-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dfc1-151">version</span><span class="sxs-lookup"><span data-stu-id="7dfc1-151">version</span></span>|<span data-ttu-id="7dfc1-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7dfc1-152">Int32</span></span>|<span data-ttu-id="7dfc1-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-153">Version of the device configuration.</span></span> <span data-ttu-id="7dfc1-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dfc1-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="7dfc1-155">响应</span><span class="sxs-lookup"><span data-stu-id="7dfc1-155">Response</span></span>
<span data-ttu-id="7dfc1-156">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-156">If successful, this method returns a `200 OK` response code and an updated [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dfc1-157">示例</span><span class="sxs-lookup"><span data-stu-id="7dfc1-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="7dfc1-158">请求</span><span class="sxs-lookup"><span data-stu-id="7dfc1-158">Request</span></span>
<span data-ttu-id="7dfc1-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 170

{
  "@odata.type": "#microsoft.graph.macOSDeviceFeaturesConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="7dfc1-160">响应</span><span class="sxs-lookup"><span data-stu-id="7dfc1-160">Response</span></span>
<span data-ttu-id="7dfc1-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7dfc1-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



