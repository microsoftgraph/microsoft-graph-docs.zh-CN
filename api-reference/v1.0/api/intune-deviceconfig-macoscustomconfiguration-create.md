---
title: 创建 macOSCustomConfiguration
description: 创建新的 macOSCustomConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 90583d103211f374ed761813a033000546fbc036
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514394"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="d6b36-103">创建 macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d6b36-103">Create macOSCustomConfiguration</span></span>

<span data-ttu-id="d6b36-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6b36-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d6b36-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6b36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6b36-106">创建新的 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6b36-106">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6b36-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6b36-107">Prerequisites</span></span>
<span data-ttu-id="d6b36-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6b36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6b36-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6b36-110">Permission type</span></span>|<span data-ttu-id="d6b36-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d6b36-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6b36-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6b36-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6b36-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6b36-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6b36-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6b36-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6b36-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6b36-115">Not supported.</span></span>|
|<span data-ttu-id="d6b36-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6b36-116">Application</span></span>|<span data-ttu-id="d6b36-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6b36-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6b36-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6b36-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d6b36-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6b36-119">Request headers</span></span>
|<span data-ttu-id="d6b36-120">标头</span><span class="sxs-lookup"><span data-stu-id="d6b36-120">Header</span></span>|<span data-ttu-id="d6b36-121">值</span><span class="sxs-lookup"><span data-stu-id="d6b36-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6b36-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6b36-122">Authorization</span></span>|<span data-ttu-id="d6b36-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6b36-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6b36-124">接受</span><span class="sxs-lookup"><span data-stu-id="d6b36-124">Accept</span></span>|<span data-ttu-id="d6b36-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6b36-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6b36-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6b36-126">Request body</span></span>
<span data-ttu-id="d6b36-127">在请求正文中，提供 macOSCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6b36-127">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="d6b36-128">下表显示了创建 macOSCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d6b36-128">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="d6b36-129">属性</span><span class="sxs-lookup"><span data-stu-id="d6b36-129">Property</span></span>|<span data-ttu-id="d6b36-130">类型</span><span class="sxs-lookup"><span data-stu-id="d6b36-130">Type</span></span>|<span data-ttu-id="d6b36-131">说明</span><span class="sxs-lookup"><span data-stu-id="d6b36-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6b36-132">id</span><span class="sxs-lookup"><span data-stu-id="d6b36-132">id</span></span>|<span data-ttu-id="d6b36-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d6b36-133">String</span></span>|<span data-ttu-id="d6b36-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d6b36-134">Key of the entity.</span></span> <span data-ttu-id="d6b36-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6b36-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6b36-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6b36-136">lastModifiedDateTime</span></span>|<span data-ttu-id="d6b36-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6b36-137">DateTimeOffset</span></span>|<span data-ttu-id="d6b36-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d6b36-138">DateTime the object was last modified.</span></span> <span data-ttu-id="d6b36-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6b36-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6b36-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6b36-140">createdDateTime</span></span>|<span data-ttu-id="d6b36-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6b36-141">DateTimeOffset</span></span>|<span data-ttu-id="d6b36-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d6b36-142">DateTime the object was created.</span></span> <span data-ttu-id="d6b36-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6b36-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6b36-144">说明</span><span class="sxs-lookup"><span data-stu-id="d6b36-144">description</span></span>|<span data-ttu-id="d6b36-145">String</span><span class="sxs-lookup"><span data-stu-id="d6b36-145">String</span></span>|<span data-ttu-id="d6b36-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d6b36-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d6b36-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6b36-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6b36-148">displayName</span><span class="sxs-lookup"><span data-stu-id="d6b36-148">displayName</span></span>|<span data-ttu-id="d6b36-149">字符串</span><span class="sxs-lookup"><span data-stu-id="d6b36-149">String</span></span>|<span data-ttu-id="d6b36-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d6b36-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d6b36-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6b36-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6b36-152">version</span><span class="sxs-lookup"><span data-stu-id="d6b36-152">version</span></span>|<span data-ttu-id="d6b36-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d6b36-153">Int32</span></span>|<span data-ttu-id="d6b36-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d6b36-154">Version of the device configuration.</span></span> <span data-ttu-id="d6b36-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d6b36-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d6b36-156">payloadName</span><span class="sxs-lookup"><span data-stu-id="d6b36-156">payloadName</span></span>|<span data-ttu-id="d6b36-157">字符串</span><span class="sxs-lookup"><span data-stu-id="d6b36-157">String</span></span>|<span data-ttu-id="d6b36-158">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="d6b36-158">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="d6b36-159">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d6b36-159">payloadFileName</span></span>|<span data-ttu-id="d6b36-160">String</span><span class="sxs-lookup"><span data-stu-id="d6b36-160">String</span></span>|<span data-ttu-id="d6b36-161">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="d6b36-161">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="d6b36-162">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="d6b36-162">\*.xml).</span></span>|
|<span data-ttu-id="d6b36-163">payload</span><span class="sxs-lookup"><span data-stu-id="d6b36-163">payload</span></span>|<span data-ttu-id="d6b36-164">Binary</span><span class="sxs-lookup"><span data-stu-id="d6b36-164">Binary</span></span>|<span data-ttu-id="d6b36-165">有效负载。</span><span class="sxs-lookup"><span data-stu-id="d6b36-165">Payload.</span></span> <span data-ttu-id="d6b36-166">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="d6b36-166">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="d6b36-167">响应</span><span class="sxs-lookup"><span data-stu-id="d6b36-167">Response</span></span>
<span data-ttu-id="d6b36-168">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d6b36-168">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6b36-169">示例</span><span class="sxs-lookup"><span data-stu-id="d6b36-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6b36-170">请求</span><span class="sxs-lookup"><span data-stu-id="d6b36-170">Request</span></span>
<span data-ttu-id="d6b36-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6b36-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="d6b36-172">响应</span><span class="sxs-lookup"><span data-stu-id="d6b36-172">Response</span></span>
<span data-ttu-id="d6b36-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6b36-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




