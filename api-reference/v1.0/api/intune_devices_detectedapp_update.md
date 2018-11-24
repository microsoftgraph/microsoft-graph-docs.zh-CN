# <a name="update-detectedapp"></a><span data-ttu-id="73d82-101">更新 detectedApp</span><span class="sxs-lookup"><span data-stu-id="73d82-101">Update detectedApp</span></span>

> <span data-ttu-id="73d82-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="73d82-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73d82-103">更新 [detectedApp](../resources/intune_devices_detectedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="73d82-103">Update the properties of a [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73d82-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="73d82-104">Prerequisites</span></span>
<span data-ttu-id="73d82-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="73d82-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73d82-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="73d82-107">Permission type</span></span>|<span data-ttu-id="73d82-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73d82-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73d82-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73d82-109">Delegated (work or school account)</span></span>|<span data-ttu-id="73d82-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73d82-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="73d82-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73d82-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73d82-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="73d82-112">Not supported.</span></span>|
|<span data-ttu-id="73d82-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="73d82-113">Application</span></span>|<span data-ttu-id="73d82-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="73d82-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73d82-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73d82-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/detectedApps/{detectedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="73d82-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="73d82-116">Request headers</span></span>
|<span data-ttu-id="73d82-117">标头</span><span class="sxs-lookup"><span data-stu-id="73d82-117">Header</span></span>|<span data-ttu-id="73d82-118">值</span><span class="sxs-lookup"><span data-stu-id="73d82-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73d82-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="73d82-119">Authorization</span></span>|<span data-ttu-id="73d82-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73d82-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73d82-121">Accept</span><span class="sxs-lookup"><span data-stu-id="73d82-121">Accept</span></span>|<span data-ttu-id="73d82-122">application/json</span><span class="sxs-lookup"><span data-stu-id="73d82-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73d82-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="73d82-123">Request body</span></span>
<span data-ttu-id="73d82-124">在请求正文中，提供 [detectedApp](../resources/intune_devices_detectedapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73d82-124">In the request body, supply a JSON representation for the [detectedApp](../resources/intune_devices_detectedapp.md) object.</span></span>

<span data-ttu-id="73d82-125">下表显示创建 [detectedApp](../resources/intune_devices_detectedapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73d82-125">The following table shows the properties that are required when you create the [detectedApp](../resources/intune_devices_detectedapp.md).</span></span>

|<span data-ttu-id="73d82-126">属性</span><span class="sxs-lookup"><span data-stu-id="73d82-126">Property</span></span>|<span data-ttu-id="73d82-127">类型</span><span class="sxs-lookup"><span data-stu-id="73d82-127">Type</span></span>|<span data-ttu-id="73d82-128">说明</span><span class="sxs-lookup"><span data-stu-id="73d82-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73d82-129">id</span><span class="sxs-lookup"><span data-stu-id="73d82-129">id</span></span>|<span data-ttu-id="73d82-130">String</span><span class="sxs-lookup"><span data-stu-id="73d82-130">String</span></span>|<span data-ttu-id="73d82-131">检测到的应用程序的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="73d82-131">The unique Identifier for the detected application.</span></span> <span data-ttu-id="73d82-132">创建此应用程序时，Intune 将自动生成它。</span><span class="sxs-lookup"><span data-stu-id="73d82-132">This is automatically generated by Intune at the time the application is created.</span></span> <span data-ttu-id="73d82-133">只读。</span><span class="sxs-lookup"><span data-stu-id="73d82-133">Read-only.</span></span>|
|<span data-ttu-id="73d82-134">displayName</span><span class="sxs-lookup"><span data-stu-id="73d82-134">displayName</span></span>|<span data-ttu-id="73d82-135">String</span><span class="sxs-lookup"><span data-stu-id="73d82-135">String</span></span>|<span data-ttu-id="73d82-136">发现的应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="73d82-136">Name of the discovered application.</span></span> <span data-ttu-id="73d82-137">只读</span><span class="sxs-lookup"><span data-stu-id="73d82-137">Read-only</span></span>|
|<span data-ttu-id="73d82-138">version</span><span class="sxs-lookup"><span data-stu-id="73d82-138">version</span></span>|<span data-ttu-id="73d82-139">String</span><span class="sxs-lookup"><span data-stu-id="73d82-139">String</span></span>|<span data-ttu-id="73d82-140">发现的应用程序的版本。</span><span class="sxs-lookup"><span data-stu-id="73d82-140">Version of the discovered application.</span></span> <span data-ttu-id="73d82-141">只读</span><span class="sxs-lookup"><span data-stu-id="73d82-141">Read-only</span></span>|
|<span data-ttu-id="73d82-142">sizeInByte</span><span class="sxs-lookup"><span data-stu-id="73d82-142">sizeInByte</span></span>|<span data-ttu-id="73d82-143">Int64</span><span class="sxs-lookup"><span data-stu-id="73d82-143">Int64</span></span>|<span data-ttu-id="73d82-144">发现的应用程序的大小，以字节为单位。</span><span class="sxs-lookup"><span data-stu-id="73d82-144">Discovered application size in bytes.</span></span> <span data-ttu-id="73d82-145">只读</span><span class="sxs-lookup"><span data-stu-id="73d82-145">Read-only</span></span>|
|<span data-ttu-id="73d82-146">deviceCount</span><span class="sxs-lookup"><span data-stu-id="73d82-146">deviceCount</span></span>|<span data-ttu-id="73d82-147">Int32</span><span class="sxs-lookup"><span data-stu-id="73d82-147">Int32</span></span>|<span data-ttu-id="73d82-148">已安装此应用程序的设备数量</span><span class="sxs-lookup"><span data-stu-id="73d82-148">The number of devices that have installed this application</span></span>|



## <a name="response"></a><span data-ttu-id="73d82-149">响应</span><span class="sxs-lookup"><span data-stu-id="73d82-149">Response</span></span>
<span data-ttu-id="73d82-150">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [detectedApp](../resources/intune_devices_detectedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="73d82-150">If successful, this method returns a `200 OK` response code and an updated [detectedApp](../resources/intune_devices_detectedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73d82-151">示例</span><span class="sxs-lookup"><span data-stu-id="73d82-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="73d82-152">请求</span><span class="sxs-lookup"><span data-stu-id="73d82-152">Request</span></span>
<span data-ttu-id="73d82-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73d82-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/detectedApps/{detectedAppId}
Content-type: application/json
Content-length: 167

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="73d82-154">响应</span><span class="sxs-lookup"><span data-stu-id="73d82-154">Response</span></span>
<span data-ttu-id="73d82-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73d82-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "@odata.type": "#microsoft.graph.detectedApp",
  "id": "caf60db6-0db6-caf6-b60d-f6cab60df6ca",
  "displayName": "Display Name value",
  "version": "Version value",
  "sizeInByte": 10,
  "deviceCount": 11
}
```



