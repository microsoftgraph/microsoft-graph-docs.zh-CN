---
title: 更新 deviceManagementBooleanSettingInstance
description: 更新 deviceManagementBooleanSettingInstance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c4eb3e34aaed2e45770ccd287ae78777d44d363d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154586"
---
# <a name="update-devicemanagementbooleansettinginstance"></a><span data-ttu-id="50b59-103">更新 deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="50b59-103">Update deviceManagementBooleanSettingInstance</span></span>

<span data-ttu-id="50b59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="50b59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="50b59-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="50b59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50b59-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="50b59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50b59-107">更新 [deviceManagementBooleanSettingInstance 对象](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="50b59-107">Update the properties of a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="50b59-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="50b59-108">Prerequisites</span></span>
<span data-ttu-id="50b59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50b59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50b59-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="50b59-111">Permission type</span></span>|<span data-ttu-id="50b59-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50b59-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="50b59-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50b59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="50b59-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b59-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="50b59-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50b59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="50b59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="50b59-116">Not supported.</span></span>|
|<span data-ttu-id="50b59-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="50b59-117">Application</span></span>|<span data-ttu-id="50b59-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50b59-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="50b59-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50b59-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="50b59-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="50b59-120">Request headers</span></span>
|<span data-ttu-id="50b59-121">标头</span><span class="sxs-lookup"><span data-stu-id="50b59-121">Header</span></span>|<span data-ttu-id="50b59-122">值</span><span class="sxs-lookup"><span data-stu-id="50b59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="50b59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="50b59-123">Authorization</span></span>|<span data-ttu-id="50b59-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="50b59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="50b59-125">接受</span><span class="sxs-lookup"><span data-stu-id="50b59-125">Accept</span></span>|<span data-ttu-id="50b59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="50b59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50b59-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="50b59-127">Request body</span></span>
<span data-ttu-id="50b59-128">在请求正文中，提供 [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="50b59-128">In the request body, supply a JSON representation for the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

<span data-ttu-id="50b59-129">下表显示创建 [deviceManagementBooleanSettingInstance 时所需的属性](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)。</span><span class="sxs-lookup"><span data-stu-id="50b59-129">The following table shows the properties that are required when you create the [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md).</span></span>

|<span data-ttu-id="50b59-130">属性</span><span class="sxs-lookup"><span data-stu-id="50b59-130">Property</span></span>|<span data-ttu-id="50b59-131">类型</span><span class="sxs-lookup"><span data-stu-id="50b59-131">Type</span></span>|<span data-ttu-id="50b59-132">说明</span><span class="sxs-lookup"><span data-stu-id="50b59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50b59-133">id</span><span class="sxs-lookup"><span data-stu-id="50b59-133">id</span></span>|<span data-ttu-id="50b59-134">String</span><span class="sxs-lookup"><span data-stu-id="50b59-134">String</span></span>|<span data-ttu-id="50b59-135">设置实例 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="50b59-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="50b59-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="50b59-136">definitionId</span></span>|<span data-ttu-id="50b59-137">String</span><span class="sxs-lookup"><span data-stu-id="50b59-137">String</span></span>|<span data-ttu-id="50b59-138">此实例的设置定义的 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="50b59-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="50b59-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="50b59-139">valueJson</span></span>|<span data-ttu-id="50b59-140">String</span><span class="sxs-lookup"><span data-stu-id="50b59-140">String</span></span>|<span data-ttu-id="50b59-141">值的 JSON 表示形式 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="50b59-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="50b59-142">value</span><span class="sxs-lookup"><span data-stu-id="50b59-142">value</span></span>|<span data-ttu-id="50b59-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="50b59-143">Boolean</span></span>|<span data-ttu-id="50b59-144">布尔值</span><span class="sxs-lookup"><span data-stu-id="50b59-144">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="50b59-145">响应</span><span class="sxs-lookup"><span data-stu-id="50b59-145">Response</span></span>
<span data-ttu-id="50b59-146">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="50b59-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50b59-147">示例</span><span class="sxs-lookup"><span data-stu-id="50b59-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="50b59-148">请求</span><span class="sxs-lookup"><span data-stu-id="50b59-148">Request</span></span>
<span data-ttu-id="50b59-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50b59-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="50b59-150">响应</span><span class="sxs-lookup"><span data-stu-id="50b59-150">Response</span></span>
<span data-ttu-id="50b59-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50b59-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




