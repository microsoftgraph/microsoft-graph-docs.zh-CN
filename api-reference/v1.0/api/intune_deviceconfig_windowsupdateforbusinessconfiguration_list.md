# <a name="list-windowsupdateforbusinessconfigurations"></a><span data-ttu-id="db450-101">列出 windowsUpdateForBusinessConfigurations</span><span class="sxs-lookup"><span data-stu-id="db450-101">List windowsUpdateForBusinessConfigurations</span></span>

> <span data-ttu-id="db450-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="db450-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db450-103">列出 [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="db450-103">List properties and relationships of the [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db450-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="db450-104">Prerequisites</span></span>
<span data-ttu-id="db450-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="db450-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="db450-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="db450-107">Permission type</span></span>|<span data-ttu-id="db450-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db450-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db450-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db450-109">Delegated (work or school account)</span></span>|<span data-ttu-id="db450-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="db450-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="db450-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db450-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db450-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="db450-112">Not supported.</span></span>|
|<span data-ttu-id="db450-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="db450-113">Application</span></span>|<span data-ttu-id="db450-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db450-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db450-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db450-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="db450-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="db450-116">Request headers</span></span>
|<span data-ttu-id="db450-117">标头</span><span class="sxs-lookup"><span data-stu-id="db450-117">Header</span></span>|<span data-ttu-id="db450-118">值</span><span class="sxs-lookup"><span data-stu-id="db450-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db450-119">授权</span><span class="sxs-lookup"><span data-stu-id="db450-119">Authorization</span></span>|<span data-ttu-id="db450-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db450-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db450-121">Accept</span><span class="sxs-lookup"><span data-stu-id="db450-121">Accept</span></span>|<span data-ttu-id="db450-122">application/json</span><span class="sxs-lookup"><span data-stu-id="db450-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db450-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="db450-123">Request body</span></span>
<span data-ttu-id="db450-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="db450-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="db450-125">响应</span><span class="sxs-lookup"><span data-stu-id="db450-125">Response</span></span>
<span data-ttu-id="db450-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="db450-126">If successful, this method returns a `200 OK` response code and a collection of [windowsUpdateForBusinessConfiguration](../resources/intune_deviceconfig_windowsupdateforbusinessconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db450-127">示例</span><span class="sxs-lookup"><span data-stu-id="db450-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="db450-128">请求</span><span class="sxs-lookup"><span data-stu-id="db450-128">Request</span></span>
<span data-ttu-id="db450-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db450-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="db450-130">响应</span><span class="sxs-lookup"><span data-stu-id="db450-130">Response</span></span>
<span data-ttu-id="db450-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db450-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUpdateForBusinessConfiguration",
      "id": "4928dd6a-dd6a-4928-6add-28496add2849",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "deliveryOptimizationMode": "httpOnly",
      "prereleaseFeatures": "settingsOnly",
      "automaticUpdateMode": "notifyDownload",
      "microsoftUpdateServiceAllowed": true,
      "driversExcluded": true,
      "installationSchedule": {
        "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall",
        "scheduledInstallDay": "everyday",
        "scheduledInstallTime": "11:59:31.3170000"
      },
      "qualityUpdatesDeferralPeriodInDays": 2,
      "featureUpdatesDeferralPeriodInDays": 2,
      "qualityUpdatesPaused": true,
      "featureUpdatesPaused": true,
      "qualityUpdatesPauseExpiryDateTime": "2017-01-01T00:00:22.9594683-08:00",
      "featureUpdatesPauseExpiryDateTime": "2016-12-31T23:58:08.068669-08:00",
      "businessReadyUpdatesOnly": "all"
    }
  ]
}
```








