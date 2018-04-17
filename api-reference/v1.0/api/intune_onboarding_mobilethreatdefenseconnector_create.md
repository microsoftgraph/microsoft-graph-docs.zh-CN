# <a name="create-mobilethreatdefenseconnector"></a><span data-ttu-id="f6750-101">创建 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="f6750-101">Create mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="f6750-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f6750-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f6750-103">创建新的 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6750-103">Create a new [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f6750-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f6750-104">Prerequisites</span></span>
<span data-ttu-id="f6750-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f6750-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f6750-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f6750-107">Permission type</span></span>|<span data-ttu-id="f6750-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f6750-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f6750-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f6750-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f6750-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f6750-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f6750-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f6750-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f6750-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6750-112">Not supported.</span></span>|
|<span data-ttu-id="f6750-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f6750-113">Application</span></span>|<span data-ttu-id="f6750-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f6750-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f6750-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6750-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/mobileThreatDefenseConnectors
```

## <a name="request-headers"></a><span data-ttu-id="f6750-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6750-116">Request headers</span></span>
|<span data-ttu-id="f6750-117">标头</span><span class="sxs-lookup"><span data-stu-id="f6750-117">Header</span></span>|<span data-ttu-id="f6750-118">值</span><span class="sxs-lookup"><span data-stu-id="f6750-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f6750-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6750-119">Authorization</span></span>|<span data-ttu-id="f6750-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f6750-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f6750-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f6750-121">Accept</span></span>|<span data-ttu-id="f6750-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f6750-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f6750-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6750-123">Request body</span></span>
<span data-ttu-id="f6750-124">在请求正文中，提供 mobileThreatDefenseConnector 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6750-124">In the request body, supply a JSON representation for the mobileThreatDefenseConnector object.</span></span>

<span data-ttu-id="f6750-125">下表显示创建 mobileThreatDefenseConnector 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f6750-125">The following table shows the properties that are required when you create the mobileThreatDefenseConnector.</span></span>

|<span data-ttu-id="f6750-126">属性</span><span class="sxs-lookup"><span data-stu-id="f6750-126">Property</span></span>|<span data-ttu-id="f6750-127">类型</span><span class="sxs-lookup"><span data-stu-id="f6750-127">Type</span></span>|<span data-ttu-id="f6750-128">说明</span><span class="sxs-lookup"><span data-stu-id="f6750-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6750-129">id</span><span class="sxs-lookup"><span data-stu-id="f6750-129">id</span></span>|<span data-ttu-id="f6750-130">String</span><span class="sxs-lookup"><span data-stu-id="f6750-130">String</span></span>|<span data-ttu-id="f6750-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="f6750-131">Not yet documented</span></span>|
|<span data-ttu-id="f6750-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="f6750-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="f6750-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f6750-133">DateTimeOffset</span></span>|<span data-ttu-id="f6750-134">从数据同步合作伙伴接收到上一个检测信号的日期/时间</span><span class="sxs-lookup"><span data-stu-id="f6750-134">DateTime of last Heartbeat recieved from the Data Sync Partner</span></span>|
|<span data-ttu-id="f6750-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="f6750-135">partnerState</span></span>|<span data-ttu-id="f6750-136">String</span><span class="sxs-lookup"><span data-stu-id="f6750-136">String</span></span>|<span data-ttu-id="f6750-137">此帐户数据同步合作伙伴状态可能的值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="f6750-137">Data Sync Partner state for this account Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="f6750-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="f6750-138">androidEnabled</span></span>|<span data-ttu-id="f6750-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6750-139">Boolean</span></span>|<span data-ttu-id="f6750-140">对于 Android 设备，设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="f6750-140">For Android, set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="f6750-141">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="f6750-141">iosEnabled</span></span>|<span data-ttu-id="f6750-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6750-142">Boolean</span></span>|<span data-ttu-id="f6750-143">对于 iOS 设备，获取或设置在合规性评估期间是否应使用来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="f6750-143">For IOS, get or set whether data from the data sync partner should be used during compliance evaluations</span></span>|
|<span data-ttu-id="f6750-144">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="f6750-144">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="f6750-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6750-145">Boolean</span></span>|<span data-ttu-id="f6750-146">对于 Android 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="f6750-146">For Android, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="f6750-147">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="f6750-147">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="f6750-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6750-148">Boolean</span></span>|<span data-ttu-id="f6750-149">对于 iOS 设备，设置 Intune 是否必须在使设备兼容之前接收来自数据同步合作伙伴的数据</span><span class="sxs-lookup"><span data-stu-id="f6750-149">For IOS, set whether Intune must receive data from the data sync partner prior to marking a device compliant</span></span>|
|<span data-ttu-id="f6750-150">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="f6750-150">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="f6750-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="f6750-151">Boolean</span></span>|<span data-ttu-id="f6750-152">获取或设置是否阻止不符合数据同步合作伙伴最低版本要求的启用平台上的设备</span><span class="sxs-lookup"><span data-stu-id="f6750-152">Get or set whether to block devices on the enabled platforms that do not meet the minimum version requirements of the Data Sync Partner</span></span>|
|<span data-ttu-id="f6750-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="f6750-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="f6750-154">Int32</span><span class="sxs-lookup"><span data-stu-id="f6750-154">Int32</span></span>|<span data-ttu-id="f6750-155">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="f6750-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="f6750-156">响应</span><span class="sxs-lookup"><span data-stu-id="f6750-156">Response</span></span>
<span data-ttu-id="f6750-157">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f6750-157">If successful, this method returns a `201 Created` response code and a [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f6750-158">示例</span><span class="sxs-lookup"><span data-stu-id="f6750-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="f6750-159">请求</span><span class="sxs-lookup"><span data-stu-id="f6750-159">Request</span></span>
<span data-ttu-id="f6750-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f6750-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors
Content-type: application/json
Content-length: 414

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="f6750-161">响应</span><span class="sxs-lookup"><span data-stu-id="f6750-161">Response</span></span>
<span data-ttu-id="f6750-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6750-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "iosEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



