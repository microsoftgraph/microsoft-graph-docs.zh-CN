---
title: 更新 importedWindowsAutopilotDeviceIdentityUpload
description: 更新 importedWindowsAutopilotDeviceIdentityUpload 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2b63e6ce8da089d81dc019f902aaffc154f0becd
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37364030"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="c8c7c-103">更新 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="c8c7c-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="c8c7c-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8c7c-105">更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-105">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c8c7c-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="c8c7c-106">Prerequisites</span></span>
<span data-ttu-id="c8c7c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8c7c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8c7c-109">Permission type</span></span>|<span data-ttu-id="c8c7c-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c8c7c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c8c7c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8c7c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c8c7c-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c8c7c-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c8c7c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8c7c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c8c7c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-114">Not supported.</span></span>|
|<span data-ttu-id="c8c7c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8c7c-115">Application</span></span>|<span data-ttu-id="c8c7c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c8c7c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8c7c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="c8c7c-118">请求头</span><span class="sxs-lookup"><span data-stu-id="c8c7c-118">Request headers</span></span>
|<span data-ttu-id="c8c7c-119">标头</span><span class="sxs-lookup"><span data-stu-id="c8c7c-119">Header</span></span>|<span data-ttu-id="c8c7c-120">值</span><span class="sxs-lookup"><span data-stu-id="c8c7c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c8c7c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8c7c-121">Authorization</span></span>|<span data-ttu-id="c8c7c-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c8c7c-123">接受</span><span class="sxs-lookup"><span data-stu-id="c8c7c-123">Accept</span></span>|<span data-ttu-id="c8c7c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="c8c7c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c8c7c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8c7c-125">Request body</span></span>
<span data-ttu-id="c8c7c-126">在请求正文中，提供[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="c8c7c-127">下表显示创建[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="c8c7c-128">属性</span><span class="sxs-lookup"><span data-stu-id="c8c7c-128">Property</span></span>|<span data-ttu-id="c8c7c-129">类型</span><span class="sxs-lookup"><span data-stu-id="c8c7c-129">Type</span></span>|<span data-ttu-id="c8c7c-130">说明</span><span class="sxs-lookup"><span data-stu-id="c8c7c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8c7c-131">id</span><span class="sxs-lookup"><span data-stu-id="c8c7c-131">id</span></span>|<span data-ttu-id="c8c7c-132">String</span><span class="sxs-lookup"><span data-stu-id="c8c7c-132">String</span></span>|<span data-ttu-id="c8c7c-133">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="c8c7c-133">The GUID for the object</span></span>|
|<span data-ttu-id="c8c7c-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="c8c7c-134">createdDateTimeUtc</span></span>|<span data-ttu-id="c8c7c-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c8c7c-135">DateTimeOffset</span></span>|<span data-ttu-id="c8c7c-136">创建实体时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="c8c7c-137">status</span><span class="sxs-lookup"><span data-stu-id="c8c7c-137">status</span></span>|[<span data-ttu-id="c8c7c-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="c8c7c-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="c8c7c-139">上载状态。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-139">Upload status.</span></span> <span data-ttu-id="c8c7c-140">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="c8c7c-141">响应</span><span class="sxs-lookup"><span data-stu-id="c8c7c-141">Response</span></span>
<span data-ttu-id="c8c7c-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-142">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c8c7c-143">示例</span><span class="sxs-lookup"><span data-stu-id="c8c7c-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="c8c7c-144">请求</span><span class="sxs-lookup"><span data-stu-id="c8c7c-144">Request</span></span>
<span data-ttu-id="c8c7c-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="c8c7c-146">响应</span><span class="sxs-lookup"><span data-stu-id="c8c7c-146">Response</span></span>
<span data-ttu-id="c8c7c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c8c7c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "id": "8d639524-9524-8d63-2495-638d2495638d",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```




