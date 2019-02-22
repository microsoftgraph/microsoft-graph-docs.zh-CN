---
title: 更新 importedWindowsAutopilotDeviceIdentityUpload
description: 更新 importedWindowsAutopilotDeviceIdentityUpload 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4fa2c38224d57dc7750b95b2a339ba0bb10b29f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145582"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="16cdb-103">更新 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="16cdb-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="16cdb-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="16cdb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="16cdb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16cdb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16cdb-106">更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="16cdb-106">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="16cdb-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="16cdb-107">Prerequisites</span></span>
<span data-ttu-id="16cdb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="16cdb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="16cdb-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="16cdb-110">Permission type</span></span>|<span data-ttu-id="16cdb-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="16cdb-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16cdb-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16cdb-112">Delegated (work or school account)</span></span>|<span data-ttu-id="16cdb-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16cdb-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16cdb-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16cdb-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16cdb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="16cdb-115">Not supported.</span></span>|
|<span data-ttu-id="16cdb-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="16cdb-116">Application</span></span>|<span data-ttu-id="16cdb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="16cdb-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16cdb-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16cdb-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="16cdb-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="16cdb-119">Request headers</span></span>
|<span data-ttu-id="16cdb-120">标头</span><span class="sxs-lookup"><span data-stu-id="16cdb-120">Header</span></span>|<span data-ttu-id="16cdb-121">值</span><span class="sxs-lookup"><span data-stu-id="16cdb-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16cdb-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="16cdb-122">Authorization</span></span>|<span data-ttu-id="16cdb-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="16cdb-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16cdb-124">Accept</span><span class="sxs-lookup"><span data-stu-id="16cdb-124">Accept</span></span>|<span data-ttu-id="16cdb-125">application/json</span><span class="sxs-lookup"><span data-stu-id="16cdb-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16cdb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="16cdb-126">Request body</span></span>
<span data-ttu-id="16cdb-127">在请求正文中, 提供[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16cdb-127">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="16cdb-128">下表显示创建[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="16cdb-128">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="16cdb-129">属性</span><span class="sxs-lookup"><span data-stu-id="16cdb-129">Property</span></span>|<span data-ttu-id="16cdb-130">类型</span><span class="sxs-lookup"><span data-stu-id="16cdb-130">Type</span></span>|<span data-ttu-id="16cdb-131">说明</span><span class="sxs-lookup"><span data-stu-id="16cdb-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16cdb-132">id</span><span class="sxs-lookup"><span data-stu-id="16cdb-132">id</span></span>|<span data-ttu-id="16cdb-133">字符串</span><span class="sxs-lookup"><span data-stu-id="16cdb-133">String</span></span>|<span data-ttu-id="16cdb-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="16cdb-134">The GUID for the object</span></span>|
|<span data-ttu-id="16cdb-135">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="16cdb-135">createdDateTimeUtc</span></span>|<span data-ttu-id="16cdb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16cdb-136">DateTimeOffset</span></span>|<span data-ttu-id="16cdb-137">创建实体时的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="16cdb-137">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="16cdb-138">status</span><span class="sxs-lookup"><span data-stu-id="16cdb-138">status</span></span>|[<span data-ttu-id="16cdb-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="16cdb-139">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="16cdb-140">上载状态。</span><span class="sxs-lookup"><span data-stu-id="16cdb-140">Upload status.</span></span> <span data-ttu-id="16cdb-141">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="16cdb-141">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="16cdb-142">响应</span><span class="sxs-lookup"><span data-stu-id="16cdb-142">Response</span></span>
<span data-ttu-id="16cdb-143">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="16cdb-143">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16cdb-144">示例</span><span class="sxs-lookup"><span data-stu-id="16cdb-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="16cdb-145">请求</span><span class="sxs-lookup"><span data-stu-id="16cdb-145">Request</span></span>
<span data-ttu-id="16cdb-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16cdb-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentityUpload",
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="16cdb-147">响应</span><span class="sxs-lookup"><span data-stu-id="16cdb-147">Response</span></span>
<span data-ttu-id="16cdb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16cdb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




