---
title: 更新 deviceManagementIntent
description: 更新 deviceManagementIntent 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 606fb1eeb718e80aaef5e966f6cac29d79a980ca
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42471188"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="34140-103">更新 deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="34140-103">Update deviceManagementIntent</span></span>

<span data-ttu-id="34140-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="34140-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34140-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="34140-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34140-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="34140-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34140-107">更新[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="34140-107">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34140-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="34140-108">Prerequisites</span></span>
<span data-ttu-id="34140-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="34140-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34140-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="34140-111">Permission type</span></span>|<span data-ttu-id="34140-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="34140-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34140-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="34140-113">Delegated (work or school account)</span></span>|<span data-ttu-id="34140-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34140-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34140-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="34140-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34140-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="34140-116">Not supported.</span></span>|
|<span data-ttu-id="34140-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="34140-117">Application</span></span>|<span data-ttu-id="34140-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34140-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="34140-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="34140-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="34140-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="34140-120">Request headers</span></span>
|<span data-ttu-id="34140-121">标头</span><span class="sxs-lookup"><span data-stu-id="34140-121">Header</span></span>|<span data-ttu-id="34140-122">值</span><span class="sxs-lookup"><span data-stu-id="34140-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34140-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="34140-123">Authorization</span></span>|<span data-ttu-id="34140-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="34140-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34140-125">接受</span><span class="sxs-lookup"><span data-stu-id="34140-125">Accept</span></span>|<span data-ttu-id="34140-126">application/json</span><span class="sxs-lookup"><span data-stu-id="34140-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34140-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="34140-127">Request body</span></span>
<span data-ttu-id="34140-128">在请求正文中，提供[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="34140-128">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="34140-129">下表显示创建[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="34140-129">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="34140-130">属性</span><span class="sxs-lookup"><span data-stu-id="34140-130">Property</span></span>|<span data-ttu-id="34140-131">类型</span><span class="sxs-lookup"><span data-stu-id="34140-131">Type</span></span>|<span data-ttu-id="34140-132">说明</span><span class="sxs-lookup"><span data-stu-id="34140-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34140-133">id</span><span class="sxs-lookup"><span data-stu-id="34140-133">id</span></span>|<span data-ttu-id="34140-134">字符串</span><span class="sxs-lookup"><span data-stu-id="34140-134">String</span></span>|<span data-ttu-id="34140-135">意向 ID</span><span class="sxs-lookup"><span data-stu-id="34140-135">The intent ID</span></span>|
|<span data-ttu-id="34140-136">displayName</span><span class="sxs-lookup"><span data-stu-id="34140-136">displayName</span></span>|<span data-ttu-id="34140-137">String</span><span class="sxs-lookup"><span data-stu-id="34140-137">String</span></span>|<span data-ttu-id="34140-138">用户给定的显示名称</span><span class="sxs-lookup"><span data-stu-id="34140-138">The user given display name</span></span>|
|<span data-ttu-id="34140-139">说明</span><span class="sxs-lookup"><span data-stu-id="34140-139">description</span></span>|<span data-ttu-id="34140-140">String</span><span class="sxs-lookup"><span data-stu-id="34140-140">String</span></span>|<span data-ttu-id="34140-141">用户提供的说明</span><span class="sxs-lookup"><span data-stu-id="34140-141">The user given description</span></span>|
|<span data-ttu-id="34140-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="34140-142">isAssigned</span></span>|<span data-ttu-id="34140-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="34140-143">Boolean</span></span>|<span data-ttu-id="34140-144">指示是否将意向分配给用户</span><span class="sxs-lookup"><span data-stu-id="34140-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="34140-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34140-145">lastModifiedDateTime</span></span>|<span data-ttu-id="34140-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34140-146">DateTimeOffset</span></span>|<span data-ttu-id="34140-147">上次修改意向的时间</span><span class="sxs-lookup"><span data-stu-id="34140-147">When the intent was last modified</span></span>|
|<span data-ttu-id="34140-148">templateId</span><span class="sxs-lookup"><span data-stu-id="34140-148">templateId</span></span>|<span data-ttu-id="34140-149">String</span><span class="sxs-lookup"><span data-stu-id="34140-149">String</span></span>|<span data-ttu-id="34140-150">创建此目的的模板的 ID （如果有）</span><span class="sxs-lookup"><span data-stu-id="34140-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="34140-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="34140-151">roleScopeTagIds</span></span>|<span data-ttu-id="34140-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="34140-152">String collection</span></span>|<span data-ttu-id="34140-153">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="34140-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="34140-154">响应</span><span class="sxs-lookup"><span data-stu-id="34140-154">Response</span></span>
<span data-ttu-id="34140-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="34140-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34140-156">示例</span><span class="sxs-lookup"><span data-stu-id="34140-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="34140-157">请求</span><span class="sxs-lookup"><span data-stu-id="34140-157">Request</span></span>
<span data-ttu-id="34140-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="34140-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="34140-159">响应</span><span class="sxs-lookup"><span data-stu-id="34140-159">Response</span></span>
<span data-ttu-id="34140-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="34140-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.deviceManagementIntent",
  "id": "f972c33e-c33e-f972-3ec3-72f93ec372f9",
  "displayName": "Display Name value",
  "description": "Description value",
  "isAssigned": true,
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "templateId": "Template Id value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





