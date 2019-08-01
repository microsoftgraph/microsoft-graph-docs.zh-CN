---
title: 更新 androidCustomConfiguration
description: 更新 androidCustomConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e82caa438c0c6a3813468f2d5ff5f097587a9672
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019650"
---
# <a name="update-androidcustomconfiguration"></a><span data-ttu-id="df8cc-103">更新 androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="df8cc-103">Update androidCustomConfiguration</span></span>

> <span data-ttu-id="df8cc-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df8cc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df8cc-105">更新 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="df8cc-105">Update the properties of a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df8cc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="df8cc-106">Prerequisites</span></span>
<span data-ttu-id="df8cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df8cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df8cc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="df8cc-109">Permission type</span></span>|<span data-ttu-id="df8cc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df8cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df8cc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df8cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="df8cc-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df8cc-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="df8cc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df8cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df8cc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="df8cc-114">Not supported.</span></span>|
|<span data-ttu-id="df8cc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="df8cc-115">Application</span></span>|<span data-ttu-id="df8cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df8cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df8cc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df8cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="df8cc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="df8cc-118">Request headers</span></span>
|<span data-ttu-id="df8cc-119">标头</span><span class="sxs-lookup"><span data-stu-id="df8cc-119">Header</span></span>|<span data-ttu-id="df8cc-120">值</span><span class="sxs-lookup"><span data-stu-id="df8cc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df8cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="df8cc-121">Authorization</span></span>|<span data-ttu-id="df8cc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df8cc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df8cc-123">接受</span><span class="sxs-lookup"><span data-stu-id="df8cc-123">Accept</span></span>|<span data-ttu-id="df8cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="df8cc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df8cc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="df8cc-125">Request body</span></span>
<span data-ttu-id="df8cc-126">在请求正文中，提供 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df8cc-126">In the request body, supply a JSON representation for the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>

<span data-ttu-id="df8cc-127">下表显示了创建 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="df8cc-127">The following table shows the properties that are required when you create the [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

|<span data-ttu-id="df8cc-128">属性</span><span class="sxs-lookup"><span data-stu-id="df8cc-128">Property</span></span>|<span data-ttu-id="df8cc-129">类型</span><span class="sxs-lookup"><span data-stu-id="df8cc-129">Type</span></span>|<span data-ttu-id="df8cc-130">说明</span><span class="sxs-lookup"><span data-stu-id="df8cc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="df8cc-131">id</span><span class="sxs-lookup"><span data-stu-id="df8cc-131">id</span></span>|<span data-ttu-id="df8cc-132">字符串</span><span class="sxs-lookup"><span data-stu-id="df8cc-132">String</span></span>|<span data-ttu-id="df8cc-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="df8cc-133">Key of the entity.</span></span> <span data-ttu-id="df8cc-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df8cc-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df8cc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="df8cc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="df8cc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df8cc-136">DateTimeOffset</span></span>|<span data-ttu-id="df8cc-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df8cc-137">DateTime the object was last modified.</span></span> <span data-ttu-id="df8cc-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df8cc-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df8cc-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="df8cc-139">createdDateTime</span></span>|<span data-ttu-id="df8cc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="df8cc-140">DateTimeOffset</span></span>|<span data-ttu-id="df8cc-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="df8cc-141">DateTime the object was created.</span></span> <span data-ttu-id="df8cc-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df8cc-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df8cc-143">说明</span><span class="sxs-lookup"><span data-stu-id="df8cc-143">description</span></span>|<span data-ttu-id="df8cc-144">String</span><span class="sxs-lookup"><span data-stu-id="df8cc-144">String</span></span>|<span data-ttu-id="df8cc-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="df8cc-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="df8cc-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df8cc-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df8cc-147">displayName</span><span class="sxs-lookup"><span data-stu-id="df8cc-147">displayName</span></span>|<span data-ttu-id="df8cc-148">String</span><span class="sxs-lookup"><span data-stu-id="df8cc-148">String</span></span>|<span data-ttu-id="df8cc-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="df8cc-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="df8cc-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df8cc-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df8cc-151">version</span><span class="sxs-lookup"><span data-stu-id="df8cc-151">version</span></span>|<span data-ttu-id="df8cc-152">Int32</span><span class="sxs-lookup"><span data-stu-id="df8cc-152">Int32</span></span>|<span data-ttu-id="df8cc-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="df8cc-153">Version of the device configuration.</span></span> <span data-ttu-id="df8cc-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="df8cc-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="df8cc-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="df8cc-155">omaSettings</span></span>|<span data-ttu-id="df8cc-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="df8cc-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="df8cc-157">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="df8cc-157">OMA settings.</span></span> <span data-ttu-id="df8cc-158">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="df8cc-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="df8cc-159">响应</span><span class="sxs-lookup"><span data-stu-id="df8cc-159">Response</span></span>
<span data-ttu-id="df8cc-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df8cc-160">If successful, this method returns a `200 OK` response code and an updated [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df8cc-161">示例</span><span class="sxs-lookup"><span data-stu-id="df8cc-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="df8cc-162">请求</span><span class="sxs-lookup"><span data-stu-id="df8cc-162">Request</span></span>
<span data-ttu-id="df8cc-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df8cc-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 402

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="df8cc-164">响应</span><span class="sxs-lookup"><span data-stu-id="df8cc-164">Response</span></span>
<span data-ttu-id="df8cc-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df8cc-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.androidCustomConfiguration",
  "id": "619b5e6d-5e6d-619b-6d5e-9b616d5e9b61",
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



