---
title: 更新 deviceManagementComplexSettingInstance
description: 更新 deviceManagementComplexSettingInstance 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 232f2367f1d326c98254b0055c22252de596e2ec
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36343767"
---
# <a name="update-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="84a39-103">更新 deviceManagementComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="84a39-103">Update deviceManagementComplexSettingInstance</span></span>

> <span data-ttu-id="84a39-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84a39-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84a39-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84a39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84a39-106">更新[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="84a39-106">Update the properties of a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84a39-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="84a39-107">Prerequisites</span></span>
<span data-ttu-id="84a39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84a39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84a39-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="84a39-110">Permission type</span></span>|<span data-ttu-id="84a39-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84a39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84a39-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84a39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="84a39-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a39-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84a39-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84a39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84a39-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="84a39-115">Not supported.</span></span>|
|<span data-ttu-id="84a39-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="84a39-116">Application</span></span>|<span data-ttu-id="84a39-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84a39-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84a39-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84a39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings/{deviceManagementSettingInstanceId}
PATCH /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings/{deviceManagementSettingInstanceId}
```

## <a name="request-headers"></a><span data-ttu-id="84a39-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="84a39-119">Request headers</span></span>
|<span data-ttu-id="84a39-120">标头</span><span class="sxs-lookup"><span data-stu-id="84a39-120">Header</span></span>|<span data-ttu-id="84a39-121">值</span><span class="sxs-lookup"><span data-stu-id="84a39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84a39-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="84a39-122">Authorization</span></span>|<span data-ttu-id="84a39-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84a39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84a39-124">接受</span><span class="sxs-lookup"><span data-stu-id="84a39-124">Accept</span></span>|<span data-ttu-id="84a39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="84a39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84a39-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="84a39-126">Request body</span></span>
<span data-ttu-id="84a39-127">在请求正文中, 提供[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84a39-127">In the request body, supply a JSON representation for the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="84a39-128">下表显示创建[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="84a39-128">The following table shows the properties that are required when you create the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="84a39-129">属性</span><span class="sxs-lookup"><span data-stu-id="84a39-129">Property</span></span>|<span data-ttu-id="84a39-130">类型</span><span class="sxs-lookup"><span data-stu-id="84a39-130">Type</span></span>|<span data-ttu-id="84a39-131">说明</span><span class="sxs-lookup"><span data-stu-id="84a39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84a39-132">id</span><span class="sxs-lookup"><span data-stu-id="84a39-132">id</span></span>|<span data-ttu-id="84a39-133">String</span><span class="sxs-lookup"><span data-stu-id="84a39-133">String</span></span>|<span data-ttu-id="84a39-134">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="84a39-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="84a39-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="84a39-135">definitionId</span></span>|<span data-ttu-id="84a39-136">String</span><span class="sxs-lookup"><span data-stu-id="84a39-136">String</span></span>|<span data-ttu-id="84a39-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="84a39-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="84a39-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="84a39-138">valueJson</span></span>|<span data-ttu-id="84a39-139">String</span><span class="sxs-lookup"><span data-stu-id="84a39-139">String</span></span>|<span data-ttu-id="84a39-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="84a39-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="84a39-141">响应</span><span class="sxs-lookup"><span data-stu-id="84a39-141">Response</span></span>
<span data-ttu-id="84a39-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="84a39-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84a39-143">示例</span><span class="sxs-lookup"><span data-stu-id="84a39-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="84a39-144">请求</span><span class="sxs-lookup"><span data-stu-id="84a39-144">Request</span></span>
<span data-ttu-id="84a39-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84a39-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 158

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="84a39-146">响应</span><span class="sxs-lookup"><span data-stu-id="84a39-146">Response</span></span>
<span data-ttu-id="84a39-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84a39-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 207

{
  "@odata.type": "#microsoft.graph.deviceManagementComplexSettingInstance",
  "id": "4deb3935-3935-4deb-3539-eb4d3539eb4d",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```






