---
title: 创建 importedWindowsAutopilotDeviceIdentityUpload
description: 创建新的 importedWindowsAutopilotDeviceIdentityUpload 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6449402db0af2a79cbeddd22468adbf5592cb6ce
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020869"
---
# <a name="create-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="79b39-103">创建 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="79b39-103">Create importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="79b39-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="79b39-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="79b39-105">创建新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79b39-105">Create a new [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="79b39-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="79b39-106">Prerequisites</span></span>
<span data-ttu-id="79b39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="79b39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="79b39-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="79b39-109">Permission type</span></span>|<span data-ttu-id="79b39-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="79b39-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="79b39-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="79b39-111">Delegated (work or school account)</span></span>|<span data-ttu-id="79b39-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="79b39-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="79b39-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="79b39-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="79b39-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="79b39-114">Not supported.</span></span>|
|<span data-ttu-id="79b39-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="79b39-115">Application</span></span>|<span data-ttu-id="79b39-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="79b39-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="79b39-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="79b39-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads
```

## <a name="request-headers"></a><span data-ttu-id="79b39-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="79b39-118">Request headers</span></span>
|<span data-ttu-id="79b39-119">标头</span><span class="sxs-lookup"><span data-stu-id="79b39-119">Header</span></span>|<span data-ttu-id="79b39-120">值</span><span class="sxs-lookup"><span data-stu-id="79b39-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="79b39-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="79b39-121">Authorization</span></span>|<span data-ttu-id="79b39-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="79b39-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="79b39-123">接受</span><span class="sxs-lookup"><span data-stu-id="79b39-123">Accept</span></span>|<span data-ttu-id="79b39-124">application/json</span><span class="sxs-lookup"><span data-stu-id="79b39-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="79b39-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="79b39-125">Request body</span></span>
<span data-ttu-id="79b39-126">在请求正文中, 提供 importedWindowsAutopilotDeviceIdentityUpload 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="79b39-126">In the request body, supply a JSON representation for the importedWindowsAutopilotDeviceIdentityUpload object.</span></span>

<span data-ttu-id="79b39-127">下表显示创建 importedWindowsAutopilotDeviceIdentityUpload 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="79b39-127">The following table shows the properties that are required when you create the importedWindowsAutopilotDeviceIdentityUpload.</span></span>

|<span data-ttu-id="79b39-128">属性</span><span class="sxs-lookup"><span data-stu-id="79b39-128">Property</span></span>|<span data-ttu-id="79b39-129">类型</span><span class="sxs-lookup"><span data-stu-id="79b39-129">Type</span></span>|<span data-ttu-id="79b39-130">说明</span><span class="sxs-lookup"><span data-stu-id="79b39-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="79b39-131">id</span><span class="sxs-lookup"><span data-stu-id="79b39-131">id</span></span>|<span data-ttu-id="79b39-132">String</span><span class="sxs-lookup"><span data-stu-id="79b39-132">String</span></span>|<span data-ttu-id="79b39-133">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="79b39-133">The GUID for the object</span></span>|
|<span data-ttu-id="79b39-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="79b39-134">createdDateTimeUtc</span></span>|<span data-ttu-id="79b39-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="79b39-135">DateTimeOffset</span></span>|<span data-ttu-id="79b39-136">创建实体时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="79b39-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="79b39-137">status</span><span class="sxs-lookup"><span data-stu-id="79b39-137">status</span></span>|[<span data-ttu-id="79b39-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="79b39-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="79b39-139">上载状态。</span><span class="sxs-lookup"><span data-stu-id="79b39-139">Upload status.</span></span> <span data-ttu-id="79b39-140">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="79b39-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="79b39-141">响应</span><span class="sxs-lookup"><span data-stu-id="79b39-141">Response</span></span>
<span data-ttu-id="79b39-142">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="79b39-142">If successful, this method returns a `201 Created` response code and a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="79b39-143">示例</span><span class="sxs-lookup"><span data-stu-id="79b39-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="79b39-144">请求</span><span class="sxs-lookup"><span data-stu-id="79b39-144">Request</span></span>
<span data-ttu-id="79b39-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="79b39-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="79b39-146">响应</span><span class="sxs-lookup"><span data-stu-id="79b39-146">Response</span></span>
<span data-ttu-id="79b39-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="79b39-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



