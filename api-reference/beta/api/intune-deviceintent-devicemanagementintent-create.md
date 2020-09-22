---
title: 创建 deviceManagementIntent
description: 创建新的 deviceManagementIntent 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2a8e8847e57f9a79367ff848bb02be65ef5ee52
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000726"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="181b9-103">创建 deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="181b9-103">Create deviceManagementIntent</span></span>

<span data-ttu-id="181b9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="181b9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="181b9-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="181b9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="181b9-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="181b9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="181b9-107">创建新的 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="181b9-107">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="181b9-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="181b9-108">Prerequisites</span></span>
<span data-ttu-id="181b9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="181b9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="181b9-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="181b9-111">Permission type</span></span>|<span data-ttu-id="181b9-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="181b9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="181b9-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="181b9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="181b9-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181b9-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="181b9-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="181b9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="181b9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="181b9-116">Not supported.</span></span>|
|<span data-ttu-id="181b9-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="181b9-117">Application</span></span>|<span data-ttu-id="181b9-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="181b9-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="181b9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="181b9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="181b9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="181b9-120">Request headers</span></span>
|<span data-ttu-id="181b9-121">标头</span><span class="sxs-lookup"><span data-stu-id="181b9-121">Header</span></span>|<span data-ttu-id="181b9-122">值</span><span class="sxs-lookup"><span data-stu-id="181b9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="181b9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="181b9-123">Authorization</span></span>|<span data-ttu-id="181b9-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="181b9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="181b9-125">接受</span><span class="sxs-lookup"><span data-stu-id="181b9-125">Accept</span></span>|<span data-ttu-id="181b9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="181b9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="181b9-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="181b9-127">Request body</span></span>
<span data-ttu-id="181b9-128">在请求正文中，提供 deviceManagementIntent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="181b9-128">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="181b9-129">下表显示创建 deviceManagementIntent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="181b9-129">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="181b9-130">属性</span><span class="sxs-lookup"><span data-stu-id="181b9-130">Property</span></span>|<span data-ttu-id="181b9-131">类型</span><span class="sxs-lookup"><span data-stu-id="181b9-131">Type</span></span>|<span data-ttu-id="181b9-132">说明</span><span class="sxs-lookup"><span data-stu-id="181b9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="181b9-133">id</span><span class="sxs-lookup"><span data-stu-id="181b9-133">id</span></span>|<span data-ttu-id="181b9-134">String</span><span class="sxs-lookup"><span data-stu-id="181b9-134">String</span></span>|<span data-ttu-id="181b9-135">意向 ID</span><span class="sxs-lookup"><span data-stu-id="181b9-135">The intent ID</span></span>|
|<span data-ttu-id="181b9-136">displayName</span><span class="sxs-lookup"><span data-stu-id="181b9-136">displayName</span></span>|<span data-ttu-id="181b9-137">String</span><span class="sxs-lookup"><span data-stu-id="181b9-137">String</span></span>|<span data-ttu-id="181b9-138">用户给定的显示名称</span><span class="sxs-lookup"><span data-stu-id="181b9-138">The user given display name</span></span>|
|<span data-ttu-id="181b9-139">description</span><span class="sxs-lookup"><span data-stu-id="181b9-139">description</span></span>|<span data-ttu-id="181b9-140">String</span><span class="sxs-lookup"><span data-stu-id="181b9-140">String</span></span>|<span data-ttu-id="181b9-141">用户提供的说明</span><span class="sxs-lookup"><span data-stu-id="181b9-141">The user given description</span></span>|
|<span data-ttu-id="181b9-142">isAssigned</span><span class="sxs-lookup"><span data-stu-id="181b9-142">isAssigned</span></span>|<span data-ttu-id="181b9-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="181b9-143">Boolean</span></span>|<span data-ttu-id="181b9-144">指示是否将意向分配给用户</span><span class="sxs-lookup"><span data-stu-id="181b9-144">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="181b9-145">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="181b9-145">lastModifiedDateTime</span></span>|<span data-ttu-id="181b9-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="181b9-146">DateTimeOffset</span></span>|<span data-ttu-id="181b9-147">上次修改意向的时间</span><span class="sxs-lookup"><span data-stu-id="181b9-147">When the intent was last modified</span></span>|
|<span data-ttu-id="181b9-148">templateId</span><span class="sxs-lookup"><span data-stu-id="181b9-148">templateId</span></span>|<span data-ttu-id="181b9-149">String</span><span class="sxs-lookup"><span data-stu-id="181b9-149">String</span></span>|<span data-ttu-id="181b9-150">如果任何) ，则从 (创建此意向的模板的 ID</span><span class="sxs-lookup"><span data-stu-id="181b9-150">The ID of the template this intent was created from (if any)</span></span>|
|<span data-ttu-id="181b9-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="181b9-151">roleScopeTagIds</span></span>|<span data-ttu-id="181b9-152">String collection</span><span class="sxs-lookup"><span data-stu-id="181b9-152">String collection</span></span>|<span data-ttu-id="181b9-153">此实体实例的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="181b9-153">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="181b9-154">响应</span><span class="sxs-lookup"><span data-stu-id="181b9-154">Response</span></span>
<span data-ttu-id="181b9-155">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="181b9-155">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="181b9-156">示例</span><span class="sxs-lookup"><span data-stu-id="181b9-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="181b9-157">请求</span><span class="sxs-lookup"><span data-stu-id="181b9-157">Request</span></span>
<span data-ttu-id="181b9-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="181b9-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents
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

### <a name="response"></a><span data-ttu-id="181b9-159">响应</span><span class="sxs-lookup"><span data-stu-id="181b9-159">Response</span></span>
<span data-ttu-id="181b9-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="181b9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






