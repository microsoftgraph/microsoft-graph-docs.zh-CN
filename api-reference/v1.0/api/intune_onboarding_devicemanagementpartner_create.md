# <a name="create-devicemanagementpartner"></a><span data-ttu-id="622a7-101">创建 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="622a7-101">Create deviceManagementPartner</span></span>

> <span data-ttu-id="622a7-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="622a7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="622a7-103">创建新的 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="622a7-103">Create a new [plannerBucket](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="622a7-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="622a7-104">Prerequisites</span></span>
<span data-ttu-id="622a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="622a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="622a7-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="622a7-107">Permission type</span></span>|<span data-ttu-id="622a7-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="622a7-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="622a7-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="622a7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="622a7-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="622a7-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="622a7-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="622a7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="622a7-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="622a7-112">Not supported.</span></span>|
|<span data-ttu-id="622a7-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="622a7-113">Application</span></span>|<span data-ttu-id="622a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="622a7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="622a7-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="622a7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="622a7-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="622a7-116">Request headers</span></span>
|<span data-ttu-id="622a7-117">标头</span><span class="sxs-lookup"><span data-stu-id="622a7-117">Header</span></span>|<span data-ttu-id="622a7-118">值</span><span class="sxs-lookup"><span data-stu-id="622a7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="622a7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="622a7-119">Authorization</span></span>|<span data-ttu-id="622a7-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="622a7-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="622a7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="622a7-121">Accept</span></span>|<span data-ttu-id="622a7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="622a7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="622a7-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="622a7-123">Request body</span></span>
<span data-ttu-id="622a7-124">在请求正文中，提供 deviceManagementPartner 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="622a7-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="622a7-125">下表显示创建 deviceManagementPartner 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="622a7-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="622a7-126">属性</span><span class="sxs-lookup"><span data-stu-id="622a7-126">Property</span></span>|<span data-ttu-id="622a7-127">类型</span><span class="sxs-lookup"><span data-stu-id="622a7-127">Type</span></span>|<span data-ttu-id="622a7-128">说明</span><span class="sxs-lookup"><span data-stu-id="622a7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="622a7-129">id</span><span class="sxs-lookup"><span data-stu-id="622a7-129">id</span></span>|<span data-ttu-id="622a7-130">String</span><span class="sxs-lookup"><span data-stu-id="622a7-130">String</span></span>|<span data-ttu-id="622a7-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="622a7-131">Not yet documented</span></span>|
|<span data-ttu-id="622a7-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="622a7-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="622a7-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="622a7-133">DateTimeOffset</span></span>|<span data-ttu-id="622a7-134">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="622a7-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="622a7-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="622a7-135">partnerState</span></span>|<span data-ttu-id="622a7-136">String</span><span class="sxs-lookup"><span data-stu-id="622a7-136">String</span></span>|<span data-ttu-id="622a7-137">此租户的合作伙伴状态。可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="622a7-137">Partner state of this tenant Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="622a7-138">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="622a7-138">partnerAppType</span></span>|<span data-ttu-id="622a7-139">String</span><span class="sxs-lookup"><span data-stu-id="622a7-139">String</span></span>|<span data-ttu-id="622a7-140">合作伙伴应用类型。可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="622a7-140">Partner App type Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="622a7-141">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="622a7-141">singleTenantAppId</span></span>|<span data-ttu-id="622a7-142">String</span><span class="sxs-lookup"><span data-stu-id="622a7-142">String</span></span>|<span data-ttu-id="622a7-143">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="622a7-143">Partner Single tenant App id</span></span>|
|<span data-ttu-id="622a7-144">displayName</span><span class="sxs-lookup"><span data-stu-id="622a7-144">displayName</span></span>|<span data-ttu-id="622a7-145">String</span><span class="sxs-lookup"><span data-stu-id="622a7-145">String</span></span>|<span data-ttu-id="622a7-146">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="622a7-146">Partner display name</span></span>|
|<span data-ttu-id="622a7-147">isConfigured</span><span class="sxs-lookup"><span data-stu-id="622a7-147">isConfigured</span></span>|<span data-ttu-id="622a7-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="622a7-148">Boolean</span></span>|<span data-ttu-id="622a7-149">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="622a7-149">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="622a7-150">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="622a7-150">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="622a7-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="622a7-151">DateTimeOffset</span></span>|<span data-ttu-id="622a7-152">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="622a7-152">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="622a7-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="622a7-153">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="622a7-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="622a7-154">DateTimeOffset</span></span>|<span data-ttu-id="622a7-155">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="622a7-155">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="622a7-156">响应</span><span class="sxs-lookup"><span data-stu-id="622a7-156">Response</span></span>
<span data-ttu-id="622a7-157">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="622a7-157">If successful, this method returns a `201 Created` response code and a [ListItemVersion](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="622a7-158">示例</span><span class="sxs-lookup"><span data-stu-id="622a7-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="622a7-159">请求</span><span class="sxs-lookup"><span data-stu-id="622a7-159">Request</span></span>
<span data-ttu-id="622a7-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="622a7-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners
Content-type: application/json
Content-length: 502

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```

### <a name="response"></a><span data-ttu-id="622a7-161">响应</span><span class="sxs-lookup"><span data-stu-id="622a7-161">Response</span></span>
<span data-ttu-id="622a7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="622a7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 551

{
  "@odata.type": "#microsoft.graph.deviceManagementPartner",
  "id": "d21e377a-377a-d21e-7a37-1ed27a371ed2",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "unavailable",
  "partnerAppType": "singleTenantApp",
  "singleTenantAppId": "Single Tenant App Id value",
  "displayName": "Display Name value",
  "isConfigured": true,
  "whenPartnerDevicesWillBeRemovedDateTime": "2016-12-31T23:56:38.2655023-08:00",
  "whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime": "2016-12-31T23:58:42.2131231-08:00"
}
```



