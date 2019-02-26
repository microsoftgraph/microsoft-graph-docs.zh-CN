---
title: 更新 windowsPhone81CustomConfiguration
description: 更新 windowsPhone81CustomConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d9c14408373f735e1b9624895cb4392078f51842
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30257748"
---
# <a name="update-windowsphone81customconfiguration"></a><span data-ttu-id="4eeaf-103">更新 windowsPhone81CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="4eeaf-103">Update windowsPhone81CustomConfiguration</span></span>

> <span data-ttu-id="4eeaf-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4eeaf-105">更新 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-105">Update the properties of a [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4eeaf-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="4eeaf-106">Prerequisites</span></span>
<span data-ttu-id="4eeaf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4eeaf-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4eeaf-109">Permission type</span></span>|<span data-ttu-id="4eeaf-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4eeaf-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4eeaf-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4eeaf-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4eeaf-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4eeaf-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4eeaf-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4eeaf-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4eeaf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-114">Not supported.</span></span>|
|<span data-ttu-id="4eeaf-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4eeaf-115">Application</span></span>|<span data-ttu-id="4eeaf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4eeaf-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4eeaf-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="4eeaf-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4eeaf-118">Request headers</span></span>
|<span data-ttu-id="4eeaf-119">标头</span><span class="sxs-lookup"><span data-stu-id="4eeaf-119">Header</span></span>|<span data-ttu-id="4eeaf-120">值</span><span class="sxs-lookup"><span data-stu-id="4eeaf-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4eeaf-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4eeaf-121">Authorization</span></span>|<span data-ttu-id="4eeaf-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4eeaf-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4eeaf-123">Accept</span></span>|<span data-ttu-id="4eeaf-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4eeaf-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4eeaf-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4eeaf-125">Request body</span></span>
<span data-ttu-id="4eeaf-126">在请求正文中，提供 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-126">In the request body, supply a JSON representation for the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object.</span></span>

<span data-ttu-id="4eeaf-127">下表显示了创建 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-127">The following table shows the properties that are required when you create the [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md).</span></span>

|<span data-ttu-id="4eeaf-128">属性</span><span class="sxs-lookup"><span data-stu-id="4eeaf-128">Property</span></span>|<span data-ttu-id="4eeaf-129">类型</span><span class="sxs-lookup"><span data-stu-id="4eeaf-129">Type</span></span>|<span data-ttu-id="4eeaf-130">说明</span><span class="sxs-lookup"><span data-stu-id="4eeaf-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4eeaf-131">id</span><span class="sxs-lookup"><span data-stu-id="4eeaf-131">id</span></span>|<span data-ttu-id="4eeaf-132">String</span><span class="sxs-lookup"><span data-stu-id="4eeaf-132">String</span></span>|<span data-ttu-id="4eeaf-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-133">Key of the entity.</span></span> <span data-ttu-id="4eeaf-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeaf-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeaf-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4eeaf-135">lastModifiedDateTime</span></span>|<span data-ttu-id="4eeaf-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eeaf-136">DateTimeOffset</span></span>|<span data-ttu-id="4eeaf-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-137">DateTime the object was last modified.</span></span> <span data-ttu-id="4eeaf-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeaf-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeaf-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4eeaf-139">createdDateTime</span></span>|<span data-ttu-id="4eeaf-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4eeaf-140">DateTimeOffset</span></span>|<span data-ttu-id="4eeaf-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-141">DateTime the object was created.</span></span> <span data-ttu-id="4eeaf-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeaf-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeaf-143">description</span><span class="sxs-lookup"><span data-stu-id="4eeaf-143">description</span></span>|<span data-ttu-id="4eeaf-144">String</span><span class="sxs-lookup"><span data-stu-id="4eeaf-144">String</span></span>|<span data-ttu-id="4eeaf-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4eeaf-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeaf-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeaf-147">displayName</span><span class="sxs-lookup"><span data-stu-id="4eeaf-147">displayName</span></span>|<span data-ttu-id="4eeaf-148">String</span><span class="sxs-lookup"><span data-stu-id="4eeaf-148">String</span></span>|<span data-ttu-id="4eeaf-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4eeaf-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeaf-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeaf-151">version</span><span class="sxs-lookup"><span data-stu-id="4eeaf-151">version</span></span>|<span data-ttu-id="4eeaf-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4eeaf-152">Int32</span></span>|<span data-ttu-id="4eeaf-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-153">Version of the device configuration.</span></span> <span data-ttu-id="4eeaf-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4eeaf-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4eeaf-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="4eeaf-155">omaSettings</span></span>|<span data-ttu-id="4eeaf-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4eeaf-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="4eeaf-157">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-157">OMA settings.</span></span> <span data-ttu-id="4eeaf-158">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="4eeaf-159">响应</span><span class="sxs-lookup"><span data-stu-id="4eeaf-159">Response</span></span>
<span data-ttu-id="4eeaf-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-160">If successful, this method returns a `200 OK` response code and an updated [windowsPhone81CustomConfiguration](../resources/intune-deviceconfig-windowsphone81customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4eeaf-161">示例</span><span class="sxs-lookup"><span data-stu-id="4eeaf-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="4eeaf-162">请求</span><span class="sxs-lookup"><span data-stu-id="4eeaf-162">Request</span></span>
<span data-ttu-id="4eeaf-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="4eeaf-164">响应</span><span class="sxs-lookup"><span data-stu-id="4eeaf-164">Response</span></span>
<span data-ttu-id="4eeaf-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4eeaf-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



