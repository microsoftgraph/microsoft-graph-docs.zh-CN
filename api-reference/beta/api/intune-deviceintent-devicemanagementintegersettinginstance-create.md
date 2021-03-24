---
title: 创建 deviceManagementIntegerSettingInstance
description: 创建新的 deviceManagementIntegerSettingInstance 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d6948766b10001b92e58d14d3191151dd8281c64
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127114"
---
# <a name="create-devicemanagementintegersettinginstance"></a><span data-ttu-id="20540-103">创建 deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="20540-103">Create deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="20540-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="20540-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20540-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="20540-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20540-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="20540-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20540-107">创建新的 [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20540-107">Create a new [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20540-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="20540-108">Prerequisites</span></span>
<span data-ttu-id="20540-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20540-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20540-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="20540-111">Permission type</span></span>|<span data-ttu-id="20540-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20540-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20540-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20540-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20540-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20540-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="20540-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20540-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20540-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="20540-116">Not supported.</span></span>|
|<span data-ttu-id="20540-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="20540-117">Application</span></span>|<span data-ttu-id="20540-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20540-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="20540-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20540-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents/{deviceManagementIntentId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/settings
POST /deviceManagement/intents/{deviceManagementIntentId}/categories/{deviceManagementIntentSettingCategoryId}/settings
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories/{deviceManagementTemplateSettingCategoryId}/recommendedSettings
```

## <a name="request-headers"></a><span data-ttu-id="20540-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="20540-120">Request headers</span></span>
|<span data-ttu-id="20540-121">标头</span><span class="sxs-lookup"><span data-stu-id="20540-121">Header</span></span>|<span data-ttu-id="20540-122">值</span><span class="sxs-lookup"><span data-stu-id="20540-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20540-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="20540-123">Authorization</span></span>|<span data-ttu-id="20540-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="20540-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20540-125">接受</span><span class="sxs-lookup"><span data-stu-id="20540-125">Accept</span></span>|<span data-ttu-id="20540-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20540-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20540-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="20540-127">Request body</span></span>
<span data-ttu-id="20540-128">在请求正文中，提供 deviceManagementIntegerSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20540-128">In the request body, supply a JSON representation for the deviceManagementIntegerSettingInstance object.</span></span>

<span data-ttu-id="20540-129">下表显示创建 deviceManagementIntegerSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="20540-129">The following table shows the properties that are required when you create the deviceManagementIntegerSettingInstance.</span></span>

|<span data-ttu-id="20540-130">属性</span><span class="sxs-lookup"><span data-stu-id="20540-130">Property</span></span>|<span data-ttu-id="20540-131">类型</span><span class="sxs-lookup"><span data-stu-id="20540-131">Type</span></span>|<span data-ttu-id="20540-132">说明</span><span class="sxs-lookup"><span data-stu-id="20540-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20540-133">id</span><span class="sxs-lookup"><span data-stu-id="20540-133">id</span></span>|<span data-ttu-id="20540-134">String</span><span class="sxs-lookup"><span data-stu-id="20540-134">String</span></span>|<span data-ttu-id="20540-135">设置实例 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="20540-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="20540-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="20540-136">definitionId</span></span>|<span data-ttu-id="20540-137">String</span><span class="sxs-lookup"><span data-stu-id="20540-137">String</span></span>|<span data-ttu-id="20540-138">此实例的设置定义的 ID 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="20540-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="20540-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="20540-139">valueJson</span></span>|<span data-ttu-id="20540-140">String</span><span class="sxs-lookup"><span data-stu-id="20540-140">String</span></span>|<span data-ttu-id="20540-141">值的 JSON 表示形式 继承自 [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="20540-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="20540-142">值</span><span class="sxs-lookup"><span data-stu-id="20540-142">value</span></span>|<span data-ttu-id="20540-143">Int32</span><span class="sxs-lookup"><span data-stu-id="20540-143">Int32</span></span>|<span data-ttu-id="20540-144">整数值</span><span class="sxs-lookup"><span data-stu-id="20540-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="20540-145">响应</span><span class="sxs-lookup"><span data-stu-id="20540-145">Response</span></span>
<span data-ttu-id="20540-146">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20540-146">If successful, this method returns a `201 Created` response code and a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20540-147">示例</span><span class="sxs-lookup"><span data-stu-id="20540-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="20540-148">请求</span><span class="sxs-lookup"><span data-stu-id="20540-148">Request</span></span>
<span data-ttu-id="20540-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20540-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 173

{
  "@odata.type": "#microsoft.graph.deviceManagementIntegerSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": 5
}
```

### <a name="response"></a><span data-ttu-id="20540-150">响应</span><span class="sxs-lookup"><span data-stu-id="20540-150">Response</span></span>
<span data-ttu-id="20540-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20540-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




