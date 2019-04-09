---
title: 更新 deviceManagementIntegerSettingInstance
description: 更新 deviceManagementIntegerSettingInstance 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 385f569d0984db15aeb4f5b8da739a1a4ccc7b2d
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522620"
---
# <a name="update-devicemanagementintegersettinginstance"></a><span data-ttu-id="b6702-103">更新 deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="b6702-103">Update deviceManagementIntegerSettingInstance</span></span>

> <span data-ttu-id="b6702-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6702-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6702-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6702-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6702-106">更新[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b6702-106">Update the properties of a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6702-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6702-107">Prerequisites</span></span>
<span data-ttu-id="b6702-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6702-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6702-110">Permission type</span></span>|<span data-ttu-id="b6702-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6702-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6702-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6702-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b6702-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6702-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6702-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6702-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6702-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6702-115">Not supported.</span></span>|
|<span data-ttu-id="b6702-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6702-116">Application</span></span>|<span data-ttu-id="b6702-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6702-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6702-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6702-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="b6702-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6702-119">Request headers</span></span>
|<span data-ttu-id="b6702-120">标头</span><span class="sxs-lookup"><span data-stu-id="b6702-120">Header</span></span>|<span data-ttu-id="b6702-121">值</span><span class="sxs-lookup"><span data-stu-id="b6702-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6702-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6702-122">Authorization</span></span>|<span data-ttu-id="b6702-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6702-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6702-124">接受</span><span class="sxs-lookup"><span data-stu-id="b6702-124">Accept</span></span>|<span data-ttu-id="b6702-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b6702-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6702-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6702-126">Request body</span></span>
<span data-ttu-id="b6702-127">在请求正文中, 提供[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6702-127">In the request body, supply a JSON representation for the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

<span data-ttu-id="b6702-128">下表显示创建[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6702-128">The following table shows the properties that are required when you create the [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md).</span></span>

|<span data-ttu-id="b6702-129">属性</span><span class="sxs-lookup"><span data-stu-id="b6702-129">Property</span></span>|<span data-ttu-id="b6702-130">类型</span><span class="sxs-lookup"><span data-stu-id="b6702-130">Type</span></span>|<span data-ttu-id="b6702-131">说明</span><span class="sxs-lookup"><span data-stu-id="b6702-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6702-132">id</span><span class="sxs-lookup"><span data-stu-id="b6702-132">id</span></span>|<span data-ttu-id="b6702-133">String</span><span class="sxs-lookup"><span data-stu-id="b6702-133">String</span></span>|<span data-ttu-id="b6702-134">从[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="b6702-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b6702-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="b6702-135">definitionId</span></span>|<span data-ttu-id="b6702-136">String</span><span class="sxs-lookup"><span data-stu-id="b6702-136">String</span></span>|<span data-ttu-id="b6702-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="b6702-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b6702-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="b6702-138">valueJson</span></span>|<span data-ttu-id="b6702-139">String</span><span class="sxs-lookup"><span data-stu-id="b6702-139">String</span></span>|<span data-ttu-id="b6702-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6702-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="b6702-141">值</span><span class="sxs-lookup"><span data-stu-id="b6702-141">value</span></span>|<span data-ttu-id="b6702-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b6702-142">Int32</span></span>|<span data-ttu-id="b6702-143">整数值</span><span class="sxs-lookup"><span data-stu-id="b6702-143">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="b6702-144">响应</span><span class="sxs-lookup"><span data-stu-id="b6702-144">Response</span></span>
<span data-ttu-id="b6702-145">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b6702-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6702-146">示例</span><span class="sxs-lookup"><span data-stu-id="b6702-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6702-147">请求</span><span class="sxs-lookup"><span data-stu-id="b6702-147">Request</span></span>
<span data-ttu-id="b6702-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6702-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6702-149">响应</span><span class="sxs-lookup"><span data-stu-id="b6702-149">Response</span></span>
<span data-ttu-id="b6702-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6702-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







