# <a name="update-managedmobileapp"></a><span data-ttu-id="20a56-101">更新 managedMobileApp</span><span class="sxs-lookup"><span data-stu-id="20a56-101">Update managedMobileApp</span></span>

> <span data-ttu-id="20a56-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="20a56-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20a56-103">更新 [managedMobileApp](../resources/intune_mam_managedmobileapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="20a56-103">Update the properties of a [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20a56-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="20a56-104">Prerequisites</span></span>
<span data-ttu-id="20a56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="20a56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="20a56-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="20a56-107">Permission type</span></span>|<span data-ttu-id="20a56-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="20a56-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20a56-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20a56-109">Delegated (work or school account)</span></span>|<span data-ttu-id="20a56-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20a56-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="20a56-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20a56-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20a56-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="20a56-112">Not supported.</span></span>|
|<span data-ttu-id="20a56-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="20a56-113">Application</span></span>|<span data-ttu-id="20a56-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="20a56-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20a56-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20a56-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/defaultManagedAppProtections/{defaultManagedAppProtectionId}/apps/{managedMobileAppId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/apps/{managedMobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="20a56-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="20a56-116">Request headers</span></span>
|<span data-ttu-id="20a56-117">标头</span><span class="sxs-lookup"><span data-stu-id="20a56-117">Header</span></span>|<span data-ttu-id="20a56-118">值</span><span class="sxs-lookup"><span data-stu-id="20a56-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20a56-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="20a56-119">Authorization</span></span>|<span data-ttu-id="20a56-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="20a56-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20a56-121">Accept</span><span class="sxs-lookup"><span data-stu-id="20a56-121">Accept</span></span>|<span data-ttu-id="20a56-122">application/json</span><span class="sxs-lookup"><span data-stu-id="20a56-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20a56-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="20a56-123">Request body</span></span>
<span data-ttu-id="20a56-124">在请求正文中，提供 [managedMobileApp](../resources/intune_mam_managedmobileapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20a56-124">In the request body, supply a JSON representation for the [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object.</span></span>

<span data-ttu-id="20a56-125">下表显示创建 [managedMobileApp](../resources/intune_mam_managedmobileapp.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="20a56-125">The following table shows the properties that are required when you create the [managedMobileApp](../resources/intune_mam_managedmobileapp.md).</span></span>

|<span data-ttu-id="20a56-126">属性</span><span class="sxs-lookup"><span data-stu-id="20a56-126">Property</span></span>|<span data-ttu-id="20a56-127">类型</span><span class="sxs-lookup"><span data-stu-id="20a56-127">Type</span></span>|<span data-ttu-id="20a56-128">说明</span><span class="sxs-lookup"><span data-stu-id="20a56-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20a56-129">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="20a56-129">mobileAppIdentifier</span></span>|[<span data-ttu-id="20a56-130">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="20a56-130">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="20a56-131">包含其操作系统类型的应用标识符。</span><span class="sxs-lookup"><span data-stu-id="20a56-131">The identifier for an app with it's operating system type.</span></span>|
|<span data-ttu-id="20a56-132">id</span><span class="sxs-lookup"><span data-stu-id="20a56-132">id</span></span>|<span data-ttu-id="20a56-133">String</span><span class="sxs-lookup"><span data-stu-id="20a56-133">String</span></span>|<span data-ttu-id="20a56-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="20a56-134">Key of the entity.</span></span>|
|<span data-ttu-id="20a56-135">version</span><span class="sxs-lookup"><span data-stu-id="20a56-135">version</span></span>|<span data-ttu-id="20a56-136">String</span><span class="sxs-lookup"><span data-stu-id="20a56-136">String</span></span>|<span data-ttu-id="20a56-137">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="20a56-137">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="20a56-138">响应</span><span class="sxs-lookup"><span data-stu-id="20a56-138">Response</span></span>
<span data-ttu-id="20a56-139">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedMobileApp](../resources/intune_mam_managedmobileapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="20a56-139">If successful, this method returns a `200 OK` response code and an updated [managedMobileApp](../resources/intune_mam_managedmobileapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20a56-140">示例</span><span class="sxs-lookup"><span data-stu-id="20a56-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="20a56-141">请求</span><span class="sxs-lookup"><span data-stu-id="20a56-141">Request</span></span>
<span data-ttu-id="20a56-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="20a56-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/apps/{managedMobileAppId}
Content-type: application/json
Content-length: 181

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="20a56-143">响应</span><span class="sxs-lookup"><span data-stu-id="20a56-143">Response</span></span>
<span data-ttu-id="20a56-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="20a56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 230

{
  "@odata.type": "#microsoft.graph.managedMobileApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "id": "0a129715-9715-0a12-1597-120a1597120a",
  "version": "Version value"
}
```



