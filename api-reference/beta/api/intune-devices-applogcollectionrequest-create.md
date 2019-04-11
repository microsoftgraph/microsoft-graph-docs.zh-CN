---
title: 创建 appLogCollectionRequest
description: 创建新的 appLogCollectionRequest 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 716daa9f3abea68a86d9fc7947af5d9d5d2dbb91
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31792158"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="2b509-103">创建 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="2b509-103">Create appLogCollectionRequest</span></span>

> <span data-ttu-id="2b509-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2b509-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b509-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2b509-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b509-106">创建新的[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b509-106">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2b509-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2b509-107">Prerequisites</span></span>
<span data-ttu-id="2b509-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b509-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b509-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b509-110">Permission type</span></span>|<span data-ttu-id="2b509-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2b509-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b509-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b509-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2b509-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b509-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2b509-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b509-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b509-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b509-115">Not supported.</span></span>|
|<span data-ttu-id="2b509-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b509-116">Application</span></span>|<span data-ttu-id="2b509-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b509-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b509-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b509-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="2b509-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b509-119">Request headers</span></span>
|<span data-ttu-id="2b509-120">标头</span><span class="sxs-lookup"><span data-stu-id="2b509-120">Header</span></span>|<span data-ttu-id="2b509-121">值</span><span class="sxs-lookup"><span data-stu-id="2b509-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b509-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b509-122">Authorization</span></span>|<span data-ttu-id="2b509-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2b509-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b509-124">接受</span><span class="sxs-lookup"><span data-stu-id="2b509-124">Accept</span></span>|<span data-ttu-id="2b509-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2b509-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b509-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b509-126">Request body</span></span>
<span data-ttu-id="2b509-127">在请求正文中, 提供 appLogCollectionRequest 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2b509-127">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="2b509-128">下表显示创建 appLogCollectionRequest 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2b509-128">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="2b509-129">属性</span><span class="sxs-lookup"><span data-stu-id="2b509-129">Property</span></span>|<span data-ttu-id="2b509-130">类型</span><span class="sxs-lookup"><span data-stu-id="2b509-130">Type</span></span>|<span data-ttu-id="2b509-131">说明</span><span class="sxs-lookup"><span data-stu-id="2b509-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b509-132">id</span><span class="sxs-lookup"><span data-stu-id="2b509-132">id</span></span>|<span data-ttu-id="2b509-133">String</span><span class="sxs-lookup"><span data-stu-id="2b509-133">String</span></span>|<span data-ttu-id="2b509-134">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2b509-134">The unique Identifier.</span></span> <span data-ttu-id="2b509-135">这是 userId_DeviceId_AppId id。</span><span class="sxs-lookup"><span data-stu-id="2b509-135">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="2b509-136">status</span><span class="sxs-lookup"><span data-stu-id="2b509-136">status</span></span>|[<span data-ttu-id="2b509-137">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="2b509-137">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="2b509-138">日志上载状态。</span><span class="sxs-lookup"><span data-stu-id="2b509-138">Log upload status.</span></span> <span data-ttu-id="2b509-139">可取值为：`pending`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="2b509-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="2b509-140">errorMessage</span><span class="sxs-lookup"><span data-stu-id="2b509-140">errorMessage</span></span>|<span data-ttu-id="2b509-141">String</span><span class="sxs-lookup"><span data-stu-id="2b509-141">String</span></span>|<span data-ttu-id="2b509-142">在上载过程中出现的错误消息</span><span class="sxs-lookup"><span data-stu-id="2b509-142">Error message if any during the upload process</span></span>|
|<span data-ttu-id="2b509-143">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="2b509-143">customLogFolders</span></span>|<span data-ttu-id="2b509-144">String 集合</span><span class="sxs-lookup"><span data-stu-id="2b509-144">String collection</span></span>|<span data-ttu-id="2b509-145">日志文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="2b509-145">List of log folders.</span></span> |
|<span data-ttu-id="2b509-146">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2b509-146">completedDateTime</span></span>|<span data-ttu-id="2b509-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b509-147">DateTimeOffset</span></span>|<span data-ttu-id="2b509-148">上传日志请求到达终端状态的时间</span><span class="sxs-lookup"><span data-stu-id="2b509-148">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="2b509-149">响应</span><span class="sxs-lookup"><span data-stu-id="2b509-149">Response</span></span>
<span data-ttu-id="2b509-150">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2b509-150">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b509-151">示例</span><span class="sxs-lookup"><span data-stu-id="2b509-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="2b509-152">请求</span><span class="sxs-lookup"><span data-stu-id="2b509-152">Request</span></span>
<span data-ttu-id="2b509-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2b509-153">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
Content-type: application/json
Content-length: 257

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```

### <a name="response"></a><span data-ttu-id="2b509-154">响应</span><span class="sxs-lookup"><span data-stu-id="2b509-154">Response</span></span>
<span data-ttu-id="2b509-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2b509-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 306

{
  "@odata.type": "#microsoft.graph.appLogCollectionRequest",
  "id": "cca685ff-85ff-cca6-ff85-a6ccff85a6cc",
  "status": "completed",
  "errorMessage": "Error Message value",
  "customLogFolders": [
    "Custom Log Folders value"
  ],
  "completedDateTime": "2016-12-31T23:58:52.3534526-08:00"
}
```





