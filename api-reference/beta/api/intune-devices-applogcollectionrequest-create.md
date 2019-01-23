---
title: 创建 appLogCollectionRequest
description: 创建新的 appLogCollectionRequest 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c3afd1cf00ba706e3fbc1e960e649fc010ae582f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429474"
---
# <a name="create-applogcollectionrequest"></a><span data-ttu-id="3444c-103">创建 appLogCollectionRequest</span><span class="sxs-lookup"><span data-stu-id="3444c-103">Create appLogCollectionRequest</span></span>

> <span data-ttu-id="3444c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="3444c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3444c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3444c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3444c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3444c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3444c-107">创建新的[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3444c-107">Create a new [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3444c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3444c-108">Prerequisites</span></span>
<span data-ttu-id="3444c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3444c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3444c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3444c-111">Permission type</span></span>|<span data-ttu-id="3444c-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3444c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3444c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3444c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3444c-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3444c-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="3444c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3444c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3444c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3444c-116">Not supported.</span></span>|
|<span data-ttu-id="3444c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3444c-117">Application</span></span>|<span data-ttu-id="3444c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="3444c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3444c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3444c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileAppTroubleshootingEvents/{mobileAppTroubleshootingEventId}/appLogCollectionRequests
```

## <a name="request-headers"></a><span data-ttu-id="3444c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3444c-120">Request headers</span></span>
|<span data-ttu-id="3444c-121">标头</span><span class="sxs-lookup"><span data-stu-id="3444c-121">Header</span></span>|<span data-ttu-id="3444c-122">值</span><span class="sxs-lookup"><span data-stu-id="3444c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3444c-123">授权</span><span class="sxs-lookup"><span data-stu-id="3444c-123">Authorization</span></span>|<span data-ttu-id="3444c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3444c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3444c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3444c-125">Accept</span></span>|<span data-ttu-id="3444c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3444c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3444c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3444c-127">Request body</span></span>
<span data-ttu-id="3444c-128">在请求正文中，提供 appLogCollectionRequest 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3444c-128">In the request body, supply a JSON representation for the appLogCollectionRequest object.</span></span>

<span data-ttu-id="3444c-129">下表显示时创建 appLogCollectionRequest 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3444c-129">The following table shows the properties that are required when you create the appLogCollectionRequest.</span></span>

|<span data-ttu-id="3444c-130">属性</span><span class="sxs-lookup"><span data-stu-id="3444c-130">Property</span></span>|<span data-ttu-id="3444c-131">类型</span><span class="sxs-lookup"><span data-stu-id="3444c-131">Type</span></span>|<span data-ttu-id="3444c-132">说明</span><span class="sxs-lookup"><span data-stu-id="3444c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3444c-133">id</span><span class="sxs-lookup"><span data-stu-id="3444c-133">id</span></span>|<span data-ttu-id="3444c-134">String</span><span class="sxs-lookup"><span data-stu-id="3444c-134">String</span></span>|<span data-ttu-id="3444c-135">唯一的标识符。</span><span class="sxs-lookup"><span data-stu-id="3444c-135">The unique Identifier.</span></span> <span data-ttu-id="3444c-136">这是 userId_DeviceId_AppId id。</span><span class="sxs-lookup"><span data-stu-id="3444c-136">This is userId_DeviceId_AppId id.</span></span>|
|<span data-ttu-id="3444c-137">status</span><span class="sxs-lookup"><span data-stu-id="3444c-137">status</span></span>|[<span data-ttu-id="3444c-138">appLogUploadState</span><span class="sxs-lookup"><span data-stu-id="3444c-138">appLogUploadState</span></span>](../resources/intune-devices-apploguploadstate.md)|<span data-ttu-id="3444c-139">日志上载状态。</span><span class="sxs-lookup"><span data-stu-id="3444c-139">Log upload status.</span></span> <span data-ttu-id="3444c-140">可取值为：`pending`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="3444c-140">Possible values are: `pending`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="3444c-141">errorMessage</span><span class="sxs-lookup"><span data-stu-id="3444c-141">errorMessage</span></span>|<span data-ttu-id="3444c-142">String</span><span class="sxs-lookup"><span data-stu-id="3444c-142">String</span></span>|<span data-ttu-id="3444c-143">如果在上载过程中的任何错误消息</span><span class="sxs-lookup"><span data-stu-id="3444c-143">Error message if any during the upload process</span></span>|
|<span data-ttu-id="3444c-144">customLogFolders</span><span class="sxs-lookup"><span data-stu-id="3444c-144">customLogFolders</span></span>|<span data-ttu-id="3444c-145">String 集合</span><span class="sxs-lookup"><span data-stu-id="3444c-145">String collection</span></span>|<span data-ttu-id="3444c-146">日志文件文件夹的列表。</span><span class="sxs-lookup"><span data-stu-id="3444c-146">List of log folders.</span></span> |
|<span data-ttu-id="3444c-147">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="3444c-147">completedDateTime</span></span>|<span data-ttu-id="3444c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3444c-148">DateTimeOffset</span></span>|<span data-ttu-id="3444c-149">上载日志请求频率达到终端状态的时间</span><span class="sxs-lookup"><span data-stu-id="3444c-149">Time at which the upload log request reached a terminal state</span></span>|



## <a name="response"></a><span data-ttu-id="3444c-150">响应</span><span class="sxs-lookup"><span data-stu-id="3444c-150">Response</span></span>
<span data-ttu-id="3444c-151">如果成功，此方法返回`201 Created`响应代码和响应正文中的[appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3444c-151">If successful, this method returns a `201 Created` response code and a [appLogCollectionRequest](../resources/intune-devices-applogcollectionrequest.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3444c-152">示例</span><span class="sxs-lookup"><span data-stu-id="3444c-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="3444c-153">请求</span><span class="sxs-lookup"><span data-stu-id="3444c-153">Request</span></span>
<span data-ttu-id="3444c-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3444c-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3444c-155">响应</span><span class="sxs-lookup"><span data-stu-id="3444c-155">Response</span></span>
<span data-ttu-id="3444c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3444c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




