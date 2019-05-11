---
title: 更新 deviceManagementCollectionSettingInstance
description: 更新 deviceManagementCollectionSettingInstance 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1cd6c40b208b1f8e87a076a06726bac9d26cd704
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916585"
---
# <a name="update-devicemanagementcollectionsettinginstance"></a><span data-ttu-id="11155-103">更新 deviceManagementCollectionSettingInstance</span><span class="sxs-lookup"><span data-stu-id="11155-103">Update deviceManagementCollectionSettingInstance</span></span>

> <span data-ttu-id="11155-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11155-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11155-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11155-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11155-106">更新[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="11155-106">Update the properties of a [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11155-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="11155-107">Prerequisites</span></span>
<span data-ttu-id="11155-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11155-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11155-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11155-110">Permission type</span></span>|<span data-ttu-id="11155-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="11155-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11155-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11155-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11155-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11155-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="11155-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11155-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11155-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11155-115">Not supported.</span></span>|
|<span data-ttu-id="11155-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="11155-116">Application</span></span>|<span data-ttu-id="11155-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="11155-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="11155-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11155-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="11155-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="11155-119">Request headers</span></span>
|<span data-ttu-id="11155-120">标头</span><span class="sxs-lookup"><span data-stu-id="11155-120">Header</span></span>|<span data-ttu-id="11155-121">值</span><span class="sxs-lookup"><span data-stu-id="11155-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11155-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="11155-122">Authorization</span></span>|<span data-ttu-id="11155-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="11155-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11155-124">接受</span><span class="sxs-lookup"><span data-stu-id="11155-124">Accept</span></span>|<span data-ttu-id="11155-125">application/json</span><span class="sxs-lookup"><span data-stu-id="11155-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11155-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="11155-126">Request body</span></span>
<span data-ttu-id="11155-127">在请求正文中, 提供[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="11155-127">In the request body, supply a JSON representation for the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object.</span></span>

<span data-ttu-id="11155-128">下表显示创建[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="11155-128">The following table shows the properties that are required when you create the [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md).</span></span>

|<span data-ttu-id="11155-129">属性</span><span class="sxs-lookup"><span data-stu-id="11155-129">Property</span></span>|<span data-ttu-id="11155-130">类型</span><span class="sxs-lookup"><span data-stu-id="11155-130">Type</span></span>|<span data-ttu-id="11155-131">说明</span><span class="sxs-lookup"><span data-stu-id="11155-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11155-132">id</span><span class="sxs-lookup"><span data-stu-id="11155-132">id</span></span>|<span data-ttu-id="11155-133">String</span><span class="sxs-lookup"><span data-stu-id="11155-133">String</span></span>|<span data-ttu-id="11155-134">从[DeviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID</span><span class="sxs-lookup"><span data-stu-id="11155-134">The setting instance ID Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="11155-135">definitionId</span><span class="sxs-lookup"><span data-stu-id="11155-135">definitionId</span></span>|<span data-ttu-id="11155-136">String</span><span class="sxs-lookup"><span data-stu-id="11155-136">String</span></span>|<span data-ttu-id="11155-137">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID</span><span class="sxs-lookup"><span data-stu-id="11155-137">The ID of the setting definition for this instance Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|
|<span data-ttu-id="11155-138">valueJson</span><span class="sxs-lookup"><span data-stu-id="11155-138">valueJson</span></span>|<span data-ttu-id="11155-139">String</span><span class="sxs-lookup"><span data-stu-id="11155-139">String</span></span>|<span data-ttu-id="11155-140">继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="11155-140">JSON representation of the value Inherited from [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span></span>|



## <a name="response"></a><span data-ttu-id="11155-141">响应</span><span class="sxs-lookup"><span data-stu-id="11155-141">Response</span></span>
<span data-ttu-id="11155-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md)对象。</span><span class="sxs-lookup"><span data-stu-id="11155-142">If successful, this method returns a `200 OK` response code and an updated [deviceManagementCollectionSettingInstance](../resources/intune-deviceintent-devicemanagementcollectionsettinginstance.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="11155-143">示例</span><span class="sxs-lookup"><span data-stu-id="11155-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="11155-144">请求</span><span class="sxs-lookup"><span data-stu-id="11155-144">Request</span></span>
<span data-ttu-id="11155-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11155-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="11155-146">响应</span><span class="sxs-lookup"><span data-stu-id="11155-146">Response</span></span>
<span data-ttu-id="11155-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="11155-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




