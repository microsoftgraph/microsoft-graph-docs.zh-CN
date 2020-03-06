---
title: 创建 androidWorkProfileCustomConfiguration
description: 创建新的 androidWorkProfileCustomConfiguration 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f1b145a03761614f452c897bd4fa6ccb2535b43e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515257"
---
# <a name="create-androidworkprofilecustomconfiguration"></a><span data-ttu-id="3962b-103">创建 androidWorkProfileCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="3962b-103">Create androidWorkProfileCustomConfiguration</span></span>

<span data-ttu-id="3962b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3962b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3962b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3962b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3962b-106">创建新的[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3962b-106">Create a new [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3962b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3962b-107">Prerequisites</span></span>
<span data-ttu-id="3962b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3962b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3962b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3962b-110">Permission type</span></span>|<span data-ttu-id="3962b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3962b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3962b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3962b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3962b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3962b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3962b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3962b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3962b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3962b-115">Not supported.</span></span>|
|<span data-ttu-id="3962b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3962b-116">Application</span></span>|<span data-ttu-id="3962b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3962b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3962b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3962b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="3962b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3962b-119">Request headers</span></span>
|<span data-ttu-id="3962b-120">标头</span><span class="sxs-lookup"><span data-stu-id="3962b-120">Header</span></span>|<span data-ttu-id="3962b-121">值</span><span class="sxs-lookup"><span data-stu-id="3962b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3962b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3962b-122">Authorization</span></span>|<span data-ttu-id="3962b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3962b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3962b-124">接受</span><span class="sxs-lookup"><span data-stu-id="3962b-124">Accept</span></span>|<span data-ttu-id="3962b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3962b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3962b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3962b-126">Request body</span></span>
<span data-ttu-id="3962b-127">在请求正文中，提供 androidWorkProfileCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3962b-127">In the request body, supply a JSON representation for the androidWorkProfileCustomConfiguration object.</span></span>

<span data-ttu-id="3962b-128">下表显示创建 androidWorkProfileCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3962b-128">The following table shows the properties that are required when you create the androidWorkProfileCustomConfiguration.</span></span>

|<span data-ttu-id="3962b-129">属性</span><span class="sxs-lookup"><span data-stu-id="3962b-129">Property</span></span>|<span data-ttu-id="3962b-130">类型</span><span class="sxs-lookup"><span data-stu-id="3962b-130">Type</span></span>|<span data-ttu-id="3962b-131">说明</span><span class="sxs-lookup"><span data-stu-id="3962b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3962b-132">id</span><span class="sxs-lookup"><span data-stu-id="3962b-132">id</span></span>|<span data-ttu-id="3962b-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3962b-133">String</span></span>|<span data-ttu-id="3962b-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3962b-134">Key of the entity.</span></span> <span data-ttu-id="3962b-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3962b-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3962b-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3962b-136">lastModifiedDateTime</span></span>|<span data-ttu-id="3962b-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3962b-137">DateTimeOffset</span></span>|<span data-ttu-id="3962b-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3962b-138">DateTime the object was last modified.</span></span> <span data-ttu-id="3962b-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3962b-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3962b-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3962b-140">createdDateTime</span></span>|<span data-ttu-id="3962b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3962b-141">DateTimeOffset</span></span>|<span data-ttu-id="3962b-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="3962b-142">DateTime the object was created.</span></span> <span data-ttu-id="3962b-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3962b-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3962b-144">说明</span><span class="sxs-lookup"><span data-stu-id="3962b-144">description</span></span>|<span data-ttu-id="3962b-145">String</span><span class="sxs-lookup"><span data-stu-id="3962b-145">String</span></span>|<span data-ttu-id="3962b-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="3962b-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="3962b-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3962b-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3962b-148">displayName</span><span class="sxs-lookup"><span data-stu-id="3962b-148">displayName</span></span>|<span data-ttu-id="3962b-149">String</span><span class="sxs-lookup"><span data-stu-id="3962b-149">String</span></span>|<span data-ttu-id="3962b-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="3962b-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="3962b-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3962b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3962b-152">version</span><span class="sxs-lookup"><span data-stu-id="3962b-152">version</span></span>|<span data-ttu-id="3962b-153">Int32</span><span class="sxs-lookup"><span data-stu-id="3962b-153">Int32</span></span>|<span data-ttu-id="3962b-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="3962b-154">Version of the device configuration.</span></span> <span data-ttu-id="3962b-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="3962b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="3962b-156">omaSettings</span><span class="sxs-lookup"><span data-stu-id="3962b-156">omaSettings</span></span>|<span data-ttu-id="3962b-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="3962b-157">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="3962b-158">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="3962b-158">OMA settings.</span></span> <span data-ttu-id="3962b-159">该集合最多可包含 500 个元素。</span><span class="sxs-lookup"><span data-stu-id="3962b-159">This collection can contain a maximum of 500 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="3962b-160">响应</span><span class="sxs-lookup"><span data-stu-id="3962b-160">Response</span></span>
<span data-ttu-id="3962b-161">如果成功，此方法在响应`201 Created`正文中返回响应代码和[androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3962b-161">If successful, this method returns a `201 Created` response code and a [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3962b-162">示例</span><span class="sxs-lookup"><span data-stu-id="3962b-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="3962b-163">请求</span><span class="sxs-lookup"><span data-stu-id="3962b-163">Request</span></span>
<span data-ttu-id="3962b-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3962b-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3962b-165">响应</span><span class="sxs-lookup"><span data-stu-id="3962b-165">Response</span></span>
<span data-ttu-id="3962b-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3962b-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




