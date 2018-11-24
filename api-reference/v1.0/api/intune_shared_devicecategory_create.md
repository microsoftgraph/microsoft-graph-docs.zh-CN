# <a name="create-devicecategory"></a><span data-ttu-id="ea754-101">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="ea754-101">Create deviceCategory</span></span>

> <span data-ttu-id="ea754-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ea754-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ea754-103">创建新的 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea754-103">Create a new [deviceCategory](../resources/intune_shared_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ea754-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="ea754-104">Prerequisites</span></span>
<span data-ttu-id="ea754-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="ea754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ea754-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea754-107">Permission type</span></span>|<span data-ttu-id="ea754-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ea754-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ea754-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea754-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="ea754-110">&nbsp;&nbsp; **入职培训**</span><span class="sxs-lookup"><span data-stu-id="ea754-110">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="ea754-111">DeviceManagementManaged Devices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea754-111">DeviceManagementManaged Devices.ReadWrite.All</span></span>|
|<span data-ttu-id="ea754-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea754-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ea754-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea754-113">Not supported.</span></span>|
|<span data-ttu-id="ea754-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea754-114">Application</span></span>|<span data-ttu-id="ea754-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea754-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea754-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea754-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="ea754-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea754-117">Request headers</span></span>
|<span data-ttu-id="ea754-118">标头</span><span class="sxs-lookup"><span data-stu-id="ea754-118">Header</span></span>|<span data-ttu-id="ea754-119">值</span><span class="sxs-lookup"><span data-stu-id="ea754-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ea754-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea754-120">Authorization</span></span>|<span data-ttu-id="ea754-121">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ea754-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ea754-122">Accept</span><span class="sxs-lookup"><span data-stu-id="ea754-122">Accept</span></span>|<span data-ttu-id="ea754-123">application/json</span><span class="sxs-lookup"><span data-stu-id="ea754-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea754-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea754-124">Request body</span></span>
<span data-ttu-id="ea754-125">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea754-125">In the request body, supply a JSON representation for the deviceCategory object.</span></span>

<span data-ttu-id="ea754-126">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ea754-126">The following table shows the properties that are required when you create the deviceCategory.</span></span>

|<span data-ttu-id="ea754-127">属性</span><span class="sxs-lookup"><span data-stu-id="ea754-127">Property</span></span>|<span data-ttu-id="ea754-128">类型</span><span class="sxs-lookup"><span data-stu-id="ea754-128">Type</span></span>|<span data-ttu-id="ea754-129">说明</span><span class="sxs-lookup"><span data-stu-id="ea754-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea754-130">id</span><span class="sxs-lookup"><span data-stu-id="ea754-130">id</span></span>|<span data-ttu-id="ea754-131">String</span><span class="sxs-lookup"><span data-stu-id="ea754-131">String</span></span>|<span data-ttu-id="ea754-132">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ea754-132">Unique identifier for the device category.</span></span> <span data-ttu-id="ea754-133">只读。</span><span class="sxs-lookup"><span data-stu-id="ea754-133">Read-only.</span></span>|
|<span data-ttu-id="ea754-134">**入职培训**</span><span class="sxs-lookup"><span data-stu-id="ea754-134">**Onboarding**</span></span>|
|<span data-ttu-id="ea754-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ea754-135">displayName</span></span>|<span data-ttu-id="ea754-136">String</span><span class="sxs-lookup"><span data-stu-id="ea754-136">String</span></span>|<span data-ttu-id="ea754-137">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ea754-137">Display name for the device category.</span></span>|
|<span data-ttu-id="ea754-138">description</span><span class="sxs-lookup"><span data-stu-id="ea754-138">description</span></span>|<span data-ttu-id="ea754-139">String</span><span class="sxs-lookup"><span data-stu-id="ea754-139">String</span></span>|<span data-ttu-id="ea754-140">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="ea754-140">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="ea754-141">响应</span><span class="sxs-lookup"><span data-stu-id="ea754-141">Response</span></span>
<span data-ttu-id="ea754-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune_shared_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea754-142">If successful, this method returns a `201 Created` response code and a [deviceCategory](../resources/intune_shared_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea754-143">示例</span><span class="sxs-lookup"><span data-stu-id="ea754-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="ea754-144">请求</span><span class="sxs-lookup"><span data-stu-id="ea754-144">Request</span></span>
<span data-ttu-id="ea754-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea754-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories
Content-type: application/json
Content-length: 135

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="ea754-146">响应</span><span class="sxs-lookup"><span data-stu-id="ea754-146">Response</span></span>
<span data-ttu-id="ea754-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea754-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



