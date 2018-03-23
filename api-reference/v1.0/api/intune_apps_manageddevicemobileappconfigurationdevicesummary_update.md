# <a name="update-manageddevicemobileappconfigurationdevicesummary"></a><span data-ttu-id="c3f3e-101">更新 managedDeviceMobileAppConfigurationDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="c3f3e-101">Update managedDeviceMobileAppConfigurationDeviceSummary</span></span>

> <span data-ttu-id="c3f3e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c3f3e-103">更新 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-103">Update the properties of a [calendar](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c3f3e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3f3e-104">Prerequisites</span></span>
<span data-ttu-id="c3f3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c3f3e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3f3e-107">Permission type</span></span>|<span data-ttu-id="c3f3e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c3f3e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3f3e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3f3e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="c3f3e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3f3e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3f3e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3f3e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3f3e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-112">Not supported.</span></span>|
|<span data-ttu-id="c3f3e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3f3e-113">Application</span></span>|<span data-ttu-id="c3f3e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3f3e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3f3e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="c3f3e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3f3e-116">Request headers</span></span>
|<span data-ttu-id="c3f3e-117">标头</span><span class="sxs-lookup"><span data-stu-id="c3f3e-117">Header</span></span>|<span data-ttu-id="c3f3e-118">值</span><span class="sxs-lookup"><span data-stu-id="c3f3e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3f3e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3f3e-119">Authorization</span></span>|<span data-ttu-id="c3f3e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="c3f3e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="c3f3e-121">Accept</span></span>|<span data-ttu-id="c3f3e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="c3f3e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3f3e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3f3e-123">Request body</span></span>
<span data-ttu-id="c3f3e-124">在请求正文中，提供 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object.</span></span>

<span data-ttu-id="c3f3e-125">下表显示创建 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="c3f3e-126">属性</span><span class="sxs-lookup"><span data-stu-id="c3f3e-126">Property</span></span>|<span data-ttu-id="c3f3e-127">类型</span><span class="sxs-lookup"><span data-stu-id="c3f3e-127">Type</span></span>|<span data-ttu-id="c3f3e-128">说明</span><span class="sxs-lookup"><span data-stu-id="c3f3e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3f3e-129">id</span><span class="sxs-lookup"><span data-stu-id="c3f3e-129">id</span></span>|<span data-ttu-id="c3f3e-130">String</span><span class="sxs-lookup"><span data-stu-id="c3f3e-130">String</span></span>|<span data-ttu-id="c3f3e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-131">Key of the setting.</span></span>|
|<span data-ttu-id="c3f3e-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="c3f3e-132">pendingCount</span></span>|<span data-ttu-id="c3f3e-133">Int32</span><span class="sxs-lookup"><span data-stu-id="c3f3e-133">Int32</span></span>|<span data-ttu-id="c3f3e-134">待定设备的数量</span><span class="sxs-lookup"><span data-stu-id="c3f3e-134">Number of pending devices</span></span>|
|<span data-ttu-id="c3f3e-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="c3f3e-135">notApplicableCount</span></span>|<span data-ttu-id="c3f3e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c3f3e-136">Int32</span></span>|<span data-ttu-id="c3f3e-137">不适用设备的数量</span><span class="sxs-lookup"><span data-stu-id="c3f3e-137">Number of not applicable devices</span></span>|
|<span data-ttu-id="c3f3e-138">successCount</span><span class="sxs-lookup"><span data-stu-id="c3f3e-138">successCount</span></span>|<span data-ttu-id="c3f3e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="c3f3e-139">Int32</span></span>|<span data-ttu-id="c3f3e-140">成功设备的数量</span><span class="sxs-lookup"><span data-stu-id="c3f3e-140">Number of succeeded devices</span></span>|
|<span data-ttu-id="c3f3e-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="c3f3e-141">errorCount</span></span>|<span data-ttu-id="c3f3e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="c3f3e-142">Int32</span></span>|<span data-ttu-id="c3f3e-143">错误设备的数量</span><span class="sxs-lookup"><span data-stu-id="c3f3e-143">Number of error devices</span></span>|
|<span data-ttu-id="c3f3e-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="c3f3e-144">failedCount</span></span>|<span data-ttu-id="c3f3e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="c3f3e-145">Int32</span></span>|<span data-ttu-id="c3f3e-146">失败设备的数量</span><span class="sxs-lookup"><span data-stu-id="c3f3e-146">Number of failed devices</span></span>|
|<span data-ttu-id="c3f3e-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="c3f3e-147">lastUpdateDateTime</span></span>|<span data-ttu-id="c3f3e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3f3e-148">DateTimeOffset</span></span>|<span data-ttu-id="c3f3e-149">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="c3f3e-149">Last update time</span></span>|
|<span data-ttu-id="c3f3e-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="c3f3e-150">configurationVersion</span></span>|<span data-ttu-id="c3f3e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="c3f3e-151">Int32</span></span>|<span data-ttu-id="c3f3e-152">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="c3f3e-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="c3f3e-153">响应</span><span class="sxs-lookup"><span data-stu-id="c3f3e-153">Response</span></span>
<span data-ttu-id="c3f3e-154">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedDeviceMobileAppConfigurationDeviceSummary](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-154">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_manageddevicemobileappconfigurationdevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3f3e-155">示例</span><span class="sxs-lookup"><span data-stu-id="c3f3e-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3f3e-156">请求</span><span class="sxs-lookup"><span data-stu-id="c3f3e-156">Request</span></span>
<span data-ttu-id="c3f3e-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatusSummary
Content-type: application/json
Content-length: 212

{
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```

### <a name="response"></a><span data-ttu-id="c3f3e-158">响应</span><span class="sxs-lookup"><span data-stu-id="c3f3e-158">Response</span></span>
<span data-ttu-id="c3f3e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3f3e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 348

{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceSummary",
  "id": "9997c455-c455-9997-55c4-979955c49799",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```



