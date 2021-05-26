---
title: 创建 cloudPCConnectivityIssue
description: 创建新的 cloudPCConnectivityIssue 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e1d8701b0f9523c8232af5b847cdf98b5ef799e8
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665862"
---
# <a name="create-cloudpcconnectivityissue"></a><span data-ttu-id="e7c7a-103">创建 cloudPCConnectivityIssue</span><span class="sxs-lookup"><span data-stu-id="e7c7a-103">Create cloudPCConnectivityIssue</span></span>

<span data-ttu-id="e7c7a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7c7a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7c7a-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7c7a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7c7a-107">创建新的 [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-107">Create a new [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7c7a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7c7a-108">Prerequisites</span></span>
<span data-ttu-id="e7c7a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7c7a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7c7a-111">Permission type</span></span>|<span data-ttu-id="e7c7a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e7c7a-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7c7a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7c7a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7c7a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7c7a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e7c7a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7c7a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7c7a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-116">Not supported.</span></span>|
|<span data-ttu-id="e7c7a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7c7a-117">Application</span></span>|<span data-ttu-id="e7c7a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7c7a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7c7a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7c7a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cloudPCConnectivityIssues
```

## <a name="request-headers"></a><span data-ttu-id="e7c7a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7c7a-120">Request headers</span></span>
|<span data-ttu-id="e7c7a-121">标头</span><span class="sxs-lookup"><span data-stu-id="e7c7a-121">Header</span></span>|<span data-ttu-id="e7c7a-122">值</span><span class="sxs-lookup"><span data-stu-id="e7c7a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7c7a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7c7a-123">Authorization</span></span>|<span data-ttu-id="e7c7a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7c7a-125">接受</span><span class="sxs-lookup"><span data-stu-id="e7c7a-125">Accept</span></span>|<span data-ttu-id="e7c7a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7c7a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7c7a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7c7a-127">Request body</span></span>
<span data-ttu-id="e7c7a-128">在请求正文中，提供 cloudPCConnectivityIssue 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-128">In the request body, supply a JSON representation for the cloudPCConnectivityIssue object.</span></span>

<span data-ttu-id="e7c7a-129">下表显示创建 cloudPCConnectivityIssue 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-129">The following table shows the properties that are required when you create the cloudPCConnectivityIssue.</span></span>

|<span data-ttu-id="e7c7a-130">属性</span><span class="sxs-lookup"><span data-stu-id="e7c7a-130">Property</span></span>|<span data-ttu-id="e7c7a-131">类型</span><span class="sxs-lookup"><span data-stu-id="e7c7a-131">Type</span></span>|<span data-ttu-id="e7c7a-132">说明</span><span class="sxs-lookup"><span data-stu-id="e7c7a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7c7a-133">id</span><span class="sxs-lookup"><span data-stu-id="e7c7a-133">id</span></span>|<span data-ttu-id="e7c7a-134">String</span><span class="sxs-lookup"><span data-stu-id="e7c7a-134">String</span></span>|<span data-ttu-id="e7c7a-135">用户体验分析连接问题事件实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-135">The unique identifier of the user experience analytics connectivity issue event entity.</span></span>|
|<span data-ttu-id="e7c7a-136">deviceId</span><span class="sxs-lookup"><span data-stu-id="e7c7a-136">deviceId</span></span>|<span data-ttu-id="e7c7a-137">String</span><span class="sxs-lookup"><span data-stu-id="e7c7a-137">String</span></span>|<span data-ttu-id="e7c7a-138">与连接关联的设备的 Intune DeviceId。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-138">The Intune DeviceId of the device the connection is associated with.</span></span>|
|<span data-ttu-id="e7c7a-139">errorCode</span><span class="sxs-lookup"><span data-stu-id="e7c7a-139">errorCode</span></span>|<span data-ttu-id="e7c7a-140">String</span><span class="sxs-lookup"><span data-stu-id="e7c7a-140">String</span></span>|<span data-ttu-id="e7c7a-141">连接问题的错误代码。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-141">The error code of the connectivity issue.</span></span>|
|<span data-ttu-id="e7c7a-142">errorDateTime</span><span class="sxs-lookup"><span data-stu-id="e7c7a-142">errorDateTime</span></span>|<span data-ttu-id="e7c7a-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7c7a-143">DateTimeOffset</span></span>|<span data-ttu-id="e7c7a-144">连接启动的时间。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-144">The time that the connection initiated.</span></span> <span data-ttu-id="e7c7a-145">时间以 ISO 8601 格式显示，协调世界时 (UTC) 时间。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-145">The time is shown in ISO 8601 format and Coordinated Universal Time (UTC) time.</span></span>|
|<span data-ttu-id="e7c7a-146">userId</span><span class="sxs-lookup"><span data-stu-id="e7c7a-146">userId</span></span>|<span data-ttu-id="e7c7a-147">String</span><span class="sxs-lookup"><span data-stu-id="e7c7a-147">String</span></span>|<span data-ttu-id="e7c7a-148">初始化连接的用户的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-148">The unique id of user who initialize the connection.</span></span>|
|<span data-ttu-id="e7c7a-149">errorDescription</span><span class="sxs-lookup"><span data-stu-id="e7c7a-149">errorDescription</span></span>|<span data-ttu-id="e7c7a-150">String</span><span class="sxs-lookup"><span data-stu-id="e7c7a-150">String</span></span>|<span data-ttu-id="e7c7a-151">错误的详细说明。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-151">The detailed description of what went wrong.</span></span>|
|<span data-ttu-id="e7c7a-152">recommendedAction</span><span class="sxs-lookup"><span data-stu-id="e7c7a-152">recommendedAction</span></span>|<span data-ttu-id="e7c7a-153">String</span><span class="sxs-lookup"><span data-stu-id="e7c7a-153">String</span></span>|<span data-ttu-id="e7c7a-154">修复相应错误的推荐操作。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-154">The recommended action to fix the corresponding error.</span></span>|



## <a name="response"></a><span data-ttu-id="e7c7a-155">响应</span><span class="sxs-lookup"><span data-stu-id="e7c7a-155">Response</span></span>
<span data-ttu-id="e7c7a-156">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-156">If successful, this method returns a `201 Created` response code and a [cloudPCConnectivityIssue](../resources/intune-devices-cloudpcconnectivityissue.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7c7a-157">示例</span><span class="sxs-lookup"><span data-stu-id="e7c7a-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7c7a-158">请求</span><span class="sxs-lookup"><span data-stu-id="e7c7a-158">Request</span></span>
<span data-ttu-id="e7c7a-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cloudPCConnectivityIssues
Content-type: application/json
Content-length: 325

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```

### <a name="response"></a><span data-ttu-id="e7c7a-160">响应</span><span class="sxs-lookup"><span data-stu-id="e7c7a-160">Response</span></span>
<span data-ttu-id="e7c7a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7c7a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 374

{
  "@odata.type": "#microsoft.graph.cloudPCConnectivityIssue",
  "id": "e8e2bf5f-bf5f-e8e2-5fbf-e2e85fbfe2e8",
  "deviceId": "Device Id value",
  "errorCode": "Error Code value",
  "errorDateTime": "2016-12-31T23:58:20.6032957-08:00",
  "userId": "User Id value",
  "errorDescription": "Error Description value",
  "recommendedAction": "Recommended Action value"
}
```




