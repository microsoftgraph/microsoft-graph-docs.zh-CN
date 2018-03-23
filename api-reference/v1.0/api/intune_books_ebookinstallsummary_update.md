# <a name="update-ebookinstallsummary"></a><span data-ttu-id="48287-101">更新 eBookInstallSummary</span><span class="sxs-lookup"><span data-stu-id="48287-101">Update eBookInstallSummary</span></span>

> <span data-ttu-id="48287-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="48287-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="48287-103">更新 [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="48287-103">Update the properties of a [calendar](../resources/intune_books_ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="48287-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="48287-104">Prerequisites</span></span>
<span data-ttu-id="48287-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="48287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="48287-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="48287-107">Permission type</span></span>|<span data-ttu-id="48287-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="48287-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="48287-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="48287-109">Delegated (work or school account)</span></span>|<span data-ttu-id="48287-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="48287-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="48287-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="48287-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="48287-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="48287-112">Not supported.</span></span>|
|<span data-ttu-id="48287-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="48287-113">Application</span></span>|<span data-ttu-id="48287-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="48287-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="48287-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="48287-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="48287-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="48287-116">Request headers</span></span>
|<span data-ttu-id="48287-117">标头</span><span class="sxs-lookup"><span data-stu-id="48287-117">Header</span></span>|<span data-ttu-id="48287-118">值</span><span class="sxs-lookup"><span data-stu-id="48287-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="48287-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="48287-119">Authorization</span></span>|<span data-ttu-id="48287-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="48287-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="48287-121">Accept</span><span class="sxs-lookup"><span data-stu-id="48287-121">Accept</span></span>|<span data-ttu-id="48287-122">application/json</span><span class="sxs-lookup"><span data-stu-id="48287-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="48287-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="48287-123">Request body</span></span>
<span data-ttu-id="48287-124">在请求正文中，提供 [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="48287-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_books_ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="48287-125">下表显示了创建 [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="48287-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="48287-126">属性</span><span class="sxs-lookup"><span data-stu-id="48287-126">Property</span></span>|<span data-ttu-id="48287-127">类型</span><span class="sxs-lookup"><span data-stu-id="48287-127">Type</span></span>|<span data-ttu-id="48287-128">说明</span><span class="sxs-lookup"><span data-stu-id="48287-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="48287-129">id</span><span class="sxs-lookup"><span data-stu-id="48287-129">id</span></span>|<span data-ttu-id="48287-130">String</span><span class="sxs-lookup"><span data-stu-id="48287-130">String</span></span>|<span data-ttu-id="48287-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="48287-131">Key of the setting.</span></span>|
|<span data-ttu-id="48287-132">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="48287-132">installedDeviceCount</span></span>|<span data-ttu-id="48287-133">Int32</span><span class="sxs-lookup"><span data-stu-id="48287-133">Int32</span></span>|<span data-ttu-id="48287-134">已成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="48287-134">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="48287-135">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="48287-135">failedDeviceCount</span></span>|<span data-ttu-id="48287-136">Int32</span><span class="sxs-lookup"><span data-stu-id="48287-136">Int32</span></span>|<span data-ttu-id="48287-137">未能成功安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="48287-137">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="48287-138">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="48287-138">notInstalledDeviceCount</span></span>|<span data-ttu-id="48287-139">Int32</span><span class="sxs-lookup"><span data-stu-id="48287-139">Int32</span></span>|<span data-ttu-id="48287-140">未安装此书籍的设备数量。</span><span class="sxs-lookup"><span data-stu-id="48287-140">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="48287-141">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="48287-141">installedUserCount</span></span>|<span data-ttu-id="48287-142">Int32</span><span class="sxs-lookup"><span data-stu-id="48287-142">Int32</span></span>|<span data-ttu-id="48287-143">其设备全部成功安装了此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="48287-143">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="48287-144">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="48287-144">failedUserCount</span></span>|<span data-ttu-id="48287-145">Int32</span><span class="sxs-lookup"><span data-stu-id="48287-145">Int32</span></span>|<span data-ttu-id="48287-146">有 1 个或多个设备未能安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="48287-146">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="48287-147">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="48287-147">notInstalledUserCount</span></span>|<span data-ttu-id="48287-148">Int32</span><span class="sxs-lookup"><span data-stu-id="48287-148">Int32</span></span>|<span data-ttu-id="48287-149">未安装此书籍的用户数量。</span><span class="sxs-lookup"><span data-stu-id="48287-149">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="48287-150">响应</span><span class="sxs-lookup"><span data-stu-id="48287-150">Response</span></span>
<span data-ttu-id="48287-151">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="48287-151">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_books_ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="48287-152">示例</span><span class="sxs-lookup"><span data-stu-id="48287-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="48287-153">请求</span><span class="sxs-lookup"><span data-stu-id="48287-153">Request</span></span>
<span data-ttu-id="48287-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="48287-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="48287-155">响应</span><span class="sxs-lookup"><span data-stu-id="48287-155">Response</span></span>
<span data-ttu-id="48287-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="48287-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```



