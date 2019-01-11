---
title: 更新 importedWindowsAutopilotDeviceIdentityUpload
description: 更新 importedWindowsAutopilotDeviceIdentityUpload 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 76e699ebf7f0704ab6a524c1c5869339e0318ec2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894374"
---
# <a name="update-importedwindowsautopilotdeviceidentityupload"></a><span data-ttu-id="b898d-103">更新 importedWindowsAutopilotDeviceIdentityUpload</span><span class="sxs-lookup"><span data-stu-id="b898d-103">Update importedWindowsAutopilotDeviceIdentityUpload</span></span>

> <span data-ttu-id="b898d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b898d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b898d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b898d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b898d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b898d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b898d-107">更新[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b898d-107">Update the properties of a [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b898d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b898d-108">Prerequisites</span></span>
<span data-ttu-id="b898d-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b898d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b898d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b898d-111">Permission type</span></span>|<span data-ttu-id="b898d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b898d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b898d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b898d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b898d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b898d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="b898d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b898d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b898d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b898d-116">Not supported.</span></span>|
|<span data-ttu-id="b898d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b898d-117">Application</span></span>|<span data-ttu-id="b898d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b898d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b898d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b898d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
```

## <a name="request-headers"></a><span data-ttu-id="b898d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b898d-120">Request headers</span></span>
|<span data-ttu-id="b898d-121">标头</span><span class="sxs-lookup"><span data-stu-id="b898d-121">Header</span></span>|<span data-ttu-id="b898d-122">值</span><span class="sxs-lookup"><span data-stu-id="b898d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b898d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b898d-123">Authorization</span></span>|<span data-ttu-id="b898d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b898d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b898d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b898d-125">Accept</span></span>|<span data-ttu-id="b898d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b898d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b898d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b898d-127">Request body</span></span>
<span data-ttu-id="b898d-128">在请求正文中，提供[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b898d-128">In the request body, supply a JSON representation for the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object.</span></span>

<span data-ttu-id="b898d-129">下表显示时创建[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b898d-129">The following table shows the properties that are required when you create the [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md).</span></span>

|<span data-ttu-id="b898d-130">属性</span><span class="sxs-lookup"><span data-stu-id="b898d-130">Property</span></span>|<span data-ttu-id="b898d-131">类型</span><span class="sxs-lookup"><span data-stu-id="b898d-131">Type</span></span>|<span data-ttu-id="b898d-132">说明</span><span class="sxs-lookup"><span data-stu-id="b898d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b898d-133">id</span><span class="sxs-lookup"><span data-stu-id="b898d-133">id</span></span>|<span data-ttu-id="b898d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="b898d-134">String</span></span>|<span data-ttu-id="b898d-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="b898d-135">The GUID for the object</span></span>|
|<span data-ttu-id="b898d-136">createdDateTimeUtc</span><span class="sxs-lookup"><span data-stu-id="b898d-136">createdDateTimeUtc</span></span>|<span data-ttu-id="b898d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b898d-137">DateTimeOffset</span></span>|<span data-ttu-id="b898d-138">创建实体时的日期时间。</span><span class="sxs-lookup"><span data-stu-id="b898d-138">DateTime when the entity is created.</span></span>|
|<span data-ttu-id="b898d-139">status</span><span class="sxs-lookup"><span data-stu-id="b898d-139">status</span></span>|[<span data-ttu-id="b898d-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span><span class="sxs-lookup"><span data-stu-id="b898d-140">importedWindowsAutopilotDeviceIdentityUploadStatus</span></span>](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityuploadstatus.md)|<span data-ttu-id="b898d-141">上载状态。</span><span class="sxs-lookup"><span data-stu-id="b898d-141">Upload status.</span></span> <span data-ttu-id="b898d-142">可取值为：`noUpload`、`pending`、`complete`、`error`。</span><span class="sxs-lookup"><span data-stu-id="b898d-142">Possible values are: `noUpload`, `pending`, `complete`, `error`.</span></span>|



## <a name="response"></a><span data-ttu-id="b898d-143">响应</span><span class="sxs-lookup"><span data-stu-id="b898d-143">Response</span></span>
<span data-ttu-id="b898d-144">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b898d-144">If successful, this method returns a `200 OK` response code and an updated [importedWindowsAutopilotDeviceIdentityUpload](../resources/intune-enrollment-importedwindowsautopilotdeviceidentityupload.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b898d-145">示例</span><span class="sxs-lookup"><span data-stu-id="b898d-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="b898d-146">请求</span><span class="sxs-lookup"><span data-stu-id="b898d-146">Request</span></span>
<span data-ttu-id="b898d-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b898d-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}
Content-type: application/json
Content-length: 89

{
  "createdDateTimeUtc": "2016-12-31T23:59:45.8788427-08:00",
  "status": "pending"
}
```

### <a name="response"></a><span data-ttu-id="b898d-148">响应</span><span class="sxs-lookup"><span data-stu-id="b898d-148">Response</span></span>
<span data-ttu-id="b898d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b898d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





