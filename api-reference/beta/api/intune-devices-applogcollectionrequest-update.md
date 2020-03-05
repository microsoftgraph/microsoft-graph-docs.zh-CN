---
title: 更新 appLogCollectionRequest
description: 更新 appLogCollectionRequest 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aae8ff4beb63b9af188ec84cca0554e244b45156
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42469942"
---
# <a name="update-applogcollectionrequest"></a><span data-ttu-id="2a27a-103">更新 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="2a27a-103">Update appLogCollectionRequest</span></span>

<span data-ttu-id="2a27a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2a27a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a27a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a27a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a27a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a27a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a27a-107">更新[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2a27a-107">Update the properties of a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a27a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a27a-108">Prerequisites</span></span>
<span data-ttu-id="2a27a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a27a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a27a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a27a-111">Permission type</span></span>|<span data-ttu-id="2a27a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2a27a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a27a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a27a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a27a-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a27a-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="2a27a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a27a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a27a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a27a-116">Not supported.</span></span>|
|<span data-ttu-id="2a27a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a27a-117">Application</span></span>|<span data-ttu-id="2a27a-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a27a-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a27a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a27a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
```

## <a name="request-headers"></a><span data-ttu-id="2a27a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a27a-120">Request headers</span></span>
|<span data-ttu-id="2a27a-121">标头</span><span class="sxs-lookup"><span data-stu-id="2a27a-121">Header</span></span>|<span data-ttu-id="2a27a-122">值</span><span class="sxs-lookup"><span data-stu-id="2a27a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a27a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a27a-123">Authorization</span></span>|<span data-ttu-id="2a27a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a27a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a27a-125">接受</span><span class="sxs-lookup"><span data-stu-id="2a27a-125">Accept</span></span>|<span data-ttu-id="2a27a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a27a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a27a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a27a-127">Request body</span></span>
<span data-ttu-id="2a27a-128">在请求正文中，提供[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a27a-128">In the request body, supply a JSON representation for the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

<span data-ttu-id="2a27a-129">下表显示创建[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2a27a-129">The following table shows the properties that are required when you create the [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md).</span></span>

|<span data-ttu-id="2a27a-130">属性</span><span class="sxs-lookup"><span data-stu-id="2a27a-130">Property</span></span>|<span data-ttu-id="2a27a-131">类型</span><span class="sxs-lookup"><span data-stu-id="2a27a-131">Type</span></span>|<span data-ttu-id="2a27a-132">说明</span><span class="sxs-lookup"><span data-stu-id="2a27a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a27a-133">id</span><span class="sxs-lookup"><span data-stu-id="2a27a-133">id</span></span>|<span data-ttu-id="2a27a-134">String</span><span class="sxs-lookup"><span data-stu-id="2a27a-134">String</span></span>|<span data-ttu-id="2a27a-135">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="2a27a-135">The unique Identifier.</span></span> <span data-ttu-id="2a27a-136">这是 userId_DeviceId_AppId id。</span><span class="sxs-lookup"><span data-stu-id="2a27a-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="2a27a-137">status</span><span class="sxs-lookup"><span data-stu-id="2a27a-137">status</span></span>|[<span data-ttu-id="2a27a-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="2a27a-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="2a27a-139">日志上载状态。</span><span class="sxs-lookup"><span data-stu-id="2a27a-139">Log upload status.</span></span> <span data-ttu-id="2a27a-140">可取值为：`pending`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="2a27a-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="2a27a-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="2a27a-141">errorMessage</span></span>|<span data-ttu-id="2a27a-142">String</span><span class="sxs-lookup"><span data-stu-id="2a27a-142">String</span></span>|<span data-ttu-id="2a27a-143">在上载过程中出现的错误消息</span><span class="sxs-lookup"><span data-stu-id="2a27a-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="2a27a-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="2a27a-144">customLogFolders</span></span>|<span data-ttu-id="2a27a-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="2a27a-145">String collection</span></span>|<span data-ttu-id="2a27a-146">日志文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="2a27a-146">List of log folders.</span></span> |
|<span data-ttu-id="2a27a-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="2a27a-147">completedDateTime</span></span>|<span data-ttu-id="2a27a-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2a27a-148">DateTimeOffset</span></span>|<span data-ttu-id="2a27a-149">上传日志请求到达终端状态的时间</span><span class="sxs-lookup"><span data-stu-id="2a27a-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="2a27a-150">响应</span><span class="sxs-lookup"><span data-stu-id="2a27a-150">Response</span></span>
<span data-ttu-id="2a27a-151">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a27a-151">If successful, this method returns a `200 OK` response code and an updated [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a27a-152">示例</span><span class="sxs-lookup"><span data-stu-id="2a27a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a27a-153">请求</span><span class="sxs-lookup"><span data-stu-id="2a27a-153">Request</span></span>
<span data-ttu-id="2a27a-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a27a-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests/{appLogCollectionRequestId}
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

### <a name="response"></a><span data-ttu-id="2a27a-155">响应</span><span class="sxs-lookup"><span data-stu-id="2a27a-155">Response</span></span>
<span data-ttu-id="2a27a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a27a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





