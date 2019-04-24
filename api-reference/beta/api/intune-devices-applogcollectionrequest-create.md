---
title: 创建 appLogCollectionRequest
description: 创建新的 appLogCollectionRequest 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 716daa9f3abea68a86d9fc7947af5d9d5d2dbb91
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32466068"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="04e95-103">创建 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="04e95-103">Create appLogCollectionRequest</span></span>

> <span data-ttu-id="04e95-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="04e95-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04e95-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04e95-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04e95-106">创建新的[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04e95-106">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04e95-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="04e95-107">Prerequisites</span></span>
<span data-ttu-id="04e95-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="04e95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="04e95-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="04e95-110">Permission type</span></span>|<span data-ttu-id="04e95-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04e95-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04e95-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04e95-112">Delegated (work or school account)</span></span>|<span data-ttu-id="04e95-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04e95-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="04e95-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04e95-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04e95-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="04e95-115">Not supported.</span></span>|
|<span data-ttu-id="04e95-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="04e95-116">Application</span></span>|<span data-ttu-id="04e95-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="04e95-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04e95-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04e95-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="04e95-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="04e95-119">Request headers</span></span>
|<span data-ttu-id="04e95-120">标头</span><span class="sxs-lookup"><span data-stu-id="04e95-120">Header</span></span>|<span data-ttu-id="04e95-121">值</span><span class="sxs-lookup"><span data-stu-id="04e95-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04e95-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="04e95-122">Authorization</span></span>|<span data-ttu-id="04e95-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04e95-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04e95-124">接受</span><span class="sxs-lookup"><span data-stu-id="04e95-124">Accept</span></span>|<span data-ttu-id="04e95-125">application/json</span><span class="sxs-lookup"><span data-stu-id="04e95-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04e95-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="04e95-126">Request body</span></span>
<span data-ttu-id="04e95-127">在请求正文中, 提供 appLogCollectionRequest 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04e95-127">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="04e95-128">下表显示创建 appLogCollectionRequest 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="04e95-128">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="04e95-129">属性</span><span class="sxs-lookup"><span data-stu-id="04e95-129">Property</span></span>|<span data-ttu-id="04e95-130">类型</span><span class="sxs-lookup"><span data-stu-id="04e95-130">Type</span></span>|<span data-ttu-id="04e95-131">说明</span><span class="sxs-lookup"><span data-stu-id="04e95-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04e95-132">id</span><span class="sxs-lookup"><span data-stu-id="04e95-132">id</span></span>|<span data-ttu-id="04e95-133">String</span><span class="sxs-lookup"><span data-stu-id="04e95-133">String</span></span>|<span data-ttu-id="04e95-134">唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="04e95-134">The unique Identifier.</span></span> <span data-ttu-id="04e95-135">这是 userId_DeviceId_AppId id。</span><span class="sxs-lookup"><span data-stu-id="04e95-135">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="04e95-136">status</span><span class="sxs-lookup"><span data-stu-id="04e95-136">status</span></span>|[<span data-ttu-id="04e95-137">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="04e95-137">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="04e95-138">日志上载状态。</span><span class="sxs-lookup"><span data-stu-id="04e95-138">Log upload status.</span></span> <span data-ttu-id="04e95-139">可取值为：`pending`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="04e95-139">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="04e95-140">errorMessage</span><span class="sxs-lookup"><span data-stu-id="04e95-140">errorMessage</span></span>|<span data-ttu-id="04e95-141">字符串</span><span class="sxs-lookup"><span data-stu-id="04e95-141">String</span></span>|<span data-ttu-id="04e95-142">在上载过程中出现的错误消息</span><span class="sxs-lookup"><span data-stu-id="04e95-142">Error message if any during the upload process</span></span>|
|<span data-ttu-id="04e95-143">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="04e95-143">customLogFolders</span></span>|<span data-ttu-id="04e95-144">String collection</span><span class="sxs-lookup"><span data-stu-id="04e95-144">String collection</span></span>|<span data-ttu-id="04e95-145">日志文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="04e95-145">List of log folders.</span></span> |
|<span data-ttu-id="04e95-146">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="04e95-146">completedDateTime</span></span>|<span data-ttu-id="04e95-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04e95-147">DateTimeOffset</span></span>|<span data-ttu-id="04e95-148">上传日志请求到达终端状态的时间</span><span class="sxs-lookup"><span data-stu-id="04e95-148">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="04e95-149">响应</span><span class="sxs-lookup"><span data-stu-id="04e95-149">Response</span></span>
<span data-ttu-id="04e95-150">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="04e95-150">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04e95-151">示例</span><span class="sxs-lookup"><span data-stu-id="04e95-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="04e95-152">请求</span><span class="sxs-lookup"><span data-stu-id="04e95-152">Request</span></span>
<span data-ttu-id="04e95-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04e95-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="04e95-154">响应</span><span class="sxs-lookup"><span data-stu-id="04e95-154">Response</span></span>
<span data-ttu-id="04e95-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04e95-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





