---
title: 创建 androidCustomConfiguration
description: 创建新的 androidCustomConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ad23e4129d65b5dc70f10a06e4f7bef393e96d22
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966900"
---
# <a name="create-androidcustomconfiguration"></a><span data-ttu-id="ef1a2-103">创建 androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="ef1a2-103">Create androidCustomConfiguration</span></span>

> <span data-ttu-id="ef1a2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ef1a2-105">创建新的 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-105">Create a new [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ef1a2-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ef1a2-106">Prerequisites</span></span>
<span data-ttu-id="ef1a2-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ef1a2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ef1a2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ef1a2-109">Permission type</span></span>|<span data-ttu-id="ef1a2-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ef1a2-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ef1a2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ef1a2-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ef1a2-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ef1a2-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ef1a2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ef1a2-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ef1a2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-114">Not supported.</span></span>|
|<span data-ttu-id="ef1a2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ef1a2-115">Application</span></span>|<span data-ttu-id="ef1a2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ef1a2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ef1a2-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ef1a2-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ef1a2-118">Request headers</span></span>
|<span data-ttu-id="ef1a2-119">标头</span><span class="sxs-lookup"><span data-stu-id="ef1a2-119">Header</span></span>|<span data-ttu-id="ef1a2-120">值</span><span class="sxs-lookup"><span data-stu-id="ef1a2-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ef1a2-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ef1a2-121">Authorization</span></span>|<span data-ttu-id="ef1a2-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ef1a2-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ef1a2-123">Accept</span></span>|<span data-ttu-id="ef1a2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ef1a2-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ef1a2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ef1a2-125">Request body</span></span>
<span data-ttu-id="ef1a2-126">在请求正文中，提供 androidCustomConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-126">In the request body, supply a JSON representation for the androidCustomConfiguration object.</span></span>

<span data-ttu-id="ef1a2-127">下表显示了创建 androidCustomConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-127">The following table shows the properties that are required when you create the androidCustomConfiguration.</span></span>

|<span data-ttu-id="ef1a2-128">属性</span><span class="sxs-lookup"><span data-stu-id="ef1a2-128">Property</span></span>|<span data-ttu-id="ef1a2-129">类型</span><span class="sxs-lookup"><span data-stu-id="ef1a2-129">Type</span></span>|<span data-ttu-id="ef1a2-130">说明</span><span class="sxs-lookup"><span data-stu-id="ef1a2-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ef1a2-131">id</span><span class="sxs-lookup"><span data-stu-id="ef1a2-131">id</span></span>|<span data-ttu-id="ef1a2-132">String</span><span class="sxs-lookup"><span data-stu-id="ef1a2-132">String</span></span>|<span data-ttu-id="ef1a2-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-133">Key of the entity.</span></span> <span data-ttu-id="ef1a2-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1a2-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef1a2-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ef1a2-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ef1a2-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef1a2-136">DateTimeOffset</span></span>|<span data-ttu-id="ef1a2-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ef1a2-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1a2-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef1a2-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ef1a2-139">createdDateTime</span></span>|<span data-ttu-id="ef1a2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ef1a2-140">DateTimeOffset</span></span>|<span data-ttu-id="ef1a2-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-141">DateTime the object was created.</span></span> <span data-ttu-id="ef1a2-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1a2-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef1a2-143">description</span><span class="sxs-lookup"><span data-stu-id="ef1a2-143">description</span></span>|<span data-ttu-id="ef1a2-144">String</span><span class="sxs-lookup"><span data-stu-id="ef1a2-144">String</span></span>|<span data-ttu-id="ef1a2-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ef1a2-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1a2-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef1a2-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ef1a2-147">displayName</span></span>|<span data-ttu-id="ef1a2-148">String</span><span class="sxs-lookup"><span data-stu-id="ef1a2-148">String</span></span>|<span data-ttu-id="ef1a2-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ef1a2-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1a2-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef1a2-151">version</span><span class="sxs-lookup"><span data-stu-id="ef1a2-151">version</span></span>|<span data-ttu-id="ef1a2-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ef1a2-152">Int32</span></span>|<span data-ttu-id="ef1a2-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-153">Version of the device configuration.</span></span> <span data-ttu-id="ef1a2-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ef1a2-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ef1a2-155">omaSettings</span><span class="sxs-lookup"><span data-stu-id="ef1a2-155">omaSettings</span></span>|<span data-ttu-id="ef1a2-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) 集合</span><span class="sxs-lookup"><span data-stu-id="ef1a2-156">[omaSetting](../resources/intune-deviceconfig-omasetting.md) collection</span></span>|<span data-ttu-id="ef1a2-157">OMA 设置。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-157">OMA settings.</span></span> <span data-ttu-id="ef1a2-158">该集合最多可包含 1000 个元素。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-158">This collection can contain a maximum of 1000 elements.</span></span>|



## <a name="response"></a><span data-ttu-id="ef1a2-159">响应</span><span class="sxs-lookup"><span data-stu-id="ef1a2-159">Response</span></span>
<span data-ttu-id="ef1a2-160">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-160">If successful, this method returns a `201 Created` response code and a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ef1a2-161">示例</span><span class="sxs-lookup"><span data-stu-id="ef1a2-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="ef1a2-162">请求</span><span class="sxs-lookup"><span data-stu-id="ef1a2-162">Request</span></span>
<span data-ttu-id="ef1a2-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="ef1a2-164">响应</span><span class="sxs-lookup"><span data-stu-id="ef1a2-164">Response</span></span>
<span data-ttu-id="ef1a2-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ef1a2-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



