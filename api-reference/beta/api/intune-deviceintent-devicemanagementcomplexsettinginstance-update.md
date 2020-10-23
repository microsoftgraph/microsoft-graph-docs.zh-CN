---
title: 更新 deviceManagementComplexSettingInstance
description: 更新 deviceManagementComplexSettingInstance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8678509bd08b6e15aedf8059fc443bbee554a6be
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48704117"
---
# <a name="update-devicemanagementcomplexsettinginstance"></a><span data-ttu-id="65f71-103">更新 deviceManagementComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="65f71-103">Update deviceManagementComplexSettingInstance</span></span>

<span data-ttu-id="65f71-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65f71-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65f71-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65f71-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65f71-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65f71-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65f71-107">更新 [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="65f71-107">Update the properties of a [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65f71-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="65f71-108">Prerequisites</span></span>
<span data-ttu-id="65f71-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65f71-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65f71-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="65f71-111">Permission type</span></span>|<span data-ttu-id="65f71-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="65f71-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65f71-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65f71-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65f71-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65f71-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="65f71-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65f71-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65f71-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65f71-116">Not supported.</span></span>|
|<span data-ttu-id="65f71-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="65f71-117">Application</span></span>|<span data-ttu-id="65f71-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65f71-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65f71-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65f71-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="65f71-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="65f71-120">Request headers</span></span>
|<span data-ttu-id="65f71-121">标头</span><span class="sxs-lookup"><span data-stu-id="65f71-121">Header</span></span>|<span data-ttu-id="65f71-122">值</span><span class="sxs-lookup"><span data-stu-id="65f71-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65f71-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65f71-123">Authorization</span></span>|<span data-ttu-id="65f71-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65f71-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65f71-125">接受</span><span class="sxs-lookup"><span data-stu-id="65f71-125">Accept</span></span>|<span data-ttu-id="65f71-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65f71-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65f71-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="65f71-127">Request body</span></span>
<span data-ttu-id="65f71-128">在请求正文中，提供 [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65f71-128">In the request body, supply a JSON representation for the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="65f71-129">下表显示创建 [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="65f71-129">The following table shows the properties that are required when you create the [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="65f71-130">属性</span><span class="sxs-lookup"><span data-stu-id="65f71-130">Property</span></span>|<span data-ttu-id="65f71-131">类型</span><span class="sxs-lookup"><span data-stu-id="65f71-131">Type</span></span>|<span data-ttu-id="65f71-132">说明</span><span class="sxs-lookup"><span data-stu-id="65f71-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65f71-133">id</span><span class="sxs-lookup"><span data-stu-id="65f71-133">id</span></span>|<span data-ttu-id="65f71-134">String</span><span class="sxs-lookup"><span data-stu-id="65f71-134">String</span></span>|<span data-ttu-id="65f71-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="65f71-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="65f71-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="65f71-136">definitionId</span></span>|<span data-ttu-id="65f71-137">String</span><span class="sxs-lookup"><span data-stu-id="65f71-137">String</span></span>|<span data-ttu-id="65f71-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="65f71-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="65f71-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="65f71-139">valueJson</span></span>|<span data-ttu-id="65f71-140">String</span><span class="sxs-lookup"><span data-stu-id="65f71-140">String</span></span>|<span data-ttu-id="65f71-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="65f71-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="65f71-142">响应</span><span class="sxs-lookup"><span data-stu-id="65f71-142">Response</span></span>
<span data-ttu-id="65f71-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65f71-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementComplexSettingInstance](../resources/intune-deviceintent-devicemanagementcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65f71-144">示例</span><span class="sxs-lookup"><span data-stu-id="65f71-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="65f71-145">请求</span><span class="sxs-lookup"><span data-stu-id="65f71-145">Request</span></span>
<span data-ttu-id="65f71-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65f71-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65f71-147">响应</span><span class="sxs-lookup"><span data-stu-id="65f71-147">Response</span></span>
<span data-ttu-id="65f71-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65f71-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





