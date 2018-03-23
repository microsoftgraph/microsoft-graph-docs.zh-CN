# <a name="update-managedappstatusraw"></a><span data-ttu-id="0b632-101">更新 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="0b632-101">Update managedAppStatusRaw</span></span>

> <span data-ttu-id="0b632-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b632-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b632-103">更新 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0b632-103">Update the properties of a [calendar](../resources/intune_mam_managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0b632-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0b632-104">Prerequisites</span></span>
<span data-ttu-id="0b632-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0b632-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0b632-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b632-107">Permission type</span></span>|<span data-ttu-id="0b632-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0b632-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b632-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b632-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0b632-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b632-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0b632-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b632-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b632-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b632-112">Not supported.</span></span>|
|<span data-ttu-id="0b632-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="0b632-113">Application</span></span>|<span data-ttu-id="0b632-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0b632-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b632-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b632-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppStatuses/{managedAppStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="0b632-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b632-116">Request headers</span></span>
|<span data-ttu-id="0b632-117">标头</span><span class="sxs-lookup"><span data-stu-id="0b632-117">Header</span></span>|<span data-ttu-id="0b632-118">值</span><span class="sxs-lookup"><span data-stu-id="0b632-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0b632-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b632-119">Authorization</span></span>|<span data-ttu-id="0b632-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0b632-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0b632-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0b632-121">Accept</span></span>|<span data-ttu-id="0b632-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0b632-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b632-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b632-123">Request body</span></span>
<span data-ttu-id="0b632-124">在请求正文中，提供 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0b632-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_managedappstatusraw.md) object.</span></span>

<span data-ttu-id="0b632-125">下表显示创建 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0b632-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0b632-126">属性</span><span class="sxs-lookup"><span data-stu-id="0b632-126">Property</span></span>|<span data-ttu-id="0b632-127">类型</span><span class="sxs-lookup"><span data-stu-id="0b632-127">Type</span></span>|<span data-ttu-id="0b632-128">说明</span><span class="sxs-lookup"><span data-stu-id="0b632-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b632-129">displayName</span><span class="sxs-lookup"><span data-stu-id="0b632-129">displayName</span></span>|<span data-ttu-id="0b632-130">String</span><span class="sxs-lookup"><span data-stu-id="0b632-130">String</span></span>|<span data-ttu-id="0b632-131">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="0b632-131">Friendly name of the status report.</span></span> <span data-ttu-id="0b632-132">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0b632-132">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="0b632-133">id</span><span class="sxs-lookup"><span data-stu-id="0b632-133">id</span></span>|<span data-ttu-id="0b632-134">String</span><span class="sxs-lookup"><span data-stu-id="0b632-134">String</span></span>|<span data-ttu-id="0b632-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0b632-135">Key of the setting.</span></span> <span data-ttu-id="0b632-136">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0b632-136">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="0b632-137">version</span><span class="sxs-lookup"><span data-stu-id="0b632-137">version</span></span>|<span data-ttu-id="0b632-138">String</span><span class="sxs-lookup"><span data-stu-id="0b632-138">String</span></span>|<span data-ttu-id="0b632-139">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="0b632-139">Version of the entity.</span></span> <span data-ttu-id="0b632-140">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="0b632-140">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="0b632-141">content</span><span class="sxs-lookup"><span data-stu-id="0b632-141">content</span></span>|[<span data-ttu-id="0b632-142">Json</span><span class="sxs-lookup"><span data-stu-id="0b632-142">json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="0b632-143">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="0b632-143">Status report content.</span></span>|



## <a name="response"></a><span data-ttu-id="0b632-144">响应</span><span class="sxs-lookup"><span data-stu-id="0b632-144">Response</span></span>
<span data-ttu-id="0b632-145">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b632-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0b632-146">示例</span><span class="sxs-lookup"><span data-stu-id="0b632-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="0b632-147">请求</span><span class="sxs-lookup"><span data-stu-id="0b632-147">Request</span></span>
<span data-ttu-id="0b632-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0b632-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses/{managedAppStatusId}
Content-type: application/json
Content-length: 139

{
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a><span data-ttu-id="0b632-149">响应</span><span class="sxs-lookup"><span data-stu-id="0b632-149">Response</span></span>
<span data-ttu-id="0b632-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0b632-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 246

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "id": "80847581-7581-8084-8175-848081758480",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```



