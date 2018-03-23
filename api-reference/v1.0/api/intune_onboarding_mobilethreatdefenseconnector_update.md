# <a name="update-mobilethreatdefenseconnector"></a><span data-ttu-id="598bc-101">更新 mobileThreatDefenseConnector</span><span class="sxs-lookup"><span data-stu-id="598bc-101">Update mobileThreatDefenseConnector</span></span>

> <span data-ttu-id="598bc-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="598bc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="598bc-103">更新 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="598bc-103">Update the properties of a [calendar](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="598bc-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="598bc-104">Prerequisites</span></span>
<span data-ttu-id="598bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="598bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="598bc-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="598bc-107">Permission type</span></span>|<span data-ttu-id="598bc-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="598bc-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="598bc-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="598bc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="598bc-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="598bc-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="598bc-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="598bc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="598bc-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="598bc-112">Not supported.</span></span>|
|<span data-ttu-id="598bc-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="598bc-113">Application</span></span>|<span data-ttu-id="598bc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="598bc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="598bc-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="598bc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="598bc-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="598bc-116">Request headers</span></span>
|<span data-ttu-id="598bc-117">标头</span><span class="sxs-lookup"><span data-stu-id="598bc-117">Header</span></span>|<span data-ttu-id="598bc-118">值</span><span class="sxs-lookup"><span data-stu-id="598bc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="598bc-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="598bc-119">Authorization</span></span>|<span data-ttu-id="598bc-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="598bc-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="598bc-121">Accept</span><span class="sxs-lookup"><span data-stu-id="598bc-121">Accept</span></span>|<span data-ttu-id="598bc-122">application/json</span><span class="sxs-lookup"><span data-stu-id="598bc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="598bc-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="598bc-123">Request body</span></span>
<span data-ttu-id="598bc-124">在请求正文中，提供 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="598bc-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object.</span></span>

<span data-ttu-id="598bc-125">下表显示了创建 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="598bc-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="598bc-126">属性</span><span class="sxs-lookup"><span data-stu-id="598bc-126">Property</span></span>|<span data-ttu-id="598bc-127">类型</span><span class="sxs-lookup"><span data-stu-id="598bc-127">Type</span></span>|<span data-ttu-id="598bc-128">说明</span><span class="sxs-lookup"><span data-stu-id="598bc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="598bc-129">id</span><span class="sxs-lookup"><span data-stu-id="598bc-129">id</span></span>|<span data-ttu-id="598bc-130">String</span><span class="sxs-lookup"><span data-stu-id="598bc-130">String</span></span>|<span data-ttu-id="598bc-131">尚未记录</span><span class="sxs-lookup"><span data-stu-id="598bc-131">Not yet documented</span></span>|
|<span data-ttu-id="598bc-132">lastHeartbeatDateTime</span><span class="sxs-lookup"><span data-stu-id="598bc-132">lastHeartbeatDateTime</span></span>|<span data-ttu-id="598bc-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="598bc-133">DateTimeOffset</span></span>|<span data-ttu-id="598bc-134">管理员启用“连接到 MTP”选项后的上次检测信号的时间戳</span><span class="sxs-lookup"><span data-stu-id="598bc-134">Timestamp of last heartbeat after admin enabled option Connect to MTP</span></span>|
|<span data-ttu-id="598bc-135">partnerState</span><span class="sxs-lookup"><span data-stu-id="598bc-135">partnerState</span></span>|<span data-ttu-id="598bc-136">String</span><span class="sxs-lookup"><span data-stu-id="598bc-136">String</span></span>|<span data-ttu-id="598bc-137">此租户的合作伙伴状态。可取值为：`unavailable`、`available`、`enabled`、`unresponsive`。</span><span class="sxs-lookup"><span data-stu-id="598bc-137">Partner state of this tenant Possible values are: `unavailable`, `available`, `enabled`, `unresponsive`.</span></span>|
|<span data-ttu-id="598bc-138">androidEnabled</span><span class="sxs-lookup"><span data-stu-id="598bc-138">androidEnabled</span></span>|<span data-ttu-id="598bc-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="598bc-139">Boolean</span></span>|<span data-ttu-id="598bc-140">Android 切换，打开或关闭。</span><span class="sxs-lookup"><span data-stu-id="598bc-140">Android Toggle On or Off</span></span>|
|<span data-ttu-id="598bc-141">androidDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="598bc-141">androidDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="598bc-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="598bc-142">Boolean</span></span>|<span data-ttu-id="598bc-143">对于 Android，允许管理员配置必须先从数据同步合作伙伴接收到数据才能将其视为符合</span><span class="sxs-lookup"><span data-stu-id="598bc-143">For Android, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="598bc-144">iosDeviceBlockedOnMissingPartnerData</span><span class="sxs-lookup"><span data-stu-id="598bc-144">iosDeviceBlockedOnMissingPartnerData</span></span>|<span data-ttu-id="598bc-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="598bc-145">Boolean</span></span>|<span data-ttu-id="598bc-146">对于 IOS，允许管理员配置必须先从数据同步合作伙伴接收到数据才能将其视为符合</span><span class="sxs-lookup"><span data-stu-id="598bc-146">For IOS, Allows admin to config must receive data from the data sync partner prior to being considered compliant</span></span>|
|<span data-ttu-id="598bc-147">partnerUnsupportedOsVersionBlocked</span><span class="sxs-lookup"><span data-stu-id="598bc-147">partnerUnsupportedOsVersionBlocked</span></span>|<span data-ttu-id="598bc-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="598bc-148">Boolean</span></span>|<span data-ttu-id="598bc-149">允许管理员阻止启用的平台上不符合最低版本要求的设备</span><span class="sxs-lookup"><span data-stu-id="598bc-149">Allows admin to block devices on the enabled platforms that do not meet minimum version requirements</span></span>|
|<span data-ttu-id="598bc-150">iosEnabled</span><span class="sxs-lookup"><span data-stu-id="598bc-150">iosEnabled</span></span>|<span data-ttu-id="598bc-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="598bc-151">Boolean</span></span>|<span data-ttu-id="598bc-152">IOS 切换，打开或关闭。</span><span class="sxs-lookup"><span data-stu-id="598bc-152">IOS Toggle On or Off</span></span>|
|<span data-ttu-id="598bc-153">partnerUnresponsivenessThresholdInDays</span><span class="sxs-lookup"><span data-stu-id="598bc-153">partnerUnresponsivenessThresholdInDays</span></span>|<span data-ttu-id="598bc-154">Int32</span><span class="sxs-lookup"><span data-stu-id="598bc-154">Int32</span></span>|<span data-ttu-id="598bc-155">获取或设置每个租户允许此合作伙伴集成不响应的天数</span><span class="sxs-lookup"><span data-stu-id="598bc-155">Get or Set days the per tenant tolerance to unresponsiveness for this partner integration</span></span>|



## <a name="response"></a><span data-ttu-id="598bc-156">响应</span><span class="sxs-lookup"><span data-stu-id="598bc-156">Response</span></span>
<span data-ttu-id="598bc-157">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="598bc-157">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_mobilethreatdefenseconnector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="598bc-158">示例</span><span class="sxs-lookup"><span data-stu-id="598bc-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="598bc-159">请求</span><span class="sxs-lookup"><span data-stu-id="598bc-159">Request</span></span>
<span data-ttu-id="598bc-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="598bc-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/mobileThreatDefenseConnectors/{mobileThreatDefenseConnectorId}
Content-type: application/json
Content-length: 347

{
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```

### <a name="response"></a><span data-ttu-id="598bc-161">响应</span><span class="sxs-lookup"><span data-stu-id="598bc-161">Response</span></span>
<span data-ttu-id="598bc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="598bc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 463

{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "e4bede14-de14-e4be-14de-bee414debee4",
  "lastHeartbeatDateTime": "2016-12-31T23:59:37.9174975-08:00",
  "partnerState": "available",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 6
}
```



