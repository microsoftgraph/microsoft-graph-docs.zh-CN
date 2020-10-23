---
title: 更新 deviceManagementIntent
description: 更新 deviceManagementIntent 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b02c9704ba118c19290f557913d6fd44f4ac0b04
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734495"
---
# <a name="update-devicemanagementintent"></a><span data-ttu-id="29481-103">更新 deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="29481-103">Update deviceManagementIntent</span></span>

<span data-ttu-id="29481-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29481-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="29481-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="29481-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="29481-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="29481-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="29481-107">更新 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="29481-107">Update the properties of a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="29481-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="29481-108">Prerequisites</span></span>
<span data-ttu-id="29481-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29481-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29481-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="29481-111">Permission type</span></span>|<span data-ttu-id="29481-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="29481-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="29481-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29481-113">Delegated (work or school account)</span></span>|<span data-ttu-id="29481-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29481-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="29481-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29481-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="29481-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="29481-116">Not supported.</span></span>|
|<span data-ttu-id="29481-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="29481-117">Application</span></span>|<span data-ttu-id="29481-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="29481-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="29481-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29481-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/intents/{deviceManagementIntentId}
```

## <a name="request-headers"></a><span data-ttu-id="29481-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="29481-120">Request headers</span></span>
|<span data-ttu-id="29481-121">标头</span><span class="sxs-lookup"><span data-stu-id="29481-121">Header</span></span>|<span data-ttu-id="29481-122">值</span><span class="sxs-lookup"><span data-stu-id="29481-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="29481-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="29481-123">Authorization</span></span>|<span data-ttu-id="29481-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="29481-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="29481-125">接受</span><span class="sxs-lookup"><span data-stu-id="29481-125">Accept</span></span>|<span data-ttu-id="29481-126">application/json</span><span class="sxs-lookup"><span data-stu-id="29481-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="29481-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="29481-127">Request body</span></span>
<span data-ttu-id="29481-128">在请求正文中，提供 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29481-128">In the request body, supply a JSON representation for the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

<span data-ttu-id="29481-129">下表显示创建 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="29481-129">The following table shows the properties that are required when you create the [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md).</span></span>

|<span data-ttu-id="29481-130">属性</span><span class="sxs-lookup"><span data-stu-id="29481-130">Property</span></span>|<span data-ttu-id="29481-131">类型</span><span class="sxs-lookup"><span data-stu-id="29481-131">Type</span></span>|<span data-ttu-id="29481-132">说明</span><span class="sxs-lookup"><span data-stu-id="29481-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="29481-133">id</span><span class="sxs-lookup"><span data-stu-id="29481-133">id</span></span>|<span data-ttu-id="29481-134">String</span><span class="sxs-lookup"><span data-stu-id="29481-134">String</span></span>|<span data-ttu-id="29481-135">意向 ID</span><span class="sxs-lookup"><span data-stu-id="29481-135">The intent ID</span></span>|
|<span data-ttu-id="29481-136">displayName</span><span class="sxs-lookup"><span data-stu-id="29481-136">displayName</span></span>|<span data-ttu-id="29481-137">String</span><span class="sxs-lookup"><span data-stu-id="29481-137">String</span></span>|<span data-ttu-id="29481-138">用户给定的显示名称</span><span class="sxs-lookup"><span data-stu-id="29481-138">The user given display name</span></span>|
|<span data-ttu-id="29481-139">说明</span><span class="sxs-lookup"><span data-stu-id="29481-139">description</span></span>|<span data-ttu-id="29481-140">String</span><span class="sxs-lookup"><span data-stu-id="29481-140">String</span></span>|<span data-ttu-id="29481-141">用户提供的说明</span><span class="sxs-lookup"><span data-stu-id="29481-141">The user given description</span></span>|
|<span data-ttu-id="29481-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="29481-142">isAssigned</span></span>|<span data-ttu-id="29481-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="29481-143">Boolean</span></span>|<span data-ttu-id="29481-144">指示是否将意向分配给用户</span><span class="sxs-lookup"><span data-stu-id="29481-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="29481-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="29481-145">lastModifiedDateTime</span></span>|<span data-ttu-id="29481-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="29481-146">DateTimeOffset</span></span>|<span data-ttu-id="29481-147">上次修改意向的时间</span><span class="sxs-lookup"><span data-stu-id="29481-147">When the intent was last modified</span></span>|
|<span data-ttu-id="29481-148">templateId</span><span class="sxs-lookup"><span data-stu-id="29481-148">templateId</span></span>|<span data-ttu-id="29481-149">String</span><span class="sxs-lookup"><span data-stu-id="29481-149">String</span></span>|<span data-ttu-id="29481-150">如果任何) ，则从 (创建此意向的模板的 ID</span><span class="sxs-lookup"><span data-stu-id="29481-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="29481-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="29481-151">roleScopeTagIds</span></span>|<span data-ttu-id="29481-152">String collection</span><span class="sxs-lookup"><span data-stu-id="29481-152">String collection</span></span>|<span data-ttu-id="29481-153">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="29481-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="29481-154">响应</span><span class="sxs-lookup"><span data-stu-id="29481-154">Response</span></span>
<span data-ttu-id="29481-155">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="29481-155">If successful, this method returns a `200 OK` response code and an updated [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29481-156">示例</span><span class="sxs-lookup"><span data-stu-id="29481-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="29481-157">请求</span><span class="sxs-lookup"><span data-stu-id="29481-157">Request</span></span>
<span data-ttu-id="29481-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="29481-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="29481-159">响应</span><span class="sxs-lookup"><span data-stu-id="29481-159">Response</span></span>
<span data-ttu-id="29481-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="29481-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





