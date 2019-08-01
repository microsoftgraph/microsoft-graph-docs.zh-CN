---
title: 创建 windowsPhone81CustomConfiguration
description: 创建新的 windowsPhone81CustomConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 815293d1fac3804a0fb8e02b8113984fcaf3f8d9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997118"
---
# <a name="create-windowsphone81customconfiguration"></a><span data-ttu-id="4b525-103">创建 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="4b525-103">Create windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="4b525-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b525-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b525-105">创建新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b525-105">Create a new [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4b525-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4b525-106">Prerequisites</span></span>
<span data-ttu-id="4b525-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4b525-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4b525-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4b525-109">Permission type</span></span>|<span data-ttu-id="4b525-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4b525-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4b525-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4b525-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4b525-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4b525-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4b525-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4b525-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4b525-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b525-114">Not supported.</span></span>|
|<span data-ttu-id="4b525-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4b525-115">Application</span></span>|<span data-ttu-id="4b525-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4b525-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4b525-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4b525-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4b525-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4b525-118">Request headers</span></span>
|<span data-ttu-id="4b525-119">标头</span><span class="sxs-lookup"><span data-stu-id="4b525-119">Header</span></span>|<span data-ttu-id="4b525-120">值</span><span class="sxs-lookup"><span data-stu-id="4b525-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4b525-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4b525-121">Authorization</span></span>|<span data-ttu-id="4b525-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4b525-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4b525-123">接受</span><span class="sxs-lookup"><span data-stu-id="4b525-123">Accept</span></span>|<span data-ttu-id="4b525-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4b525-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4b525-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4b525-125">Request body</span></span>
<span data-ttu-id="4b525-126">在请求正文中，提供 windowsPhone81CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4b525-126">In the request body, supply a JSON representation for the windowsPhone81CustomConfiguration object.</span></span>

<span data-ttu-id="4b525-127">下表显示了创建 windowsPhone81CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4b525-127">The following table shows the properties that are required when you create the windowsPhone81CustomConfiguration.</span></span>

|<span data-ttu-id="4b525-128">属性</span><span class="sxs-lookup"><span data-stu-id="4b525-128">Property</span></span>|<span data-ttu-id="4b525-129">类型</span><span class="sxs-lookup"><span data-stu-id="4b525-129">Type</span></span>|<span data-ttu-id="4b525-130">说明</span><span class="sxs-lookup"><span data-stu-id="4b525-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b525-131">id</span><span class="sxs-lookup"><span data-stu-id="4b525-131">id</span></span>|<span data-ttu-id="4b525-132">字符串</span><span class="sxs-lookup"><span data-stu-id="4b525-132">String</span></span>|<span data-ttu-id="4b525-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4b525-133">Key of the entity.</span></span> <span data-ttu-id="4b525-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b525-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b525-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4b525-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4b525-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b525-136">DateTimeOffset</span></span>|<span data-ttu-id="4b525-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4b525-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4b525-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b525-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b525-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4b525-139">createdDateTime</span></span>|<span data-ttu-id="4b525-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b525-140">DateTimeOffset</span></span>|<span data-ttu-id="4b525-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4b525-141">DateTime the object was created.</span></span> <span data-ttu-id="4b525-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b525-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b525-143">说明</span><span class="sxs-lookup"><span data-stu-id="4b525-143">description</span></span>|<span data-ttu-id="4b525-144">String</span><span class="sxs-lookup"><span data-stu-id="4b525-144">String</span></span>|<span data-ttu-id="4b525-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4b525-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4b525-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b525-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b525-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4b525-147">displayName</span></span>|<span data-ttu-id="4b525-148">String</span><span class="sxs-lookup"><span data-stu-id="4b525-148">String</span></span>|<span data-ttu-id="4b525-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4b525-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4b525-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b525-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b525-151">version</span><span class="sxs-lookup"><span data-stu-id="4b525-151">version</span></span>|<span data-ttu-id="4b525-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4b525-152">Int32</span></span>|<span data-ttu-id="4b525-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4b525-153">Version of the device configuration.</span></span> <span data-ttu-id="4b525-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4b525-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4b525-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="4b525-155">omaSettings</span></span>|<span data-ttu-id="4b525-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4b525-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="4b525-157">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="4b525-157">OMA settings.</span></span> <span data-ttu-id="4b525-158">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="4b525-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4b525-159">响应</span><span class="sxs-lookup"><span data-stu-id="4b525-159">Response</span></span>
<span data-ttu-id="4b525-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4b525-160">If successful, this method returns a `201 Created` response code and a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4b525-161">示例</span><span class="sxs-lookup"><span data-stu-id="4b525-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="4b525-162">请求</span><span class="sxs-lookup"><span data-stu-id="4b525-162">Request</span></span>
<span data-ttu-id="4b525-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4b525-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 409

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="4b525-164">响应</span><span class="sxs-lookup"><span data-stu-id="4b525-164">Response</span></span>
<span data-ttu-id="4b525-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4b525-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 581

{
  "@odata.type": "#microsoft.graph.windowsPhone81CustomConfiguration",
  "id": "0d98693c-693c-0d98-3c69-980d3c69980d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSettingInteger",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value",
      "value": 5
    }
  ]
}
```



