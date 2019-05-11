---
title: 更新 deviceManagementIntent
description: 更新 deviceManagementIntent 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d61a86001e85f58a9c0f8fa1cb719453029e4fe2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916437"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="2b319-103">更新 deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="2b319-103">Update deviceManagementIntent</span></span>

> <span data-ttu-id="2b319-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b319-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b319-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b319-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b319-106">更新[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2b319-106">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b319-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2b319-107">Prerequisites</span></span>
<span data-ttu-id="2b319-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b319-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b319-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b319-110">Permission type</span></span>|<span data-ttu-id="2b319-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2b319-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b319-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b319-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b319-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b319-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2b319-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b319-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b319-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b319-115">Not supported.</span></span>|
|<span data-ttu-id="2b319-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b319-116">Application</span></span>|<span data-ttu-id="2b319-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b319-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b319-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b319-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="2b319-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b319-119">Request headers</span></span>
|<span data-ttu-id="2b319-120">标头</span><span class="sxs-lookup"><span data-stu-id="2b319-120">Header</span></span>|<span data-ttu-id="2b319-121">值</span><span class="sxs-lookup"><span data-stu-id="2b319-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b319-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b319-122">Authorization</span></span>|<span data-ttu-id="2b319-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2b319-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b319-124">接受</span><span class="sxs-lookup"><span data-stu-id="2b319-124">Accept</span></span>|<span data-ttu-id="2b319-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b319-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b319-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b319-126">Request body</span></span>
<span data-ttu-id="2b319-127">在请求正文中, 提供[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b319-127">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="2b319-128">下表显示创建[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2b319-128">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="2b319-129">属性</span><span class="sxs-lookup"><span data-stu-id="2b319-129">Property</span></span>|<span data-ttu-id="2b319-130">类型</span><span class="sxs-lookup"><span data-stu-id="2b319-130">Type</span></span>|<span data-ttu-id="2b319-131">说明</span><span class="sxs-lookup"><span data-stu-id="2b319-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b319-132">id</span><span class="sxs-lookup"><span data-stu-id="2b319-132">id</span></span>|<span data-ttu-id="2b319-133">字符串</span><span class="sxs-lookup"><span data-stu-id="2b319-133">String</span></span>|<span data-ttu-id="2b319-134">意向 ID</span><span class="sxs-lookup"><span data-stu-id="2b319-134">The intent ID</span></span>|
|<span data-ttu-id="2b319-135">displayName</span><span class="sxs-lookup"><span data-stu-id="2b319-135">displayName</span></span>|<span data-ttu-id="2b319-136">String</span><span class="sxs-lookup"><span data-stu-id="2b319-136">String</span></span>|<span data-ttu-id="2b319-137">用户给定的显示名称</span><span class="sxs-lookup"><span data-stu-id="2b319-137">The user given display name</span></span>|
|<span data-ttu-id="2b319-138">说明</span><span class="sxs-lookup"><span data-stu-id="2b319-138">description</span></span>|<span data-ttu-id="2b319-139">String</span><span class="sxs-lookup"><span data-stu-id="2b319-139">String</span></span>|<span data-ttu-id="2b319-140">用户提供的说明</span><span class="sxs-lookup"><span data-stu-id="2b319-140">The user given description</span></span>|
|<span data-ttu-id="2b319-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="2b319-141">isAssigned</span></span>|<span data-ttu-id="2b319-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="2b319-142">Boolean</span></span>|<span data-ttu-id="2b319-143">指示是否将意向分配给用户</span><span class="sxs-lookup"><span data-stu-id="2b319-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="2b319-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b319-144">lastModifiedDateTime</span></span>|<span data-ttu-id="2b319-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b319-145">DateTimeOffset</span></span>|<span data-ttu-id="2b319-146">上次修改意向的时间</span><span class="sxs-lookup"><span data-stu-id="2b319-146">When the intent was last modified</span></span>|
|<span data-ttu-id="2b319-147">templateId</span><span class="sxs-lookup"><span data-stu-id="2b319-147">templateId</span></span>|<span data-ttu-id="2b319-148">String</span><span class="sxs-lookup"><span data-stu-id="2b319-148">String</span></span>|<span data-ttu-id="2b319-149">创建此目的的模板的 ID (如果有)</span><span class="sxs-lookup"><span data-stu-id="2b319-149">The ID of the template this intent was created from (if any)</span></span>|



## <a name="response"></a><span data-ttu-id="2b319-150">响应</span><span class="sxs-lookup"><span data-stu-id="2b319-150">Response</span></span>
<span data-ttu-id="2b319-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b319-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b319-152">示例</span><span class="sxs-lookup"><span data-stu-id="2b319-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b319-153">请求</span><span class="sxs-lookup"><span data-stu-id="2b319-153">Request</span></span>
<span data-ttu-id="2b319-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b319-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
Content-type: application/json
Content-length: 204

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value"
}
```

### <a name="response"></a><span data-ttu-id="2b319-155">响应</span><span class="sxs-lookup"><span data-stu-id="2b319-155">Response</span></span>
<span data-ttu-id="2b319-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b319-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 317

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value"
}
```




