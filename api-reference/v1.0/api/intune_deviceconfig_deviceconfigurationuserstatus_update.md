# <a name="update-deviceconfigurationuserstatus"></a><span data-ttu-id="e0c9d-101">更新 deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="e0c9d-101">Update deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="e0c9d-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0c9d-103">更新 [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-103">Update the properties of a [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0c9d-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e0c9d-104">Prerequisites</span></span>
<span data-ttu-id="e0c9d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e0c9d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e0c9d-107">Permission type</span></span>|<span data-ttu-id="e0c9d-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e0c9d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0c9d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e0c9d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e0c9d-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0c9d-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0c9d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e0c9d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0c9d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-112">Not supported.</span></span>|
|<span data-ttu-id="e0c9d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e0c9d-113">Application</span></span>|<span data-ttu-id="e0c9d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0c9d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e0c9d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="e0c9d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e0c9d-116">Request headers</span></span>
|<span data-ttu-id="e0c9d-117">标头</span><span class="sxs-lookup"><span data-stu-id="e0c9d-117">Header</span></span>|<span data-ttu-id="e0c9d-118">值</span><span class="sxs-lookup"><span data-stu-id="e0c9d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0c9d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e0c9d-119">Authorization</span></span>|<span data-ttu-id="e0c9d-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0c9d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e0c9d-121">Accept</span></span>|<span data-ttu-id="e0c9d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e0c9d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0c9d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e0c9d-123">Request body</span></span>
<span data-ttu-id="e0c9d-124">在请求正文中，提供 [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-124">In the request body, supply a JSON representation for the [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.</span></span>

<span data-ttu-id="e0c9d-125">下表显示创建 [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-125">The following table shows the properties that are required when you create the [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md).</span></span>

|<span data-ttu-id="e0c9d-126">属性</span><span class="sxs-lookup"><span data-stu-id="e0c9d-126">Property</span></span>|<span data-ttu-id="e0c9d-127">类型</span><span class="sxs-lookup"><span data-stu-id="e0c9d-127">Type</span></span>|<span data-ttu-id="e0c9d-128">说明</span><span class="sxs-lookup"><span data-stu-id="e0c9d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0c9d-129">id</span><span class="sxs-lookup"><span data-stu-id="e0c9d-129">id</span></span>|<span data-ttu-id="e0c9d-130">String</span><span class="sxs-lookup"><span data-stu-id="e0c9d-130">String</span></span>|<span data-ttu-id="e0c9d-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-131">Key of the entity.</span></span>|
|<span data-ttu-id="e0c9d-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e0c9d-132">userDisplayName</span></span>|<span data-ttu-id="e0c9d-133">String</span><span class="sxs-lookup"><span data-stu-id="e0c9d-133">String</span></span>|<span data-ttu-id="e0c9d-134">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="e0c9d-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="e0c9d-135">devicesCount</span></span>|<span data-ttu-id="e0c9d-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e0c9d-136">Int32</span></span>|<span data-ttu-id="e0c9d-137">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-137">Devices count for that user.</span></span>|
|<span data-ttu-id="e0c9d-138">status</span><span class="sxs-lookup"><span data-stu-id="e0c9d-138">status</span></span>|[<span data-ttu-id="e0c9d-139">complianceStatus</span><span class="sxs-lookup"><span data-stu-id="e0c9d-139">complianceStatus</span></span>](../resources/intune_shared_compliancestatus.md)|<span data-ttu-id="e0c9d-140">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-140">Compliance status of the policy report.</span></span> <span data-ttu-id="e0c9d-141">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.</span></span>|
|<span data-ttu-id="e0c9d-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0c9d-142">lastReportedDateTime</span></span>|<span data-ttu-id="e0c9d-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0c9d-143">DateTimeOffset</span></span>|<span data-ttu-id="e0c9d-144">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="e0c9d-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e0c9d-145">userPrincipalName</span></span>|<span data-ttu-id="e0c9d-146">String</span><span class="sxs-lookup"><span data-stu-id="e0c9d-146">String</span></span>|<span data-ttu-id="e0c9d-147">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-147">UserPrincipalName.</span></span>|



## <a name="response"></a><span data-ttu-id="e0c9d-148">响应</span><span class="sxs-lookup"><span data-stu-id="e0c9d-148">Response</span></span>
<span data-ttu-id="e0c9d-149">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-149">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0c9d-150">示例</span><span class="sxs-lookup"><span data-stu-id="e0c9d-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0c9d-151">请求</span><span class="sxs-lookup"><span data-stu-id="e0c9d-151">Request</span></span>
<span data-ttu-id="e0c9d-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses/{deviceConfigurationUserStatusId}
Content-type: application/json
Content-length: 290

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="e0c9d-153">响应</span><span class="sxs-lookup"><span data-stu-id="e0c9d-153">Response</span></span>
<span data-ttu-id="e0c9d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e0c9d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 339

{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStatus",
  "id": "7e323db2-3db2-7e32-b23d-327eb23d327e",
  "userDisplayName": "User Display Name value",
  "devicesCount": 12,
  "status": "notApplicable",
  "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
  "userPrincipalName": "User Principal Name value"
}
```



