# <a name="create-mobileappcontentfile"></a><span data-ttu-id="6a101-101">创建 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="6a101-101">Create mobileAppContentFile</span></span>

> <span data-ttu-id="6a101-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6a101-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6a101-103">创建新的 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a101-103">Create a new [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6a101-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a101-104">Prerequisites</span></span>
<span data-ttu-id="6a101-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6a101-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6a101-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a101-107">Permission type</span></span>|<span data-ttu-id="6a101-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a101-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a101-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a101-109">Delegated (work or school account)</span></span>|<span data-ttu-id="6a101-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a101-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a101-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a101-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a101-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a101-112">Not supported.</span></span>|
|<span data-ttu-id="6a101-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a101-113">Application</span></span>|<span data-ttu-id="6a101-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a101-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a101-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a101-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="6a101-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a101-116">Request headers</span></span>
|<span data-ttu-id="6a101-117">标头</span><span class="sxs-lookup"><span data-stu-id="6a101-117">Header</span></span>|<span data-ttu-id="6a101-118">值</span><span class="sxs-lookup"><span data-stu-id="6a101-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a101-119">授权</span><span class="sxs-lookup"><span data-stu-id="6a101-119">Authorization</span></span>|<span data-ttu-id="6a101-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a101-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a101-121">接受</span><span class="sxs-lookup"><span data-stu-id="6a101-121">Accept</span></span>|<span data-ttu-id="6a101-122">application/json</span><span class="sxs-lookup"><span data-stu-id="6a101-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a101-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a101-123">Request body</span></span>
<span data-ttu-id="6a101-124">在请求正文中，提供 mobileAppContentFile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a101-124">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="6a101-125">下表显示了创建 mobileAppContentFile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a101-125">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="6a101-126">属性</span><span class="sxs-lookup"><span data-stu-id="6a101-126">Property</span></span>|<span data-ttu-id="6a101-127">类型</span><span class="sxs-lookup"><span data-stu-id="6a101-127">Type</span></span>|<span data-ttu-id="6a101-128">说明</span><span class="sxs-lookup"><span data-stu-id="6a101-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a101-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="6a101-129">azureStorageUri</span></span>|<span data-ttu-id="6a101-130">字符串</span><span class="sxs-lookup"><span data-stu-id="6a101-130">String</span></span>|<span data-ttu-id="6a101-131">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="6a101-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="6a101-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="6a101-132">isCommitted</span></span>|<span data-ttu-id="6a101-133">布尔</span><span class="sxs-lookup"><span data-stu-id="6a101-133">Boolean</span></span>|<span data-ttu-id="6a101-134">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="6a101-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="6a101-135">id</span><span class="sxs-lookup"><span data-stu-id="6a101-135">id</span></span>|<span data-ttu-id="6a101-136">字符串</span><span class="sxs-lookup"><span data-stu-id="6a101-136">String</span></span>|<span data-ttu-id="6a101-137">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="6a101-137">The File Id.</span></span>|
|<span data-ttu-id="6a101-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a101-138">createdDateTime</span></span>|<span data-ttu-id="6a101-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a101-139">DateTimeOffset</span></span>|<span data-ttu-id="6a101-140">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="6a101-140">The time the file was created.</span></span>|
|<span data-ttu-id="6a101-141">name</span><span class="sxs-lookup"><span data-stu-id="6a101-141">name</span></span>|<span data-ttu-id="6a101-142">字符串</span><span class="sxs-lookup"><span data-stu-id="6a101-142">String</span></span>|<span data-ttu-id="6a101-143">文件名称。</span><span class="sxs-lookup"><span data-stu-id="6a101-143">the file name.</span></span>|
|<span data-ttu-id="6a101-144">size</span><span class="sxs-lookup"><span data-stu-id="6a101-144">size</span></span>|<span data-ttu-id="6a101-145">Int64</span><span class="sxs-lookup"><span data-stu-id="6a101-145">Int64</span></span>|<span data-ttu-id="6a101-146">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="6a101-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="6a101-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="6a101-147">sizeEncrypted</span></span>|<span data-ttu-id="6a101-148">Int64</span><span class="sxs-lookup"><span data-stu-id="6a101-148">Int64</span></span>|<span data-ttu-id="6a101-149">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="6a101-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="6a101-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="6a101-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="6a101-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a101-151">DateTimeOffset</span></span>|<span data-ttu-id="6a101-152">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="6a101-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="6a101-153">manifest</span><span class="sxs-lookup"><span data-stu-id="6a101-153">manifest</span></span>|<span data-ttu-id="6a101-154">Binary</span><span class="sxs-lookup"><span data-stu-id="6a101-154">Binary</span></span>|<span data-ttu-id="6a101-155">清单信息。</span><span class="sxs-lookup"><span data-stu-id="6a101-155">The manifest information.</span></span>|
|<span data-ttu-id="6a101-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="6a101-156">uploadState</span></span>|[<span data-ttu-id="6a101-157">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="6a101-157">mobileAppContentFileUploadState</span></span>](../resources/intune_apps_mobileappcontentfileuploadstate.md)|<span data-ttu-id="6a101-158">当前上传请求的状态。</span><span class="sxs-lookup"><span data-stu-id="6a101-158">The state of the current upload request.</span></span> <span data-ttu-id="6a101-159">可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="6a101-159">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="6a101-160">响应</span><span class="sxs-lookup"><span data-stu-id="6a101-160">Response</span></span>
<span data-ttu-id="6a101-161">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a101-161">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a101-162">示例</span><span class="sxs-lookup"><span data-stu-id="6a101-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="6a101-163">请求</span><span class="sxs-lookup"><span data-stu-id="6a101-163">Request</span></span>
<span data-ttu-id="6a101-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a101-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6a101-165">响应</span><span class="sxs-lookup"><span data-stu-id="6a101-165">Response</span></span>
<span data-ttu-id="6a101-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a101-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








