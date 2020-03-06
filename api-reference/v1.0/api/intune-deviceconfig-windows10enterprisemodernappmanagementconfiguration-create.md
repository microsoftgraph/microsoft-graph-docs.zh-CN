---
title: 创建 windows10EnterpriseModernAppManagementConfiguration
description: 创建新的 windows10EnterpriseModernAppManagementConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1a3545a308b670fdb46db3c931ac2bfab43d34a9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42514082"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="f3762-103">创建 windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="f3762-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="f3762-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3762-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3762-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3762-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3762-106">创建新的 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3762-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3762-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f3762-107">Prerequisites</span></span>
<span data-ttu-id="f3762-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3762-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3762-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3762-110">Permission type</span></span>|<span data-ttu-id="f3762-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f3762-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3762-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3762-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3762-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3762-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f3762-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3762-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3762-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3762-115">Not supported.</span></span>|
|<span data-ttu-id="f3762-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3762-116">Application</span></span>|<span data-ttu-id="f3762-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3762-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3762-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3762-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f3762-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3762-119">Request headers</span></span>
|<span data-ttu-id="f3762-120">标头</span><span class="sxs-lookup"><span data-stu-id="f3762-120">Header</span></span>|<span data-ttu-id="f3762-121">值</span><span class="sxs-lookup"><span data-stu-id="f3762-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3762-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3762-122">Authorization</span></span>|<span data-ttu-id="f3762-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f3762-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3762-124">接受</span><span class="sxs-lookup"><span data-stu-id="f3762-124">Accept</span></span>|<span data-ttu-id="f3762-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3762-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3762-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3762-126">Request body</span></span>
<span data-ttu-id="f3762-127">在请求正文中，提供 windows10EnterpriseModernAppManagementConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3762-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="f3762-128">下表显示创建 windows10EnterpriseModernAppManagementConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f3762-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="f3762-129">属性</span><span class="sxs-lookup"><span data-stu-id="f3762-129">Property</span></span>|<span data-ttu-id="f3762-130">类型</span><span class="sxs-lookup"><span data-stu-id="f3762-130">Type</span></span>|<span data-ttu-id="f3762-131">说明</span><span class="sxs-lookup"><span data-stu-id="f3762-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3762-132">id</span><span class="sxs-lookup"><span data-stu-id="f3762-132">id</span></span>|<span data-ttu-id="f3762-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f3762-133">String</span></span>|<span data-ttu-id="f3762-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f3762-134">Key of the entity.</span></span> <span data-ttu-id="f3762-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3762-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3762-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f3762-136">lastModifiedDateTime</span></span>|<span data-ttu-id="f3762-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3762-137">DateTimeOffset</span></span>|<span data-ttu-id="f3762-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f3762-138">DateTime the object was last modified.</span></span> <span data-ttu-id="f3762-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3762-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3762-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f3762-140">createdDateTime</span></span>|<span data-ttu-id="f3762-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3762-141">DateTimeOffset</span></span>|<span data-ttu-id="f3762-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="f3762-142">DateTime the object was created.</span></span> <span data-ttu-id="f3762-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3762-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3762-144">说明</span><span class="sxs-lookup"><span data-stu-id="f3762-144">description</span></span>|<span data-ttu-id="f3762-145">String</span><span class="sxs-lookup"><span data-stu-id="f3762-145">String</span></span>|<span data-ttu-id="f3762-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="f3762-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f3762-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3762-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3762-148">displayName</span><span class="sxs-lookup"><span data-stu-id="f3762-148">displayName</span></span>|<span data-ttu-id="f3762-149">String</span><span class="sxs-lookup"><span data-stu-id="f3762-149">String</span></span>|<span data-ttu-id="f3762-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="f3762-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f3762-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3762-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3762-152">version</span><span class="sxs-lookup"><span data-stu-id="f3762-152">version</span></span>|<span data-ttu-id="f3762-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f3762-153">Int32</span></span>|<span data-ttu-id="f3762-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="f3762-154">Version of the device configuration.</span></span> <span data-ttu-id="f3762-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f3762-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f3762-156">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="f3762-156">uninstallBuiltInApps</span></span>|<span data-ttu-id="f3762-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="f3762-157">Boolean</span></span>|<span data-ttu-id="f3762-158">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="f3762-158">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="f3762-159">响应</span><span class="sxs-lookup"><span data-stu-id="f3762-159">Response</span></span>
<span data-ttu-id="f3762-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f3762-160">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f3762-161">示例</span><span class="sxs-lookup"><span data-stu-id="f3762-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3762-162">请求</span><span class="sxs-lookup"><span data-stu-id="f3762-162">Request</span></span>
<span data-ttu-id="f3762-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3762-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="f3762-164">响应</span><span class="sxs-lookup"><span data-stu-id="f3762-164">Response</span></span>
<span data-ttu-id="f3762-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3762-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




