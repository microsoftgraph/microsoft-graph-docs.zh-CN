---
title: 更新 mobileAppContentFile
description: 更新 mobileAppContentFile 对象的属性。
ms.openlocfilehash: 224ebd8ad72dfd1b7e205354df17e87ed50eea62
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042403"
---
# <a name="update-mobileappcontentfile"></a><span data-ttu-id="a1e08-103">更新 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="a1e08-103">Update mobileAppContentFile</span></span>

> <span data-ttu-id="a1e08-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a1e08-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1e08-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a1e08-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a1e08-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a1e08-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1e08-107">更新 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a1e08-107">Update the properties of a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1e08-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1e08-108">Prerequisites</span></span>
<span data-ttu-id="a1e08-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a1e08-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e08-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1e08-111">Permission type</span></span>|<span data-ttu-id="a1e08-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1e08-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1e08-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1e08-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1e08-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1e08-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1e08-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1e08-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1e08-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1e08-116">Not supported.</span></span>|
|<span data-ttu-id="a1e08-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1e08-117">Application</span></span>|<span data-ttu-id="a1e08-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1e08-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1e08-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1e08-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="a1e08-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1e08-120">Request headers</span></span>
|<span data-ttu-id="a1e08-121">标头</span><span class="sxs-lookup"><span data-stu-id="a1e08-121">Header</span></span>|<span data-ttu-id="a1e08-122">值</span><span class="sxs-lookup"><span data-stu-id="a1e08-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1e08-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1e08-123">Authorization</span></span>|<span data-ttu-id="a1e08-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1e08-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1e08-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a1e08-125">Accept</span></span>|<span data-ttu-id="a1e08-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a1e08-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1e08-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1e08-127">Request body</span></span>
<span data-ttu-id="a1e08-128">在请求正文中，提供 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1e08-128">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="a1e08-129">下表显示了创建 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1e08-129">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md).</span></span>

|<span data-ttu-id="a1e08-130">属性</span><span class="sxs-lookup"><span data-stu-id="a1e08-130">Property</span></span>|<span data-ttu-id="a1e08-131">类型</span><span class="sxs-lookup"><span data-stu-id="a1e08-131">Type</span></span>|<span data-ttu-id="a1e08-132">说明</span><span class="sxs-lookup"><span data-stu-id="a1e08-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1e08-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="a1e08-133">azureStorageUri</span></span>|<span data-ttu-id="a1e08-134">String</span><span class="sxs-lookup"><span data-stu-id="a1e08-134">String</span></span>|<span data-ttu-id="a1e08-135">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="a1e08-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="a1e08-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="a1e08-136">isCommitted</span></span>|<span data-ttu-id="a1e08-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="a1e08-137">Boolean</span></span>|<span data-ttu-id="a1e08-138">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="a1e08-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="a1e08-139">id</span><span class="sxs-lookup"><span data-stu-id="a1e08-139">id</span></span>|<span data-ttu-id="a1e08-140">String</span><span class="sxs-lookup"><span data-stu-id="a1e08-140">String</span></span>|<span data-ttu-id="a1e08-141">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="a1e08-141">The File Id.</span></span>|
|<span data-ttu-id="a1e08-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e08-142">createdDateTime</span></span>|<span data-ttu-id="a1e08-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e08-143">DateTimeOffset</span></span>|<span data-ttu-id="a1e08-144">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="a1e08-144">The time the file was created.</span></span>|
|<span data-ttu-id="a1e08-145">name</span><span class="sxs-lookup"><span data-stu-id="a1e08-145">name</span></span>|<span data-ttu-id="a1e08-146">String</span><span class="sxs-lookup"><span data-stu-id="a1e08-146">String</span></span>|<span data-ttu-id="a1e08-147">文件名称。</span><span class="sxs-lookup"><span data-stu-id="a1e08-147">the file name.</span></span>|
|<span data-ttu-id="a1e08-148">size</span><span class="sxs-lookup"><span data-stu-id="a1e08-148">size</span></span>|<span data-ttu-id="a1e08-149">Int64</span><span class="sxs-lookup"><span data-stu-id="a1e08-149">Int64</span></span>|<span data-ttu-id="a1e08-150">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="a1e08-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="a1e08-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="a1e08-151">sizeEncrypted</span></span>|<span data-ttu-id="a1e08-152">Int64</span><span class="sxs-lookup"><span data-stu-id="a1e08-152">Int64</span></span>|<span data-ttu-id="a1e08-153">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="a1e08-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="a1e08-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a1e08-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="a1e08-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1e08-155">DateTimeOffset</span></span>|<span data-ttu-id="a1e08-156">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="a1e08-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="a1e08-157">manifest</span><span class="sxs-lookup"><span data-stu-id="a1e08-157">manifest</span></span>|<span data-ttu-id="a1e08-158">Binary</span><span class="sxs-lookup"><span data-stu-id="a1e08-158">Binary</span></span>|<span data-ttu-id="a1e08-159">清单信息。</span><span class="sxs-lookup"><span data-stu-id="a1e08-159">The manifest information.</span></span>|
|<span data-ttu-id="a1e08-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="a1e08-160">uploadState</span></span>|[<span data-ttu-id="a1e08-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="a1e08-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="a1e08-162">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="a1e08-162">The state of the current upload request.</span></span> <span data-ttu-id="a1e08-163">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="a1e08-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="a1e08-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="a1e08-164">isFrameworkFile</span></span>|<span data-ttu-id="a1e08-165">布尔</span><span class="sxs-lookup"><span data-stu-id="a1e08-165">Boolean</span></span>|<span data-ttu-id="a1e08-166">指示文件是否框架文件的值。</span><span class="sxs-lookup"><span data-stu-id="a1e08-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="a1e08-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="a1e08-167">isDependency</span></span>|<span data-ttu-id="a1e08-168">布尔</span><span class="sxs-lookup"><span data-stu-id="a1e08-168">Boolean</span></span>|<span data-ttu-id="a1e08-169">内容的文件是否依赖关系的主要内容文件。</span><span class="sxs-lookup"><span data-stu-id="a1e08-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="a1e08-170">响应</span><span class="sxs-lookup"><span data-stu-id="a1e08-170">Response</span></span>
<span data-ttu-id="a1e08-171">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1e08-171">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1e08-172">示例</span><span class="sxs-lookup"><span data-stu-id="a1e08-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1e08-173">请求</span><span class="sxs-lookup"><span data-stu-id="a1e08-173">Request</span></span>
<span data-ttu-id="a1e08-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1e08-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 336

{
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

### <a name="response"></a><span data-ttu-id="a1e08-175">响应</span><span class="sxs-lookup"><span data-stu-id="a1e08-175">Response</span></span>
<span data-ttu-id="a1e08-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1e08-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





