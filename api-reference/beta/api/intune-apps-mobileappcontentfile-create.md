---
title: 创建 mobileAppContentFile
description: 创建新的 mobileAppContentFile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b81d338601629cbf2de871907d5e9245a500196
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49248768"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="3d020-103">创建 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="3d020-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="3d020-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3d020-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3d020-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3d020-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3d020-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3d020-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3d020-107">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d020-107">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3d020-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3d020-108">Prerequisites</span></span>
<span data-ttu-id="3d020-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d020-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d020-111">Permission type</span></span>|<span data-ttu-id="3d020-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3d020-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3d020-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d020-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3d020-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d020-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3d020-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d020-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3d020-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3d020-116">Not supported.</span></span>|
|<span data-ttu-id="3d020-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d020-117">Application</span></span>|<span data-ttu-id="3d020-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d020-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3d020-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d020-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="3d020-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3d020-120">Request headers</span></span>
|<span data-ttu-id="3d020-121">标头</span><span class="sxs-lookup"><span data-stu-id="3d020-121">Header</span></span>|<span data-ttu-id="3d020-122">值</span><span class="sxs-lookup"><span data-stu-id="3d020-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3d020-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3d020-123">Authorization</span></span>|<span data-ttu-id="3d020-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3d020-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3d020-125">接受</span><span class="sxs-lookup"><span data-stu-id="3d020-125">Accept</span></span>|<span data-ttu-id="3d020-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3d020-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3d020-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3d020-127">Request body</span></span>
<span data-ttu-id="3d020-128">在请求正文中，提供 mobileAppContentFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3d020-128">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="3d020-129">下表显示了创建 mobileAppContentFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3d020-129">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="3d020-130">属性</span><span class="sxs-lookup"><span data-stu-id="3d020-130">Property</span></span>|<span data-ttu-id="3d020-131">类型</span><span class="sxs-lookup"><span data-stu-id="3d020-131">Type</span></span>|<span data-ttu-id="3d020-132">描述</span><span class="sxs-lookup"><span data-stu-id="3d020-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3d020-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="3d020-133">azureStorageUri</span></span>|<span data-ttu-id="3d020-134">String</span><span class="sxs-lookup"><span data-stu-id="3d020-134">String</span></span>|<span data-ttu-id="3d020-135">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="3d020-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="3d020-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="3d020-136">isCommitted</span></span>|<span data-ttu-id="3d020-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d020-137">Boolean</span></span>|<span data-ttu-id="3d020-138">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="3d020-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="3d020-139">id</span><span class="sxs-lookup"><span data-stu-id="3d020-139">id</span></span>|<span data-ttu-id="3d020-140">String</span><span class="sxs-lookup"><span data-stu-id="3d020-140">String</span></span>|<span data-ttu-id="3d020-141">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="3d020-141">The File Id.</span></span>|
|<span data-ttu-id="3d020-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3d020-142">createdDateTime</span></span>|<span data-ttu-id="3d020-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d020-143">DateTimeOffset</span></span>|<span data-ttu-id="3d020-144">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="3d020-144">The time the file was created.</span></span>|
|<span data-ttu-id="3d020-145">name</span><span class="sxs-lookup"><span data-stu-id="3d020-145">name</span></span>|<span data-ttu-id="3d020-146">String</span><span class="sxs-lookup"><span data-stu-id="3d020-146">String</span></span>|<span data-ttu-id="3d020-147">文件名称。</span><span class="sxs-lookup"><span data-stu-id="3d020-147">the file name.</span></span>|
|<span data-ttu-id="3d020-148">size</span><span class="sxs-lookup"><span data-stu-id="3d020-148">size</span></span>|<span data-ttu-id="3d020-149">Int64</span><span class="sxs-lookup"><span data-stu-id="3d020-149">Int64</span></span>|<span data-ttu-id="3d020-150">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="3d020-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="3d020-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="3d020-151">sizeEncrypted</span></span>|<span data-ttu-id="3d020-152">Int64</span><span class="sxs-lookup"><span data-stu-id="3d020-152">Int64</span></span>|<span data-ttu-id="3d020-153">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="3d020-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="3d020-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3d020-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="3d020-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3d020-155">DateTimeOffset</span></span>|<span data-ttu-id="3d020-156">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="3d020-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="3d020-157">manifest</span><span class="sxs-lookup"><span data-stu-id="3d020-157">manifest</span></span>|<span data-ttu-id="3d020-158">Binary</span><span class="sxs-lookup"><span data-stu-id="3d020-158">Binary</span></span>|<span data-ttu-id="3d020-159">清单信息。</span><span class="sxs-lookup"><span data-stu-id="3d020-159">The manifest information.</span></span>|
|<span data-ttu-id="3d020-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="3d020-160">uploadState</span></span>|[<span data-ttu-id="3d020-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="3d020-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="3d020-162">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="3d020-162">The state of the current upload request.</span></span> <span data-ttu-id="3d020-163">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="3d020-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="3d020-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="3d020-164">isFrameworkFile</span></span>|<span data-ttu-id="3d020-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d020-165">Boolean</span></span>|<span data-ttu-id="3d020-166">一个指示文件是否为框架文件的值。</span><span class="sxs-lookup"><span data-stu-id="3d020-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="3d020-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="3d020-167">isDependency</span></span>|<span data-ttu-id="3d020-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="3d020-168">Boolean</span></span>|<span data-ttu-id="3d020-169">内容文件是否依赖于主要内容文件。</span><span class="sxs-lookup"><span data-stu-id="3d020-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="3d020-170">响应</span><span class="sxs-lookup"><span data-stu-id="3d020-170">Response</span></span>
<span data-ttu-id="3d020-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3d020-171">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3d020-172">示例</span><span class="sxs-lookup"><span data-stu-id="3d020-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="3d020-173">请求</span><span class="sxs-lookup"><span data-stu-id="3d020-173">Request</span></span>
<span data-ttu-id="3d020-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3d020-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3d020-175">响应</span><span class="sxs-lookup"><span data-stu-id="3d020-175">Response</span></span>
<span data-ttu-id="3d020-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3d020-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




