# <a name="create-devicecategory"></a><span data-ttu-id="1bf62-101">创建 deviceCategory</span><span class="sxs-lookup"><span data-stu-id="1bf62-101">Create deviceCategory</span></span>

> <span data-ttu-id="1bf62-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1bf62-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1bf62-103">创建新的 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1bf62-103">Create a new [plannerBucket](../resources/intune_onboarding_devicecategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1bf62-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="1bf62-104">Prerequisites</span></span>
<span data-ttu-id="1bf62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="1bf62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1bf62-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="1bf62-107">Permission type</span></span>|<span data-ttu-id="1bf62-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1bf62-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1bf62-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1bf62-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1bf62-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1bf62-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1bf62-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1bf62-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1bf62-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bf62-112">Not supported.</span></span>|
|<span data-ttu-id="1bf62-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="1bf62-113">Application</span></span>|<span data-ttu-id="1bf62-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1bf62-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1bf62-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1bf62-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCategories
```

## <a name="request-headers"></a><span data-ttu-id="1bf62-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="1bf62-116">Request headers</span></span>
|<span data-ttu-id="1bf62-117">标头</span><span class="sxs-lookup"><span data-stu-id="1bf62-117">Header</span></span>|<span data-ttu-id="1bf62-118">值</span><span class="sxs-lookup"><span data-stu-id="1bf62-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1bf62-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1bf62-119">Authorization</span></span>|<span data-ttu-id="1bf62-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1bf62-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="1bf62-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1bf62-121">Accept</span></span>|<span data-ttu-id="1bf62-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1bf62-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1bf62-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="1bf62-123">Request body</span></span>
<span data-ttu-id="1bf62-124">在请求正文中，提供 deviceCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1bf62-124">In the request body, supply a JSON representation of Table object.</span></span>

<span data-ttu-id="1bf62-125">下表显示创建 deviceCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1bf62-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="1bf62-126">属性</span><span class="sxs-lookup"><span data-stu-id="1bf62-126">Property</span></span>|<span data-ttu-id="1bf62-127">类型</span><span class="sxs-lookup"><span data-stu-id="1bf62-127">Type</span></span>|<span data-ttu-id="1bf62-128">说明</span><span class="sxs-lookup"><span data-stu-id="1bf62-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1bf62-129">id</span><span class="sxs-lookup"><span data-stu-id="1bf62-129">id</span></span>|<span data-ttu-id="1bf62-130">String</span><span class="sxs-lookup"><span data-stu-id="1bf62-130">String</span></span>|<span data-ttu-id="1bf62-131">设备类别的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="1bf62-131">Unique identifier for the device category.</span></span> <span data-ttu-id="1bf62-132">只读。</span><span class="sxs-lookup"><span data-stu-id="1bf62-132">Read-only.</span></span>|
|<span data-ttu-id="1bf62-133">displayName</span><span class="sxs-lookup"><span data-stu-id="1bf62-133">displayName</span></span>|<span data-ttu-id="1bf62-134">String</span><span class="sxs-lookup"><span data-stu-id="1bf62-134">String</span></span>|<span data-ttu-id="1bf62-135">设备类别的显示名称。</span><span class="sxs-lookup"><span data-stu-id="1bf62-135">Display name for the device category.</span></span>|
|<span data-ttu-id="1bf62-136">description</span><span class="sxs-lookup"><span data-stu-id="1bf62-136">description</span></span>|<span data-ttu-id="1bf62-137">String</span><span class="sxs-lookup"><span data-stu-id="1bf62-137">String</span></span>|<span data-ttu-id="1bf62-138">设备类别的可选说明。</span><span class="sxs-lookup"><span data-stu-id="1bf62-138">Optional description for the device category.</span></span>|



## <a name="response"></a><span data-ttu-id="1bf62-139">响应</span><span class="sxs-lookup"><span data-stu-id="1bf62-139">Response</span></span>
<span data-ttu-id="1bf62-140">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceCategory](../resources/intune_onboarding_devicecategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1bf62-140">If successful, this method returns a `201 Created` response code and [plannerBucketTaskBoardTaskFormat](../resources/intune_onboarding_devicecategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1bf62-141">示例</span><span class="sxs-lookup"><span data-stu-id="1bf62-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="1bf62-142">请求</span><span class="sxs-lookup"><span data-stu-id="1bf62-142">Request</span></span>
<span data-ttu-id="1bf62-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1bf62-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1bf62-144">响应</span><span class="sxs-lookup"><span data-stu-id="1bf62-144">Response</span></span>
<span data-ttu-id="1bf62-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1bf62-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



