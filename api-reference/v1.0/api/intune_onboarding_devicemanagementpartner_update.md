# <a name="update-devicemanagementpartner"></a><span data-ttu-id="16962-101">更新 deviceManagementPartner</span><span class="sxs-lookup"><span data-stu-id="16962-101">Update deviceManagementPartner</span></span>

> <span data-ttu-id="16962-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="16962-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16962-103">更新 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="16962-103">Update the properties of a [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16962-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="16962-104">Prerequisites</span></span>
<span data-ttu-id="16962-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="16962-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="16962-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="16962-107">Permission type</span></span>|<span data-ttu-id="16962-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="16962-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16962-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="16962-109">Delegated (work or school account)</span></span>|<span data-ttu-id="16962-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16962-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="16962-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="16962-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16962-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="16962-112">Not supported.</span></span>|
|<span data-ttu-id="16962-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="16962-113">Application</span></span>|<span data-ttu-id="16962-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="16962-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16962-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="16962-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="16962-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="16962-116">Request headers</span></span>
|<span data-ttu-id="16962-117">标头</span><span class="sxs-lookup"><span data-stu-id="16962-117">Header</span></span>|<span data-ttu-id="16962-118">值</span><span class="sxs-lookup"><span data-stu-id="16962-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16962-119">授权</span><span class="sxs-lookup"><span data-stu-id="16962-119">Authorization</span></span>|<span data-ttu-id="16962-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="16962-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16962-121">接受</span><span class="sxs-lookup"><span data-stu-id="16962-121">Accept</span></span>|<span data-ttu-id="16962-122">application/json</span><span class="sxs-lookup"><span data-stu-id="16962-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16962-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="16962-123">Request body</span></span>
<span data-ttu-id="16962-124">在请求正文中，提供 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="16962-124">In the request body, supply a JSON representation for the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object.</span></span>

<span data-ttu-id="16962-125">下表显示创建 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="16962-125">The following table shows the properties that are required when you create the [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md).</span></span>

