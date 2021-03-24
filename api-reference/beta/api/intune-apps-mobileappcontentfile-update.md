---
title: 更新 mobileAppContentFile
description: 更新 mobileAppContentFile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92beb4907c47548634422816425ee10d98fbbcb2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143232"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="2374e-103">更新 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="2374e-103">Update mobileAppContentFile</span></span>

<span data-ttu-id="2374e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2374e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2374e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2374e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2374e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2374e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2374e-107">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2374e-107">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2374e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2374e-108">Prerequisites</span></span>
<span data-ttu-id="2374e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2374e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2374e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2374e-111">Permission type</span></span>|<span data-ttu-id="2374e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2374e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2374e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2374e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2374e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2374e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2374e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2374e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2374e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2374e-116">Not supported.</span></span>|
|<span data-ttu-id="2374e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2374e-117">Application</span></span>|<span data-ttu-id="2374e-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2374e-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2374e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2374e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="2374e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2374e-120">Request headers</span></span>
|<span data-ttu-id="2374e-121">标头</span><span class="sxs-lookup"><span data-stu-id="2374e-121">Header</span></span>|<span data-ttu-id="2374e-122">值</span><span class="sxs-lookup"><span data-stu-id="2374e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2374e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2374e-123">Authorization</span></span>|<span data-ttu-id="2374e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2374e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2374e-125">接受</span><span class="sxs-lookup"><span data-stu-id="2374e-125">Accept</span></span>|<span data-ttu-id="2374e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2374e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2374e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2374e-127">Request body</span></span>
<span data-ttu-id="2374e-128">在请求正文中，提供 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2374e-128">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="2374e-129">下表显示了创建 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2374e-129">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="2374e-130">属性</span><span class="sxs-lookup"><span data-stu-id="2374e-130">Property</span></span>|<span data-ttu-id="2374e-131">类型</span><span class="sxs-lookup"><span data-stu-id="2374e-131">Type</span></span>|<span data-ttu-id="2374e-132">说明</span><span class="sxs-lookup"><span data-stu-id="2374e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2374e-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="2374e-133">azureStorageUri</span></span>|<span data-ttu-id="2374e-134">String</span><span class="sxs-lookup"><span data-stu-id="2374e-134">String</span></span>|<span data-ttu-id="2374e-135">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="2374e-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="2374e-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="2374e-136">isCommitted</span></span>|<span data-ttu-id="2374e-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="2374e-137">Boolean</span></span>|<span data-ttu-id="2374e-138">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="2374e-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="2374e-139">id</span><span class="sxs-lookup"><span data-stu-id="2374e-139">id</span></span>|<span data-ttu-id="2374e-140">String</span><span class="sxs-lookup"><span data-stu-id="2374e-140">String</span></span>|<span data-ttu-id="2374e-141">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="2374e-141">The File Id.</span></span>|
|<span data-ttu-id="2374e-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2374e-142">createdDateTime</span></span>|<span data-ttu-id="2374e-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2374e-143">DateTimeOffset</span></span>|<span data-ttu-id="2374e-144">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="2374e-144">The time the file was created.</span></span>|
|<span data-ttu-id="2374e-145">name</span><span class="sxs-lookup"><span data-stu-id="2374e-145">name</span></span>|<span data-ttu-id="2374e-146">String</span><span class="sxs-lookup"><span data-stu-id="2374e-146">String</span></span>|<span data-ttu-id="2374e-147">文件名称。</span><span class="sxs-lookup"><span data-stu-id="2374e-147">the file name.</span></span>|
|<span data-ttu-id="2374e-148">size</span><span class="sxs-lookup"><span data-stu-id="2374e-148">size</span></span>|<span data-ttu-id="2374e-149">Int64</span><span class="sxs-lookup"><span data-stu-id="2374e-149">Int64</span></span>|<span data-ttu-id="2374e-150">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="2374e-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="2374e-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="2374e-151">sizeEncrypted</span></span>|<span data-ttu-id="2374e-152">Int64</span><span class="sxs-lookup"><span data-stu-id="2374e-152">Int64</span></span>|<span data-ttu-id="2374e-153">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="2374e-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="2374e-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2374e-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="2374e-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2374e-155">DateTimeOffset</span></span>|<span data-ttu-id="2374e-156">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="2374e-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="2374e-157">manifest</span><span class="sxs-lookup"><span data-stu-id="2374e-157">manifest</span></span>|<span data-ttu-id="2374e-158">Binary</span><span class="sxs-lookup"><span data-stu-id="2374e-158">Binary</span></span>|<span data-ttu-id="2374e-159">清单信息。</span><span class="sxs-lookup"><span data-stu-id="2374e-159">The manifest information.</span></span>|
|<span data-ttu-id="2374e-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="2374e-160">uploadState</span></span>|[<span data-ttu-id="2374e-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="2374e-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="2374e-162">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="2374e-162">The state of the current upload request.</span></span> <span data-ttu-id="2374e-163">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="2374e-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="2374e-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="2374e-164">isFrameworkFile</span></span>|<span data-ttu-id="2374e-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="2374e-165">Boolean</span></span>|<span data-ttu-id="2374e-166">一个值，指示文件是否是框架文件。</span><span class="sxs-lookup"><span data-stu-id="2374e-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="2374e-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="2374e-167">isDependency</span></span>|<span data-ttu-id="2374e-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="2374e-168">Boolean</span></span>|<span data-ttu-id="2374e-169">内容文件是否依赖于主内容文件。</span><span class="sxs-lookup"><span data-stu-id="2374e-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="2374e-170">响应</span><span class="sxs-lookup"><span data-stu-id="2374e-170">Response</span></span>
<span data-ttu-id="2374e-171">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2374e-171">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2374e-172">示例</span><span class="sxs-lookup"><span data-stu-id="2374e-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="2374e-173">请求</span><span class="sxs-lookup"><span data-stu-id="2374e-173">Request</span></span>
<span data-ttu-id="2374e-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2374e-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2374e-175">响应</span><span class="sxs-lookup"><span data-stu-id="2374e-175">Response</span></span>
<span data-ttu-id="2374e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2374e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




