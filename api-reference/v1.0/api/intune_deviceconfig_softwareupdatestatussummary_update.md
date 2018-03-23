# <a name="update-softwareupdatestatussummary"></a><span data-ttu-id="d457e-101">更新 softwareUpdateStatusSummary</span><span class="sxs-lookup"><span data-stu-id="d457e-101">Update softwareUpdateStatusSummary</span></span>

> <span data-ttu-id="d457e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d457e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d457e-103">更新 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d457e-103">Update the properties of a [calendar](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d457e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d457e-104">Prerequisites</span></span>
<span data-ttu-id="d457e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d457e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d457e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d457e-107">Permission type</span></span>|<span data-ttu-id="d457e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d457e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d457e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d457e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d457e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d457e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d457e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d457e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d457e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d457e-112">Not supported.</span></span>|
|<span data-ttu-id="d457e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d457e-113">Application</span></span>|<span data-ttu-id="d457e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d457e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d457e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d457e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/softwareUpdateStatusSummary
```

## <a name="request-headers"></a><span data-ttu-id="d457e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="d457e-116">Request headers</span></span>
|<span data-ttu-id="d457e-117">标头</span><span class="sxs-lookup"><span data-stu-id="d457e-117">Header</span></span>|<span data-ttu-id="d457e-118">值</span><span class="sxs-lookup"><span data-stu-id="d457e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d457e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d457e-119">Authorization</span></span>|<span data-ttu-id="d457e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d457e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d457e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d457e-121">Accept</span></span>|<span data-ttu-id="d457e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d457e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d457e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="d457e-123">Request body</span></span>
<span data-ttu-id="d457e-124">在请求正文中，提供 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d457e-124">In the request body, supply a JSON representation of [Calendar](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object.</span></span>

<span data-ttu-id="d457e-125">下表显示了创建 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d457e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d457e-126">属性</span><span class="sxs-lookup"><span data-stu-id="d457e-126">Property</span></span>|<span data-ttu-id="d457e-127">类型</span><span class="sxs-lookup"><span data-stu-id="d457e-127">Type</span></span>|<span data-ttu-id="d457e-128">说明</span><span class="sxs-lookup"><span data-stu-id="d457e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d457e-129">id</span><span class="sxs-lookup"><span data-stu-id="d457e-129">id</span></span>|<span data-ttu-id="d457e-130">String</span><span class="sxs-lookup"><span data-stu-id="d457e-130">String</span></span>|<span data-ttu-id="d457e-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d457e-131">Key of the setting.</span></span>|
|<span data-ttu-id="d457e-132">displayName</span><span class="sxs-lookup"><span data-stu-id="d457e-132">displayName</span></span>|<span data-ttu-id="d457e-133">String</span><span class="sxs-lookup"><span data-stu-id="d457e-133">String</span></span>|<span data-ttu-id="d457e-134">策略的名称。</span><span class="sxs-lookup"><span data-stu-id="d457e-134">The name of the site policy to apply</span></span>|
|<span data-ttu-id="d457e-135">compliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d457e-135">compliantDeviceCount</span></span>|<span data-ttu-id="d457e-136">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-136">Int32</span></span>|<span data-ttu-id="d457e-137">兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-137">Number of compliant devices.</span></span>|
|<span data-ttu-id="d457e-138">nonCompliantDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d457e-138">nonCompliantDeviceCount</span></span>|<span data-ttu-id="d457e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-139">Int32</span></span>|<span data-ttu-id="d457e-140">不兼容设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-140">Number of non compliant devices.</span></span>|
|<span data-ttu-id="d457e-141">remediatedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d457e-141">remediatedDeviceCount</span></span>|<span data-ttu-id="d457e-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-142">Int32</span></span>|<span data-ttu-id="d457e-143">已修复设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-143">Number of remediated devices.</span></span>|
|<span data-ttu-id="d457e-144">errorDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d457e-144">errorDeviceCount</span></span>|<span data-ttu-id="d457e-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-145">Int32</span></span>|<span data-ttu-id="d457e-146">出现错误的设备数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-146">Number of devices had error.</span></span>|
|<span data-ttu-id="d457e-147">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d457e-147">unknownDeviceCount</span></span>|<span data-ttu-id="d457e-148">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-148">Int32</span></span>|<span data-ttu-id="d457e-149">未知设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-149">Number of unknown devices.</span></span>|
|<span data-ttu-id="d457e-150">conflictDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d457e-150">conflictDeviceCount</span></span>|<span data-ttu-id="d457e-151">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-151">Int32</span></span>|<span data-ttu-id="d457e-152">冲突设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-152">Number of conflict devices.</span></span>|
|<span data-ttu-id="d457e-153">notApplicableDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d457e-153">notApplicableDeviceCount</span></span>|<span data-ttu-id="d457e-154">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-154">Int32</span></span>|<span data-ttu-id="d457e-155">不适用设备的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-155">Number of not applicable devices.</span></span>|
|<span data-ttu-id="d457e-156">compliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d457e-156">compliantUserCount</span></span>|<span data-ttu-id="d457e-157">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-157">Int32</span></span>|<span data-ttu-id="d457e-158">兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-158">Number of users: 542</span></span>|
|<span data-ttu-id="d457e-159">nonCompliantUserCount</span><span class="sxs-lookup"><span data-stu-id="d457e-159">nonCompliantUserCount</span></span>|<span data-ttu-id="d457e-160">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-160">Int32</span></span>|<span data-ttu-id="d457e-161">不兼容用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-161">Number of non compliant users.</span></span>|
|<span data-ttu-id="d457e-162">remediatedUserCount</span><span class="sxs-lookup"><span data-stu-id="d457e-162">remediatedUserCount</span></span>|<span data-ttu-id="d457e-163">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-163">Int32</span></span>|<span data-ttu-id="d457e-164">已修复用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-164">Number of users: 542</span></span>|
|<span data-ttu-id="d457e-165">errorUserCount</span><span class="sxs-lookup"><span data-stu-id="d457e-165">errorUserCount</span></span>|<span data-ttu-id="d457e-166">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-166">Int32</span></span>|<span data-ttu-id="d457e-167">出现错误的用户数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-167">Number of users had error.</span></span>|
|<span data-ttu-id="d457e-168">unknownUserCount</span><span class="sxs-lookup"><span data-stu-id="d457e-168">unknownUserCount</span></span>|<span data-ttu-id="d457e-169">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-169">Int32</span></span>|<span data-ttu-id="d457e-170">未知用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-170">Number of users: 542</span></span>|
|<span data-ttu-id="d457e-171">conflictUserCount</span><span class="sxs-lookup"><span data-stu-id="d457e-171">conflictUserCount</span></span>|<span data-ttu-id="d457e-172">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-172">Int32</span></span>|<span data-ttu-id="d457e-173">冲突用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-173">Number of users: 542</span></span>|
|<span data-ttu-id="d457e-174">notApplicableUserCount</span><span class="sxs-lookup"><span data-stu-id="d457e-174">notApplicableUserCount</span></span>|<span data-ttu-id="d457e-175">Int32</span><span class="sxs-lookup"><span data-stu-id="d457e-175">Int32</span></span>|<span data-ttu-id="d457e-176">不适用用户的数量。</span><span class="sxs-lookup"><span data-stu-id="d457e-176">Number of not applicable users.</span></span>|



## <a name="response"></a><span data-ttu-id="d457e-177">响应</span><span class="sxs-lookup"><span data-stu-id="d457e-177">Response</span></span>
<span data-ttu-id="d457e-178">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [softwareUpdateStatusSummary](../resources/intune_deviceconfig_softwareupdatestatussummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d457e-178">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_softwareupdatestatussummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d457e-179">示例</span><span class="sxs-lookup"><span data-stu-id="d457e-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="d457e-180">请求</span><span class="sxs-lookup"><span data-stu-id="d457e-180">Request</span></span>
<span data-ttu-id="d457e-181">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d457e-181">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/softwareUpdateStatusSummary
Content-type: application/json
Content-length: 452

{
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```

### <a name="response"></a><span data-ttu-id="d457e-182">响应</span><span class="sxs-lookup"><span data-stu-id="d457e-182">Response</span></span>
<span data-ttu-id="d457e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d457e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 567

{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "4f71421f-421f-4f71-1f42-714f1f42714f",
  "displayName": "Display Name value",
  "compliantDeviceCount": 4,
  "nonCompliantDeviceCount": 7,
  "remediatedDeviceCount": 5,
  "errorDeviceCount": 0,
  "unknownDeviceCount": 2,
  "conflictDeviceCount": 3,
  "notApplicableDeviceCount": 8,
  "compliantUserCount": 2,
  "nonCompliantUserCount": 5,
  "remediatedUserCount": 3,
  "errorUserCount": 14,
  "unknownUserCount": 0,
  "conflictUserCount": 1,
  "notApplicableUserCount": 6
}
```



