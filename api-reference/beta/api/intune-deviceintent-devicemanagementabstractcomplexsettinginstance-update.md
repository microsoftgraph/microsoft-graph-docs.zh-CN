---
title: 更新 deviceManagementAbstractComplexSettingInstance
description: 更新 deviceManagementAbstractComplexSettingInstance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5feb4eccfd8594f7e8264a62a416bca4c8dd8f51
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47974392"
---
# <a name="update-devicemanagementabstractcomplexsettinginstance"></a><span data-ttu-id="b569f-103">更新 deviceManagementAbstractComplexSettingInstance</span><span class="sxs-lookup"><span data-stu-id="b569f-103">Update deviceManagementAbstractComplexSettingInstance</span></span>

<span data-ttu-id="b569f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b569f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b569f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b569f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b569f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b569f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b569f-107">更新 [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b569f-107">Update the properties of a [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b569f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b569f-108">Prerequisites</span></span>
<span data-ttu-id="b569f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b569f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b569f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b569f-111">Permission type</span></span>|<span data-ttu-id="b569f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b569f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b569f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b569f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b569f-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b569f-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b569f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b569f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b569f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b569f-116">Not supported.</span></span>|
|<span data-ttu-id="b569f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b569f-117">Application</span></span>|<span data-ttu-id="b569f-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b569f-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b569f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b569f-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b569f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b569f-120">Request headers</span></span>
|<span data-ttu-id="b569f-121">标头</span><span class="sxs-lookup"><span data-stu-id="b569f-121">Header</span></span>|<span data-ttu-id="b569f-122">值</span><span class="sxs-lookup"><span data-stu-id="b569f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b569f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b569f-123">Authorization</span></span>|<span data-ttu-id="b569f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b569f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b569f-125">接受</span><span class="sxs-lookup"><span data-stu-id="b569f-125">Accept</span></span>|<span data-ttu-id="b569f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b569f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b569f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b569f-127">Request body</span></span>
<span data-ttu-id="b569f-128">在请求正文中，提供 [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b569f-128">In the request body, supply a JSON representation for the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object.</span></span>

<span data-ttu-id="b569f-129">下表显示创建 [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b569f-129">The following table shows the properties that are required when you create the [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md).</span></span>

|<span data-ttu-id="b569f-130">属性</span><span class="sxs-lookup"><span data-stu-id="b569f-130">Property</span></span>|<span data-ttu-id="b569f-131">类型</span><span class="sxs-lookup"><span data-stu-id="b569f-131">Type</span></span>|<span data-ttu-id="b569f-132">说明</span><span class="sxs-lookup"><span data-stu-id="b569f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b569f-133">id</span><span class="sxs-lookup"><span data-stu-id="b569f-133">id</span></span>|<span data-ttu-id="b569f-134">String</span><span class="sxs-lookup"><span data-stu-id="b569f-134">String</span></span>|<span data-ttu-id="b569f-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="b569f-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b569f-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="b569f-136">definitionId</span></span>|<span data-ttu-id="b569f-137">String</span><span class="sxs-lookup"><span data-stu-id="b569f-137">String</span></span>|<span data-ttu-id="b569f-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="b569f-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b569f-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="b569f-139">valueJson</span></span>|<span data-ttu-id="b569f-140">String</span><span class="sxs-lookup"><span data-stu-id="b569f-140">String</span></span>|<span data-ttu-id="b569f-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b569f-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b569f-142">implementationId</span><span class="sxs-lookup"><span data-stu-id="b569f-142">implementationId</span></span>|<span data-ttu-id="b569f-143">String</span><span class="sxs-lookup"><span data-stu-id="b569f-143">String</span></span>|<span data-ttu-id="b569f-144">此复杂设置的所选实现的定义 ID</span><span class="sxs-lookup"><span data-stu-id="b569f-144">The definition ID for the chosen implementation of this complex setting</span></span>|



## <a name="response"></a><span data-ttu-id="b569f-145">响应</span><span class="sxs-lookup"><span data-stu-id="b569f-145">Response</span></span>
<span data-ttu-id="b569f-146">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b569f-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b569f-147">示例</span><span class="sxs-lookup"><span data-stu-id="b569f-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="b569f-148">请求</span><span class="sxs-lookup"><span data-stu-id="b569f-148">Request</span></span>
<span data-ttu-id="b569f-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b569f-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 216

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```

### <a name="response"></a><span data-ttu-id="b569f-150">响应</span><span class="sxs-lookup"><span data-stu-id="b569f-150">Response</span></span>
<span data-ttu-id="b569f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b569f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 265

{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "433e9565-9565-433e-6595-3e4365953e43",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "implementationId": "Implementation Id value"
}
```






