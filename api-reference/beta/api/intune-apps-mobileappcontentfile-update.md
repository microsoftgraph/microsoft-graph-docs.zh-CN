---
title: 更新 mobileAppContentFile
description: 更新 mobileAppContentFile 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0b13499d73179206ef2a5f9859b11a8e60201f81
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935126"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="7ac17-103">更新 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="7ac17-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="7ac17-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7ac17-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac17-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ac17-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac17-106">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="7ac17-106">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ac17-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ac17-107">Prerequisites</span></span>
<span data-ttu-id="7ac17-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ac17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ac17-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ac17-110">Permission type</span></span>|<span data-ttu-id="7ac17-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ac17-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ac17-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac17-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7ac17-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ac17-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ac17-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ac17-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ac17-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ac17-115">Not supported.</span></span>|
|<span data-ttu-id="7ac17-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ac17-116">Application</span></span>|<span data-ttu-id="7ac17-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ac17-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ac17-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ac17-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="7ac17-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ac17-119">Request headers</span></span>
|<span data-ttu-id="7ac17-120">标头</span><span class="sxs-lookup"><span data-stu-id="7ac17-120">Header</span></span>|<span data-ttu-id="7ac17-121">值</span><span class="sxs-lookup"><span data-stu-id="7ac17-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ac17-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ac17-122">Authorization</span></span>|<span data-ttu-id="7ac17-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ac17-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ac17-124">接受</span><span class="sxs-lookup"><span data-stu-id="7ac17-124">Accept</span></span>|<span data-ttu-id="7ac17-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7ac17-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ac17-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ac17-126">Request body</span></span>
<span data-ttu-id="7ac17-127">在请求正文中，提供 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ac17-127">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="7ac17-128">下表显示了创建 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ac17-128">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="7ac17-129">属性</span><span class="sxs-lookup"><span data-stu-id="7ac17-129">Property</span></span>|<span data-ttu-id="7ac17-130">类型</span><span class="sxs-lookup"><span data-stu-id="7ac17-130">Type</span></span>|<span data-ttu-id="7ac17-131">说明</span><span class="sxs-lookup"><span data-stu-id="7ac17-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac17-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="7ac17-132">azureStorageUri</span></span>|<span data-ttu-id="7ac17-133">String</span><span class="sxs-lookup"><span data-stu-id="7ac17-133">String</span></span>|<span data-ttu-id="7ac17-134">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="7ac17-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="7ac17-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="7ac17-135">isCommitted</span></span>|<span data-ttu-id="7ac17-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac17-136">Boolean</span></span>|<span data-ttu-id="7ac17-137">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="7ac17-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="7ac17-138">id</span><span class="sxs-lookup"><span data-stu-id="7ac17-138">id</span></span>|<span data-ttu-id="7ac17-139">String</span><span class="sxs-lookup"><span data-stu-id="7ac17-139">String</span></span>|<span data-ttu-id="7ac17-140">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="7ac17-140">The File Id.</span></span>|
|<span data-ttu-id="7ac17-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac17-141">createdDateTime</span></span>|<span data-ttu-id="7ac17-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac17-142">DateTimeOffset</span></span>|<span data-ttu-id="7ac17-143">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="7ac17-143">The time the file was created.</span></span>|
|<span data-ttu-id="7ac17-144">name</span><span class="sxs-lookup"><span data-stu-id="7ac17-144">name</span></span>|<span data-ttu-id="7ac17-145">String</span><span class="sxs-lookup"><span data-stu-id="7ac17-145">String</span></span>|<span data-ttu-id="7ac17-146">文件名称。</span><span class="sxs-lookup"><span data-stu-id="7ac17-146">the file name.</span></span>|
|<span data-ttu-id="7ac17-147">size</span><span class="sxs-lookup"><span data-stu-id="7ac17-147">size</span></span>|<span data-ttu-id="7ac17-148">Int64</span><span class="sxs-lookup"><span data-stu-id="7ac17-148">Int64</span></span>|<span data-ttu-id="7ac17-149">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="7ac17-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="7ac17-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="7ac17-150">sizeEncrypted</span></span>|<span data-ttu-id="7ac17-151">Int64</span><span class="sxs-lookup"><span data-stu-id="7ac17-151">Int64</span></span>|<span data-ttu-id="7ac17-152">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="7ac17-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="7ac17-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="7ac17-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="7ac17-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7ac17-154">DateTimeOffset</span></span>|<span data-ttu-id="7ac17-155">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="7ac17-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="7ac17-156">manifest</span><span class="sxs-lookup"><span data-stu-id="7ac17-156">manifest</span></span>|<span data-ttu-id="7ac17-157">Binary</span><span class="sxs-lookup"><span data-stu-id="7ac17-157">Binary</span></span>|<span data-ttu-id="7ac17-158">清单信息。</span><span class="sxs-lookup"><span data-stu-id="7ac17-158">The manifest information.</span></span>|
|<span data-ttu-id="7ac17-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="7ac17-159">uploadState</span></span>|[<span data-ttu-id="7ac17-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="7ac17-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="7ac17-161">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="7ac17-161">The state of the current upload request.</span></span> <span data-ttu-id="7ac17-162">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="7ac17-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="7ac17-163">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="7ac17-163">isFrameworkFile</span></span>|<span data-ttu-id="7ac17-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac17-164">Boolean</span></span>|<span data-ttu-id="7ac17-165">一个指示文件是否为框架文件的值。</span><span class="sxs-lookup"><span data-stu-id="7ac17-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="7ac17-166">isDependency</span><span class="sxs-lookup"><span data-stu-id="7ac17-166">isDependency</span></span>|<span data-ttu-id="7ac17-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="7ac17-167">Boolean</span></span>|<span data-ttu-id="7ac17-168">内容文件是否依赖于主要内容文件。</span><span class="sxs-lookup"><span data-stu-id="7ac17-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="7ac17-169">响应</span><span class="sxs-lookup"><span data-stu-id="7ac17-169">Response</span></span>
<span data-ttu-id="7ac17-170">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ac17-170">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ac17-171">示例</span><span class="sxs-lookup"><span data-stu-id="7ac17-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ac17-172">请求</span><span class="sxs-lookup"><span data-stu-id="7ac17-172">Request</span></span>
<span data-ttu-id="7ac17-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ac17-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 395

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```

### <a name="response"></a><span data-ttu-id="7ac17-174">响应</span><span class="sxs-lookup"><span data-stu-id="7ac17-174">Response</span></span>
<span data-ttu-id="7ac17-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ac17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 503

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
  "uploadState": "transientError",
  "isFrameworkFile": true,
  "isDependency": true
}
```




