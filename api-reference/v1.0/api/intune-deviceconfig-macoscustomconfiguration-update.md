---
title: 更新 macOSCustomConfiguration
description: 更新 macOSCustomConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a009d87943343c0ca918f49bdd4efb489bfc575b
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366004"
---
# <a name="update-macoscustomconfiguration"></a><span data-ttu-id="8fdcd-103">更新 macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="8fdcd-103">Update macOSCustomConfiguration</span></span>

> <span data-ttu-id="8fdcd-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fdcd-105">更新 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-105">Update the properties of a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fdcd-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="8fdcd-106">Prerequisites</span></span>
<span data-ttu-id="8fdcd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fdcd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8fdcd-109">Permission type</span></span>|<span data-ttu-id="8fdcd-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8fdcd-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fdcd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8fdcd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8fdcd-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fdcd-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8fdcd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8fdcd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fdcd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-114">Not supported.</span></span>|
|<span data-ttu-id="8fdcd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8fdcd-115">Application</span></span>|<span data-ttu-id="8fdcd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fdcd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8fdcd-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="8fdcd-118">请求头</span><span class="sxs-lookup"><span data-stu-id="8fdcd-118">Request headers</span></span>
|<span data-ttu-id="8fdcd-119">标头</span><span class="sxs-lookup"><span data-stu-id="8fdcd-119">Header</span></span>|<span data-ttu-id="8fdcd-120">值</span><span class="sxs-lookup"><span data-stu-id="8fdcd-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fdcd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fdcd-121">Authorization</span></span>|<span data-ttu-id="8fdcd-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fdcd-123">接受</span><span class="sxs-lookup"><span data-stu-id="8fdcd-123">Accept</span></span>|<span data-ttu-id="8fdcd-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8fdcd-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fdcd-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8fdcd-125">Request body</span></span>
<span data-ttu-id="8fdcd-126">在请求正文中，提供 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-126">In the request body, supply a JSON representation for the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

<span data-ttu-id="8fdcd-127">下表显示了创建 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-127">The following table shows the properties that are required when you create the [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md).</span></span>

|<span data-ttu-id="8fdcd-128">属性</span><span class="sxs-lookup"><span data-stu-id="8fdcd-128">Property</span></span>|<span data-ttu-id="8fdcd-129">类型</span><span class="sxs-lookup"><span data-stu-id="8fdcd-129">Type</span></span>|<span data-ttu-id="8fdcd-130">说明</span><span class="sxs-lookup"><span data-stu-id="8fdcd-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fdcd-131">id</span><span class="sxs-lookup"><span data-stu-id="8fdcd-131">id</span></span>|<span data-ttu-id="8fdcd-132">字符串</span><span class="sxs-lookup"><span data-stu-id="8fdcd-132">String</span></span>|<span data-ttu-id="8fdcd-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-133">Key of the entity.</span></span> <span data-ttu-id="8fdcd-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fdcd-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fdcd-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8fdcd-135">lastModifiedDateTime</span></span>|<span data-ttu-id="8fdcd-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fdcd-136">DateTimeOffset</span></span>|<span data-ttu-id="8fdcd-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-137">DateTime the object was last modified.</span></span> <span data-ttu-id="8fdcd-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fdcd-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fdcd-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8fdcd-139">createdDateTime</span></span>|<span data-ttu-id="8fdcd-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8fdcd-140">DateTimeOffset</span></span>|<span data-ttu-id="8fdcd-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-141">DateTime the object was created.</span></span> <span data-ttu-id="8fdcd-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fdcd-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fdcd-143">说明</span><span class="sxs-lookup"><span data-stu-id="8fdcd-143">description</span></span>|<span data-ttu-id="8fdcd-144">String</span><span class="sxs-lookup"><span data-stu-id="8fdcd-144">String</span></span>|<span data-ttu-id="8fdcd-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8fdcd-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fdcd-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fdcd-147">displayName</span><span class="sxs-lookup"><span data-stu-id="8fdcd-147">displayName</span></span>|<span data-ttu-id="8fdcd-148">字符串</span><span class="sxs-lookup"><span data-stu-id="8fdcd-148">String</span></span>|<span data-ttu-id="8fdcd-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8fdcd-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fdcd-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fdcd-151">version</span><span class="sxs-lookup"><span data-stu-id="8fdcd-151">version</span></span>|<span data-ttu-id="8fdcd-152">Int32</span><span class="sxs-lookup"><span data-stu-id="8fdcd-152">Int32</span></span>|<span data-ttu-id="8fdcd-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-153">Version of the device configuration.</span></span> <span data-ttu-id="8fdcd-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8fdcd-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8fdcd-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="8fdcd-155">payloadName</span></span>|<span data-ttu-id="8fdcd-156">String</span><span class="sxs-lookup"><span data-stu-id="8fdcd-156">String</span></span>|<span data-ttu-id="8fdcd-157">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="8fdcd-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="8fdcd-158">payloadFileName</span></span>|<span data-ttu-id="8fdcd-159">String</span><span class="sxs-lookup"><span data-stu-id="8fdcd-159">String</span></span>|<span data-ttu-id="8fdcd-160">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="8fdcd-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="8fdcd-161">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-161">\*.xml).</span></span>|
|<span data-ttu-id="8fdcd-162">payload</span><span class="sxs-lookup"><span data-stu-id="8fdcd-162">payload</span></span>|<span data-ttu-id="8fdcd-163">Binary</span><span class="sxs-lookup"><span data-stu-id="8fdcd-163">Binary</span></span>|<span data-ttu-id="8fdcd-164">有效负载。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-164">Payload.</span></span> <span data-ttu-id="8fdcd-165">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="8fdcd-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="8fdcd-166">响应</span><span class="sxs-lookup"><span data-stu-id="8fdcd-166">Response</span></span>
<span data-ttu-id="8fdcd-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-167">If successful, this method returns a `200 OK` response code and an updated [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fdcd-168">示例</span><span class="sxs-lookup"><span data-stu-id="8fdcd-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fdcd-169">请求</span><span class="sxs-lookup"><span data-stu-id="8fdcd-169">Request</span></span>
<span data-ttu-id="8fdcd-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 281

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "payloadName": "Payload Name value",
  "payloadFileName": "Payload File Name value",
  "payload": "cGF5bG9hZA=="
}
```

### <a name="response"></a><span data-ttu-id="8fdcd-171">响应</span><span class="sxs-lookup"><span data-stu-id="8fdcd-171">Response</span></span>
<span data-ttu-id="8fdcd-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8fdcd-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 453

{
  "@odata.type": "#microsoft.graph.macOSCustomConfiguration",
  "id": "a253835d-835d-a253-5d83-53a25d8353a2",
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




