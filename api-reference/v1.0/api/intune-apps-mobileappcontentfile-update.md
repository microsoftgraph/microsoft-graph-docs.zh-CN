---
title: 更新 mobileAppContentFile
description: 更新 mobileAppContentFile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1e2d577685e2f1764446993486d1a3d845d4824a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758748"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="3511f-103">更新 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="3511f-103">Update mobileAppContentFile</span></span>

<span data-ttu-id="3511f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3511f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3511f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3511f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3511f-106">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3511f-106">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3511f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3511f-107">Prerequisites</span></span>
<span data-ttu-id="3511f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3511f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3511f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3511f-110">Permission type</span></span>|<span data-ttu-id="3511f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3511f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3511f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3511f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3511f-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3511f-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3511f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3511f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3511f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3511f-115">Not supported.</span></span>|
|<span data-ttu-id="3511f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3511f-116">Application</span></span>|<span data-ttu-id="3511f-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3511f-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3511f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3511f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="3511f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3511f-119">Request headers</span></span>
|<span data-ttu-id="3511f-120">标头</span><span class="sxs-lookup"><span data-stu-id="3511f-120">Header</span></span>|<span data-ttu-id="3511f-121">值</span><span class="sxs-lookup"><span data-stu-id="3511f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3511f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3511f-122">Authorization</span></span>|<span data-ttu-id="3511f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3511f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3511f-124">接受</span><span class="sxs-lookup"><span data-stu-id="3511f-124">Accept</span></span>|<span data-ttu-id="3511f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3511f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3511f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3511f-126">Request body</span></span>
<span data-ttu-id="3511f-127">在请求正文中，提供 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3511f-127">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="3511f-128">下表显示了创建 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3511f-128">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="3511f-129">属性</span><span class="sxs-lookup"><span data-stu-id="3511f-129">Property</span></span>|<span data-ttu-id="3511f-130">类型</span><span class="sxs-lookup"><span data-stu-id="3511f-130">Type</span></span>|<span data-ttu-id="3511f-131">说明</span><span class="sxs-lookup"><span data-stu-id="3511f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3511f-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="3511f-132">azureStorageUri</span></span>|<span data-ttu-id="3511f-133">String</span><span class="sxs-lookup"><span data-stu-id="3511f-133">String</span></span>|<span data-ttu-id="3511f-134">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="3511f-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="3511f-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="3511f-135">isCommitted</span></span>|<span data-ttu-id="3511f-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="3511f-136">Boolean</span></span>|<span data-ttu-id="3511f-137">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="3511f-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="3511f-138">id</span><span class="sxs-lookup"><span data-stu-id="3511f-138">id</span></span>|<span data-ttu-id="3511f-139">String</span><span class="sxs-lookup"><span data-stu-id="3511f-139">String</span></span>|<span data-ttu-id="3511f-140">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="3511f-140">The File Id.</span></span>|
|<span data-ttu-id="3511f-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3511f-141">createdDateTime</span></span>|<span data-ttu-id="3511f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3511f-142">DateTimeOffset</span></span>|<span data-ttu-id="3511f-143">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="3511f-143">The time the file was created.</span></span>|
|<span data-ttu-id="3511f-144">name</span><span class="sxs-lookup"><span data-stu-id="3511f-144">name</span></span>|<span data-ttu-id="3511f-145">String</span><span class="sxs-lookup"><span data-stu-id="3511f-145">String</span></span>|<span data-ttu-id="3511f-146">文件名称。</span><span class="sxs-lookup"><span data-stu-id="3511f-146">the file name.</span></span>|
|<span data-ttu-id="3511f-147">size</span><span class="sxs-lookup"><span data-stu-id="3511f-147">size</span></span>|<span data-ttu-id="3511f-148">Int64</span><span class="sxs-lookup"><span data-stu-id="3511f-148">Int64</span></span>|<span data-ttu-id="3511f-149">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="3511f-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="3511f-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="3511f-150">sizeEncrypted</span></span>|<span data-ttu-id="3511f-151">Int64</span><span class="sxs-lookup"><span data-stu-id="3511f-151">Int64</span></span>|<span data-ttu-id="3511f-152">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="3511f-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="3511f-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3511f-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="3511f-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3511f-154">DateTimeOffset</span></span>|<span data-ttu-id="3511f-155">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="3511f-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="3511f-156">manifest</span><span class="sxs-lookup"><span data-stu-id="3511f-156">manifest</span></span>|<span data-ttu-id="3511f-157">Binary</span><span class="sxs-lookup"><span data-stu-id="3511f-157">Binary</span></span>|<span data-ttu-id="3511f-158">清单信息。</span><span class="sxs-lookup"><span data-stu-id="3511f-158">The manifest information.</span></span>|
|<span data-ttu-id="3511f-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="3511f-159">uploadState</span></span>|[<span data-ttu-id="3511f-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="3511f-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="3511f-161">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="3511f-161">The state of the current upload request.</span></span> <span data-ttu-id="3511f-162">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="3511f-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="3511f-163">响应</span><span class="sxs-lookup"><span data-stu-id="3511f-163">Response</span></span>
<span data-ttu-id="3511f-164">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3511f-164">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3511f-165">示例</span><span class="sxs-lookup"><span data-stu-id="3511f-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="3511f-166">请求</span><span class="sxs-lookup"><span data-stu-id="3511f-166">Request</span></span>
<span data-ttu-id="3511f-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3511f-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="3511f-168">响应</span><span class="sxs-lookup"><span data-stu-id="3511f-168">Response</span></span>
<span data-ttu-id="3511f-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3511f-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```




