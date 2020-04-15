---
title: 创建 androidWorkProfileCustomConfiguration
description: 创建新的 androidWorkProfileCustomConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 17d4c8c2c78b2710fdbeed5286c4e2daff6f66fd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401266"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="2d9f5-103">创建 androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="2d9f5-103">Create androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="2d9f5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2d9f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d9f5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d9f5-106">创建新的[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-106">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2d9f5-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2d9f5-107">Prerequisites</span></span>
<span data-ttu-id="2d9f5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2d9f5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2d9f5-110">Permission type</span></span>|<span data-ttu-id="2d9f5-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2d9f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d9f5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2d9f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2d9f5-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d9f5-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2d9f5-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2d9f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d9f5-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-115">Not supported.</span></span>|
|<span data-ttu-id="2d9f5-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2d9f5-116">Application</span></span>|<span data-ttu-id="2d9f5-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d9f5-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2d9f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="2d9f5-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2d9f5-119">Request headers</span></span>
|<span data-ttu-id="2d9f5-120">标头</span><span class="sxs-lookup"><span data-stu-id="2d9f5-120">Header</span></span>|<span data-ttu-id="2d9f5-121">值</span><span class="sxs-lookup"><span data-stu-id="2d9f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d9f5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d9f5-122">Authorization</span></span>|<span data-ttu-id="2d9f5-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2d9f5-124">接受</span><span class="sxs-lookup"><span data-stu-id="2d9f5-124">Accept</span></span>|<span data-ttu-id="2d9f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2d9f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d9f5-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2d9f5-126">Request body</span></span>
<span data-ttu-id="2d9f5-127">在请求正文中，提供 androidWorkProfileCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-127">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="2d9f5-128">下表显示创建 androidWorkProfileCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-128">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="2d9f5-129">属性</span><span class="sxs-lookup"><span data-stu-id="2d9f5-129">Property</span></span>|<span data-ttu-id="2d9f5-130">类型</span><span class="sxs-lookup"><span data-stu-id="2d9f5-130">Type</span></span>|<span data-ttu-id="2d9f5-131">说明</span><span class="sxs-lookup"><span data-stu-id="2d9f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d9f5-132">id</span><span class="sxs-lookup"><span data-stu-id="2d9f5-132">id</span></span>|<span data-ttu-id="2d9f5-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2d9f5-133">String</span></span>|<span data-ttu-id="2d9f5-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-134">Key of the entity.</span></span> <span data-ttu-id="2d9f5-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d9f5-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f5-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2d9f5-136">lastModifiedDateTime</span></span>|<span data-ttu-id="2d9f5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d9f5-137">DateTimeOffset</span></span>|<span data-ttu-id="2d9f5-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-138">DateTime the object was last modified.</span></span> <span data-ttu-id="2d9f5-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d9f5-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f5-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2d9f5-140">createdDateTime</span></span>|<span data-ttu-id="2d9f5-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2d9f5-141">DateTimeOffset</span></span>|<span data-ttu-id="2d9f5-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-142">DateTime the object was created.</span></span> <span data-ttu-id="2d9f5-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d9f5-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f5-144">description</span><span class="sxs-lookup"><span data-stu-id="2d9f5-144">description</span></span>|<span data-ttu-id="2d9f5-145">String</span><span class="sxs-lookup"><span data-stu-id="2d9f5-145">String</span></span>|<span data-ttu-id="2d9f5-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="2d9f5-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d9f5-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f5-148">displayName</span><span class="sxs-lookup"><span data-stu-id="2d9f5-148">displayName</span></span>|<span data-ttu-id="2d9f5-149">String</span><span class="sxs-lookup"><span data-stu-id="2d9f5-149">String</span></span>|<span data-ttu-id="2d9f5-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="2d9f5-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d9f5-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f5-152">version</span><span class="sxs-lookup"><span data-stu-id="2d9f5-152">version</span></span>|<span data-ttu-id="2d9f5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="2d9f5-153">Int32</span></span>|<span data-ttu-id="2d9f5-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-154">Version of the device configuration.</span></span> <span data-ttu-id="2d9f5-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2d9f5-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="2d9f5-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="2d9f5-156">omaSettings</span></span>|<span data-ttu-id="2d9f5-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2d9f5-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="2d9f5-158">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-158">OMA settings.</span></span> <span data-ttu-id="2d9f5-159">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-159">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="2d9f5-160">响应</span><span class="sxs-lookup"><span data-stu-id="2d9f5-160">Response</span></span>
<span data-ttu-id="2d9f5-161">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-161">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d9f5-162">示例</span><span class="sxs-lookup"><span data-stu-id="2d9f5-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="2d9f5-163">请求</span><span class="sxs-lookup"><span data-stu-id="2d9f5-163">Request</span></span>
<span data-ttu-id="2d9f5-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 413

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
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

### <a name="response"></a><span data-ttu-id="2d9f5-165">响应</span><span class="sxs-lookup"><span data-stu-id="2d9f5-165">Response</span></span>
<span data-ttu-id="2d9f5-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2d9f5-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 585

{
  "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
  "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
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






