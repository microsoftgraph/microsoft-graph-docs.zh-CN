# <a name="create-managedappstatusraw"></a><span data-ttu-id="7339b-101">创建 managedAppStatusRaw</span><span class="sxs-lookup"><span data-stu-id="7339b-101">Create managedAppStatusRaw</span></span>

> <span data-ttu-id="7339b-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7339b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7339b-103">创建新的 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7339b-103">Create a new [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7339b-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="7339b-104">Prerequisites</span></span>
<span data-ttu-id="7339b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7339b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="7339b-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="7339b-107">Permission type</span></span>|<span data-ttu-id="7339b-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7339b-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7339b-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7339b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="7339b-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7339b-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7339b-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7339b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7339b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="7339b-112">Not supported.</span></span>|
|<span data-ttu-id="7339b-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="7339b-113">Application</span></span>|<span data-ttu-id="7339b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7339b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7339b-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7339b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppStatuses
```

## <a name="request-headers"></a><span data-ttu-id="7339b-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="7339b-116">Request headers</span></span>
|<span data-ttu-id="7339b-117">标头</span><span class="sxs-lookup"><span data-stu-id="7339b-117">Header</span></span>|<span data-ttu-id="7339b-118">值</span><span class="sxs-lookup"><span data-stu-id="7339b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7339b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="7339b-119">Authorization</span></span>|<span data-ttu-id="7339b-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7339b-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7339b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="7339b-121">Accept</span></span>|<span data-ttu-id="7339b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="7339b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7339b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7339b-123">Request body</span></span>
<span data-ttu-id="7339b-124">在请求正文中，提供 managedAppStatusRaw 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7339b-124">In the request body, supply a JSON representation for the managedAppStatusRaw object.</span></span>

<span data-ttu-id="7339b-125">下表显示创建 managedAppStatusRaw 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7339b-125">The following table shows the properties that are required when you create the managedAppStatusRaw.</span></span>

|<span data-ttu-id="7339b-126">属性</span><span class="sxs-lookup"><span data-stu-id="7339b-126">Property</span></span>|<span data-ttu-id="7339b-127">类型</span><span class="sxs-lookup"><span data-stu-id="7339b-127">Type</span></span>|<span data-ttu-id="7339b-128">说明</span><span class="sxs-lookup"><span data-stu-id="7339b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7339b-129">displayName</span><span class="sxs-lookup"><span data-stu-id="7339b-129">displayName</span></span>|<span data-ttu-id="7339b-130">String</span><span class="sxs-lookup"><span data-stu-id="7339b-130">String</span></span>|<span data-ttu-id="7339b-131">状态报告的友好名称。</span><span class="sxs-lookup"><span data-stu-id="7339b-131">Friendly name of the status report.</span></span> <span data-ttu-id="7339b-132">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7339b-132">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="7339b-133">id</span><span class="sxs-lookup"><span data-stu-id="7339b-133">id</span></span>|<span data-ttu-id="7339b-134">String</span><span class="sxs-lookup"><span data-stu-id="7339b-134">String</span></span>|<span data-ttu-id="7339b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7339b-135">Key of the entity.</span></span> <span data-ttu-id="7339b-136">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7339b-136">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="7339b-137">version</span><span class="sxs-lookup"><span data-stu-id="7339b-137">version</span></span>|<span data-ttu-id="7339b-138">String</span><span class="sxs-lookup"><span data-stu-id="7339b-138">String</span></span>|<span data-ttu-id="7339b-139">实体的版本。</span><span class="sxs-lookup"><span data-stu-id="7339b-139">Version of the entity.</span></span> <span data-ttu-id="7339b-140">继承自 [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span><span class="sxs-lookup"><span data-stu-id="7339b-140">Inherited from [managedAppStatus](../resources/intune_mam_managedappstatus.md)</span></span>|
|<span data-ttu-id="7339b-141">content</span><span class="sxs-lookup"><span data-stu-id="7339b-141">content</span></span>|[<span data-ttu-id="7339b-142">Json</span><span class="sxs-lookup"><span data-stu-id="7339b-142">Json</span></span>](../resources/intune_mam_json.md)|<span data-ttu-id="7339b-143">状态报告内容。</span><span class="sxs-lookup"><span data-stu-id="7339b-143">Status report content.</span></span>|



## <a name="response"></a><span data-ttu-id="7339b-144">响应</span><span class="sxs-lookup"><span data-stu-id="7339b-144">Response</span></span>
<span data-ttu-id="7339b-145">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7339b-145">If successful, this method returns a `201 Created` response code and a [managedAppStatusRaw](../resources/intune_mam_managedappstatusraw.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7339b-146">示例</span><span class="sxs-lookup"><span data-stu-id="7339b-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="7339b-147">请求</span><span class="sxs-lookup"><span data-stu-id="7339b-147">Request</span></span>
<span data-ttu-id="7339b-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7339b-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppStatuses
Content-type: application/json
Content-length: 197

{
  "@odata.type": "#microsoft.graph.managedAppStatusRaw",
  "displayName": "Display Name value",
  "version": "Version value",
  "content": {
    "@odata.type": "microsoft.graph.Json"
  }
}
```

### <a name="response"></a><span data-ttu-id="7339b-149">响应</span><span class="sxs-lookup"><span data-stu-id="7339b-149">Response</span></span>
<span data-ttu-id="7339b-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7339b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



