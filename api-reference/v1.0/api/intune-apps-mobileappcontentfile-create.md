---
title: 创建 mobileAppContentFile
description: 创建新的 mobileAppContentFile 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28d8ff58b4808e44cbcd2278c7e4169f4c2ccb03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515944"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="e05bd-103">创建 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="e05bd-103">Create mobileAppContentFile</span></span>

<span data-ttu-id="e05bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e05bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e05bd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e05bd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e05bd-106">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e05bd-106">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e05bd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e05bd-107">Prerequisites</span></span>
<span data-ttu-id="e05bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e05bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e05bd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e05bd-110">Permission type</span></span>|<span data-ttu-id="e05bd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e05bd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e05bd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e05bd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e05bd-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e05bd-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e05bd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e05bd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e05bd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e05bd-115">Not supported.</span></span>|
|<span data-ttu-id="e05bd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e05bd-116">Application</span></span>|<span data-ttu-id="e05bd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="e05bd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e05bd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e05bd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="e05bd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e05bd-119">Request headers</span></span>
|<span data-ttu-id="e05bd-120">标头</span><span class="sxs-lookup"><span data-stu-id="e05bd-120">Header</span></span>|<span data-ttu-id="e05bd-121">值</span><span class="sxs-lookup"><span data-stu-id="e05bd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e05bd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e05bd-122">Authorization</span></span>|<span data-ttu-id="e05bd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e05bd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e05bd-124">接受</span><span class="sxs-lookup"><span data-stu-id="e05bd-124">Accept</span></span>|<span data-ttu-id="e05bd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e05bd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e05bd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e05bd-126">Request body</span></span>
<span data-ttu-id="e05bd-127">在请求正文中，提供 mobileAppContentFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e05bd-127">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="e05bd-128">下表显示了创建 mobileAppContentFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e05bd-128">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="e05bd-129">属性</span><span class="sxs-lookup"><span data-stu-id="e05bd-129">Property</span></span>|<span data-ttu-id="e05bd-130">类型</span><span class="sxs-lookup"><span data-stu-id="e05bd-130">Type</span></span>|<span data-ttu-id="e05bd-131">说明</span><span class="sxs-lookup"><span data-stu-id="e05bd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e05bd-132">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="e05bd-132">azureStorageUri</span></span>|<span data-ttu-id="e05bd-133">String</span><span class="sxs-lookup"><span data-stu-id="e05bd-133">String</span></span>|<span data-ttu-id="e05bd-134">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="e05bd-134">The Azure Storage URI.</span></span>|
|<span data-ttu-id="e05bd-135">isCommitted</span><span class="sxs-lookup"><span data-stu-id="e05bd-135">isCommitted</span></span>|<span data-ttu-id="e05bd-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e05bd-136">Boolean</span></span>|<span data-ttu-id="e05bd-137">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="e05bd-137">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="e05bd-138">id</span><span class="sxs-lookup"><span data-stu-id="e05bd-138">id</span></span>|<span data-ttu-id="e05bd-139">String</span><span class="sxs-lookup"><span data-stu-id="e05bd-139">String</span></span>|<span data-ttu-id="e05bd-140">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="e05bd-140">The File Id.</span></span>|
|<span data-ttu-id="e05bd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e05bd-141">createdDateTime</span></span>|<span data-ttu-id="e05bd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e05bd-142">DateTimeOffset</span></span>|<span data-ttu-id="e05bd-143">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="e05bd-143">The time the file was created.</span></span>|
|<span data-ttu-id="e05bd-144">name</span><span class="sxs-lookup"><span data-stu-id="e05bd-144">name</span></span>|<span data-ttu-id="e05bd-145">字符串</span><span class="sxs-lookup"><span data-stu-id="e05bd-145">String</span></span>|<span data-ttu-id="e05bd-146">文件名称。</span><span class="sxs-lookup"><span data-stu-id="e05bd-146">the file name.</span></span>|
|<span data-ttu-id="e05bd-147">size</span><span class="sxs-lookup"><span data-stu-id="e05bd-147">size</span></span>|<span data-ttu-id="e05bd-148">Int64</span><span class="sxs-lookup"><span data-stu-id="e05bd-148">Int64</span></span>|<span data-ttu-id="e05bd-149">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="e05bd-149">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="e05bd-150">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="e05bd-150">sizeEncrypted</span></span>|<span data-ttu-id="e05bd-151">Int64</span><span class="sxs-lookup"><span data-stu-id="e05bd-151">Int64</span></span>|<span data-ttu-id="e05bd-152">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="e05bd-152">The size of the file after encryption.</span></span>|
|<span data-ttu-id="e05bd-153">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e05bd-153">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="e05bd-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e05bd-154">DateTimeOffset</span></span>|<span data-ttu-id="e05bd-155">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="e05bd-155">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="e05bd-156">manifest</span><span class="sxs-lookup"><span data-stu-id="e05bd-156">manifest</span></span>|<span data-ttu-id="e05bd-157">Binary</span><span class="sxs-lookup"><span data-stu-id="e05bd-157">Binary</span></span>|<span data-ttu-id="e05bd-158">清单信息。</span><span class="sxs-lookup"><span data-stu-id="e05bd-158">The manifest information.</span></span>|
|<span data-ttu-id="e05bd-159">uploadState</span><span class="sxs-lookup"><span data-stu-id="e05bd-159">uploadState</span></span>|[<span data-ttu-id="e05bd-160">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="e05bd-160">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="e05bd-161">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="e05bd-161">The state of the current upload request.</span></span> <span data-ttu-id="e05bd-162">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="e05bd-162">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="e05bd-163">响应</span><span class="sxs-lookup"><span data-stu-id="e05bd-163">Response</span></span>
<span data-ttu-id="e05bd-164">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e05bd-164">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e05bd-165">示例</span><span class="sxs-lookup"><span data-stu-id="e05bd-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="e05bd-166">请求</span><span class="sxs-lookup"><span data-stu-id="e05bd-166">Request</span></span>
<span data-ttu-id="e05bd-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e05bd-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e05bd-168">响应</span><span class="sxs-lookup"><span data-stu-id="e05bd-168">Response</span></span>
<span data-ttu-id="e05bd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e05bd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




