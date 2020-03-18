---
title: 更新 deviceManagementCollectionSettingInstance
description: 更新 deviceManagementCollectionSettingInstance 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2e0645eabf3d59e1b581c9e7753415be0802dffa
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42730541"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="a0cbe-103">更新 deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="a0cbe-103">Update deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="a0cbe-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0cbe-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0cbe-106">更新[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-106">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a0cbe-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a0cbe-107">Prerequisites</span></span>
<span data-ttu-id="a0cbe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a0cbe-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a0cbe-110">Permission type</span></span>|<span data-ttu-id="a0cbe-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a0cbe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a0cbe-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a0cbe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a0cbe-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0cbe-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a0cbe-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a0cbe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a0cbe-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-115">Not supported.</span></span>|
|<span data-ttu-id="a0cbe-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a0cbe-116">Application</span></span>|<span data-ttu-id="a0cbe-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a0cbe-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a0cbe-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a0cbe-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="a0cbe-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a0cbe-119">Request headers</span></span>
|<span data-ttu-id="a0cbe-120">标头</span><span class="sxs-lookup"><span data-stu-id="a0cbe-120">Header</span></span>|<span data-ttu-id="a0cbe-121">值</span><span class="sxs-lookup"><span data-stu-id="a0cbe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a0cbe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a0cbe-122">Authorization</span></span>|<span data-ttu-id="a0cbe-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a0cbe-124">接受</span><span class="sxs-lookup"><span data-stu-id="a0cbe-124">Accept</span></span>|<span data-ttu-id="a0cbe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a0cbe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a0cbe-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a0cbe-126">Request body</span></span>
<span data-ttu-id="a0cbe-127">在请求正文中，提供[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="a0cbe-128">下表显示创建[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="a0cbe-129">属性</span><span class="sxs-lookup"><span data-stu-id="a0cbe-129">Property</span></span>|<span data-ttu-id="a0cbe-130">类型</span><span class="sxs-lookup"><span data-stu-id="a0cbe-130">Type</span></span>|<span data-ttu-id="a0cbe-131">说明</span><span class="sxs-lookup"><span data-stu-id="a0cbe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0cbe-132">id</span><span class="sxs-lookup"><span data-stu-id="a0cbe-132">id</span></span>|<span data-ttu-id="a0cbe-133">String</span><span class="sxs-lookup"><span data-stu-id="a0cbe-133">String</span></span>|<span data-ttu-id="a0cbe-134">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="a0cbe-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="a0cbe-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="a0cbe-135">definitionId</span></span>|<span data-ttu-id="a0cbe-136">String</span><span class="sxs-lookup"><span data-stu-id="a0cbe-136">String</span></span>|<span data-ttu-id="a0cbe-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="a0cbe-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="a0cbe-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="a0cbe-138">valueJson</span></span>|<span data-ttu-id="a0cbe-139">String</span><span class="sxs-lookup"><span data-stu-id="a0cbe-139">String</span></span>|<span data-ttu-id="a0cbe-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a0cbe-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="a0cbe-141">响应</span><span class="sxs-lookup"><span data-stu-id="a0cbe-141">Response</span></span>
<span data-ttu-id="a0cbe-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a0cbe-143">示例</span><span class="sxs-lookup"><span data-stu-id="a0cbe-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="a0cbe-144">请求</span><span class="sxs-lookup"><span data-stu-id="a0cbe-144">Request</span></span>
<span data-ttu-id="a0cbe-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a0cbe-146">响应</span><span class="sxs-lookup"><span data-stu-id="a0cbe-146">Response</span></span>
<span data-ttu-id="a0cbe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a0cbe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




