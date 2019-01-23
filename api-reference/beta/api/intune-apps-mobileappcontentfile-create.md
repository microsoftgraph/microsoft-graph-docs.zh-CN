---
title: 创建 mobileAppContentFile
description: 创建新的 mobileAppContentFile 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c815cfcb272e0eb79465d81702e158934ec8c42a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394241"
---
# <a name="create-mobileappcontentfile"></a><span data-ttu-id="40197-103">创建 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="40197-103">Create mobileAppContentFile</span></span>

> <span data-ttu-id="40197-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="40197-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="40197-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="40197-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="40197-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40197-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40197-107">创建新的 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40197-107">Create a new [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40197-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="40197-108">Prerequisites</span></span>
<span data-ttu-id="40197-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="40197-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="40197-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40197-111">Permission type</span></span>|<span data-ttu-id="40197-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="40197-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40197-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40197-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40197-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40197-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="40197-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40197-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40197-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40197-116">Not supported.</span></span>|
|<span data-ttu-id="40197-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="40197-117">Application</span></span>|<span data-ttu-id="40197-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="40197-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="40197-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40197-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="40197-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40197-120">Request headers</span></span>
|<span data-ttu-id="40197-121">标头</span><span class="sxs-lookup"><span data-stu-id="40197-121">Header</span></span>|<span data-ttu-id="40197-122">值</span><span class="sxs-lookup"><span data-stu-id="40197-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40197-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40197-123">Authorization</span></span>|<span data-ttu-id="40197-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40197-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40197-125">Accept</span><span class="sxs-lookup"><span data-stu-id="40197-125">Accept</span></span>|<span data-ttu-id="40197-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40197-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40197-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40197-127">Request body</span></span>
<span data-ttu-id="40197-128">在请求正文中，提供 mobileAppContentFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40197-128">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="40197-129">下表显示了创建 mobileAppContentFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="40197-129">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="40197-130">属性</span><span class="sxs-lookup"><span data-stu-id="40197-130">Property</span></span>|<span data-ttu-id="40197-131">类型</span><span class="sxs-lookup"><span data-stu-id="40197-131">Type</span></span>|<span data-ttu-id="40197-132">说明</span><span class="sxs-lookup"><span data-stu-id="40197-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40197-133">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="40197-133">azureStorageUri</span></span>|<span data-ttu-id="40197-134">String</span><span class="sxs-lookup"><span data-stu-id="40197-134">String</span></span>|<span data-ttu-id="40197-135">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="40197-135">The Azure Storage URI.</span></span>|
|<span data-ttu-id="40197-136">isCommitted</span><span class="sxs-lookup"><span data-stu-id="40197-136">isCommitted</span></span>|<span data-ttu-id="40197-137">Boolean</span><span class="sxs-lookup"><span data-stu-id="40197-137">Boolean</span></span>|<span data-ttu-id="40197-138">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="40197-138">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="40197-139">id</span><span class="sxs-lookup"><span data-stu-id="40197-139">id</span></span>|<span data-ttu-id="40197-140">String</span><span class="sxs-lookup"><span data-stu-id="40197-140">String</span></span>|<span data-ttu-id="40197-141">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="40197-141">The File Id.</span></span>|
|<span data-ttu-id="40197-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="40197-142">createdDateTime</span></span>|<span data-ttu-id="40197-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40197-143">DateTimeOffset</span></span>|<span data-ttu-id="40197-144">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="40197-144">The time the file was created.</span></span>|
|<span data-ttu-id="40197-145">name</span><span class="sxs-lookup"><span data-stu-id="40197-145">name</span></span>|<span data-ttu-id="40197-146">String</span><span class="sxs-lookup"><span data-stu-id="40197-146">String</span></span>|<span data-ttu-id="40197-147">文件名称。</span><span class="sxs-lookup"><span data-stu-id="40197-147">the file name.</span></span>|
|<span data-ttu-id="40197-148">size</span><span class="sxs-lookup"><span data-stu-id="40197-148">size</span></span>|<span data-ttu-id="40197-149">Int64</span><span class="sxs-lookup"><span data-stu-id="40197-149">Int64</span></span>|<span data-ttu-id="40197-150">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="40197-150">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="40197-151">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="40197-151">sizeEncrypted</span></span>|<span data-ttu-id="40197-152">Int64</span><span class="sxs-lookup"><span data-stu-id="40197-152">Int64</span></span>|<span data-ttu-id="40197-153">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="40197-153">The size of the file after encryption.</span></span>|
|<span data-ttu-id="40197-154">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="40197-154">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="40197-155">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="40197-155">DateTimeOffset</span></span>|<span data-ttu-id="40197-156">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="40197-156">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="40197-157">manifest</span><span class="sxs-lookup"><span data-stu-id="40197-157">manifest</span></span>|<span data-ttu-id="40197-158">Binary</span><span class="sxs-lookup"><span data-stu-id="40197-158">Binary</span></span>|<span data-ttu-id="40197-159">清单信息。</span><span class="sxs-lookup"><span data-stu-id="40197-159">The manifest information.</span></span>|
|<span data-ttu-id="40197-160">uploadState</span><span class="sxs-lookup"><span data-stu-id="40197-160">uploadState</span></span>|[<span data-ttu-id="40197-161">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="40197-161">mobileAppContentFileUploadState</span></span>](../resources/intune-apps-mobileappcontentfileuploadstate.md)|<span data-ttu-id="40197-162">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="40197-162">The state of the current upload request.</span></span> <span data-ttu-id="40197-163">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="40197-163">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|
|<span data-ttu-id="40197-164">isFrameworkFile</span><span class="sxs-lookup"><span data-stu-id="40197-164">isFrameworkFile</span></span>|<span data-ttu-id="40197-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="40197-165">Boolean</span></span>|<span data-ttu-id="40197-166">指示文件是否框架文件的值。</span><span class="sxs-lookup"><span data-stu-id="40197-166">A value indicating whether the file is a framework file.</span></span>|
|<span data-ttu-id="40197-167">isDependency</span><span class="sxs-lookup"><span data-stu-id="40197-167">isDependency</span></span>|<span data-ttu-id="40197-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="40197-168">Boolean</span></span>|<span data-ttu-id="40197-169">内容的文件是否依赖关系的主要内容文件。</span><span class="sxs-lookup"><span data-stu-id="40197-169">Whether the content file is a dependency for the main content file.</span></span>|



## <a name="response"></a><span data-ttu-id="40197-170">响应</span><span class="sxs-lookup"><span data-stu-id="40197-170">Response</span></span>
<span data-ttu-id="40197-171">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40197-171">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune-apps-mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40197-172">示例</span><span class="sxs-lookup"><span data-stu-id="40197-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="40197-173">请求</span><span class="sxs-lookup"><span data-stu-id="40197-173">Request</span></span>
<span data-ttu-id="40197-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40197-174">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="40197-175">响应</span><span class="sxs-lookup"><span data-stu-id="40197-175">Response</span></span>
<span data-ttu-id="40197-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40197-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




