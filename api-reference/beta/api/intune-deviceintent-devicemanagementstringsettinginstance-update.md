---
title: 更新 deviceManagementStringSettingInstance
description: 更新 deviceManagementStringSettingInstance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3e6cb2c5f64c6920f5a4540c7e4b5c5fb32da92
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43381498"
---
# <a name="update-devicemanagementstringsettinginstance"></a><span data-ttu-id="03442-103">更新 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="03442-103">Update deviceManagementStringSettingInstance</span></span>

<span data-ttu-id="03442-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03442-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03442-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03442-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03442-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03442-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03442-107">更新[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="03442-107">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03442-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03442-108">Prerequisites</span></span>
<span data-ttu-id="03442-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03442-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03442-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03442-111">Permission type</span></span>|<span data-ttu-id="03442-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03442-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03442-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03442-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03442-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03442-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="03442-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03442-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03442-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03442-116">Not supported.</span></span>|
|<span data-ttu-id="03442-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03442-117">Application</span></span>|<span data-ttu-id="03442-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03442-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03442-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03442-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="03442-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03442-120">Request headers</span></span>
|<span data-ttu-id="03442-121">标头</span><span class="sxs-lookup"><span data-stu-id="03442-121">Header</span></span>|<span data-ttu-id="03442-122">值</span><span class="sxs-lookup"><span data-stu-id="03442-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03442-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03442-123">Authorization</span></span>|<span data-ttu-id="03442-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03442-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03442-125">接受</span><span class="sxs-lookup"><span data-stu-id="03442-125">Accept</span></span>|<span data-ttu-id="03442-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03442-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03442-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03442-127">Request body</span></span>
<span data-ttu-id="03442-128">在请求正文中，提供[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03442-128">In the request body, supply a JSON representation for the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

<span data-ttu-id="03442-129">下表显示创建[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03442-129">The following table shows the properties that are required when you create the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>

|<span data-ttu-id="03442-130">属性</span><span class="sxs-lookup"><span data-stu-id="03442-130">Property</span></span>|<span data-ttu-id="03442-131">类型</span><span class="sxs-lookup"><span data-stu-id="03442-131">Type</span></span>|<span data-ttu-id="03442-132">说明</span><span class="sxs-lookup"><span data-stu-id="03442-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03442-133">id</span><span class="sxs-lookup"><span data-stu-id="03442-133">id</span></span>|<span data-ttu-id="03442-134">字符串</span><span class="sxs-lookup"><span data-stu-id="03442-134">String</span></span>|<span data-ttu-id="03442-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="03442-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="03442-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="03442-136">definitionId</span></span>|<span data-ttu-id="03442-137">字符串</span><span class="sxs-lookup"><span data-stu-id="03442-137">String</span></span>|<span data-ttu-id="03442-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="03442-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="03442-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="03442-139">valueJson</span></span>|<span data-ttu-id="03442-140">字符串</span><span class="sxs-lookup"><span data-stu-id="03442-140">String</span></span>|<span data-ttu-id="03442-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03442-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="03442-142">value</span><span class="sxs-lookup"><span data-stu-id="03442-142">value</span></span>|<span data-ttu-id="03442-143">String</span><span class="sxs-lookup"><span data-stu-id="03442-143">String</span></span>|<span data-ttu-id="03442-144">字符串值</span><span class="sxs-lookup"><span data-stu-id="03442-144">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="03442-145">响应</span><span class="sxs-lookup"><span data-stu-id="03442-145">Response</span></span>
<span data-ttu-id="03442-146">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="03442-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03442-147">示例</span><span class="sxs-lookup"><span data-stu-id="03442-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="03442-148">请求</span><span class="sxs-lookup"><span data-stu-id="03442-148">Request</span></span>
<span data-ttu-id="03442-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03442-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 184

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```

### <a name="response"></a><span data-ttu-id="03442-150">响应</span><span class="sxs-lookup"><span data-stu-id="03442-150">Response</span></span>
<span data-ttu-id="03442-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="03442-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 233

{
  "@odata.type": "#microsoft.graph.deviceManagementStringSettingInstance",
  "id": "fef30638-0638-fef3-3806-f3fe3806f3fe",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": "Value value"
}
```



