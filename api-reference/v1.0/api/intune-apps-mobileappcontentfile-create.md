---
title: 创建 mobileAppContentFile
description: 创建新的 mobileAppContentFile 对象。
author: tfitzmac
ms.openlocfilehash: 9fba589cdb04d6c0258b18cb17da4c96441123e2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27331505"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="d9e13-103">创建 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="d9e13-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="d9e13-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9e13-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9e13-105">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9e13-105">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9e13-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9e13-106">Prerequisites</span></span>
<span data-ttu-id="d9e13-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d9e13-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9e13-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9e13-109">Permission type</span></span>|<span data-ttu-id="d9e13-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9e13-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9e13-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9e13-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9e13-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9e13-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9e13-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9e13-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9e13-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9e13-114">Not supported.</span></span>|
|<span data-ttu-id="d9e13-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9e13-115">Application</span></span>|<span data-ttu-id="d9e13-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9e13-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9e13-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9e13-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="d9e13-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9e13-118">Request headers</span></span>
|<span data-ttu-id="d9e13-119">标头</span><span class="sxs-lookup"><span data-stu-id="d9e13-119">Header</span></span>|<span data-ttu-id="d9e13-120">值</span><span class="sxs-lookup"><span data-stu-id="d9e13-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9e13-121">授权</span><span class="sxs-lookup"><span data-stu-id="d9e13-121">Authorization</span></span>|<span data-ttu-id="d9e13-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9e13-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9e13-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d9e13-123">Accept</span></span>|<span data-ttu-id="d9e13-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d9e13-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9e13-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9e13-125">Request body</span></span>
<span data-ttu-id="d9e13-126">在请求正文中，提供 mobileAppContentFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9e13-126">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="d9e13-127">下表显示了创建 mobileAppContentFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9e13-127">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="d9e13-128">属性</span><span class="sxs-lookup"><span data-stu-id="d9e13-128">Property</span></span>|<span data-ttu-id="d9e13-129">类型</span><span class="sxs-lookup"><span data-stu-id="d9e13-129">Type</span></span>|<span data-ttu-id="d9e13-130">说明</span><span class="sxs-lookup"><span data-stu-id="d9e13-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9e13-131">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="d9e13-131">azureStorageUri</span></span>|<span data-ttu-id="d9e13-132">String</span><span class="sxs-lookup"><span data-stu-id="d9e13-132">String</span></span>|<span data-ttu-id="d9e13-133">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="d9e13-133">The Azure Storage URI.</span></span>|
|<span data-ttu-id="d9e13-134">isCommitted</span><span class="sxs-lookup"><span data-stu-id="d9e13-134">isCommitted</span></span>|<span data-ttu-id="d9e13-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="d9e13-135">Boolean</span></span>|<span data-ttu-id="d9e13-136">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="d9e13-136">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="d9e13-137">id</span><span class="sxs-lookup"><span data-stu-id="d9e13-137">id</span></span>|<span data-ttu-id="d9e13-138">String</span><span class="sxs-lookup"><span data-stu-id="d9e13-138">String</span></span>|<span data-ttu-id="d9e13-139">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="d9e13-139">The File Id.</span></span>|
|<span data-ttu-id="d9e13-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e13-140">createdDateTime</span></span>|<span data-ttu-id="d9e13-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e13-141">DateTimeOffset</span></span>|<span data-ttu-id="d9e13-142">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="d9e13-142">The time the file was created.</span></span>|
|<span data-ttu-id="d9e13-143">name</span><span class="sxs-lookup"><span data-stu-id="d9e13-143">name</span></span>|<span data-ttu-id="d9e13-144">String</span><span class="sxs-lookup"><span data-stu-id="d9e13-144">String</span></span>|<span data-ttu-id="d9e13-145">文件名称。</span><span class="sxs-lookup"><span data-stu-id="d9e13-145">the file name.</span></span>|
|<span data-ttu-id="d9e13-146">size</span><span class="sxs-lookup"><span data-stu-id="d9e13-146">size</span></span>|<span data-ttu-id="d9e13-147">Int64</span><span class="sxs-lookup"><span data-stu-id="d9e13-147">Int64</span></span>|<span data-ttu-id="d9e13-148">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="d9e13-148">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="d9e13-149">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="d9e13-149">sizeEncrypted</span></span>|<span data-ttu-id="d9e13-150">Int64</span><span class="sxs-lookup"><span data-stu-id="d9e13-150">Int64</span></span>|<span data-ttu-id="d9e13-151">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="d9e13-151">The size of the file after encryption.</span></span>|
|<span data-ttu-id="d9e13-152">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="d9e13-152">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="d9e13-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d9e13-153">DateTimeOffset</span></span>|<span data-ttu-id="d9e13-154">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="d9e13-154">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="d9e13-155">manifest</span><span class="sxs-lookup"><span data-stu-id="d9e13-155">manifest</span></span>|<span data-ttu-id="d9e13-156">Binary</span><span class="sxs-lookup"><span data-stu-id="d9e13-156">Binary</span></span>|<span data-ttu-id="d9e13-157">清单信息。</span><span class="sxs-lookup"><span data-stu-id="d9e13-157">The manifest information.</span></span>|
|<span data-ttu-id="d9e13-158">uploadState</span><span class="sxs-lookup"><span data-stu-id="d9e13-158">uploadState</span></span>|[<span data-ttu-id="d9e13-159">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="d9e13-159">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="d9e13-160">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="d9e13-160">The state of the current upload request.</span></span> <span data-ttu-id="d9e13-161">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="d9e13-161">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="d9e13-162">响应</span><span class="sxs-lookup"><span data-stu-id="d9e13-162">Response</span></span>
<span data-ttu-id="d9e13-163">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9e13-163">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9e13-164">示例</span><span class="sxs-lookup"><span data-stu-id="d9e13-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9e13-165">请求</span><span class="sxs-lookup"><span data-stu-id="d9e13-165">Request</span></span>
<span data-ttu-id="d9e13-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9e13-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9e13-167">响应</span><span class="sxs-lookup"><span data-stu-id="d9e13-167">Response</span></span>
<span data-ttu-id="d9e13-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9e13-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



