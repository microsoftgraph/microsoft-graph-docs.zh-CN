# <a name="update-mobileappcontentfile"></a><span data-ttu-id="a2973-101">更新 mobileAppContentFile</span><span class="sxs-lookup"><span data-stu-id="a2973-101">Update mobileAppContentFile</span></span>

> <span data-ttu-id="a2973-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a2973-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2973-103">更新 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2973-103">Update the properties of a [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2973-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2973-104">Prerequisites</span></span>
<span data-ttu-id="a2973-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a2973-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a2973-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2973-107">Permission type</span></span>|<span data-ttu-id="a2973-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2973-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2973-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2973-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a2973-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2973-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2973-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2973-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2973-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2973-112">Not supported.</span></span>|
|<span data-ttu-id="a2973-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2973-113">Application</span></span>|<span data-ttu-id="a2973-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2973-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2973-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2973-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
```

## <a name="request-headers"></a><span data-ttu-id="a2973-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2973-116">Request headers</span></span>
|<span data-ttu-id="a2973-117">标头</span><span class="sxs-lookup"><span data-stu-id="a2973-117">Header</span></span>|<span data-ttu-id="a2973-118">值</span><span class="sxs-lookup"><span data-stu-id="a2973-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2973-119">授权</span><span class="sxs-lookup"><span data-stu-id="a2973-119">Authorization</span></span>|<span data-ttu-id="a2973-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2973-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2973-121">接受</span><span class="sxs-lookup"><span data-stu-id="a2973-121">Accept</span></span>|<span data-ttu-id="a2973-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a2973-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2973-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2973-123">Request body</span></span>
<span data-ttu-id="a2973-124">在请求正文中，提供 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2973-124">In the request body, supply a JSON representation for the [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>

<span data-ttu-id="a2973-125">下表显示了创建 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2973-125">The following table shows the properties that are required when you create the [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md).</span></span>

|<span data-ttu-id="a2973-126">属性</span><span class="sxs-lookup"><span data-stu-id="a2973-126">Property</span></span>|<span data-ttu-id="a2973-127">类型</span><span class="sxs-lookup"><span data-stu-id="a2973-127">Type</span></span>|<span data-ttu-id="a2973-128">说明</span><span class="sxs-lookup"><span data-stu-id="a2973-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2973-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="a2973-129">azureStorageUri</span></span>|<span data-ttu-id="a2973-130">字符串</span><span class="sxs-lookup"><span data-stu-id="a2973-130">String</span></span>|<span data-ttu-id="a2973-131">Azure 存储 URI。</span><span class="sxs-lookup"><span data-stu-id="a2973-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="a2973-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="a2973-132">isCommitted</span></span>|<span data-ttu-id="a2973-133">布尔值</span><span class="sxs-lookup"><span data-stu-id="a2973-133">Boolean</span></span>|<span data-ttu-id="a2973-134">指示文件是否已提交的值。</span><span class="sxs-lookup"><span data-stu-id="a2973-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="a2973-135">id</span><span class="sxs-lookup"><span data-stu-id="a2973-135">id</span></span>|<span data-ttu-id="a2973-136">字符串</span><span class="sxs-lookup"><span data-stu-id="a2973-136">String</span></span>|<span data-ttu-id="a2973-137">文件 ID。</span><span class="sxs-lookup"><span data-stu-id="a2973-137">The File Id.</span></span>|
|<span data-ttu-id="a2973-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2973-138">createdDateTime</span></span>|<span data-ttu-id="a2973-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2973-139">DateTimeOffset</span></span>|<span data-ttu-id="a2973-140">创建文件的时间。</span><span class="sxs-lookup"><span data-stu-id="a2973-140">The time the file was created.</span></span>|
|<span data-ttu-id="a2973-141">名称</span><span class="sxs-lookup"><span data-stu-id="a2973-141">name</span></span>|<span data-ttu-id="a2973-142">字符串</span><span class="sxs-lookup"><span data-stu-id="a2973-142">String</span></span>|<span data-ttu-id="a2973-143">文件名称。</span><span class="sxs-lookup"><span data-stu-id="a2973-143">the file name.</span></span>|
|<span data-ttu-id="a2973-144">大小</span><span class="sxs-lookup"><span data-stu-id="a2973-144">size</span></span>|<span data-ttu-id="a2973-145">Int64</span><span class="sxs-lookup"><span data-stu-id="a2973-145">Int64</span></span>|<span data-ttu-id="a2973-146">加密前的文件大小。</span><span class="sxs-lookup"><span data-stu-id="a2973-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="a2973-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="a2973-147">sizeEncrypted</span></span>|<span data-ttu-id="a2973-148">Int64</span><span class="sxs-lookup"><span data-stu-id="a2973-148">Int64</span></span>|<span data-ttu-id="a2973-149">加密后的文件大小。</span><span class="sxs-lookup"><span data-stu-id="a2973-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="a2973-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a2973-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="a2973-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2973-151">DateTimeOffset</span></span>|<span data-ttu-id="a2973-152">Azure 存储 URI 的到期时间。</span><span class="sxs-lookup"><span data-stu-id="a2973-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="a2973-153">清单</span><span class="sxs-lookup"><span data-stu-id="a2973-153">manifest</span></span>|<span data-ttu-id="a2973-154">二进制</span><span class="sxs-lookup"><span data-stu-id="a2973-154">Binary</span></span>|<span data-ttu-id="a2973-155">清单信息。</span><span class="sxs-lookup"><span data-stu-id="a2973-155">The manifest information.</span></span>|
|<span data-ttu-id="a2973-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="a2973-156">uploadState</span></span>|[<span data-ttu-id="a2973-157">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="a2973-157">mobileAppContentFileUploadState</span></span>](../resources/intune_apps_mobileappcontentfileuploadstate.md)|<span data-ttu-id="a2973-p102">当前上载请求的状态。可取值为：`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut`。</span><span class="sxs-lookup"><span data-stu-id="a2973-p102">The state of the current upload request. The possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="a2973-160">响应</span><span class="sxs-lookup"><span data-stu-id="a2973-160">Response</span></span>
<span data-ttu-id="a2973-161">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a2973-161">If successful, this method returns a `200 OK` response code and an updated [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2973-162">示例</span><span class="sxs-lookup"><span data-stu-id="a2973-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2973-163">请求</span><span class="sxs-lookup"><span data-stu-id="a2973-163">Request</span></span>
<span data-ttu-id="a2973-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2973-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files/{mobileAppContentFileId}
Content-type: application/json
Content-length: 283

{
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

### <a name="response"></a><span data-ttu-id="a2973-165">响应</span><span class="sxs-lookup"><span data-stu-id="a2973-165">Response</span></span>
<span data-ttu-id="a2973-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2973-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








