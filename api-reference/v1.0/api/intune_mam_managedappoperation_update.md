# <a name="update-managedappoperation"></a><span data-ttu-id="33d2d-101">更新 managedAppOperation</span><span class="sxs-lookup"><span data-stu-id="33d2d-101">Update managedAppOperation</span></span>

> <span data-ttu-id="33d2d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="33d2d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33d2d-103">更新 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="33d2d-103">Update the properties of a [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33d2d-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="33d2d-104">Prerequisites</span></span>
<span data-ttu-id="33d2d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="33d2d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="33d2d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="33d2d-107">Permission type</span></span>|<span data-ttu-id="33d2d-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="33d2d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33d2d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="33d2d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="33d2d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="33d2d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="33d2d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="33d2d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33d2d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="33d2d-112">Not supported.</span></span>|
|<span data-ttu-id="33d2d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="33d2d-113">Application</span></span>|<span data-ttu-id="33d2d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="33d2d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33d2d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="33d2d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="33d2d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="33d2d-116">Request headers</span></span>
|<span data-ttu-id="33d2d-117">标头</span><span class="sxs-lookup"><span data-stu-id="33d2d-117">Header</span></span>|<span data-ttu-id="33d2d-118">值</span><span class="sxs-lookup"><span data-stu-id="33d2d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33d2d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="33d2d-119">Authorization</span></span>|<span data-ttu-id="33d2d-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="33d2d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33d2d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="33d2d-121">Accept</span></span>|<span data-ttu-id="33d2d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="33d2d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33d2d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="33d2d-123">Request body</span></span>
<span data-ttu-id="33d2d-124">在请求正文中，提供 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="33d2d-124">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>

<span data-ttu-id="33d2d-125">下表显示创建 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="33d2d-125">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span></span>

|<span data-ttu-id="33d2d-126">属性</span><span class="sxs-lookup"><span data-stu-id="33d2d-126">Property</span></span>|<span data-ttu-id="33d2d-127">类型</span><span class="sxs-lookup"><span data-stu-id="33d2d-127">Type</span></span>|<span data-ttu-id="33d2d-128">说明</span><span class="sxs-lookup"><span data-stu-id="33d2d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33d2d-129">displayName</span><span class="sxs-lookup"><span data-stu-id="33d2d-129">displayName</span></span>|<span data-ttu-id="33d2d-130">String</span><span class="sxs-lookup"><span data-stu-id="33d2d-130">String</span></span>|<span data-ttu-id="33d2d-131">操作名称。</span><span class="sxs-lookup"><span data-stu-id="33d2d-131">The operation name.</span></span>|
|<span data-ttu-id="33d2d-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="33d2d-132">lastModifiedDateTime</span></span>|<span data-ttu-id="33d2d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="33d2d-133">DateTimeOffset</span></span>|<span data-ttu-id="33d2d-134">上次修改应用操作的时间。</span><span class="sxs-lookup"><span data-stu-id="33d2d-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="33d2d-135">state</span><span class="sxs-lookup"><span data-stu-id="33d2d-135">state</span></span>|<span data-ttu-id="33d2d-136">String</span><span class="sxs-lookup"><span data-stu-id="33d2d-136">String</span></span>|<span data-ttu-id="33d2d-137">操作的当前状态</span><span class="sxs-lookup"><span data-stu-id="33d2d-137">The current state of the operation</span></span>|
|<span data-ttu-id="33d2d-138">id</span><span class="sxs-lookup"><span data-stu-id="33d2d-138">id</span></span>|<span data-ttu-id="33d2d-139">String</span><span class="sxs-lookup"><span data-stu-id="33d2d-139">String</span></span>|<span data-ttu-id="33d2d-140">实体的键。</span><span class="sxs-lookup"><span data-stu-id="33d2d-140">Key of the entity.</span></span>|
|<span data-ttu-id="33d2d-141">version</span><span class="sxs-lookup"><span data-stu-id="33d2d-141">version</span></span>|<span data-ttu-id="33d2d-142">String</span><span class="sxs-lookup"><span data-stu-id="33d2d-142">String</span></span>|<span data-ttu-id="33d2d-143">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="33d2d-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="33d2d-144">响应</span><span class="sxs-lookup"><span data-stu-id="33d2d-144">Response</span></span>
<span data-ttu-id="33d2d-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppOperation](../resources/intune_mam_managedappoperation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="33d2d-145">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune_mam_managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33d2d-146">示例</span><span class="sxs-lookup"><span data-stu-id="33d2d-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="33d2d-147">请求</span><span class="sxs-lookup"><span data-stu-id="33d2d-147">Request</span></span>
<span data-ttu-id="33d2d-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="33d2d-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 159

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="33d2d-149">响应</span><span class="sxs-lookup"><span data-stu-id="33d2d-149">Response</span></span>
<span data-ttu-id="33d2d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="33d2d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```



