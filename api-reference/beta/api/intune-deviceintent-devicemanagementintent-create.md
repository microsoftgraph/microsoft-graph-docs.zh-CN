---
title: 创建 deviceManagementIntent
description: 创建新的 deviceManagementIntent 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b4f3fa68dada15f80592ae771f0cd1854b7e4b62
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33916370"
---
# <a name="create-devicemanagementintent"></a><span data-ttu-id="b00fa-103">创建 deviceManagementIntent</span><span class="sxs-lookup"><span data-stu-id="b00fa-103">Create deviceManagementIntent</span></span>

> <span data-ttu-id="b00fa-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b00fa-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b00fa-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b00fa-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b00fa-106">创建新的[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b00fa-106">Create a new [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b00fa-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b00fa-107">Prerequisites</span></span>
<span data-ttu-id="b00fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b00fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b00fa-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b00fa-110">Permission type</span></span>|<span data-ttu-id="b00fa-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b00fa-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b00fa-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b00fa-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b00fa-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b00fa-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b00fa-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b00fa-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b00fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b00fa-115">Not supported.</span></span>|
|<span data-ttu-id="b00fa-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b00fa-116">Application</span></span>|<span data-ttu-id="b00fa-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b00fa-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b00fa-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b00fa-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/intents
```

## <a name="request-headers"></a><span data-ttu-id="b00fa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b00fa-119">Request headers</span></span>
|<span data-ttu-id="b00fa-120">标头</span><span class="sxs-lookup"><span data-stu-id="b00fa-120">Header</span></span>|<span data-ttu-id="b00fa-121">值</span><span class="sxs-lookup"><span data-stu-id="b00fa-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b00fa-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b00fa-122">Authorization</span></span>|<span data-ttu-id="b00fa-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b00fa-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b00fa-124">接受</span><span class="sxs-lookup"><span data-stu-id="b00fa-124">Accept</span></span>|<span data-ttu-id="b00fa-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b00fa-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b00fa-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b00fa-126">Request body</span></span>
<span data-ttu-id="b00fa-127">在请求正文中, 提供 deviceManagementIntent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b00fa-127">In the request body, supply a JSON representation for the deviceManagementIntent object.</span></span>

<span data-ttu-id="b00fa-128">下表显示创建 deviceManagementIntent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b00fa-128">The following table shows the properties that are required when you create the deviceManagementIntent.</span></span>

|<span data-ttu-id="b00fa-129">属性</span><span class="sxs-lookup"><span data-stu-id="b00fa-129">Property</span></span>|<span data-ttu-id="b00fa-130">类型</span><span class="sxs-lookup"><span data-stu-id="b00fa-130">Type</span></span>|<span data-ttu-id="b00fa-131">说明</span><span class="sxs-lookup"><span data-stu-id="b00fa-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b00fa-132">id</span><span class="sxs-lookup"><span data-stu-id="b00fa-132">id</span></span>|<span data-ttu-id="b00fa-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b00fa-133">String</span></span>|<span data-ttu-id="b00fa-134">意向 ID</span><span class="sxs-lookup"><span data-stu-id="b00fa-134">The intent ID</span></span>|
|<span data-ttu-id="b00fa-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b00fa-135">displayName</span></span>|<span data-ttu-id="b00fa-136">String</span><span class="sxs-lookup"><span data-stu-id="b00fa-136">String</span></span>|<span data-ttu-id="b00fa-137">用户给定的显示名称</span><span class="sxs-lookup"><span data-stu-id="b00fa-137">The user given display name</span></span>|
|<span data-ttu-id="b00fa-138">说明</span><span class="sxs-lookup"><span data-stu-id="b00fa-138">description</span></span>|<span data-ttu-id="b00fa-139">String</span><span class="sxs-lookup"><span data-stu-id="b00fa-139">String</span></span>|<span data-ttu-id="b00fa-140">用户提供的说明</span><span class="sxs-lookup"><span data-stu-id="b00fa-140">The user given description</span></span>|
|<span data-ttu-id="b00fa-141">isAssigned</span><span class="sxs-lookup"><span data-stu-id="b00fa-141">isAssigned</span></span>|<span data-ttu-id="b00fa-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="b00fa-142">Boolean</span></span>|<span data-ttu-id="b00fa-143">指示是否将意向分配给用户</span><span class="sxs-lookup"><span data-stu-id="b00fa-143">Signifies whether or not the intent is assigned to users</span></span>|
|<span data-ttu-id="b00fa-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b00fa-144">lastModifiedDateTime</span></span>|<span data-ttu-id="b00fa-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b00fa-145">DateTimeOffset</span></span>|<span data-ttu-id="b00fa-146">上次修改意向的时间</span><span class="sxs-lookup"><span data-stu-id="b00fa-146">When the intent was last modified</span></span>|
|<span data-ttu-id="b00fa-147">templateId</span><span class="sxs-lookup"><span data-stu-id="b00fa-147">templateId</span></span>|<span data-ttu-id="b00fa-148">String</span><span class="sxs-lookup"><span data-stu-id="b00fa-148">String</span></span>|<span data-ttu-id="b00fa-149">创建此目的的模板的 ID (如果有)</span><span class="sxs-lookup"><span data-stu-id="b00fa-149">The ID of the template this intent was created from (if any)</span></span>|



## <a name="response"></a><span data-ttu-id="b00fa-150">响应</span><span class="sxs-lookup"><span data-stu-id="b00fa-150">Response</span></span>
<span data-ttu-id="b00fa-151">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b00fa-151">If successful, this method returns a `201 Created` response code and a [deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b00fa-152">示例</span><span class="sxs-lookup"><span data-stu-id="b00fa-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="b00fa-153">请求</span><span class="sxs-lookup"><span data-stu-id="b00fa-153">Request</span></span>
<span data-ttu-id="b00fa-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b00fa-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/intents
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

### <a name="response"></a><span data-ttu-id="b00fa-155">响应</span><span class="sxs-lookup"><span data-stu-id="b00fa-155">Response</span></span>
<span data-ttu-id="b00fa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b00fa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




