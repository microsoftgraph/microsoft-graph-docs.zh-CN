---
title: 创建 iosCustomConfiguration
description: 创建新的 iosCustomConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 2b445ae1e8025eb90426c51580890c765842b622
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328804"
---
# <a name="create-ioscustomconfiguration"></a><span data-ttu-id="00ea9-103">创建 iosCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="00ea9-103">Create iosCustomConfiguration</span></span>

> <span data-ttu-id="00ea9-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="00ea9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="00ea9-105">创建新的 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00ea9-105">Create a new [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="00ea9-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="00ea9-106">Prerequisites</span></span>
<span data-ttu-id="00ea9-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="00ea9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00ea9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="00ea9-109">Permission type</span></span>|<span data-ttu-id="00ea9-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="00ea9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00ea9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00ea9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="00ea9-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00ea9-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="00ea9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00ea9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00ea9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="00ea9-114">Not supported.</span></span>|
|<span data-ttu-id="00ea9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="00ea9-115">Application</span></span>|<span data-ttu-id="00ea9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="00ea9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="00ea9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00ea9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="00ea9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="00ea9-118">Request headers</span></span>
|<span data-ttu-id="00ea9-119">标头</span><span class="sxs-lookup"><span data-stu-id="00ea9-119">Header</span></span>|<span data-ttu-id="00ea9-120">值</span><span class="sxs-lookup"><span data-stu-id="00ea9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="00ea9-121">授权</span><span class="sxs-lookup"><span data-stu-id="00ea9-121">Authorization</span></span>|<span data-ttu-id="00ea9-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="00ea9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="00ea9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="00ea9-123">Accept</span></span>|<span data-ttu-id="00ea9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="00ea9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="00ea9-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="00ea9-125">Request body</span></span>
<span data-ttu-id="00ea9-126">在请求正文中，提供 iosCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00ea9-126">In the request body, supply a JSON representation for the iosCustomConfiguration object.</span></span>

<span data-ttu-id="00ea9-127">下表显示创建 iosCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="00ea9-127">The following table shows the properties that are required when you create the iosCustomConfiguration.</span></span>

|<span data-ttu-id="00ea9-128">属性</span><span class="sxs-lookup"><span data-stu-id="00ea9-128">Property</span></span>|<span data-ttu-id="00ea9-129">类型</span><span class="sxs-lookup"><span data-stu-id="00ea9-129">Type</span></span>|<span data-ttu-id="00ea9-130">说明</span><span class="sxs-lookup"><span data-stu-id="00ea9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="00ea9-131">id</span><span class="sxs-lookup"><span data-stu-id="00ea9-131">id</span></span>|<span data-ttu-id="00ea9-132">String</span><span class="sxs-lookup"><span data-stu-id="00ea9-132">String</span></span>|<span data-ttu-id="00ea9-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="00ea9-133">Key of the entity.</span></span> <span data-ttu-id="00ea9-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00ea9-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00ea9-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="00ea9-135">lastModifiedDateTime</span></span>|<span data-ttu-id="00ea9-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00ea9-136">DateTimeOffset</span></span>|<span data-ttu-id="00ea9-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="00ea9-137">DateTime the object was last modified.</span></span> <span data-ttu-id="00ea9-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00ea9-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00ea9-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="00ea9-139">createdDateTime</span></span>|<span data-ttu-id="00ea9-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="00ea9-140">DateTimeOffset</span></span>|<span data-ttu-id="00ea9-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="00ea9-141">DateTime the object was created.</span></span> <span data-ttu-id="00ea9-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00ea9-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00ea9-143">description</span><span class="sxs-lookup"><span data-stu-id="00ea9-143">description</span></span>|<span data-ttu-id="00ea9-144">String</span><span class="sxs-lookup"><span data-stu-id="00ea9-144">String</span></span>|<span data-ttu-id="00ea9-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="00ea9-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="00ea9-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00ea9-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00ea9-147">displayName</span><span class="sxs-lookup"><span data-stu-id="00ea9-147">displayName</span></span>|<span data-ttu-id="00ea9-148">String</span><span class="sxs-lookup"><span data-stu-id="00ea9-148">String</span></span>|<span data-ttu-id="00ea9-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="00ea9-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="00ea9-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00ea9-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00ea9-151">version</span><span class="sxs-lookup"><span data-stu-id="00ea9-151">version</span></span>|<span data-ttu-id="00ea9-152">Int32</span><span class="sxs-lookup"><span data-stu-id="00ea9-152">Int32</span></span>|<span data-ttu-id="00ea9-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="00ea9-153">Version of the device configuration.</span></span> <span data-ttu-id="00ea9-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="00ea9-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="00ea9-155">payloadName</span><span class="sxs-lookup"><span data-stu-id="00ea9-155">payloadName</span></span>|<span data-ttu-id="00ea9-156">String</span><span class="sxs-lookup"><span data-stu-id="00ea9-156">String</span></span>|<span data-ttu-id="00ea9-157">向用户显示的名称。</span><span class="sxs-lookup"><span data-stu-id="00ea9-157">Name that is displayed to the user.</span></span>|
|<span data-ttu-id="00ea9-158">payloadFileName</span><span class="sxs-lookup"><span data-stu-id="00ea9-158">payloadFileName</span></span>|<span data-ttu-id="00ea9-159">String</span><span class="sxs-lookup"><span data-stu-id="00ea9-159">String</span></span>|<span data-ttu-id="00ea9-160">有效负载文件名 (\*.mobileconfig</span><span class="sxs-lookup"><span data-stu-id="00ea9-160">Payload file name (\*.mobileconfig</span></span> | <span data-ttu-id="00ea9-161">\*.xml)。</span><span class="sxs-lookup"><span data-stu-id="00ea9-161">\*.xml).</span></span>|
|<span data-ttu-id="00ea9-162">payload</span><span class="sxs-lookup"><span data-stu-id="00ea9-162">payload</span></span>|<span data-ttu-id="00ea9-163">Binary</span><span class="sxs-lookup"><span data-stu-id="00ea9-163">Binary</span></span>|<span data-ttu-id="00ea9-164">有效负载。</span><span class="sxs-lookup"><span data-stu-id="00ea9-164">Payload.</span></span> <span data-ttu-id="00ea9-165">（UTF8 编码的字节数组）</span><span class="sxs-lookup"><span data-stu-id="00ea9-165">(UTF8 encoded byte array)</span></span>|



## <a name="response"></a><span data-ttu-id="00ea9-166">响应</span><span class="sxs-lookup"><span data-stu-id="00ea9-166">Response</span></span>
<span data-ttu-id="00ea9-167">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00ea9-167">If successful, this method returns a `201 Created` response code and a [iosCustomConfiguration](../resources/intune-deviceconfig-ioscustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="00ea9-168">示例</span><span class="sxs-lookup"><span data-stu-id="00ea9-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="00ea9-169">请求</span><span class="sxs-lookup"><span data-stu-id="00ea9-169">Request</span></span>
<span data-ttu-id="00ea9-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00ea9-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="00ea9-171">响应</span><span class="sxs-lookup"><span data-stu-id="00ea9-171">Response</span></span>
<span data-ttu-id="00ea9-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00ea9-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



