---
title: 创建 mobileAppContentFile
description: 创建新的 mobileAppContentFile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 221222dc6ea212d02fd89cd83a528e022f873cc9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35960816"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="f0407-103">创建 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="f0407-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="f0407-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0407-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0407-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0407-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0407-106">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0407-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0407-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f0407-107">Prerequisites</span></span>
<span data-ttu-id="f0407-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f0407-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0407-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f0407-110">Permission type</span></span>|<span data-ttu-id="f0407-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f0407-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0407-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f0407-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0407-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0407-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f0407-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f0407-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0407-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0407-115">Not supported.</span></span>|
|<span data-ttu-id="f0407-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f0407-116">Application</span></span>|<span data-ttu-id="f0407-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f0407-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0407-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f0407-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="f0407-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f0407-119">Request headers</span></span>
|<span data-ttu-id="f0407-120">标头</span><span class="sxs-lookup"><span data-stu-id="f0407-120">Header</span></span>|<span data-ttu-id="f0407-121">值</span><span class="sxs-lookup"><span data-stu-id="f0407-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0407-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f0407-122">Authorization</span></span>|<span data-ttu-id="f0407-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f0407-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0407-124">接受</span><span class="sxs-lookup"><span data-stu-id="f0407-124">Accept</span></span>|<span data-ttu-id="f0407-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0407-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0407-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f0407-126">Request body</span></span>
<span data-ttu-id="f0407-127">在请求正文中，提供 mobileAppContentFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0407-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="f0407-128">下表显示了创建 mobileAppContentFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f0407-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="f0407-129">属性</span><span class="sxs-lookup"><span data-stu-id="f0407-129">Property</span></span>|<span data-ttu-id="f0407-130">类型</span><span class="sxs-lookup"><span data-stu-id="f0407-130">Type</span></span>|<span data-ttu-id="f0407-131">说明</span><span class="sxs-lookup"><span data-stu-id="f0407-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0407-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="f0407-132">azureStorageUri</span></span>|<span data-ttu-id="f0407-133">String</span><span class="sxs-lookup"><span data-stu-id="f0407-133">String</span></span>|<span data-ttu-id="f0407-134">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="f0407-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="f0407-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="f0407-135">isCommitted</span></span>|<span data-ttu-id="f0407-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0407-136">Boolean</span></span>|<span data-ttu-id="f0407-137">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="f0407-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="f0407-138">id</span><span class="sxs-lookup"><span data-stu-id="f0407-138">id</span></span>|<span data-ttu-id="f0407-139">String</span><span class="sxs-lookup"><span data-stu-id="f0407-139">String</span></span>|<span data-ttu-id="f0407-140">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="f0407-140">The File Id.</span></span>|
|<span data-ttu-id="f0407-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0407-141">createdDateTime</span></span>|<span data-ttu-id="f0407-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0407-142">DateTimeOffset</span></span>|<span data-ttu-id="f0407-143">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="f0407-143">The time the file was created.</span></span>|
|<span data-ttu-id="f0407-144">name</span><span class="sxs-lookup"><span data-stu-id="f0407-144">name</span></span>|<span data-ttu-id="f0407-145">String</span><span class="sxs-lookup"><span data-stu-id="f0407-145">String</span></span>|<span data-ttu-id="f0407-146">文件名称。</span><span class="sxs-lookup"><span data-stu-id="f0407-146">the file name.</span></span>|
|<span data-ttu-id="f0407-147">size</span><span class="sxs-lookup"><span data-stu-id="f0407-147">size</span></span>|<span data-ttu-id="f0407-148">Int64</span><span class="sxs-lookup"><span data-stu-id="f0407-148">Int64</span></span>|<span data-ttu-id="f0407-149">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="f0407-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="f0407-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="f0407-150">sizeEncrypted</span></span>|<span data-ttu-id="f0407-151">Int64</span><span class="sxs-lookup"><span data-stu-id="f0407-151">Int64</span></span>|<span data-ttu-id="f0407-152">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="f0407-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="f0407-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f0407-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="f0407-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0407-154">DateTimeOffset</span></span>|<span data-ttu-id="f0407-155">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="f0407-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="f0407-156">manifest</span><span class="sxs-lookup"><span data-stu-id="f0407-156">manifest</span></span>|<span data-ttu-id="f0407-157">Binary</span><span class="sxs-lookup"><span data-stu-id="f0407-157">Binary</span></span>|<span data-ttu-id="f0407-158">清单信息。</span><span class="sxs-lookup"><span data-stu-id="f0407-158">The manifest information.</span></span>|
|<span data-ttu-id="f0407-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="f0407-159">uploadState</span></span>|[<span data-ttu-id="f0407-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="f0407-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="f0407-161">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="f0407-161">The state of the current upload request.</span></span> <span data-ttu-id="f0407-162">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="f0407-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="f0407-163">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="f0407-163">isFrameworkFile</span></span>|<span data-ttu-id="f0407-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0407-164">Boolean</span></span>|<span data-ttu-id="f0407-165">一个指示文件是否为框架文件的值。</span><span class="sxs-lookup"><span data-stu-id="f0407-165">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="f0407-166">isDependency</span><span class="sxs-lookup"><span data-stu-id="f0407-166">isDependency</span></span>|<span data-ttu-id="f0407-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0407-167">Boolean</span></span>|<span data-ttu-id="f0407-168">内容文件是否依赖于主要内容文件。</span><span class="sxs-lookup"><span data-stu-id="f0407-168">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="f0407-169">响应</span><span class="sxs-lookup"><span data-stu-id="f0407-169">Response</span></span>
<span data-ttu-id="f0407-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f0407-170">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0407-171">示例</span><span class="sxs-lookup"><span data-stu-id="f0407-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0407-172">请求</span><span class="sxs-lookup"><span data-stu-id="f0407-172">Request</span></span>
<span data-ttu-id="f0407-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f0407-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
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

### <a name="response"></a><span data-ttu-id="f0407-174">响应</span><span class="sxs-lookup"><span data-stu-id="f0407-174">Response</span></span>
<span data-ttu-id="f0407-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f0407-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