|<span data-ttu-id="16962-126">属性</span><span class="sxs-lookup"><span data-stu-id="16962-126">Property</span></span>|<span data-ttu-id="16962-127">类型</span><span class="sxs-lookup"><span data-stu-id="16962-127">Type</span></span>|<span data-ttu-id="16962-128">说明</span><span class="sxs-lookup"><span data-stu-id="16962-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16962-129">ID</span><span class="sxs-lookup"><span data-stu-id="16962-129">id</span></span>|<span data-ttu-id="16962-130">字符串</span><span class="sxs-lookup"><span data-stu-id="16962-130">String</span></span>|<span data-ttu-id="16962-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="16962-131">Not yet documented</span></span>|
|<span data-ttu-id="16962-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="16962-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="16962-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16962-133">DateTimeOffset</span></span>|<span data-ttu-id="16962-134">管理员启用“连接到设备管理合作伙伴”选项后上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="16962-134">Timestamp of last heartbeat after admin enabled option Connect to Device management Partner</span></span>|
|<span data-ttu-id="16962-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="16962-135">partnerState</span></span>|[<span data-ttu-id="16962-136">deviceManagementPartnerTenantState</span><span class="sxs-lookup"><span data-stu-id="16962-136">deviceManagementPartnerTenantState</span></span>](../resources/intune_onboarding_devicemanagementpartnertenantstate.md)|<span data-ttu-id="16962-137">此租户的合作伙伴状态。</span><span class="sxs-lookup"><span data-stu-id="16962-137">Partner state of this tenant Possible values are: , , , .</span></span> <span data-ttu-id="16962-138">可取值为：`unknown`、`unavailable`、`enabled`、`terminated`、`rejected`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="16962-138">Possible values are: `unknown`, `unavailable`, `enabled`, `terminated`, `rejected`, `unresponsive`.</span></span>|
|<span data-ttu-id="16962-139">partnerAppType</span><span class="sxs-lookup"><span data-stu-id="16962-139">partnerAppType</span></span>|[<span data-ttu-id="16962-140">deviceManagementPartnerAppType</span><span class="sxs-lookup"><span data-stu-id="16962-140">deviceManagementPartnerAppType</span></span>](../resources/intune_onboarding_devicemanagementpartnerapptype.md)|<span data-ttu-id="16962-141">合作伙伴应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="16962-141">Partner App Type.</span></span> <span data-ttu-id="16962-142">可取值为：`unknown`、`singleTenantApp`、`multiTenantApp`。</span><span class="sxs-lookup"><span data-stu-id="16962-142">Possible values are: `unknown`, `singleTenantApp`, `multiTenantApp`.</span></span>|
|<span data-ttu-id="16962-143">singleTenantAppId</span><span class="sxs-lookup"><span data-stu-id="16962-143">singleTenantAppId</span></span>|<span data-ttu-id="16962-144">字符串</span><span class="sxs-lookup"><span data-stu-id="16962-144">String</span></span>|<span data-ttu-id="16962-145">合作伙伴单个租户应用 ID</span><span class="sxs-lookup"><span data-stu-id="16962-145">Partner Single tenant App id</span></span>|
|<span data-ttu-id="16962-146">displayName</span><span class="sxs-lookup"><span data-stu-id="16962-146">displayName</span></span>|<span data-ttu-id="16962-147">字符串</span><span class="sxs-lookup"><span data-stu-id="16962-147">String</span></span>|<span data-ttu-id="16962-148">合作伙伴显示名称</span><span class="sxs-lookup"><span data-stu-id="16962-148">Partner display name</span></span>|
|<span data-ttu-id="16962-149">isConfigured</span><span class="sxs-lookup"><span data-stu-id="16962-149">isConfigured</span></span>|<span data-ttu-id="16962-150">布尔</span><span class="sxs-lookup"><span data-stu-id="16962-150">Boolean</span></span>|<span data-ttu-id="16962-151">是否配置了设备管理合作伙伴</span><span class="sxs-lookup"><span data-stu-id="16962-151">Whether device management partner is configured or not</span></span>|
|<span data-ttu-id="16962-152">whenPartnerDevicesWillBeRemovedDateTime</span><span class="sxs-lookup"><span data-stu-id="16962-152">whenPartnerDevicesWillBeRemovedDateTime</span></span>|<span data-ttu-id="16962-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16962-153">DateTimeOffset</span></span>|<span data-ttu-id="16962-154">要删除 PartnerDevices 时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="16962-154">DateTime in UTC when PartnerDevices will be removed</span></span>|
|<span data-ttu-id="16962-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span><span class="sxs-lookup"><span data-stu-id="16962-155">whenPartnerDevicesWillBeMarkedAsNonCompliantDateTime</span></span>|<span data-ttu-id="16962-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="16962-156">DateTimeOffset</span></span>|<span data-ttu-id="16962-157">PartnerDevices 将被标记为“不符合”时的日期/时间（UTC 时间）</span><span class="sxs-lookup"><span data-stu-id="16962-157">DateTime in UTC when PartnerDevices will be marked as NonCompliant</span></span>|



## <a name="response"></a><span data-ttu-id="16962-158">响应</span><span class="sxs-lookup"><span data-stu-id="16962-158">Response</span></span>
<span data-ttu-id="16962-159">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="16962-159">If successful, this method returns a `200 OK` response code and an updated [deviceManagementPartner](../resources/intune_onboarding_devicemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16962-160">示例</span><span class="sxs-lookup"><span data-stu-id="16962-160">Example</span></span>
### <a name="request"></a><span data-ttu-id="16962-161">请求</span><span class="sxs-lookup"><span data-stu-id="16962-161">Request</span></span>
<span data-ttu-id="16962-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="16962-162">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceManagementPartners/{deviceManagementPartnerId}
Content-type: application/json
Content-length: 440

{
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

### <a name="response"></a><span data-ttu-id="16962-163">响应</span><span class="sxs-lookup"><span data-stu-id="16962-163">Response</span></span>
<span data-ttu-id="16962-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="16962-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








