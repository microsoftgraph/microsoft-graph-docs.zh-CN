---
title: 创建 deviceManagementIntegerSettingInstance
description: 创建新的 deviceManagementIntegerSettingInstance 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c3815ba08bd426353cc6119b11a2109ec36314c8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43328998"
---
# <a name="create-devicemanagementintegersettinginstance"></a><span data-ttu-id="230ad-103">创建 deviceManagementIntegerSettingInstance</span><span class="sxs-lookup"><span data-stu-id="230ad-103">Create deviceManagementIntegerSettingInstance</span></span>

<span data-ttu-id="230ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="230ad-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="230ad-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="230ad-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="230ad-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="230ad-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="230ad-107">创建新的[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="230ad-107">Create a new [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="230ad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="230ad-108">Prerequisites</span></span>
<span data-ttu-id="230ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="230ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="230ad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="230ad-111">Permission type</span></span>|<span data-ttu-id="230ad-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="230ad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="230ad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="230ad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="230ad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="230ad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="230ad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="230ad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="230ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="230ad-116">Not supported.</span></span>|
|<span data-ttu-id="230ad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="230ad-117">Application</span></span>|<span data-ttu-id="230ad-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="230ad-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="230ad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="230ad-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="230ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="230ad-120">Request headers</span></span>
|<span data-ttu-id="230ad-121">标头</span><span class="sxs-lookup"><span data-stu-id="230ad-121">Header</span></span>|<span data-ttu-id="230ad-122">值</span><span class="sxs-lookup"><span data-stu-id="230ad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="230ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="230ad-123">Authorization</span></span>|<span data-ttu-id="230ad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="230ad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="230ad-125">接受</span><span class="sxs-lookup"><span data-stu-id="230ad-125">Accept</span></span>|<span data-ttu-id="230ad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="230ad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="230ad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="230ad-127">Request body</span></span>
<span data-ttu-id="230ad-128">在请求正文中，提供 deviceManagementIntegerSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="230ad-128">In the request body, supply a JSON representation for the deviceManagementIntegerSettingInstance object.</span></span>

<span data-ttu-id="230ad-129">下表显示创建 deviceManagementIntegerSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="230ad-129">The following table shows the properties that are required when you create the deviceManagementIntegerSettingInstance.</span></span>

|<span data-ttu-id="230ad-130">属性</span><span class="sxs-lookup"><span data-stu-id="230ad-130">Property</span></span>|<span data-ttu-id="230ad-131">类型</span><span class="sxs-lookup"><span data-stu-id="230ad-131">Type</span></span>|<span data-ttu-id="230ad-132">说明</span><span class="sxs-lookup"><span data-stu-id="230ad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="230ad-133">id</span><span class="sxs-lookup"><span data-stu-id="230ad-133">id</span></span>|<span data-ttu-id="230ad-134">字符串</span><span class="sxs-lookup"><span data-stu-id="230ad-134">String</span></span>|<span data-ttu-id="230ad-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="230ad-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="230ad-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="230ad-136">definitionId</span></span>|<span data-ttu-id="230ad-137">字符串</span><span class="sxs-lookup"><span data-stu-id="230ad-137">String</span></span>|<span data-ttu-id="230ad-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="230ad-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="230ad-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="230ad-139">valueJson</span></span>|<span data-ttu-id="230ad-140">字符串</span><span class="sxs-lookup"><span data-stu-id="230ad-140">String</span></span>|<span data-ttu-id="230ad-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="230ad-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="230ad-142">值</span><span class="sxs-lookup"><span data-stu-id="230ad-142">value</span></span>|<span data-ttu-id="230ad-143">Int32</span><span class="sxs-lookup"><span data-stu-id="230ad-143">Int32</span></span>|<span data-ttu-id="230ad-144">整数值</span><span class="sxs-lookup"><span data-stu-id="230ad-144">The integer value</span></span>|



## <a name="response"></a><span data-ttu-id="230ad-145">响应</span><span class="sxs-lookup"><span data-stu-id="230ad-145">Response</span></span>
<span data-ttu-id="230ad-146">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="230ad-146">If successful, this method returns a `201 Created` response code and a [deviceManagementIntegerSettingInstance](../resources/intune-deviceintent-devicemanagementintegersettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="230ad-147">示例</span><span class="sxs-lookup"><span data-stu-id="230ad-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="230ad-148">请求</span><span class="sxs-lookup"><span data-stu-id="230ad-148">Request</span></span>
<span data-ttu-id="230ad-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="230ad-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="230ad-150">响应</span><span class="sxs-lookup"><span data-stu-id="230ad-150">Response</span></span>
<span data-ttu-id="230ad-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="230ad-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



