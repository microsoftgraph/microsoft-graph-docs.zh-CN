---
title: 创建 windows10CustomConfiguration
description: 创建新的 windows10CustomConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7f0c06c078f2e1adb1089f997084555613a29c7d
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756209"
---
# <a name="create-windows10customconfiguration"></a><span data-ttu-id="8b00c-103">创建 windows10CustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="8b00c-103">Create windows10CustomConfiguration</span></span>

<span data-ttu-id="8b00c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b00c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b00c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b00c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b00c-106">创建新的 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b00c-106">Create a new [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b00c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8b00c-107">Prerequisites</span></span>
<span data-ttu-id="8b00c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b00c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b00c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b00c-110">Permission type</span></span>|<span data-ttu-id="8b00c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8b00c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b00c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b00c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b00c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b00c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8b00c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b00c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b00c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b00c-115">Not supported.</span></span>|
|<span data-ttu-id="8b00c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b00c-116">Application</span></span>|<span data-ttu-id="8b00c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b00c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b00c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b00c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="8b00c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b00c-119">Request headers</span></span>
|<span data-ttu-id="8b00c-120">标头</span><span class="sxs-lookup"><span data-stu-id="8b00c-120">Header</span></span>|<span data-ttu-id="8b00c-121">值</span><span class="sxs-lookup"><span data-stu-id="8b00c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b00c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b00c-122">Authorization</span></span>|<span data-ttu-id="8b00c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8b00c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b00c-124">接受</span><span class="sxs-lookup"><span data-stu-id="8b00c-124">Accept</span></span>|<span data-ttu-id="8b00c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b00c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b00c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b00c-126">Request body</span></span>
<span data-ttu-id="8b00c-127">在请求正文中，提供 windows10CustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b00c-127">In the request body, supply a JSON representation for the windows10CustomConfiguration object.</span></span>

<span data-ttu-id="8b00c-128">下表显示了创建 windows10CustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8b00c-128">The following table shows the properties that are required when you create the windows10CustomConfiguration.</span></span>

|<span data-ttu-id="8b00c-129">属性</span><span class="sxs-lookup"><span data-stu-id="8b00c-129">Property</span></span>|<span data-ttu-id="8b00c-130">类型</span><span class="sxs-lookup"><span data-stu-id="8b00c-130">Type</span></span>|<span data-ttu-id="8b00c-131">说明</span><span class="sxs-lookup"><span data-stu-id="8b00c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b00c-132">id</span><span class="sxs-lookup"><span data-stu-id="8b00c-132">id</span></span>|<span data-ttu-id="8b00c-133">String</span><span class="sxs-lookup"><span data-stu-id="8b00c-133">String</span></span>|<span data-ttu-id="8b00c-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8b00c-134">Key of the entity.</span></span> <span data-ttu-id="8b00c-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b00c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b00c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8b00c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="8b00c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b00c-137">DateTimeOffset</span></span>|<span data-ttu-id="8b00c-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8b00c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="8b00c-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b00c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b00c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8b00c-140">createdDateTime</span></span>|<span data-ttu-id="8b00c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8b00c-141">DateTimeOffset</span></span>|<span data-ttu-id="8b00c-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="8b00c-142">DateTime the object was created.</span></span> <span data-ttu-id="8b00c-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b00c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b00c-144">说明</span><span class="sxs-lookup"><span data-stu-id="8b00c-144">description</span></span>|<span data-ttu-id="8b00c-145">String</span><span class="sxs-lookup"><span data-stu-id="8b00c-145">String</span></span>|<span data-ttu-id="8b00c-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="8b00c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="8b00c-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b00c-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b00c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="8b00c-148">displayName</span></span>|<span data-ttu-id="8b00c-149">String</span><span class="sxs-lookup"><span data-stu-id="8b00c-149">String</span></span>|<span data-ttu-id="8b00c-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="8b00c-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="8b00c-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b00c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b00c-152">version</span><span class="sxs-lookup"><span data-stu-id="8b00c-152">version</span></span>|<span data-ttu-id="8b00c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="8b00c-153">Int32</span></span>|<span data-ttu-id="8b00c-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="8b00c-154">Version of the device configuration.</span></span> <span data-ttu-id="8b00c-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="8b00c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="8b00c-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="8b00c-156">omaSettings</span></span>|<span data-ttu-id="8b00c-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8b00c-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="8b00c-158">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="8b00c-158">OMA settings.</span></span> <span data-ttu-id="8b00c-159">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="8b00c-159">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="8b00c-160">响应</span><span class="sxs-lookup"><span data-stu-id="8b00c-160">Response</span></span>
<span data-ttu-id="8b00c-161">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8b00c-161">If successful, this method returns a `201 Created` response code and a [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b00c-162">示例</span><span class="sxs-lookup"><span data-stu-id="8b00c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b00c-163">请求</span><span class="sxs-lookup"><span data-stu-id="8b00c-163">Request</span></span>
<span data-ttu-id="8b00c-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b00c-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 378

{
  "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "omaSettings": [
    {
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="8b00c-165">响应</span><span class="sxs-lookup"><span data-stu-id="8b00c-165">Response</span></span>
<span data-ttu-id="8b00c-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8b00c-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 550

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
      "@odata.type": "microsoft.graph.omaSetting",
      "displayName": "Display Name value",
      "description": "Description value",
      "omaUri": "Oma Uri value"
    }
  ]
}
```




