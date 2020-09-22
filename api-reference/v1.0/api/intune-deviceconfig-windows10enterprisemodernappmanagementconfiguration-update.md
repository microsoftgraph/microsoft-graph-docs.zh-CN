---
title: 更新 windows10EnterpriseModernAppManagementConfiguration
description: 更新 windows10EnterpriseModernAppManagementConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 367ddbac53e18440b589efce0f818cd1cb7b6882
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48066598"
---
# <a name="update-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="2d822-103">更新 windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="2d822-103">Update windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="2d822-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d822-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d822-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d822-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d822-106">更新 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2d822-106">Update the properties of a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d822-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d822-107">Prerequisites</span></span>
<span data-ttu-id="2d822-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d822-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d822-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d822-110">Permission type</span></span>|<span data-ttu-id="2d822-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2d822-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d822-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d822-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d822-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d822-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d822-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d822-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d822-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d822-115">Not supported.</span></span>|
|<span data-ttu-id="2d822-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d822-116">Application</span></span>|<span data-ttu-id="2d822-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d822-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d822-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d822-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2d822-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d822-119">Request headers</span></span>
|<span data-ttu-id="2d822-120">标头</span><span class="sxs-lookup"><span data-stu-id="2d822-120">Header</span></span>|<span data-ttu-id="2d822-121">值</span><span class="sxs-lookup"><span data-stu-id="2d822-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d822-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d822-122">Authorization</span></span>|<span data-ttu-id="2d822-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d822-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d822-124">接受</span><span class="sxs-lookup"><span data-stu-id="2d822-124">Accept</span></span>|<span data-ttu-id="2d822-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d822-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d822-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d822-126">Request body</span></span>
<span data-ttu-id="2d822-127">在请求正文中，提供 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d822-127">In the request body, supply a JSON representation for the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

<span data-ttu-id="2d822-128">下表显示创建 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2d822-128">The following table shows the properties that are required when you create the [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md).</span></span>

|<span data-ttu-id="2d822-129">属性</span><span class="sxs-lookup"><span data-stu-id="2d822-129">Property</span></span>|<span data-ttu-id="2d822-130">类型</span><span class="sxs-lookup"><span data-stu-id="2d822-130">Type</span></span>|<span data-ttu-id="2d822-131">说明</span><span class="sxs-lookup"><span data-stu-id="2d822-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d822-132">id</span><span class="sxs-lookup"><span data-stu-id="2d822-132">id</span></span>|<span data-ttu-id="2d822-133">String</span><span class="sxs-lookup"><span data-stu-id="2d822-133">String</span></span>|<span data-ttu-id="2d822-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2d822-134">Key of the entity.</span></span> <span data-ttu-id="2d822-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d822-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d822-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d822-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2d822-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d822-137">DateTimeOffset</span></span>|<span data-ttu-id="2d822-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2d822-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2d822-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d822-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d822-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d822-140">createdDateTime</span></span>|<span data-ttu-id="2d822-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d822-141">DateTimeOffset</span></span>|<span data-ttu-id="2d822-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2d822-142">DateTime the object was created.</span></span> <span data-ttu-id="2d822-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d822-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d822-144">description</span><span class="sxs-lookup"><span data-stu-id="2d822-144">description</span></span>|<span data-ttu-id="2d822-145">String</span><span class="sxs-lookup"><span data-stu-id="2d822-145">String</span></span>|<span data-ttu-id="2d822-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2d822-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d822-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d822-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d822-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2d822-148">displayName</span></span>|<span data-ttu-id="2d822-149">String</span><span class="sxs-lookup"><span data-stu-id="2d822-149">String</span></span>|<span data-ttu-id="2d822-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2d822-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d822-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d822-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d822-152">version</span><span class="sxs-lookup"><span data-stu-id="2d822-152">version</span></span>|<span data-ttu-id="2d822-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2d822-153">Int32</span></span>|<span data-ttu-id="2d822-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2d822-154">Version of the device configuration.</span></span> <span data-ttu-id="2d822-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d822-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d822-156">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="2d822-156">uninstallBuiltInApps</span></span>|<span data-ttu-id="2d822-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="2d822-157">Boolean</span></span>|<span data-ttu-id="2d822-158">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="2d822-158">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="2d822-159">响应</span><span class="sxs-lookup"><span data-stu-id="2d822-159">Response</span></span>
<span data-ttu-id="2d822-160">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2d822-160">If successful, this method returns a `200 OK` response code and an updated [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d822-161">示例</span><span class="sxs-lookup"><span data-stu-id="2d822-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d822-162">请求</span><span class="sxs-lookup"><span data-stu-id="2d822-162">Request</span></span>
<span data-ttu-id="2d822-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d822-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 222

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```

### <a name="response"></a><span data-ttu-id="2d822-164">响应</span><span class="sxs-lookup"><span data-stu-id="2d822-164">Response</span></span>
<span data-ttu-id="2d822-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d822-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 394

{
  "@odata.type": "#microsoft.graph.windows10EnterpriseModernAppManagementConfiguration",
  "id": "d6577687-7687-d657-8776-57d6877657d6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "uninstallBuiltInApps": true
}
```









