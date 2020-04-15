---
title: 创建 importedWindowsAutopilotDeviceIdentityUpload
description: 创建新的 importedWindowsAutopilotDeviceIdentityUpload 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9cb9f9de78e70c45fa98e24607e06a087d0f61a9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471360"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="6afa4-103">创建 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="6afa4-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

<span data-ttu-id="6afa4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6afa4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6afa4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6afa4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6afa4-106">创建新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6afa4-106">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6afa4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="6afa4-107">Prerequisites</span></span>
<span data-ttu-id="6afa4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6afa4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6afa4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6afa4-110">Permission type</span></span>|<span data-ttu-id="6afa4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6afa4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6afa4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6afa4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6afa4-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6afa4-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6afa4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6afa4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6afa4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6afa4-115">Not supported.</span></span>|
|<span data-ttu-id="6afa4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6afa4-116">Application</span></span>|<span data-ttu-id="6afa4-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6afa4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6afa4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6afa4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="6afa4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6afa4-119">Request headers</span></span>
|<span data-ttu-id="6afa4-120">标头</span><span class="sxs-lookup"><span data-stu-id="6afa4-120">Header</span></span>|<span data-ttu-id="6afa4-121">值</span><span class="sxs-lookup"><span data-stu-id="6afa4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6afa4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6afa4-122">Authorization</span></span>|<span data-ttu-id="6afa4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6afa4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6afa4-124">接受</span><span class="sxs-lookup"><span data-stu-id="6afa4-124">Accept</span></span>|<span data-ttu-id="6afa4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6afa4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6afa4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6afa4-126">Request body</span></span>
<span data-ttu-id="6afa4-127">在请求正文中，提供 importedWindowsAutopilotDeviceIdentityUpload 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6afa4-127">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="6afa4-128">下表显示创建 importedWindowsAutopilotDeviceIdentityUpload 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6afa4-128">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="6afa4-129">属性</span><span class="sxs-lookup"><span data-stu-id="6afa4-129">Property</span></span>|<span data-ttu-id="6afa4-130">类型</span><span class="sxs-lookup"><span data-stu-id="6afa4-130">Type</span></span>|<span data-ttu-id="6afa4-131">说明</span><span class="sxs-lookup"><span data-stu-id="6afa4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6afa4-132">id</span><span class="sxs-lookup"><span data-stu-id="6afa4-132">id</span></span>|<span data-ttu-id="6afa4-133">String</span><span class="sxs-lookup"><span data-stu-id="6afa4-133">String</span></span>|<span data-ttu-id="6afa4-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="6afa4-134">The GUID for the object</span></span>|
|<span data-ttu-id="6afa4-135">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="6afa4-135">createdDateTimeUtc</span></span>|<span data-ttu-id="6afa4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6afa4-136">DateTimeOffset</span></span>|<span data-ttu-id="6afa4-137">创建实体时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6afa4-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="6afa4-138">状态</span><span class="sxs-lookup"><span data-stu-id="6afa4-138">status</span></span>|[<span data-ttu-id="6afa4-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="6afa4-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="6afa4-140">上载状态。</span><span class="sxs-lookup"><span data-stu-id="6afa4-140">Upload status.</span></span> <span data-ttu-id="6afa4-141">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="6afa4-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="6afa4-142">响应</span><span class="sxs-lookup"><span data-stu-id="6afa4-142">Response</span></span>
<span data-ttu-id="6afa4-143">如果成功，此方法在响应`201 Created`正文中返回响应代码和[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6afa4-143">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6afa4-144">示例</span><span class="sxs-lookup"><span data-stu-id="6afa4-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="6afa4-145">请求</span><span class="sxs-lookup"><span data-stu-id="6afa4-145">Request</span></span>
<span data-ttu-id="6afa4-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6afa4-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="6afa4-147">响应</span><span class="sxs-lookup"><span data-stu-id="6afa4-147">Response</span></span>
<span data-ttu-id="6afa4-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6afa4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```






