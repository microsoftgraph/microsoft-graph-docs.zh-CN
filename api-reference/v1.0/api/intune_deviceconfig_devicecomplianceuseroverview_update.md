# <a name="update-devicecomplianceuseroverview"></a><span data-ttu-id="04001-101">更新 deviceComplianceUserOverview</span><span class="sxs-lookup"><span data-stu-id="04001-101">Update deviceComplianceUserOverview</span></span>

> <span data-ttu-id="04001-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="04001-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="04001-103">更新 [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="04001-103">Update the properties of a [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="04001-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="04001-104">Prerequisites</span></span>
<span data-ttu-id="04001-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="04001-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="04001-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="04001-107">Permission type</span></span>|<span data-ttu-id="04001-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04001-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04001-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04001-109">Delegated (work or school account)</span></span>|<span data-ttu-id="04001-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04001-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04001-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04001-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04001-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="04001-112">Not supported.</span></span>|
|<span data-ttu-id="04001-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="04001-113">Application</span></span>|<span data-ttu-id="04001-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="04001-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04001-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04001-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
```

## <a name="request-headers"></a><span data-ttu-id="04001-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="04001-116">Request headers</span></span>
|<span data-ttu-id="04001-117">标头</span><span class="sxs-lookup"><span data-stu-id="04001-117">Header</span></span>|<span data-ttu-id="04001-118">值</span><span class="sxs-lookup"><span data-stu-id="04001-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04001-119">授权</span><span class="sxs-lookup"><span data-stu-id="04001-119">Authorization</span></span>|<span data-ttu-id="04001-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04001-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04001-121">接受</span><span class="sxs-lookup"><span data-stu-id="04001-121">Accept</span></span>|<span data-ttu-id="04001-122">application/json</span><span class="sxs-lookup"><span data-stu-id="04001-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04001-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="04001-123">Request body</span></span>
<span data-ttu-id="04001-124">在请求正文中，提供 [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04001-124">In the request body, supply a JSON representation for the [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object.</span></span>

<span data-ttu-id="04001-125">下表显示了创建 [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="04001-125">The following table shows the properties that are required when you create the [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md).</span></span>

|<span data-ttu-id="04001-126">属性</span><span class="sxs-lookup"><span data-stu-id="04001-126">Property</span></span>|<span data-ttu-id="04001-127">类型</span><span class="sxs-lookup"><span data-stu-id="04001-127">Type</span></span>|<span data-ttu-id="04001-128">说明</span><span class="sxs-lookup"><span data-stu-id="04001-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04001-129">ID</span><span class="sxs-lookup"><span data-stu-id="04001-129">id</span></span>|<span data-ttu-id="04001-130">字符串</span><span class="sxs-lookup"><span data-stu-id="04001-130">String</span></span>|<span data-ttu-id="04001-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="04001-131">Key of the entity.</span></span>|
|<span data-ttu-id="04001-132">pendingCount</span><span class="sxs-lookup"><span data-stu-id="04001-132">pendingCount</span></span>|<span data-ttu-id="04001-133">Int32</span><span class="sxs-lookup"><span data-stu-id="04001-133">Int32</span></span>|<span data-ttu-id="04001-134">待定用户的数量</span><span class="sxs-lookup"><span data-stu-id="04001-134">Number of pending Users</span></span>|
|<span data-ttu-id="04001-135">notApplicableCount</span><span class="sxs-lookup"><span data-stu-id="04001-135">notApplicableCount</span></span>|<span data-ttu-id="04001-136">Int32</span><span class="sxs-lookup"><span data-stu-id="04001-136">Int32</span></span>|<span data-ttu-id="04001-137">不适用用户的数量</span><span class="sxs-lookup"><span data-stu-id="04001-137">Number of not applicable users.</span></span>|
|<span data-ttu-id="04001-138">successCount</span><span class="sxs-lookup"><span data-stu-id="04001-138">successCount</span></span>|<span data-ttu-id="04001-139">Int32</span><span class="sxs-lookup"><span data-stu-id="04001-139">Int32</span></span>|<span data-ttu-id="04001-140">成功用户的数量</span><span class="sxs-lookup"><span data-stu-id="04001-140">Number of succeeded Users</span></span>|
|<span data-ttu-id="04001-141">errorCount</span><span class="sxs-lookup"><span data-stu-id="04001-141">errorCount</span></span>|<span data-ttu-id="04001-142">Int32</span><span class="sxs-lookup"><span data-stu-id="04001-142">Int32</span></span>|<span data-ttu-id="04001-143">错误用户的数量</span><span class="sxs-lookup"><span data-stu-id="04001-143">Number of error Users</span></span>|
|<span data-ttu-id="04001-144">failedCount</span><span class="sxs-lookup"><span data-stu-id="04001-144">failedCount</span></span>|<span data-ttu-id="04001-145">Int32</span><span class="sxs-lookup"><span data-stu-id="04001-145">Int32</span></span>|<span data-ttu-id="04001-146">失败用户的数量</span><span class="sxs-lookup"><span data-stu-id="04001-146">Number of failed Users</span></span>|
|<span data-ttu-id="04001-147">lastUpdateDateTime</span><span class="sxs-lookup"><span data-stu-id="04001-147">lastUpdateDateTime</span></span>|<span data-ttu-id="04001-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="04001-148">DateTimeOffset</span></span>|<span data-ttu-id="04001-149">上次更新时间</span><span class="sxs-lookup"><span data-stu-id="04001-149">Last update time</span></span>|
|<span data-ttu-id="04001-150">configurationVersion</span><span class="sxs-lookup"><span data-stu-id="04001-150">configurationVersion</span></span>|<span data-ttu-id="04001-151">Int32</span><span class="sxs-lookup"><span data-stu-id="04001-151">Int32</span></span>|<span data-ttu-id="04001-152">用于此概述的策略版本</span><span class="sxs-lookup"><span data-stu-id="04001-152">Version of the policy for that overview</span></span>|



## <a name="response"></a><span data-ttu-id="04001-153">响应</span><span class="sxs-lookup"><span data-stu-id="04001-153">Response</span></span>
<span data-ttu-id="04001-154">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="04001-154">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceUserOverview](../resources/intune_deviceconfig_devicecomplianceuseroverview.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="04001-155">示例</span><span class="sxs-lookup"><span data-stu-id="04001-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="04001-156">请求</span><span class="sxs-lookup"><span data-stu-id="04001-156">Request</span></span>
<span data-ttu-id="04001-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04001-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/userStatusOverview
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

### <a name="response"></a><span data-ttu-id="04001-158">响应</span><span class="sxs-lookup"><span data-stu-id="04001-158">Response</span></span>
<span data-ttu-id="04001-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04001-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 328

{
  "@odata.type": "#microsoft.graph.deviceComplianceUserOverview",
  "id": "2d4f5bf4-5bf4-2d4f-f45b-4f2df45b4f2d",
  "pendingCount": 12,
  "notApplicableCount": 2,
  "successCount": 12,
  "errorCount": 10,
  "failedCount": 11,
  "lastUpdateDateTime": "2016-12-31T23:58:21.6459442-08:00",
  "configurationVersion": 4
}
```








