---
title: 更新 deviceManagementStringSettingInstance
description: 更新 deviceManagementStringSettingInstance 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf84fbd078faf49418bdba41beb172adc1aef0c2
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523656"
---
# <a name="update-devicemanagementstringsettinginstance"></a><span data-ttu-id="2ff5b-103">更新 deviceManagementStringSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2ff5b-103">Update deviceManagementStringSettingInstance</span></span>

> <span data-ttu-id="2ff5b-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ff5b-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ff5b-106">更新[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-106">Update the properties of a [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ff5b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ff5b-107">Prerequisites</span></span>
<span data-ttu-id="2ff5b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ff5b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ff5b-110">Permission type</span></span>|<span data-ttu-id="2ff5b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ff5b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ff5b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ff5b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2ff5b-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ff5b-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ff5b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ff5b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ff5b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-115">Not supported.</span></span>|
|<span data-ttu-id="2ff5b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ff5b-116">Application</span></span>|<span data-ttu-id="2ff5b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ff5b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ff5b-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2ff5b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ff5b-119">Request headers</span></span>
|<span data-ttu-id="2ff5b-120">标头</span><span class="sxs-lookup"><span data-stu-id="2ff5b-120">Header</span></span>|<span data-ttu-id="2ff5b-121">值</span><span class="sxs-lookup"><span data-stu-id="2ff5b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ff5b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ff5b-122">Authorization</span></span>|<span data-ttu-id="2ff5b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ff5b-124">接受</span><span class="sxs-lookup"><span data-stu-id="2ff5b-124">Accept</span></span>|<span data-ttu-id="2ff5b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2ff5b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ff5b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ff5b-126">Request body</span></span>
<span data-ttu-id="2ff5b-127">在请求正文中, 提供[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-127">In the request body, supply a JSON representation for the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object.</span></span>

<span data-ttu-id="2ff5b-128">下表显示创建[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-128">The following table shows the properties that are required when you create the [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md).</span></span>

|<span data-ttu-id="2ff5b-129">属性</span><span class="sxs-lookup"><span data-stu-id="2ff5b-129">Property</span></span>|<span data-ttu-id="2ff5b-130">类型</span><span class="sxs-lookup"><span data-stu-id="2ff5b-130">Type</span></span>|<span data-ttu-id="2ff5b-131">说明</span><span class="sxs-lookup"><span data-stu-id="2ff5b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ff5b-132">id</span><span class="sxs-lookup"><span data-stu-id="2ff5b-132">id</span></span>|<span data-ttu-id="2ff5b-133">String</span><span class="sxs-lookup"><span data-stu-id="2ff5b-133">String</span></span>|<span data-ttu-id="2ff5b-134">从[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="2ff5b-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2ff5b-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="2ff5b-135">definitionId</span></span>|<span data-ttu-id="2ff5b-136">String</span><span class="sxs-lookup"><span data-stu-id="2ff5b-136">String</span></span>|<span data-ttu-id="2ff5b-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="2ff5b-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2ff5b-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="2ff5b-138">valueJson</span></span>|<span data-ttu-id="2ff5b-139">String</span><span class="sxs-lookup"><span data-stu-id="2ff5b-139">String</span></span>|<span data-ttu-id="2ff5b-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ff5b-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2ff5b-141">value</span><span class="sxs-lookup"><span data-stu-id="2ff5b-141">value</span></span>|<span data-ttu-id="2ff5b-142">String</span><span class="sxs-lookup"><span data-stu-id="2ff5b-142">String</span></span>|<span data-ttu-id="2ff5b-143">字符串值</span><span class="sxs-lookup"><span data-stu-id="2ff5b-143">The string value</span></span>|



## <a name="response"></a><span data-ttu-id="2ff5b-144">响应</span><span class="sxs-lookup"><span data-stu-id="2ff5b-144">Response</span></span>
<span data-ttu-id="2ff5b-145">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-145">If successful, this method returns a `200 OK` response code and an updated [deviceManagementStringSettingInstance](../resources/intune-deviceintent-devicemanagementstringsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ff5b-146">示例</span><span class="sxs-lookup"><span data-stu-id="2ff5b-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ff5b-147">请求</span><span class="sxs-lookup"><span data-stu-id="2ff5b-147">Request</span></span>
<span data-ttu-id="2ff5b-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2ff5b-149">响应</span><span class="sxs-lookup"><span data-stu-id="2ff5b-149">Response</span></span>
<span data-ttu-id="2ff5b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ff5b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







