# <a name="create-userinstallstatesummary"></a><span data-ttu-id="cd1ab-101">创建 userInstallStateSummary</span><span class="sxs-lookup"><span data-stu-id="cd1ab-101">Create userInstallStateSummary</span></span>

> <span data-ttu-id="cd1ab-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd1ab-103">创建新的 [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-103">Create a new [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd1ab-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd1ab-104">Prerequisites</span></span>
<span data-ttu-id="cd1ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cd1ab-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd1ab-107">Permission type</span></span>|<span data-ttu-id="cd1ab-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd1ab-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd1ab-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd1ab-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cd1ab-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd1ab-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cd1ab-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd1ab-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd1ab-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-112">Not supported.</span></span>|
|<span data-ttu-id="cd1ab-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd1ab-113">Application</span></span>|<span data-ttu-id="cd1ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd1ab-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd1ab-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="cd1ab-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd1ab-116">Request headers</span></span>
|<span data-ttu-id="cd1ab-117">标头</span><span class="sxs-lookup"><span data-stu-id="cd1ab-117">Header</span></span>|<span data-ttu-id="cd1ab-118">值</span><span class="sxs-lookup"><span data-stu-id="cd1ab-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd1ab-119">授权</span><span class="sxs-lookup"><span data-stu-id="cd1ab-119">Authorization</span></span>|<span data-ttu-id="cd1ab-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd1ab-121">Accept</span><span class="sxs-lookup"><span data-stu-id="cd1ab-121">Accept</span></span>|<span data-ttu-id="cd1ab-122">application/json</span><span class="sxs-lookup"><span data-stu-id="cd1ab-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd1ab-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd1ab-123">Request body</span></span>
<span data-ttu-id="cd1ab-124">在请求正文中，提供 userInstallStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-124">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="cd1ab-125">下表显示创建 userInstallStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-125">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="cd1ab-126">属性</span><span class="sxs-lookup"><span data-stu-id="cd1ab-126">Property</span></span>|<span data-ttu-id="cd1ab-127">类型</span><span class="sxs-lookup"><span data-stu-id="cd1ab-127">Type</span></span>|<span data-ttu-id="cd1ab-128">说明</span><span class="sxs-lookup"><span data-stu-id="cd1ab-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cd1ab-129">ID</span><span class="sxs-lookup"><span data-stu-id="cd1ab-129">id</span></span>|<span data-ttu-id="cd1ab-130">字符串</span><span class="sxs-lookup"><span data-stu-id="cd1ab-130">String</span></span>|<span data-ttu-id="cd1ab-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-131">Key of the entity.</span></span>|
|<span data-ttu-id="cd1ab-132">userName</span><span class="sxs-lookup"><span data-stu-id="cd1ab-132">userName</span></span>|<span data-ttu-id="cd1ab-133">字符串</span><span class="sxs-lookup"><span data-stu-id="cd1ab-133">String</span></span>|<span data-ttu-id="cd1ab-134">用户名。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-134">User name.</span></span>|
|<span data-ttu-id="cd1ab-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd1ab-135">installedDeviceCount</span></span>|<span data-ttu-id="cd1ab-136">Int32</span><span class="sxs-lookup"><span data-stu-id="cd1ab-136">Int32</span></span>|<span data-ttu-id="cd1ab-137">已安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-137">Installed Device Count.</span></span>|
|<span data-ttu-id="cd1ab-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd1ab-138">failedDeviceCount</span></span>|<span data-ttu-id="cd1ab-139">Int32</span><span class="sxs-lookup"><span data-stu-id="cd1ab-139">Int32</span></span>|<span data-ttu-id="cd1ab-140">已失败设备的计数。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-140">Failed Device Count.</span></span>|
|<span data-ttu-id="cd1ab-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="cd1ab-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="cd1ab-142">Int32</span><span class="sxs-lookup"><span data-stu-id="cd1ab-142">Int32</span></span>|<span data-ttu-id="cd1ab-143">未安装设备的计数。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-143">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="cd1ab-144">响应</span><span class="sxs-lookup"><span data-stu-id="cd1ab-144">Response</span></span>
<span data-ttu-id="cd1ab-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-145">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd1ab-146">示例</span><span class="sxs-lookup"><span data-stu-id="cd1ab-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd1ab-147">请求</span><span class="sxs-lookup"><span data-stu-id="cd1ab-147">Request</span></span>
<span data-ttu-id="cd1ab-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="cd1ab-149">响应</span><span class="sxs-lookup"><span data-stu-id="cd1ab-149">Response</span></span>
<span data-ttu-id="cd1ab-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd1ab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```








