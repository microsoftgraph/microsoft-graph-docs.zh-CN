---
title: 更新 importedWindowsAutopilotDeviceIdentityUpload
description: 更新 importedWindowsAutopilotDeviceIdentityUpload 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 225259f74791e003aefc506cde69a7f32c98485e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870852"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="2e1ff-103">更新 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="2e1ff-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="2e1ff-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e1ff-105">更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-105">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e1ff-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="2e1ff-106">Prerequisites</span></span>
<span data-ttu-id="2e1ff-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2e1ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e1ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e1ff-109">Permission type</span></span>|<span data-ttu-id="2e1ff-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2e1ff-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e1ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e1ff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2e1ff-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e1ff-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2e1ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e1ff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e1ff-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-114">Not supported.</span></span>|
|<span data-ttu-id="2e1ff-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e1ff-115">Application</span></span>|<span data-ttu-id="2e1ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e1ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e1ff-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="2e1ff-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e1ff-118">Request headers</span></span>
|<span data-ttu-id="2e1ff-119">标头</span><span class="sxs-lookup"><span data-stu-id="2e1ff-119">Header</span></span>|<span data-ttu-id="2e1ff-120">值</span><span class="sxs-lookup"><span data-stu-id="2e1ff-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e1ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e1ff-121">Authorization</span></span>|<span data-ttu-id="2e1ff-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e1ff-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2e1ff-123">Accept</span></span>|<span data-ttu-id="2e1ff-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2e1ff-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e1ff-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e1ff-125">Request body</span></span>
<span data-ttu-id="2e1ff-126">在请求正文中，提供[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-126">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="2e1ff-127">下表显示时创建[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-127">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="2e1ff-128">属性</span><span class="sxs-lookup"><span data-stu-id="2e1ff-128">Property</span></span>|<span data-ttu-id="2e1ff-129">类型</span><span class="sxs-lookup"><span data-stu-id="2e1ff-129">Type</span></span>|<span data-ttu-id="2e1ff-130">说明</span><span class="sxs-lookup"><span data-stu-id="2e1ff-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e1ff-131">id</span><span class="sxs-lookup"><span data-stu-id="2e1ff-131">id</span></span>|<span data-ttu-id="2e1ff-132">字符串</span><span class="sxs-lookup"><span data-stu-id="2e1ff-132">String</span></span>|<span data-ttu-id="2e1ff-133">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="2e1ff-133">The GUID for the object</span></span>|
|<span data-ttu-id="2e1ff-134">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="2e1ff-134">createdDateTimeUtc</span></span>|<span data-ttu-id="2e1ff-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e1ff-135">DateTimeOffset</span></span>|<span data-ttu-id="2e1ff-136">创建实体时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-136">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="2e1ff-137">status</span><span class="sxs-lookup"><span data-stu-id="2e1ff-137">status</span></span>|[<span data-ttu-id="2e1ff-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="2e1ff-138">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="2e1ff-139">上载状态。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-139">Upload status.</span></span> <span data-ttu-id="2e1ff-140">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-140">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="2e1ff-141">响应</span><span class="sxs-lookup"><span data-stu-id="2e1ff-141">Response</span></span>
<span data-ttu-id="2e1ff-142">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-142">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e1ff-143">示例</span><span class="sxs-lookup"><span data-stu-id="2e1ff-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e1ff-144">请求</span><span class="sxs-lookup"><span data-stu-id="2e1ff-144">Request</span></span>
<span data-ttu-id="2e1ff-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2e1ff-146">响应</span><span class="sxs-lookup"><span data-stu-id="2e1ff-146">Response</span></span>
<span data-ttu-id="2e1ff-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2e1ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



