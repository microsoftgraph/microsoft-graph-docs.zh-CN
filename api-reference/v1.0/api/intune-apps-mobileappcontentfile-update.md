---
title: 更新 mobileAppContentFile
description: 更新 mobileAppContentFile 对象的属性。
ms.openlocfilehash: b3a25c3ccce6598f12d6742546cca0f61679a138
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008307"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="f2a52-103">更新 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="f2a52-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="f2a52-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f2a52-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2a52-105">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f2a52-105">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2a52-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f2a52-106">Prerequisites</span></span>
<span data-ttu-id="f2a52-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f2a52-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2a52-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2a52-109">Permission type</span></span>|<span data-ttu-id="f2a52-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f2a52-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2a52-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2a52-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f2a52-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2a52-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f2a52-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2a52-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2a52-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2a52-114">Not supported.</span></span>|
|<span data-ttu-id="f2a52-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2a52-115">Application</span></span>|<span data-ttu-id="f2a52-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2a52-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2a52-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2a52-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="f2a52-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2a52-118">Request headers</span></span>
|<span data-ttu-id="f2a52-119">标头</span><span class="sxs-lookup"><span data-stu-id="f2a52-119">Header</span></span>|<span data-ttu-id="f2a52-120">值</span><span class="sxs-lookup"><span data-stu-id="f2a52-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2a52-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2a52-121">Authorization</span></span>|<span data-ttu-id="f2a52-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f2a52-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2a52-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f2a52-123">Accept</span></span>|<span data-ttu-id="f2a52-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f2a52-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2a52-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2a52-125">Request body</span></span>
<span data-ttu-id="f2a52-126">在请求正文中，提供 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2a52-126">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="f2a52-127">下表显示了创建 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2a52-127">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="f2a52-128">属性</span><span class="sxs-lookup"><span data-stu-id="f2a52-128">Property</span></span>|<span data-ttu-id="f2a52-129">类型</span><span class="sxs-lookup"><span data-stu-id="f2a52-129">Type</span></span>|<span data-ttu-id="f2a52-130">说明</span><span class="sxs-lookup"><span data-stu-id="f2a52-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2a52-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="f2a52-131">azureStorageUri</span></span>|<span data-ttu-id="f2a52-132">String</span><span class="sxs-lookup"><span data-stu-id="f2a52-132">String</span></span>|<span data-ttu-id="f2a52-133">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="f2a52-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="f2a52-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="f2a52-134">isCommitted</span></span>|<span data-ttu-id="f2a52-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2a52-135">Boolean</span></span>|<span data-ttu-id="f2a52-136">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="f2a52-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="f2a52-137">id</span><span class="sxs-lookup"><span data-stu-id="f2a52-137">id</span></span>|<span data-ttu-id="f2a52-138">String</span><span class="sxs-lookup"><span data-stu-id="f2a52-138">String</span></span>|<span data-ttu-id="f2a52-139">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="f2a52-139">The File Id.</span></span>|
|<span data-ttu-id="f2a52-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f2a52-140">createdDateTime</span></span>|<span data-ttu-id="f2a52-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2a52-141">DateTimeOffset</span></span>|<span data-ttu-id="f2a52-142">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="f2a52-142">The time the file was created.</span></span>|
|<span data-ttu-id="f2a52-143">name</span><span class="sxs-lookup"><span data-stu-id="f2a52-143">name</span></span>|<span data-ttu-id="f2a52-144">String</span><span class="sxs-lookup"><span data-stu-id="f2a52-144">String</span></span>|<span data-ttu-id="f2a52-145">文件名称。</span><span class="sxs-lookup"><span data-stu-id="f2a52-145">the file name.</span></span>|
|<span data-ttu-id="f2a52-146">size</span><span class="sxs-lookup"><span data-stu-id="f2a52-146">size</span></span>|<span data-ttu-id="f2a52-147">Int64</span><span class="sxs-lookup"><span data-stu-id="f2a52-147">Int64</span></span>|<span data-ttu-id="f2a52-148">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="f2a52-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="f2a52-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="f2a52-149">sizeEncrypted</span></span>|<span data-ttu-id="f2a52-150">Int64</span><span class="sxs-lookup"><span data-stu-id="f2a52-150">Int64</span></span>|<span data-ttu-id="f2a52-151">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="f2a52-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="f2a52-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="f2a52-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="f2a52-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f2a52-153">DateTimeOffset</span></span>|<span data-ttu-id="f2a52-154">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="f2a52-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="f2a52-155">manifest</span><span class="sxs-lookup"><span data-stu-id="f2a52-155">manifest</span></span>|<span data-ttu-id="f2a52-156">Binary</span><span class="sxs-lookup"><span data-stu-id="f2a52-156">Binary</span></span>|<span data-ttu-id="f2a52-157">清单信息。</span><span class="sxs-lookup"><span data-stu-id="f2a52-157">The manifest information.</span></span>|
|<span data-ttu-id="f2a52-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="f2a52-158">uploadState</span></span>|[<span data-ttu-id="f2a52-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="f2a52-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="f2a52-160">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="f2a52-160">The state of the current upload request.</span></span> <span data-ttu-id="f2a52-161">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="f2a52-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="f2a52-162">响应</span><span class="sxs-lookup"><span data-stu-id="f2a52-162">Response</span></span>
<span data-ttu-id="f2a52-163">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2a52-163">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2a52-164">示例</span><span class="sxs-lookup"><span data-stu-id="f2a52-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2a52-165">请求</span><span class="sxs-lookup"><span data-stu-id="f2a52-165">Request</span></span>
<span data-ttu-id="f2a52-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2a52-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f2a52-167">响应</span><span class="sxs-lookup"><span data-stu-id="f2a52-167">Response</span></span>
<span data-ttu-id="f2a52-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2a52-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



