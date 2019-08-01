---
title: 创建 windows10CustomConfiguration
description: 创建新的 windows10CustomConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f96011e85d155ca1b40249cc46359a82975a5d6e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36016928"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="a188c-103">创建 windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="a188c-103">Create windows10CustomConfiguration</span></span>

> <span data-ttu-id="a188c-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a188c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a188c-105">创建新的 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a188c-105">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a188c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a188c-106">Prerequisites</span></span>
<span data-ttu-id="a188c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a188c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a188c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a188c-109">Permission type</span></span>|<span data-ttu-id="a188c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a188c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a188c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a188c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a188c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a188c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a188c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a188c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a188c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a188c-114">Not supported.</span></span>|
|<span data-ttu-id="a188c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a188c-115">Application</span></span>|<span data-ttu-id="a188c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a188c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a188c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a188c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a188c-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a188c-118">Request headers</span></span>
|<span data-ttu-id="a188c-119">标头</span><span class="sxs-lookup"><span data-stu-id="a188c-119">Header</span></span>|<span data-ttu-id="a188c-120">值</span><span class="sxs-lookup"><span data-stu-id="a188c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a188c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a188c-121">Authorization</span></span>|<span data-ttu-id="a188c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a188c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a188c-123">接受</span><span class="sxs-lookup"><span data-stu-id="a188c-123">Accept</span></span>|<span data-ttu-id="a188c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a188c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a188c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a188c-125">Request body</span></span>
<span data-ttu-id="a188c-126">在请求正文中，提供 windows10CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a188c-126">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="a188c-127">下表显示了创建 windows10CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a188c-127">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="a188c-128">属性</span><span class="sxs-lookup"><span data-stu-id="a188c-128">Property</span></span>|<span data-ttu-id="a188c-129">类型</span><span class="sxs-lookup"><span data-stu-id="a188c-129">Type</span></span>|<span data-ttu-id="a188c-130">说明</span><span class="sxs-lookup"><span data-stu-id="a188c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a188c-131">id</span><span class="sxs-lookup"><span data-stu-id="a188c-131">id</span></span>|<span data-ttu-id="a188c-132">字符串</span><span class="sxs-lookup"><span data-stu-id="a188c-132">String</span></span>|<span data-ttu-id="a188c-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a188c-133">Key of the entity.</span></span> <span data-ttu-id="a188c-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a188c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a188c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a188c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="a188c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a188c-136">DateTimeOffset</span></span>|<span data-ttu-id="a188c-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a188c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="a188c-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a188c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a188c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a188c-139">createdDateTime</span></span>|<span data-ttu-id="a188c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a188c-140">DateTimeOffset</span></span>|<span data-ttu-id="a188c-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a188c-141">DateTime the object was created.</span></span> <span data-ttu-id="a188c-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a188c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a188c-143">说明</span><span class="sxs-lookup"><span data-stu-id="a188c-143">description</span></span>|<span data-ttu-id="a188c-144">String</span><span class="sxs-lookup"><span data-stu-id="a188c-144">String</span></span>|<span data-ttu-id="a188c-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a188c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a188c-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a188c-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a188c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="a188c-147">displayName</span></span>|<span data-ttu-id="a188c-148">String</span><span class="sxs-lookup"><span data-stu-id="a188c-148">String</span></span>|<span data-ttu-id="a188c-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a188c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a188c-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a188c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a188c-151">version</span><span class="sxs-lookup"><span data-stu-id="a188c-151">version</span></span>|<span data-ttu-id="a188c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="a188c-152">Int32</span></span>|<span data-ttu-id="a188c-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a188c-153">Version of the device configuration.</span></span> <span data-ttu-id="a188c-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a188c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a188c-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="a188c-155">omaSettings</span></span>|<span data-ttu-id="a188c-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a188c-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="a188c-157">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="a188c-157">OMA settings.</span></span> <span data-ttu-id="a188c-158">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="a188c-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="a188c-159">响应</span><span class="sxs-lookup"><span data-stu-id="a188c-159">Response</span></span>
<span data-ttu-id="a188c-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a188c-160">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a188c-161">示例</span><span class="sxs-lookup"><span data-stu-id="a188c-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="a188c-162">请求</span><span class="sxs-lookup"><span data-stu-id="a188c-162">Request</span></span>
<span data-ttu-id="a188c-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a188c-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 404

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="a188c-164">响应</span><span class="sxs-lookup"><span data-stu-id="a188c-164">Response</span></span>
<span data-ttu-id="a188c-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a188c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 576

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
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



