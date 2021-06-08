---
title: 创建 windows10EnterpriseModernAppManagementConfiguration
description: 创建新的 windows10EnterpriseModernAppManagementConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d24727218a61ba03302857e9a3b079a0e40d876
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52760543"
---
# <a name="create-windows10enterprisemodernappmanagementconfiguration"></a><span data-ttu-id="adadb-103">创建 windows10EnterpriseModernAppManagementConfiguration</span><span class="sxs-lookup"><span data-stu-id="adadb-103">Create windows10EnterpriseModernAppManagementConfiguration</span></span>

<span data-ttu-id="adadb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adadb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="adadb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="adadb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adadb-106">创建新的 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="adadb-106">Create a new [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adadb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="adadb-107">Prerequisites</span></span>
<span data-ttu-id="adadb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adadb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adadb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="adadb-110">Permission type</span></span>|<span data-ttu-id="adadb-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adadb-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adadb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adadb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="adadb-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adadb-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="adadb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adadb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adadb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="adadb-115">Not supported.</span></span>|
|<span data-ttu-id="adadb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="adadb-116">Application</span></span>|<span data-ttu-id="adadb-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adadb-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="adadb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adadb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="adadb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="adadb-119">Request headers</span></span>
|<span data-ttu-id="adadb-120">标头</span><span class="sxs-lookup"><span data-stu-id="adadb-120">Header</span></span>|<span data-ttu-id="adadb-121">值</span><span class="sxs-lookup"><span data-stu-id="adadb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adadb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="adadb-122">Authorization</span></span>|<span data-ttu-id="adadb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="adadb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adadb-124">接受</span><span class="sxs-lookup"><span data-stu-id="adadb-124">Accept</span></span>|<span data-ttu-id="adadb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="adadb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adadb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="adadb-126">Request body</span></span>
<span data-ttu-id="adadb-127">在请求正文中，提供 windows10EnterpriseModernAppManagementConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adadb-127">In the request body, supply a JSON representation for the windows10EnterpriseModernAppManagementConfiguration object.</span></span>

<span data-ttu-id="adadb-128">下表显示创建 windows10EnterpriseModernAppManagementConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="adadb-128">The following table shows the properties that are required when you create the windows10EnterpriseModernAppManagementConfiguration.</span></span>

|<span data-ttu-id="adadb-129">属性</span><span class="sxs-lookup"><span data-stu-id="adadb-129">Property</span></span>|<span data-ttu-id="adadb-130">类型</span><span class="sxs-lookup"><span data-stu-id="adadb-130">Type</span></span>|<span data-ttu-id="adadb-131">说明</span><span class="sxs-lookup"><span data-stu-id="adadb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="adadb-132">id</span><span class="sxs-lookup"><span data-stu-id="adadb-132">id</span></span>|<span data-ttu-id="adadb-133">String</span><span class="sxs-lookup"><span data-stu-id="adadb-133">String</span></span>|<span data-ttu-id="adadb-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="adadb-134">Key of the entity.</span></span> <span data-ttu-id="adadb-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adadb-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adadb-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="adadb-136">lastModifiedDateTime</span></span>|<span data-ttu-id="adadb-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adadb-137">DateTimeOffset</span></span>|<span data-ttu-id="adadb-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="adadb-138">DateTime the object was last modified.</span></span> <span data-ttu-id="adadb-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adadb-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adadb-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="adadb-140">createdDateTime</span></span>|<span data-ttu-id="adadb-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adadb-141">DateTimeOffset</span></span>|<span data-ttu-id="adadb-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="adadb-142">DateTime the object was created.</span></span> <span data-ttu-id="adadb-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adadb-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adadb-144">description</span><span class="sxs-lookup"><span data-stu-id="adadb-144">description</span></span>|<span data-ttu-id="adadb-145">String</span><span class="sxs-lookup"><span data-stu-id="adadb-145">String</span></span>|<span data-ttu-id="adadb-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="adadb-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="adadb-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adadb-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adadb-148">displayName</span><span class="sxs-lookup"><span data-stu-id="adadb-148">displayName</span></span>|<span data-ttu-id="adadb-149">String</span><span class="sxs-lookup"><span data-stu-id="adadb-149">String</span></span>|<span data-ttu-id="adadb-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="adadb-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="adadb-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adadb-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adadb-152">version</span><span class="sxs-lookup"><span data-stu-id="adadb-152">version</span></span>|<span data-ttu-id="adadb-153">Int32</span><span class="sxs-lookup"><span data-stu-id="adadb-153">Int32</span></span>|<span data-ttu-id="adadb-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="adadb-154">Version of the device configuration.</span></span> <span data-ttu-id="adadb-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="adadb-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="adadb-156">uninstallBuiltInApps</span><span class="sxs-lookup"><span data-stu-id="adadb-156">uninstallBuiltInApps</span></span>|<span data-ttu-id="adadb-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="adadb-157">Boolean</span></span>|<span data-ttu-id="adadb-158">指示是否卸载内置 Windows 应用的固定列表。</span><span class="sxs-lookup"><span data-stu-id="adadb-158">Indicates whether or not to uninstall a fixed list of built-in Windows apps.</span></span>|



## <a name="response"></a><span data-ttu-id="adadb-159">响应</span><span class="sxs-lookup"><span data-stu-id="adadb-159">Response</span></span>
<span data-ttu-id="adadb-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="adadb-160">If successful, this method returns a `201 Created` response code and a [windows10EnterpriseModernAppManagementConfiguration](../resources/intune-deviceconfig-windows10enterprisemodernappmanagementconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adadb-161">示例</span><span class="sxs-lookup"><span data-stu-id="adadb-161">Example</span></span>

### <a name="request"></a><span data-ttu-id="adadb-162">请求</span><span class="sxs-lookup"><span data-stu-id="adadb-162">Request</span></span>
<span data-ttu-id="adadb-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="adadb-163">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="adadb-164">响应</span><span class="sxs-lookup"><span data-stu-id="adadb-164">Response</span></span>
<span data-ttu-id="adadb-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="adadb-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




