---
title: 更新 deviceManagementIntent
description: 更新 deviceManagementIntent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d73b31e74b56355e46f79ff9c5961f605f2f4fc
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523978"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="04089-103">更新 deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="04089-103">Update deviceManagementIntent</span></span>

> <span data-ttu-id="04089-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04089-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04089-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04089-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04089-106">更新[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04089-106">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04089-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="04089-107">Prerequisites</span></span>
<span data-ttu-id="04089-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04089-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04089-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="04089-110">Permission type</span></span>|<span data-ttu-id="04089-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04089-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04089-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04089-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04089-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04089-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04089-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04089-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04089-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="04089-115">Not supported.</span></span>|
|<span data-ttu-id="04089-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="04089-116">Application</span></span>|<span data-ttu-id="04089-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="04089-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04089-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04089-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="04089-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="04089-119">Request headers</span></span>
|<span data-ttu-id="04089-120">标头</span><span class="sxs-lookup"><span data-stu-id="04089-120">Header</span></span>|<span data-ttu-id="04089-121">值</span><span class="sxs-lookup"><span data-stu-id="04089-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04089-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04089-122">Authorization</span></span>|<span data-ttu-id="04089-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04089-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04089-124">接受</span><span class="sxs-lookup"><span data-stu-id="04089-124">Accept</span></span>|<span data-ttu-id="04089-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04089-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04089-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="04089-126">Request body</span></span>
<span data-ttu-id="04089-127">在请求正文中, 提供[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04089-127">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="04089-128">下表显示创建[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="04089-128">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="04089-129">属性</span><span class="sxs-lookup"><span data-stu-id="04089-129">Property</span></span>|<span data-ttu-id="04089-130">类型</span><span class="sxs-lookup"><span data-stu-id="04089-130">Type</span></span>|<span data-ttu-id="04089-131">说明</span><span class="sxs-lookup"><span data-stu-id="04089-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04089-132">id</span><span class="sxs-lookup"><span data-stu-id="04089-132">id</span></span>|<span data-ttu-id="04089-133">String</span><span class="sxs-lookup"><span data-stu-id="04089-133">String</span></span>|<span data-ttu-id="04089-134">意向 ID</span><span class="sxs-lookup"><span data-stu-id="04089-134">The intent ID</span></span>|
|<span data-ttu-id="04089-135">displayName</span><span class="sxs-lookup"><span data-stu-id="04089-135">displayName</span></span>|<span data-ttu-id="04089-136">String</span><span class="sxs-lookup"><span data-stu-id="04089-136">String</span></span>|<span data-ttu-id="04089-137">用户给定的显示名称</span><span class="sxs-lookup"><span data-stu-id="04089-137">The user given display name</span></span>|
|<span data-ttu-id="04089-138">description</span><span class="sxs-lookup"><span data-stu-id="04089-138">description</span></span>|<span data-ttu-id="04089-139">String</span><span class="sxs-lookup"><span data-stu-id="04089-139">String</span></span>|<span data-ttu-id="04089-140">用户提供的说明</span><span class="sxs-lookup"><span data-stu-id="04089-140">The user given description</span></span>|
|<span data-ttu-id="04089-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="04089-141">isAssigned</span></span>|<span data-ttu-id="04089-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="04089-142">Boolean</span></span>|<span data-ttu-id="04089-143">指示是否将意向分配给用户</span><span class="sxs-lookup"><span data-stu-id="04089-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="04089-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="04089-144">lastModifiedDateTime</span></span>|<span data-ttu-id="04089-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04089-145">DateTimeOffset</span></span>|<span data-ttu-id="04089-146">上次修改意向的时间</span><span class="sxs-lookup"><span data-stu-id="04089-146">When the intent was last modified</span></span>|
|<span data-ttu-id="04089-147">templateId</span><span class="sxs-lookup"><span data-stu-id="04089-147">templateId</span></span>|<span data-ttu-id="04089-148">String</span><span class="sxs-lookup"><span data-stu-id="04089-148">String</span></span>|<span data-ttu-id="04089-149">创建此目的的模板的 ID (如果有)</span><span class="sxs-lookup"><span data-stu-id="04089-149">The ID of the template this intent was created from (if any)</span></span>|



## <a name="response"></a><span data-ttu-id="04089-150">响应</span><span class="sxs-lookup"><span data-stu-id="04089-150">Response</span></span>
<span data-ttu-id="04089-151">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04089-151">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04089-152">示例</span><span class="sxs-lookup"><span data-stu-id="04089-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="04089-153">请求</span><span class="sxs-lookup"><span data-stu-id="04089-153">Request</span></span>
<span data-ttu-id="04089-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04089-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04089-155">响应</span><span class="sxs-lookup"><span data-stu-id="04089-155">Response</span></span>
<span data-ttu-id="04089-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04089-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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







