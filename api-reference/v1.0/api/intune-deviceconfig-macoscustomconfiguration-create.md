---
title: 创建 macOSCustomConfiguration
description: 创建新的 macOSCustomConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1e39435d63e48aca44ffde8a9c3cdaaa80a8b169
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961818"
---
# <a name="create-macoscustomconfiguration"></a><span data-ttu-id="d0dec-103">创建 macOSCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="d0dec-103">Create macOSCustomConfiguration</span></span>

> <span data-ttu-id="d0dec-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d0dec-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0dec-105">创建新的 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0dec-105">Create a new [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d0dec-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0dec-106">Prerequisites</span></span>
<span data-ttu-id="d0dec-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d0dec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0dec-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0dec-109">Permission type</span></span>|<span data-ttu-id="d0dec-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0dec-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0dec-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0dec-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d0dec-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0dec-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d0dec-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0dec-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0dec-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0dec-114">Not supported.</span></span>|
|<span data-ttu-id="d0dec-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0dec-115">Application</span></span>|<span data-ttu-id="d0dec-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0dec-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0dec-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0dec-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d0dec-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0dec-118">Request headers</span></span>
|<span data-ttu-id="d0dec-119">标头</span><span class="sxs-lookup"><span data-stu-id="d0dec-119">Header</span></span>|<span data-ttu-id="d0dec-120">值</span><span class="sxs-lookup"><span data-stu-id="d0dec-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0dec-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0dec-121">Authorization</span></span>|<span data-ttu-id="d0dec-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0dec-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0dec-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d0dec-123">Accept</span></span>|<span data-ttu-id="d0dec-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d0dec-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0dec-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0dec-125">Request body</span></span>
<span data-ttu-id="d0dec-126">在请求正文中，提供 macOSCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0dec-126">In the request body, supply a JSON representation for the macOSCustomConfiguration object.</span></span>

<span data-ttu-id="d0dec-127">下表显示了创建 macOSCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d0dec-127">The following table shows the properties that are required when you create the macOSCustomConfiguration.</span></span>

|<span data-ttu-id="d0dec-128">属性</span><span class="sxs-lookup"><span data-stu-id="d0dec-128">Property</span></span>|<span data-ttu-id="d0dec-129">类型</span><span class="sxs-lookup"><span data-stu-id="d0dec-129">Type</span></span>|<span data-ttu-id="d0dec-130">说明</span><span class="sxs-lookup"><span data-stu-id="d0dec-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0dec-131">id</span><span class="sxs-lookup"><span data-stu-id="d0dec-131">id</span></span>|<span data-ttu-id="d0dec-132">String</span><span class="sxs-lookup"><span data-stu-id="d0dec-132">String</span></span>|<span data-ttu-id="d0dec-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d0dec-133">Key of the entity.</span></span> <span data-ttu-id="d0dec-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0dec-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0dec-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d0dec-135">lastModifiedDateTime</span></span>|<span data-ttu-id="d0dec-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0dec-136">DateTimeOffset</span></span>|<span data-ttu-id="d0dec-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d0dec-137">DateTime the object was last modified.</span></span> <span data-ttu-id="d0dec-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0dec-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0dec-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d0dec-139">createdDateTime</span></span>|<span data-ttu-id="d0dec-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d0dec-140">DateTimeOffset</span></span>|<span data-ttu-id="d0dec-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="d0dec-141">DateTime the object was created.</span></span> <span data-ttu-id="d0dec-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0dec-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0dec-143">description</span><span class="sxs-lookup"><span data-stu-id="d0dec-143">description</span></span>|<span data-ttu-id="d0dec-144">String</span><span class="sxs-lookup"><span data-stu-id="d0dec-144">String</span></span>|<span data-ttu-id="d0dec-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="d0dec-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="d0dec-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0dec-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0dec-147">displayName</span><span class="sxs-lookup"><span data-stu-id="d0dec-147">displayName</span></span>|<span data-ttu-id="d0dec-148">String</span><span class="sxs-lookup"><span data-stu-id="d0dec-148">String</span></span>|<span data-ttu-id="d0dec-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="d0dec-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="d0dec-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0dec-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0dec-151">version</span><span class="sxs-lookup"><span data-stu-id="d0dec-151">version</span></span>|<span data-ttu-id="d0dec-152">Int32</span><span class="sxs-lookup"><span data-stu-id="d0dec-152">Int32</span></span>|<span data-ttu-id="d0dec-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="d0dec-153">Version of the device configuration.</span></span> <span data-ttu-id="d0dec-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="d0dec-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="d0dec-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="d0dec-155">payloadName</span></span>|<span data-ttu-id="d0dec-156">String</span><span class="sxs-lookup"><span data-stu-id="d0dec-156">String</span></span>|<span data-ttu-id="d0dec-157">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="d0dec-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="d0dec-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="d0dec-158">payloadFileName</span></span>|<span data-ttu-id="d0dec-159">String</span><span class="sxs-lookup"><span data-stu-id="d0dec-159">String</span></span>|<span data-ttu-id="d0dec-160">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="d0dec-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="d0dec-161">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="d0dec-161">\*.xml).</span></span>|
|<span data-ttu-id="d0dec-162">payload</span><span class="sxs-lookup"><span data-stu-id="d0dec-162">payload</span></span>|<span data-ttu-id="d0dec-163">Binary</span><span class="sxs-lookup"><span data-stu-id="d0dec-163">Binary</span></span>|<span data-ttu-id="d0dec-164">有效负载。</span><span class="sxs-lookup"><span data-stu-id="d0dec-164">Payload.</span></span> <span data-ttu-id="d0dec-165">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="d0dec-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="d0dec-166">响应</span><span class="sxs-lookup"><span data-stu-id="d0dec-166">Response</span></span>
<span data-ttu-id="d0dec-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0dec-167">If successful, this method returns a `201 Created` response code and a [macOSCustomConfiguration](../resources/intune-deviceconfig-macoscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0dec-168">示例</span><span class="sxs-lookup"><span data-stu-id="d0dec-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="d0dec-169">请求</span><span class="sxs-lookup"><span data-stu-id="d0dec-169">Request</span></span>
<span data-ttu-id="d0dec-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0dec-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d0dec-171">响应</span><span class="sxs-lookup"><span data-stu-id="d0dec-171">Response</span></span>
<span data-ttu-id="d0dec-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0dec-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



