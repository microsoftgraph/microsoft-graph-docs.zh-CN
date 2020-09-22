---
title: 创建 mobileAppContentFile
description: 创建新的 mobileAppContentFile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8f7a75bac9f17795d9a8b6f2650041ccc8518cb5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087430"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="66c5c-103">创建 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="66c5c-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="66c5c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="66c5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66c5c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66c5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66c5c-106">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66c5c-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="66c5c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="66c5c-107">Prerequisites</span></span>
<span data-ttu-id="66c5c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66c5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66c5c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66c5c-110">Permission type</span></span>|<span data-ttu-id="66c5c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="66c5c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66c5c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66c5c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="66c5c-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66c5c-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66c5c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66c5c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66c5c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66c5c-115">Not supported.</span></span>|
|<span data-ttu-id="66c5c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66c5c-116">Application</span></span>|<span data-ttu-id="66c5c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="66c5c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66c5c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66c5c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="66c5c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="66c5c-119">Request headers</span></span>
|<span data-ttu-id="66c5c-120">标头</span><span class="sxs-lookup"><span data-stu-id="66c5c-120">Header</span></span>|<span data-ttu-id="66c5c-121">值</span><span class="sxs-lookup"><span data-stu-id="66c5c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66c5c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66c5c-122">Authorization</span></span>|<span data-ttu-id="66c5c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="66c5c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66c5c-124">接受</span><span class="sxs-lookup"><span data-stu-id="66c5c-124">Accept</span></span>|<span data-ttu-id="66c5c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="66c5c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66c5c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="66c5c-126">Request body</span></span>
<span data-ttu-id="66c5c-127">在请求正文中，提供 mobileAppContentFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66c5c-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="66c5c-128">下表显示了创建 mobileAppContentFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="66c5c-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="66c5c-129">属性</span><span class="sxs-lookup"><span data-stu-id="66c5c-129">Property</span></span>|<span data-ttu-id="66c5c-130">类型</span><span class="sxs-lookup"><span data-stu-id="66c5c-130">Type</span></span>|<span data-ttu-id="66c5c-131">说明</span><span class="sxs-lookup"><span data-stu-id="66c5c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66c5c-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="66c5c-132">azureStorageUri</span></span>|<span data-ttu-id="66c5c-133">String</span><span class="sxs-lookup"><span data-stu-id="66c5c-133">String</span></span>|<span data-ttu-id="66c5c-134">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="66c5c-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="66c5c-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="66c5c-135">isCommitted</span></span>|<span data-ttu-id="66c5c-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="66c5c-136">Boolean</span></span>|<span data-ttu-id="66c5c-137">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="66c5c-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="66c5c-138">id</span><span class="sxs-lookup"><span data-stu-id="66c5c-138">id</span></span>|<span data-ttu-id="66c5c-139">String</span><span class="sxs-lookup"><span data-stu-id="66c5c-139">String</span></span>|<span data-ttu-id="66c5c-140">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="66c5c-140">The File Id.</span></span>|
|<span data-ttu-id="66c5c-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="66c5c-141">createdDateTime</span></span>|<span data-ttu-id="66c5c-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66c5c-142">DateTimeOffset</span></span>|<span data-ttu-id="66c5c-143">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="66c5c-143">The time the file was created.</span></span>|
|<span data-ttu-id="66c5c-144">name</span><span class="sxs-lookup"><span data-stu-id="66c5c-144">name</span></span>|<span data-ttu-id="66c5c-145">String</span><span class="sxs-lookup"><span data-stu-id="66c5c-145">String</span></span>|<span data-ttu-id="66c5c-146">文件名称。</span><span class="sxs-lookup"><span data-stu-id="66c5c-146">the file name.</span></span>|
|<span data-ttu-id="66c5c-147">size</span><span class="sxs-lookup"><span data-stu-id="66c5c-147">size</span></span>|<span data-ttu-id="66c5c-148">Int64</span><span class="sxs-lookup"><span data-stu-id="66c5c-148">Int64</span></span>|<span data-ttu-id="66c5c-149">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="66c5c-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="66c5c-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="66c5c-150">sizeEncrypted</span></span>|<span data-ttu-id="66c5c-151">Int64</span><span class="sxs-lookup"><span data-stu-id="66c5c-151">Int64</span></span>|<span data-ttu-id="66c5c-152">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="66c5c-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="66c5c-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="66c5c-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="66c5c-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66c5c-154">DateTimeOffset</span></span>|<span data-ttu-id="66c5c-155">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="66c5c-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="66c5c-156">manifest</span><span class="sxs-lookup"><span data-stu-id="66c5c-156">manifest</span></span>|<span data-ttu-id="66c5c-157">Binary</span><span class="sxs-lookup"><span data-stu-id="66c5c-157">Binary</span></span>|<span data-ttu-id="66c5c-158">清单信息。</span><span class="sxs-lookup"><span data-stu-id="66c5c-158">The manifest information.</span></span>|
|<span data-ttu-id="66c5c-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="66c5c-159">uploadState</span></span>|[<span data-ttu-id="66c5c-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="66c5c-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="66c5c-161">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="66c5c-161">The state of the current upload request.</span></span> <span data-ttu-id="66c5c-162">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="66c5c-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="66c5c-163">响应</span><span class="sxs-lookup"><span data-stu-id="66c5c-163">Response</span></span>
<span data-ttu-id="66c5c-164">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="66c5c-164">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66c5c-165">示例</span><span class="sxs-lookup"><span data-stu-id="66c5c-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="66c5c-166">请求</span><span class="sxs-lookup"><span data-stu-id="66c5c-166">Request</span></span>
<span data-ttu-id="66c5c-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66c5c-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
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

### <a name="response"></a><span data-ttu-id="66c5c-168">响应</span><span class="sxs-lookup"><span data-stu-id="66c5c-168">Response</span></span>
<span data-ttu-id="66c5c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66c5c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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









