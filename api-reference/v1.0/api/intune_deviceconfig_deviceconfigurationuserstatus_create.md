# <a name="create-deviceconfigurationuserstatus"></a><span data-ttu-id="5a839-101">创建 deviceConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="5a839-101">Create deviceConfigurationUserStatus</span></span>

> <span data-ttu-id="5a839-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5a839-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a839-103">创建新的 [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a839-103">Create a new [plannerBucket](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a839-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="5a839-104">Prerequisites</span></span>
<span data-ttu-id="5a839-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5a839-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a839-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a839-107">Permission type</span></span>|<span data-ttu-id="5a839-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5a839-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a839-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a839-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5a839-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a839-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5a839-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a839-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a839-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a839-112">Not supported.</span></span>|
|<span data-ttu-id="5a839-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a839-113">Application</span></span>|<span data-ttu-id="5a839-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a839-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a839-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a839-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="5a839-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a839-116">Request headers</span></span>
|<span data-ttu-id="5a839-117">标头</span><span class="sxs-lookup"><span data-stu-id="5a839-117">Header</span></span>|<span data-ttu-id="5a839-118">值</span><span class="sxs-lookup"><span data-stu-id="5a839-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a839-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a839-119">Authorization</span></span>|<span data-ttu-id="5a839-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5a839-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5a839-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5a839-121">Accept</span></span>|<span data-ttu-id="5a839-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5a839-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a839-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a839-123">Request body</span></span>
<span data-ttu-id="5a839-124">在请求正文中，提供 deviceConfigurationUserStatus 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5a839-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5a839-125">下表显示创建 deviceConfigurationUserStatus 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5a839-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5a839-126">属性</span><span class="sxs-lookup"><span data-stu-id="5a839-126">Property</span></span>|<span data-ttu-id="5a839-127">类型</span><span class="sxs-lookup"><span data-stu-id="5a839-127">Type</span></span>|<span data-ttu-id="5a839-128">说明</span><span class="sxs-lookup"><span data-stu-id="5a839-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a839-129">id</span><span class="sxs-lookup"><span data-stu-id="5a839-129">id</span></span>|<span data-ttu-id="5a839-130">String</span><span class="sxs-lookup"><span data-stu-id="5a839-130">String</span></span>|<span data-ttu-id="5a839-131">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5a839-131">Key of the setting.</span></span>|
|<span data-ttu-id="5a839-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5a839-132">userDisplayName</span></span>|<span data-ttu-id="5a839-133">String</span><span class="sxs-lookup"><span data-stu-id="5a839-133">String</span></span>|<span data-ttu-id="5a839-134">DevicePolicyStatus 的用户名。</span><span class="sxs-lookup"><span data-stu-id="5a839-134">User name of the DevicePolicyStatus.</span></span>|
|<span data-ttu-id="5a839-135">devicesCount</span><span class="sxs-lookup"><span data-stu-id="5a839-135">devicesCount</span></span>|<span data-ttu-id="5a839-136">Int32</span><span class="sxs-lookup"><span data-stu-id="5a839-136">Int32</span></span>|<span data-ttu-id="5a839-137">该用户的设备计数。</span><span class="sxs-lookup"><span data-stu-id="5a839-137">Devices count for that user.</span></span>|
|<span data-ttu-id="5a839-138">status</span><span class="sxs-lookup"><span data-stu-id="5a839-138">status</span></span>|<span data-ttu-id="5a839-139">String</span><span class="sxs-lookup"><span data-stu-id="5a839-139">String</span></span>|<span data-ttu-id="5a839-140">策略报告的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="5a839-140">Compliance status of the policy report.</span></span> <span data-ttu-id="5a839-141">可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="5a839-141">Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="5a839-142">lastReportedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a839-142">lastReportedDateTime</span></span>|<span data-ttu-id="5a839-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a839-143">DateTimeOffset</span></span>|<span data-ttu-id="5a839-144">策略报告的上次修改日期时间。</span><span class="sxs-lookup"><span data-stu-id="5a839-144">Last modified date time of the policy report.</span></span>|
|<span data-ttu-id="5a839-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="5a839-145">userPrincipalName</span></span>|<span data-ttu-id="5a839-146">String</span><span class="sxs-lookup"><span data-stu-id="5a839-146">String</span></span>|<span data-ttu-id="5a839-147">UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="5a839-147">userPrincipalName</span></span>|



## <a name="response"></a><span data-ttu-id="5a839-148">响应</span><span class="sxs-lookup"><span data-stu-id="5a839-148">Response</span></span>
<span data-ttu-id="5a839-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceConfigurationUserStatus](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a839-149">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_deviceconfig_deviceconfigurationuserstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a839-150">示例</span><span class="sxs-lookup"><span data-stu-id="5a839-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a839-151">请求</span><span class="sxs-lookup"><span data-stu-id="5a839-151">Request</span></span>
<span data-ttu-id="5a839-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5a839-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/userStatuses
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

### <a name="response"></a><span data-ttu-id="5a839-153">响应</span><span class="sxs-lookup"><span data-stu-id="5a839-153">Response</span></span>
<span data-ttu-id="5a839-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5a839-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



