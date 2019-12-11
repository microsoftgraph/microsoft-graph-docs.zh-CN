---
title: 创建 deviceManagementIntegerSettingInstance
description: 创建新的 deviceManagementIntegerSettingInstance 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f324c27ee618bff2830583a1c37386c591b72e9a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39945933"
---
# <a name="create-devicemanagementintegersettinginstance"></a><span data-ttu-id="afe8d-103">创建 deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="afe8d-103">Create deviceManagementIntegerSettingInstance</span></span>

> <span data-ttu-id="afe8d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="afe8d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afe8d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afe8d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afe8d-106">创建新的[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="afe8d-106">Create a new [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afe8d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="afe8d-107">Prerequisites</span></span>
<span data-ttu-id="afe8d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afe8d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afe8d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="afe8d-110">Permission type</span></span>|<span data-ttu-id="afe8d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="afe8d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afe8d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afe8d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="afe8d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe8d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="afe8d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afe8d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afe8d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="afe8d-115">Not supported.</span></span>|
|<span data-ttu-id="afe8d-116">Application</span><span class="sxs-lookup"><span data-stu-id="afe8d-116">Application</span></span>|<span data-ttu-id="afe8d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afe8d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afe8d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afe8d-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="afe8d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="afe8d-119">Request headers</span></span>
|<span data-ttu-id="afe8d-120">标头</span><span class="sxs-lookup"><span data-stu-id="afe8d-120">Header</span></span>|<span data-ttu-id="afe8d-121">值</span><span class="sxs-lookup"><span data-stu-id="afe8d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afe8d-122">授权</span><span class="sxs-lookup"><span data-stu-id="afe8d-122">Authorization</span></span>|<span data-ttu-id="afe8d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="afe8d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afe8d-124">接受</span><span class="sxs-lookup"><span data-stu-id="afe8d-124">Accept</span></span>|<span data-ttu-id="afe8d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="afe8d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afe8d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="afe8d-126">Request body</span></span>
<span data-ttu-id="afe8d-127">在请求正文中，提供 deviceManagementIntegerSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afe8d-127">In the request body, supply a JSON representation for the deviceManagementIntegerSettingInstance object.</span></span>

<span data-ttu-id="afe8d-128">下表显示创建 deviceManagementIntegerSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="afe8d-128">The following table shows the properties that are required when you create the deviceManagementIntegerSettingInstance.</span></span>

|<span data-ttu-id="afe8d-129">属性</span><span class="sxs-lookup"><span data-stu-id="afe8d-129">Property</span></span>|<span data-ttu-id="afe8d-130">类型</span><span class="sxs-lookup"><span data-stu-id="afe8d-130">Type</span></span>|<span data-ttu-id="afe8d-131">说明</span><span class="sxs-lookup"><span data-stu-id="afe8d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afe8d-132">id</span><span class="sxs-lookup"><span data-stu-id="afe8d-132">id</span></span>|<span data-ttu-id="afe8d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="afe8d-133">String</span></span>|<span data-ttu-id="afe8d-134">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="afe8d-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="afe8d-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="afe8d-135">definitionId</span></span>|<span data-ttu-id="afe8d-136">字符串</span><span class="sxs-lookup"><span data-stu-id="afe8d-136">String</span></span>|<span data-ttu-id="afe8d-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="afe8d-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="afe8d-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="afe8d-138">valueJson</span></span>|<span data-ttu-id="afe8d-139">字符串</span><span class="sxs-lookup"><span data-stu-id="afe8d-139">String</span></span>|<span data-ttu-id="afe8d-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="afe8d-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="afe8d-141">值</span><span class="sxs-lookup"><span data-stu-id="afe8d-141">value</span></span>|<span data-ttu-id="afe8d-142">Int32</span><span class="sxs-lookup"><span data-stu-id="afe8d-142">Int32</span></span>|<span data-ttu-id="afe8d-143">整数值</span><span class="sxs-lookup"><span data-stu-id="afe8d-143">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="afe8d-144">响应</span><span class="sxs-lookup"><span data-stu-id="afe8d-144">Response</span></span>
<span data-ttu-id="afe8d-145">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="afe8d-145">If successful, this method returns a `201 Created` response code and a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afe8d-146">示例</span><span class="sxs-lookup"><span data-stu-id="afe8d-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="afe8d-147">请求</span><span class="sxs-lookup"><span data-stu-id="afe8d-147">Request</span></span>
<span data-ttu-id="afe8d-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afe8d-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="afe8d-149">响应</span><span class="sxs-lookup"><span data-stu-id="afe8d-149">Response</span></span>
<span data-ttu-id="afe8d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afe8d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





