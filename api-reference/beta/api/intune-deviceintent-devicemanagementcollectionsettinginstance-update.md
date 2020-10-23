---
title: 更新 deviceManagementCollectionSettingInstance
description: 更新 deviceManagementCollectionSettingInstance 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f00648ec49d0bcc628611b6d3d8990e5b5327d8f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736532"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="2fb6c-103">更新 deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="2fb6c-103">Update deviceManagementCollectionSettingInstance</span></span>

<span data-ttu-id="2fb6c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2fb6c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2fb6c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2fb6c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2fb6c-107">更新 [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-107">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2fb6c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2fb6c-108">Prerequisites</span></span>
<span data-ttu-id="2fb6c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2fb6c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2fb6c-111">Permission type</span></span>|<span data-ttu-id="2fb6c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2fb6c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2fb6c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2fb6c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2fb6c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fb6c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2fb6c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2fb6c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2fb6c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-116">Not supported.</span></span>|
|<span data-ttu-id="2fb6c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2fb6c-117">Application</span></span>|<span data-ttu-id="2fb6c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2fb6c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2fb6c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2fb6c-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="2fb6c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2fb6c-120">Request headers</span></span>
|<span data-ttu-id="2fb6c-121">标头</span><span class="sxs-lookup"><span data-stu-id="2fb6c-121">Header</span></span>|<span data-ttu-id="2fb6c-122">值</span><span class="sxs-lookup"><span data-stu-id="2fb6c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2fb6c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2fb6c-123">Authorization</span></span>|<span data-ttu-id="2fb6c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2fb6c-125">接受</span><span class="sxs-lookup"><span data-stu-id="2fb6c-125">Accept</span></span>|<span data-ttu-id="2fb6c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2fb6c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2fb6c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2fb6c-127">Request body</span></span>
<span data-ttu-id="2fb6c-128">在请求正文中，提供 [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-128">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="2fb6c-129">下表显示创建 [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-129">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="2fb6c-130">属性</span><span class="sxs-lookup"><span data-stu-id="2fb6c-130">Property</span></span>|<span data-ttu-id="2fb6c-131">类型</span><span class="sxs-lookup"><span data-stu-id="2fb6c-131">Type</span></span>|<span data-ttu-id="2fb6c-132">说明</span><span class="sxs-lookup"><span data-stu-id="2fb6c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2fb6c-133">id</span><span class="sxs-lookup"><span data-stu-id="2fb6c-133">id</span></span>|<span data-ttu-id="2fb6c-134">String</span><span class="sxs-lookup"><span data-stu-id="2fb6c-134">String</span></span>|<span data-ttu-id="2fb6c-135">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="2fb6c-135">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2fb6c-136">definitionId</span><span class="sxs-lookup"><span data-stu-id="2fb6c-136">definitionId</span></span>|<span data-ttu-id="2fb6c-137">String</span><span class="sxs-lookup"><span data-stu-id="2fb6c-137">String</span></span>|<span data-ttu-id="2fb6c-138">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="2fb6c-138">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="2fb6c-139">valueJson</span><span class="sxs-lookup"><span data-stu-id="2fb6c-139">valueJson</span></span>|<span data-ttu-id="2fb6c-140">String</span><span class="sxs-lookup"><span data-stu-id="2fb6c-140">String</span></span>|<span data-ttu-id="2fb6c-141">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2fb6c-141">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="2fb6c-142">响应</span><span class="sxs-lookup"><span data-stu-id="2fb6c-142">Response</span></span>
<span data-ttu-id="2fb6c-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-143">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2fb6c-144">示例</span><span class="sxs-lookup"><span data-stu-id="2fb6c-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="2fb6c-145">请求</span><span class="sxs-lookup"><span data-stu-id="2fb6c-145">Request</span></span>
<span data-ttu-id="2fb6c-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/settings/{deviceManagementSettingInstanceId}
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```

### <a name="response"></a><span data-ttu-id="2fb6c-147">响应</span><span class="sxs-lookup"><span data-stu-id="2fb6c-147">Response</span></span>
<span data-ttu-id="2fb6c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2fb6c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.deviceManagementCollectionSettingInstance",
  "id": "6ce278f7-78f7-6ce2-f778-e26cf778e26c",
  "definitionId": "Definition Id value",
  "valueJson": "Value Json value"
}
```





