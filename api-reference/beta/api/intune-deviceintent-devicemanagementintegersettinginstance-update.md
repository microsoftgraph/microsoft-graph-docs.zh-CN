---
title: 更新 deviceManagementIntegerSettingInstance
description: 更新 deviceManagementIntegerSettingInstance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7b90a762699336fe0874790d5e0553c077b80095
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132091"
---
# <a name="update-devicemanagementintegersettinginstance"></a><span data-ttu-id="57cc7-103">更新 deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="57cc7-103">Update deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="57cc7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57cc7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57cc7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="57cc7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="57cc7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="57cc7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57cc7-107">更新 [deviceManagementIntegerSettingInstance 对象](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="57cc7-107">Update the properties of a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="57cc7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="57cc7-108">Prerequisites</span></span>
<span data-ttu-id="57cc7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="57cc7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="57cc7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="57cc7-111">Permission type</span></span>|<span data-ttu-id="57cc7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="57cc7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="57cc7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="57cc7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="57cc7-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57cc7-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="57cc7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="57cc7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="57cc7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="57cc7-116">Not supported.</span></span>|
|<span data-ttu-id="57cc7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="57cc7-117">Application</span></span>|<span data-ttu-id="57cc7-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="57cc7-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="57cc7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="57cc7-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="57cc7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="57cc7-120">Request headers</span></span>
|<span data-ttu-id="57cc7-121">标头</span><span class="sxs-lookup"><span data-stu-id="57cc7-121">Header</span></span>|<span data-ttu-id="57cc7-122">值</span><span class="sxs-lookup"><span data-stu-id="57cc7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="57cc7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="57cc7-123">Authorization</span></span>|<span data-ttu-id="57cc7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="57cc7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="57cc7-125">接受</span><span class="sxs-lookup"><span data-stu-id="57cc7-125">Accept</span></span>|<span data-ttu-id="57cc7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="57cc7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="57cc7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="57cc7-127">Request body</span></span>
<span data-ttu-id="57cc7-128">在请求正文中，提供 [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="57cc7-128">In the request body, supply a JSON representation for the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

<span data-ttu-id="57cc7-129">下表显示创建 [deviceManagementIntegerSettingInstance 时所需的属性](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)。</span><span class="sxs-lookup"><span data-stu-id="57cc7-129">The following table shows the properties that are required when you create the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

|<span data-ttu-id="57cc7-130">属性</span><span class="sxs-lookup"><span data-stu-id="57cc7-130">Property</span></span>|<span data-ttu-id="57cc7-131">类型</span><span class="sxs-lookup"><span data-stu-id="57cc7-131">Type</span></span>|<span data-ttu-id="57cc7-132">说明</span><span class="sxs-lookup"><span data-stu-id="57cc7-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57cc7-133">id</span><span class="sxs-lookup"><span data-stu-id="57cc7-133">id</span></span>|<span data-ttu-id="57cc7-134">String</span><span class="sxs-lookup"><span data-stu-id="57cc7-134">String</span></span>|<span data-ttu-id="57cc7-135">设置实例 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="57cc7-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="57cc7-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="57cc7-136">definitionId</span></span>|<span data-ttu-id="57cc7-137">String</span><span class="sxs-lookup"><span data-stu-id="57cc7-137">String</span></span>|<span data-ttu-id="57cc7-138">此实例的设置定义的 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="57cc7-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="57cc7-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="57cc7-139">valueJson</span></span>|<span data-ttu-id="57cc7-140">String</span><span class="sxs-lookup"><span data-stu-id="57cc7-140">String</span></span>|<span data-ttu-id="57cc7-141">值的 JSON 表示形式 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="57cc7-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="57cc7-142">值</span><span class="sxs-lookup"><span data-stu-id="57cc7-142">value</span></span>|<span data-ttu-id="57cc7-143">Int32</span><span class="sxs-lookup"><span data-stu-id="57cc7-143">Int32</span></span>|<span data-ttu-id="57cc7-144">整数值</span><span class="sxs-lookup"><span data-stu-id="57cc7-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="57cc7-145">响应</span><span class="sxs-lookup"><span data-stu-id="57cc7-145">Response</span></span>
<span data-ttu-id="57cc7-146">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="57cc7-146">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="57cc7-147">示例</span><span class="sxs-lookup"><span data-stu-id="57cc7-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="57cc7-148">请求</span><span class="sxs-lookup"><span data-stu-id="57cc7-148">Request</span></span>
<span data-ttu-id="57cc7-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="57cc7-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="57cc7-150">响应</span><span class="sxs-lookup"><span data-stu-id="57cc7-150">Response</span></span>
<span data-ttu-id="57cc7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="57cc7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "id": "60468ce7-8ce7-6046-e78c-4660e78c4660",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```




