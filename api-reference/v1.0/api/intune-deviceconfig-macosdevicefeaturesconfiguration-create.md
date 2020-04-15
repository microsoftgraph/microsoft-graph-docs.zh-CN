---
title: 创建 macOSDeviceFeaturesConfiguration
description: 创建新的 macOSDeviceFeaturesConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd9f79177adff2886f57bc3d8b288e5246ecaa77
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466000"
---
# <a name="create-macosdevicefeaturesconfiguration"></a><span data-ttu-id="a3b78-103">创建 macOSDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="a3b78-103">Create macOSDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="a3b78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3b78-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3b78-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3b78-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3b78-106">创建新的 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3b78-106">Create a new [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3b78-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3b78-107">Prerequisites</span></span>
<span data-ttu-id="a3b78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3b78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3b78-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3b78-110">Permission type</span></span>|<span data-ttu-id="a3b78-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a3b78-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3b78-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3b78-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a3b78-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3b78-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3b78-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3b78-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3b78-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3b78-115">Not supported.</span></span>|
|<span data-ttu-id="a3b78-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3b78-116">Application</span></span>|<span data-ttu-id="a3b78-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3b78-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3b78-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3b78-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a3b78-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3b78-119">Request headers</span></span>
|<span data-ttu-id="a3b78-120">标头</span><span class="sxs-lookup"><span data-stu-id="a3b78-120">Header</span></span>|<span data-ttu-id="a3b78-121">值</span><span class="sxs-lookup"><span data-stu-id="a3b78-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3b78-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3b78-122">Authorization</span></span>|<span data-ttu-id="a3b78-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a3b78-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3b78-124">接受</span><span class="sxs-lookup"><span data-stu-id="a3b78-124">Accept</span></span>|<span data-ttu-id="a3b78-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a3b78-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3b78-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3b78-126">Request body</span></span>
<span data-ttu-id="a3b78-127">在请求正文中，提供 macOSDeviceFeaturesConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3b78-127">In the request body, supply a JSON representation for the macOSDeviceFeaturesConfiguration object.</span></span>

<span data-ttu-id="a3b78-128">下表显示创建 macOSDeviceFeaturesConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a3b78-128">The following table shows the properties that are required when you create the macOSDeviceFeaturesConfiguration.</span></span>

|<span data-ttu-id="a3b78-129">属性</span><span class="sxs-lookup"><span data-stu-id="a3b78-129">Property</span></span>|<span data-ttu-id="a3b78-130">类型</span><span class="sxs-lookup"><span data-stu-id="a3b78-130">Type</span></span>|<span data-ttu-id="a3b78-131">说明</span><span class="sxs-lookup"><span data-stu-id="a3b78-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3b78-132">id</span><span class="sxs-lookup"><span data-stu-id="a3b78-132">id</span></span>|<span data-ttu-id="a3b78-133">字符串</span><span class="sxs-lookup"><span data-stu-id="a3b78-133">String</span></span>|<span data-ttu-id="a3b78-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a3b78-134">Key of the entity.</span></span> <span data-ttu-id="a3b78-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3b78-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b78-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3b78-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a3b78-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3b78-137">DateTimeOffset</span></span>|<span data-ttu-id="a3b78-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a3b78-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a3b78-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3b78-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b78-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3b78-140">createdDateTime</span></span>|<span data-ttu-id="a3b78-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3b78-141">DateTimeOffset</span></span>|<span data-ttu-id="a3b78-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a3b78-142">DateTime the object was created.</span></span> <span data-ttu-id="a3b78-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3b78-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b78-144">description</span><span class="sxs-lookup"><span data-stu-id="a3b78-144">description</span></span>|<span data-ttu-id="a3b78-145">String</span><span class="sxs-lookup"><span data-stu-id="a3b78-145">String</span></span>|<span data-ttu-id="a3b78-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a3b78-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3b78-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3b78-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b78-148">displayName</span><span class="sxs-lookup"><span data-stu-id="a3b78-148">displayName</span></span>|<span data-ttu-id="a3b78-149">String</span><span class="sxs-lookup"><span data-stu-id="a3b78-149">String</span></span>|<span data-ttu-id="a3b78-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a3b78-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3b78-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3b78-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3b78-152">version</span><span class="sxs-lookup"><span data-stu-id="a3b78-152">version</span></span>|<span data-ttu-id="a3b78-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a3b78-153">Int32</span></span>|<span data-ttu-id="a3b78-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a3b78-154">Version of the device configuration.</span></span> <span data-ttu-id="a3b78-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a3b78-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a3b78-156">响应</span><span class="sxs-lookup"><span data-stu-id="a3b78-156">Response</span></span>
<span data-ttu-id="a3b78-157">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3b78-157">If successful, this method returns a `201 Created` response code and a [macOSDeviceFeaturesConfiguration](../resources/intune-deviceconfig-macosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3b78-158">示例</span><span class="sxs-lookup"><span data-stu-id="a3b78-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3b78-159">请求</span><span class="sxs-lookup"><span data-stu-id="a3b78-159">Request</span></span>
<span data-ttu-id="a3b78-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3b78-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a3b78-161">响应</span><span class="sxs-lookup"><span data-stu-id="a3b78-161">Response</span></span>
<span data-ttu-id="a3b78-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a3b78-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






