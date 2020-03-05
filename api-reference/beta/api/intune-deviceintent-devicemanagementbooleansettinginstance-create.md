---
title: 创建 deviceManagementBooleanSettingInstance
description: 创建新的 deviceManagementBooleanSettingInstance 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: efb1048ffe3371272efcf6c8c54e366ba42bb2a7
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42472763"
---
# <a name="create-devicemanagementbooleansettinginstance"></a><span data-ttu-id="9a588-103">创建 deviceManagementBooleanSettingInstance</span><span class="sxs-lookup"><span data-stu-id="9a588-103">Create deviceManagementBooleanSettingInstance</span></span>

<span data-ttu-id="9a588-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9a588-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a588-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a588-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a588-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a588-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a588-107">创建新的[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a588-107">Create a new [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9a588-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9a588-108">Prerequisites</span></span>
<span data-ttu-id="9a588-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9a588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9a588-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9a588-111">Permission type</span></span>|<span data-ttu-id="9a588-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9a588-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9a588-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9a588-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9a588-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a588-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9a588-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9a588-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9a588-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9a588-116">Not supported.</span></span>|
|<span data-ttu-id="9a588-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9a588-117">Application</span></span>|<span data-ttu-id="9a588-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9a588-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9a588-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9a588-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="9a588-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9a588-120">Request headers</span></span>
|<span data-ttu-id="9a588-121">标头</span><span class="sxs-lookup"><span data-stu-id="9a588-121">Header</span></span>|<span data-ttu-id="9a588-122">值</span><span class="sxs-lookup"><span data-stu-id="9a588-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9a588-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9a588-123">Authorization</span></span>|<span data-ttu-id="9a588-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9a588-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9a588-125">接受</span><span class="sxs-lookup"><span data-stu-id="9a588-125">Accept</span></span>|<span data-ttu-id="9a588-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9a588-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9a588-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9a588-127">Request body</span></span>
<span data-ttu-id="9a588-128">在请求正文中，提供 deviceManagementBooleanSettingInstance 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9a588-128">In the request body, supply a JSON representation for the deviceManagementBooleanSettingInstance object.</span></span>

<span data-ttu-id="9a588-129">下表显示创建 deviceManagementBooleanSettingInstance 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9a588-129">The following table shows the properties that are required when you create the deviceManagementBooleanSettingInstance.</span></span>

|<span data-ttu-id="9a588-130">属性</span><span class="sxs-lookup"><span data-stu-id="9a588-130">Property</span></span>|<span data-ttu-id="9a588-131">类型</span><span class="sxs-lookup"><span data-stu-id="9a588-131">Type</span></span>|<span data-ttu-id="9a588-132">说明</span><span class="sxs-lookup"><span data-stu-id="9a588-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a588-133">id</span><span class="sxs-lookup"><span data-stu-id="9a588-133">id</span></span>|<span data-ttu-id="9a588-134">String</span><span class="sxs-lookup"><span data-stu-id="9a588-134">String</span></span>|<span data-ttu-id="9a588-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="9a588-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9a588-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="9a588-136">definitionId</span></span>|<span data-ttu-id="9a588-137">String</span><span class="sxs-lookup"><span data-stu-id="9a588-137">String</span></span>|<span data-ttu-id="9a588-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="9a588-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9a588-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="9a588-139">valueJson</span></span>|<span data-ttu-id="9a588-140">String</span><span class="sxs-lookup"><span data-stu-id="9a588-140">String</span></span>|<span data-ttu-id="9a588-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9a588-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="9a588-142">value</span><span class="sxs-lookup"><span data-stu-id="9a588-142">value</span></span>|<span data-ttu-id="9a588-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="9a588-143">Boolean</span></span>|<span data-ttu-id="9a588-144">布尔值</span><span class="sxs-lookup"><span data-stu-id="9a588-144">The boolean value</span></span>|



## <a name="response"></a><span data-ttu-id="9a588-145">响应</span><span class="sxs-lookup"><span data-stu-id="9a588-145">Response</span></span>
<span data-ttu-id="9a588-146">如果成功，此方法在响应`201 Created`正文中返回响应代码和[deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9a588-146">If successful, this method returns a `201 Created` response code and a [deviceManagementBooleanSettingInstance](../resources/intune-deviceintent-devicemanagementbooleansettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9a588-147">示例</span><span class="sxs-lookup"><span data-stu-id="9a588-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="9a588-148">请求</span><span class="sxs-lookup"><span data-stu-id="9a588-148">Request</span></span>
<span data-ttu-id="9a588-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9a588-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings
Content-type: application/json
Content-length: 176

{
  "@odata.type": "#microsoft.graph.deviceManagementBooleanSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value",
  "value": true
}
```

### <a name="response"></a><span data-ttu-id="9a588-150">响应</span><span class="sxs-lookup"><span data-stu-id="9a588-150">Response</span></span>
<span data-ttu-id="9a588-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9a588-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





