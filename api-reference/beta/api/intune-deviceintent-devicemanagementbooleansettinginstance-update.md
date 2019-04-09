---
title: 更新 deviceManagementBooleanSettingInstance
description: 更新 deviceManagementBooleanSettingInstance 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6345fa1883cb8e909cad1859cfde96de1c4ffcb1
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522613"
---
# <a name="update-devicemanagementbooleansettinginstance"></a><span data-ttu-id="35638-103">更新 deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="35638-103">Update deviceManagementBooleanSettingInstance</span></span>

> <span data-ttu-id="35638-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="35638-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35638-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="35638-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35638-106">更新[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="35638-106">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="35638-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="35638-107">Prerequisites</span></span>
<span data-ttu-id="35638-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="35638-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="35638-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="35638-110">Permission type</span></span>|<span data-ttu-id="35638-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="35638-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35638-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="35638-112">Delegated (work or school account)</span></span>|<span data-ttu-id="35638-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35638-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="35638-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="35638-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35638-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="35638-115">Not supported.</span></span>|
|<span data-ttu-id="35638-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="35638-116">Application</span></span>|<span data-ttu-id="35638-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="35638-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35638-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="35638-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="35638-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="35638-119">Request headers</span></span>
|<span data-ttu-id="35638-120">标头</span><span class="sxs-lookup"><span data-stu-id="35638-120">Header</span></span>|<span data-ttu-id="35638-121">值</span><span class="sxs-lookup"><span data-stu-id="35638-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35638-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="35638-122">Authorization</span></span>|<span data-ttu-id="35638-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="35638-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="35638-124">接受</span><span class="sxs-lookup"><span data-stu-id="35638-124">Accept</span></span>|<span data-ttu-id="35638-125">application/json</span><span class="sxs-lookup"><span data-stu-id="35638-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35638-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="35638-126">Request body</span></span>
<span data-ttu-id="35638-127">在请求正文中, 提供[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="35638-127">In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

<span data-ttu-id="35638-128">下表显示创建[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="35638-128">The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>

|<span data-ttu-id="35638-129">属性</span><span class="sxs-lookup"><span data-stu-id="35638-129">Property</span></span>|<span data-ttu-id="35638-130">类型</span><span class="sxs-lookup"><span data-stu-id="35638-130">Type</span></span>|<span data-ttu-id="35638-131">说明</span><span class="sxs-lookup"><span data-stu-id="35638-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35638-132">id</span><span class="sxs-lookup"><span data-stu-id="35638-132">id</span></span>|<span data-ttu-id="35638-133">String</span><span class="sxs-lookup"><span data-stu-id="35638-133">String</span></span>|<span data-ttu-id="35638-134">从[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="35638-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35638-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="35638-135">definitionId</span></span>|<span data-ttu-id="35638-136">String</span><span class="sxs-lookup"><span data-stu-id="35638-136">String</span></span>|<span data-ttu-id="35638-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="35638-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35638-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="35638-138">valueJson</span></span>|<span data-ttu-id="35638-139">String</span><span class="sxs-lookup"><span data-stu-id="35638-139">String</span></span>|<span data-ttu-id="35638-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="35638-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="35638-141">value</span><span class="sxs-lookup"><span data-stu-id="35638-141">value</span></span>|<span data-ttu-id="35638-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="35638-142">Boolean</span></span>|<span data-ttu-id="35638-143">布尔值</span><span class="sxs-lookup"><span data-stu-id="35638-143">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="35638-144">响应</span><span class="sxs-lookup"><span data-stu-id="35638-144">Response</span></span>
<span data-ttu-id="35638-145">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="35638-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35638-146">示例</span><span class="sxs-lookup"><span data-stu-id="35638-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="35638-147">请求</span><span class="sxs-lookup"><span data-stu-id="35638-147">Request</span></span>
<span data-ttu-id="35638-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="35638-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="35638-149">响应</span><span class="sxs-lookup"><span data-stu-id="35638-149">Response</span></span>
<span data-ttu-id="35638-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="35638-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 225

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "id": "bb9b0041-0041-bb9b-4100-9bbb41009bbb",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```







