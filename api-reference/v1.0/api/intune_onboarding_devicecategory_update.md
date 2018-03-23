# <a name="update-devicecategory"></a><span data-ttu-id="b3b44-101">更新 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="b3b44-101">Update deviceCategory</span></span>

> <span data-ttu-id="b3b44-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b3b44-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b3b44-103">更新 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b3b44-103">Update the properties of a [calendar](../resources/intune_onboarding_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b3b44-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3b44-104">Prerequisites</span></span>
<span data-ttu-id="b3b44-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b3b44-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b3b44-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3b44-107">Permission type</span></span>|<span data-ttu-id="b3b44-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3b44-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3b44-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3b44-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b3b44-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3b44-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="b3b44-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3b44-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3b44-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3b44-112">Not supported.</span></span>|
|<span data-ttu-id="b3b44-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3b44-113">Application</span></span>|<span data-ttu-id="b3b44-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3b44-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3b44-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3b44-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCategories/{deviceCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="b3b44-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3b44-116">Request headers</span></span>
|<span data-ttu-id="b3b44-117">标头</span><span class="sxs-lookup"><span data-stu-id="b3b44-117">Header</span></span>|<span data-ttu-id="b3b44-118">值</span><span class="sxs-lookup"><span data-stu-id="b3b44-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3b44-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3b44-119">Authorization</span></span>|<span data-ttu-id="b3b44-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3b44-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b3b44-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b3b44-121">Accept</span></span>|<span data-ttu-id="b3b44-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b3b44-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3b44-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3b44-123">Request body</span></span>
<span data-ttu-id="b3b44-124">在请求正文中，提供 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b3b44-124">In the request body, supply a JSON representation of [Attachment](../resources/intune_onboarding_devicecategory.md) object.</span></span>

<span data-ttu-id="b3b44-125">下表显示创建 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b3b44-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b3b44-126">属性</span><span class="sxs-lookup"><span data-stu-id="b3b44-126">Property</span></span>|<span data-ttu-id="b3b44-127">类型</span><span class="sxs-lookup"><span data-stu-id="b3b44-127">Type</span></span>|<span data-ttu-id="b3b44-128">说明</span><span class="sxs-lookup"><span data-stu-id="b3b44-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b3b44-129">id</span><span class="sxs-lookup"><span data-stu-id="b3b44-129">id</span></span>|<span data-ttu-id="b3b44-130">String</span><span class="sxs-lookup"><span data-stu-id="b3b44-130">String</span></span>|<span data-ttu-id="b3b44-131">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b3b44-131">Unique identifier for the device category.</span></span> <span data-ttu-id="b3b44-132">只读。</span><span class="sxs-lookup"><span data-stu-id="b3b44-132">Read-only.</span></span>|
|<span data-ttu-id="b3b44-133">displayName</span><span class="sxs-lookup"><span data-stu-id="b3b44-133">displayName</span></span>|<span data-ttu-id="b3b44-134">String</span><span class="sxs-lookup"><span data-stu-id="b3b44-134">String</span></span>|<span data-ttu-id="b3b44-135">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b3b44-135">Display name for the device category.</span></span>|
|<span data-ttu-id="b3b44-136">description</span><span class="sxs-lookup"><span data-stu-id="b3b44-136">description</span></span>|<span data-ttu-id="b3b44-137">String</span><span class="sxs-lookup"><span data-stu-id="b3b44-137">String</span></span>|<span data-ttu-id="b3b44-138">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="b3b44-138">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="b3b44-139">响应</span><span class="sxs-lookup"><span data-stu-id="b3b44-139">Response</span></span>
<span data-ttu-id="b3b44-140">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b3b44-140">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3b44-141">示例</span><span class="sxs-lookup"><span data-stu-id="b3b44-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="b3b44-142">请求</span><span class="sxs-lookup"><span data-stu-id="b3b44-142">Request</span></span>
<span data-ttu-id="b3b44-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3b44-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCategories/{deviceCategoryId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="b3b44-144">响应</span><span class="sxs-lookup"><span data-stu-id="b3b44-144">Response</span></span>
<span data-ttu-id="b3b44-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3b44-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 184

{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "f881b841-b841-f881-41b8-81f841b881f8",
  "displayName": "Display Name value",
  "description": "Description value"
}
```



