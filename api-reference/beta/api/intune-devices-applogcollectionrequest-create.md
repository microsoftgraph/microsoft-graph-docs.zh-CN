---
title: 创建 appLogCollectionRequest
description: 创建新的 appLogCollectionRequest 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dbd19f042c6dbfe80a4c02ec224fde5b1e5fb696
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136480"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="6528d-103">创建 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="6528d-103">Create appLogCollectionRequest</span></span>

<span data-ttu-id="6528d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6528d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6528d-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6528d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6528d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6528d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6528d-107">创建新的 [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6528d-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6528d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6528d-108">Prerequisites</span></span>
<span data-ttu-id="6528d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6528d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6528d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6528d-111">Permission type</span></span>|<span data-ttu-id="6528d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6528d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6528d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6528d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6528d-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6528d-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6528d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6528d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6528d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6528d-116">Not supported.</span></span>|
|<span data-ttu-id="6528d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6528d-117">Application</span></span>|<span data-ttu-id="6528d-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6528d-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6528d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6528d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="6528d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6528d-120">Request headers</span></span>
|<span data-ttu-id="6528d-121">标头</span><span class="sxs-lookup"><span data-stu-id="6528d-121">Header</span></span>|<span data-ttu-id="6528d-122">值</span><span class="sxs-lookup"><span data-stu-id="6528d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6528d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6528d-123">Authorization</span></span>|<span data-ttu-id="6528d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6528d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6528d-125">接受</span><span class="sxs-lookup"><span data-stu-id="6528d-125">Accept</span></span>|<span data-ttu-id="6528d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6528d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6528d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6528d-127">Request body</span></span>
<span data-ttu-id="6528d-128">在请求正文中，提供 appLogCollectionRequest 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6528d-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="6528d-129">下表显示创建 appLogCollectionRequest 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6528d-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="6528d-130">属性</span><span class="sxs-lookup"><span data-stu-id="6528d-130">Property</span></span>|<span data-ttu-id="6528d-131">类型</span><span class="sxs-lookup"><span data-stu-id="6528d-131">Type</span></span>|<span data-ttu-id="6528d-132">说明</span><span class="sxs-lookup"><span data-stu-id="6528d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6528d-133">id</span><span class="sxs-lookup"><span data-stu-id="6528d-133">id</span></span>|<span data-ttu-id="6528d-134">String</span><span class="sxs-lookup"><span data-stu-id="6528d-134">String</span></span>|<span data-ttu-id="6528d-135">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6528d-135">The unique Identifier.</span></span> <span data-ttu-id="6528d-136">这是userId_DeviceId_AppId ID。</span><span class="sxs-lookup"><span data-stu-id="6528d-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="6528d-137">状态</span><span class="sxs-lookup"><span data-stu-id="6528d-137">status</span></span>|[<span data-ttu-id="6528d-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="6528d-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="6528d-139">记录上载状态。</span><span class="sxs-lookup"><span data-stu-id="6528d-139">Log upload status.</span></span> <span data-ttu-id="6528d-140">可取值为：`pending`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="6528d-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="6528d-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="6528d-141">errorMessage</span></span>|<span data-ttu-id="6528d-142">String</span><span class="sxs-lookup"><span data-stu-id="6528d-142">String</span></span>|<span data-ttu-id="6528d-143">上传过程中出现错误消息（如果有）</span><span class="sxs-lookup"><span data-stu-id="6528d-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="6528d-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="6528d-144">customLogFolders</span></span>|<span data-ttu-id="6528d-145">String collection</span><span class="sxs-lookup"><span data-stu-id="6528d-145">String collection</span></span>|<span data-ttu-id="6528d-146">日志文件夹列表。</span><span class="sxs-lookup"><span data-stu-id="6528d-146">List of log folders.</span></span> |
|<span data-ttu-id="6528d-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="6528d-147">completedDateTime</span></span>|<span data-ttu-id="6528d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6528d-148">DateTimeOffset</span></span>|<span data-ttu-id="6528d-149">上载日志请求达到终端状态的时间</span><span class="sxs-lookup"><span data-stu-id="6528d-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="6528d-150">响应</span><span class="sxs-lookup"><span data-stu-id="6528d-150">Response</span></span>
<span data-ttu-id="6528d-151">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6528d-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6528d-152">示例</span><span class="sxs-lookup"><span data-stu-id="6528d-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="6528d-153">请求</span><span class="sxs-lookup"><span data-stu-id="6528d-153">Request</span></span>
<span data-ttu-id="6528d-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6528d-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6528d-155">响应</span><span class="sxs-lookup"><span data-stu-id="6528d-155">Response</span></span>
<span data-ttu-id="6528d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6528d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




