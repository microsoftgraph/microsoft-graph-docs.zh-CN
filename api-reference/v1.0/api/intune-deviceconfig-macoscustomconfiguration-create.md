---
title: 创建 macOSCustomConfiguration
description: 创建新的 macOSCustomConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7cbc27f253e095e8262a9bce48d16752fb2862fb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752677"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="e4daf-103">创建 macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="e4daf-103">Create macOSCustomConfiguration</span></span>

<span data-ttu-id="e4daf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4daf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4daf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4daf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4daf-106">创建新的 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4daf-106">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4daf-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4daf-107">Prerequisites</span></span>
<span data-ttu-id="e4daf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e4daf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e4daf-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4daf-110">Permission type</span></span>|<span data-ttu-id="e4daf-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e4daf-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4daf-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4daf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e4daf-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4daf-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4daf-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4daf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4daf-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4daf-115">Not supported.</span></span>|
|<span data-ttu-id="e4daf-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4daf-116">Application</span></span>|<span data-ttu-id="e4daf-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4daf-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4daf-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4daf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e4daf-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4daf-119">Request headers</span></span>
|<span data-ttu-id="e4daf-120">标头</span><span class="sxs-lookup"><span data-stu-id="e4daf-120">Header</span></span>|<span data-ttu-id="e4daf-121">值</span><span class="sxs-lookup"><span data-stu-id="e4daf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4daf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4daf-122">Authorization</span></span>|<span data-ttu-id="e4daf-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4daf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4daf-124">接受</span><span class="sxs-lookup"><span data-stu-id="e4daf-124">Accept</span></span>|<span data-ttu-id="e4daf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e4daf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4daf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4daf-126">Request body</span></span>
<span data-ttu-id="e4daf-127">在请求正文中，提供 macOSCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4daf-127">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="e4daf-128">下表显示了创建 macOSCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4daf-128">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="e4daf-129">属性</span><span class="sxs-lookup"><span data-stu-id="e4daf-129">Property</span></span>|<span data-ttu-id="e4daf-130">类型</span><span class="sxs-lookup"><span data-stu-id="e4daf-130">Type</span></span>|<span data-ttu-id="e4daf-131">说明</span><span class="sxs-lookup"><span data-stu-id="e4daf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4daf-132">id</span><span class="sxs-lookup"><span data-stu-id="e4daf-132">id</span></span>|<span data-ttu-id="e4daf-133">String</span><span class="sxs-lookup"><span data-stu-id="e4daf-133">String</span></span>|<span data-ttu-id="e4daf-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e4daf-134">Key of the entity.</span></span> <span data-ttu-id="e4daf-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4daf-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4daf-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e4daf-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e4daf-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4daf-137">DateTimeOffset</span></span>|<span data-ttu-id="e4daf-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e4daf-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e4daf-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4daf-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4daf-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e4daf-140">createdDateTime</span></span>|<span data-ttu-id="e4daf-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4daf-141">DateTimeOffset</span></span>|<span data-ttu-id="e4daf-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e4daf-142">DateTime the object was created.</span></span> <span data-ttu-id="e4daf-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4daf-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4daf-144">说明</span><span class="sxs-lookup"><span data-stu-id="e4daf-144">description</span></span>|<span data-ttu-id="e4daf-145">String</span><span class="sxs-lookup"><span data-stu-id="e4daf-145">String</span></span>|<span data-ttu-id="e4daf-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="e4daf-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e4daf-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4daf-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4daf-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e4daf-148">displayName</span></span>|<span data-ttu-id="e4daf-149">String</span><span class="sxs-lookup"><span data-stu-id="e4daf-149">String</span></span>|<span data-ttu-id="e4daf-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e4daf-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e4daf-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4daf-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4daf-152">version</span><span class="sxs-lookup"><span data-stu-id="e4daf-152">version</span></span>|<span data-ttu-id="e4daf-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e4daf-153">Int32</span></span>|<span data-ttu-id="e4daf-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="e4daf-154">Version of the device configuration.</span></span> <span data-ttu-id="e4daf-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e4daf-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e4daf-156">payloadName</span><span class="sxs-lookup"><span data-stu-id="e4daf-156">payloadName</span></span>|<span data-ttu-id="e4daf-157">String</span><span class="sxs-lookup"><span data-stu-id="e4daf-157">String</span></span>|<span data-ttu-id="e4daf-158">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="e4daf-158">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="e4daf-159">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="e4daf-159">payloadFileName</span></span>|<span data-ttu-id="e4daf-160">String</span><span class="sxs-lookup"><span data-stu-id="e4daf-160">String</span></span>|<span data-ttu-id="e4daf-161">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="e4daf-161">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="e4daf-162">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="e4daf-162">\*.xml).</span></span>|
|<span data-ttu-id="e4daf-163">payload</span><span class="sxs-lookup"><span data-stu-id="e4daf-163">payload</span></span>|<span data-ttu-id="e4daf-164">Binary</span><span class="sxs-lookup"><span data-stu-id="e4daf-164">Binary</span></span>|<span data-ttu-id="e4daf-165">有效负载。</span><span class="sxs-lookup"><span data-stu-id="e4daf-165">Payload.</span></span> <span data-ttu-id="e4daf-166">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="e4daf-166">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="e4daf-167">响应</span><span class="sxs-lookup"><span data-stu-id="e4daf-167">Response</span></span>
<span data-ttu-id="e4daf-168">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e4daf-168">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4daf-169">示例</span><span class="sxs-lookup"><span data-stu-id="e4daf-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4daf-170">请求</span><span class="sxs-lookup"><span data-stu-id="e4daf-170">Request</span></span>
<span data-ttu-id="e4daf-171">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4daf-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4daf-172">响应</span><span class="sxs-lookup"><span data-stu-id="e4daf-172">Response</span></span>
<span data-ttu-id="e4daf-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4daf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




