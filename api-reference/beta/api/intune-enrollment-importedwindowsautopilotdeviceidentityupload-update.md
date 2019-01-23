---
title: 更新 importedWindowsAutopilotDeviceIdentityUpload
description: 更新 importedWindowsAutopilotDeviceIdentityUpload 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ede84d767121d2f61d88e7d08ef971b55445f2af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407800"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="6f370-103">更新 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="6f370-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="6f370-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="6f370-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="6f370-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6f370-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f370-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f370-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f370-107">更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6f370-107">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f370-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f370-108">Prerequisites</span></span>
<span data-ttu-id="6f370-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6f370-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6f370-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f370-111">Permission type</span></span>|<span data-ttu-id="6f370-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f370-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f370-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f370-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f370-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6f370-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="6f370-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f370-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f370-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f370-116">Not supported.</span></span>|
|<span data-ttu-id="6f370-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f370-117">Application</span></span>|<span data-ttu-id="6f370-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f370-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f370-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f370-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="6f370-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f370-120">Request headers</span></span>
|<span data-ttu-id="6f370-121">标头</span><span class="sxs-lookup"><span data-stu-id="6f370-121">Header</span></span>|<span data-ttu-id="6f370-122">值</span><span class="sxs-lookup"><span data-stu-id="6f370-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f370-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f370-123">Authorization</span></span>|<span data-ttu-id="6f370-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f370-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f370-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f370-125">Accept</span></span>|<span data-ttu-id="6f370-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f370-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f370-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f370-127">Request body</span></span>
<span data-ttu-id="6f370-128">在请求正文中，提供[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6f370-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="6f370-129">下表显示时创建[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6f370-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="6f370-130">属性</span><span class="sxs-lookup"><span data-stu-id="6f370-130">Property</span></span>|<span data-ttu-id="6f370-131">类型</span><span class="sxs-lookup"><span data-stu-id="6f370-131">Type</span></span>|<span data-ttu-id="6f370-132">说明</span><span class="sxs-lookup"><span data-stu-id="6f370-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6f370-133">id</span><span class="sxs-lookup"><span data-stu-id="6f370-133">id</span></span>|<span data-ttu-id="6f370-134">String</span><span class="sxs-lookup"><span data-stu-id="6f370-134">String</span></span>|<span data-ttu-id="6f370-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="6f370-135">The GUID for the object</span></span>|
|<span data-ttu-id="6f370-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="6f370-136">createdDateTimeUtc</span></span>|<span data-ttu-id="6f370-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6f370-137">DateTimeOffset</span></span>|<span data-ttu-id="6f370-138">创建实体时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="6f370-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="6f370-139">status</span><span class="sxs-lookup"><span data-stu-id="6f370-139">status</span></span>|[<span data-ttu-id="6f370-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="6f370-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="6f370-141">上载状态。</span><span class="sxs-lookup"><span data-stu-id="6f370-141">Upload status.</span></span> <span data-ttu-id="6f370-142">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="6f370-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="6f370-143">响应</span><span class="sxs-lookup"><span data-stu-id="6f370-143">Response</span></span>
<span data-ttu-id="6f370-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6f370-144">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f370-145">示例</span><span class="sxs-lookup"><span data-stu-id="6f370-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f370-146">请求</span><span class="sxs-lookup"><span data-stu-id="6f370-146">Request</span></span>
<span data-ttu-id="6f370-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f370-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6f370-148">响应</span><span class="sxs-lookup"><span data-stu-id="6f370-148">Response</span></span>
<span data-ttu-id="6f370-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f370-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




