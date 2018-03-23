# <a name="get-windows81generalconfiguration"></a><span data-ttu-id="d938e-101">获取 windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="d938e-101">Get windows81GeneralConfiguration</span></span>

> <span data-ttu-id="d938e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d938e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d938e-103">读取 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d938e-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_deviceconfig_windows81generalconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d938e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="d938e-104">Prerequisites</span></span>
<span data-ttu-id="d938e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d938e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d938e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="d938e-107">Permission type</span></span>|<span data-ttu-id="d938e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d938e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d938e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d938e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d938e-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d938e-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d938e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d938e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d938e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d938e-112">Not supported.</span></span>|
|<span data-ttu-id="d938e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="d938e-113">Application</span></span>|<span data-ttu-id="d938e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d938e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d938e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d938e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d938e-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d938e-116">Optional query parameters</span></span>
<span data-ttu-id="d938e-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d938e-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d938e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d938e-118">Request headers</span></span>
|<span data-ttu-id="d938e-119">标头</span><span class="sxs-lookup"><span data-stu-id="d938e-119">Header</span></span>|<span data-ttu-id="d938e-120">值</span><span class="sxs-lookup"><span data-stu-id="d938e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d938e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d938e-121">Authorization</span></span>|<span data-ttu-id="d938e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d938e-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d938e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d938e-123">Accept</span></span>|<span data-ttu-id="d938e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d938e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d938e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d938e-125">Request body</span></span>
<span data-ttu-id="d938e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d938e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d938e-127">响应</span><span class="sxs-lookup"><span data-stu-id="d938e-127">Response</span></span>
<span data-ttu-id="d938e-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows81GeneralConfiguration](../resources/intune_deviceconfig_windows81generalconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d938e-128">If successful, this method returns a `200 OK` response code and a [ListItemVersion](../resources/intune_deviceconfig_windows81generalconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d938e-129">示例</span><span class="sxs-lookup"><span data-stu-id="d938e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="d938e-130">请求</span><span class="sxs-lookup"><span data-stu-id="d938e-130">Request</span></span>
<span data-ttu-id="d938e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d938e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d938e-132">响应</span><span class="sxs-lookup"><span data-stu-id="d938e-132">Response</span></span>
<span data-ttu-id="d938e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d938e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1964

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81GeneralConfiguration",
    "id": "0e9285b5-85b5-0e92-b585-920eb585920e",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "accountsBlockAddingNonMicrosoftAccountEmail": true,
    "applyOnlyToWindows81": true,
    "browserBlockAutofill": true,
    "browserBlockAutomaticDetectionOfIntranetSites": true,
    "browserBlockEnterpriseModeAccess": true,
    "browserBlockJavaScript": true,
    "browserBlockPlugins": true,
    "browserBlockPopups": true,
    "browserBlockSendingDoNotTrackHeader": true,
    "browserBlockSingleWordEntryOnIntranetSites": true,
    "browserRequireSmartScreen": true,
    "browserEnterpriseModeSiteListLocation": "Browser Enterprise Mode Site List Location value",
    "browserInternetSecurityLevel": "medium",
    "browserIntranetSecurityLevel": "low",
    "browserLoggingReportLocation": "Browser Logging Report Location value",
    "browserRequireHighSecurityForRestrictedSites": true,
    "browserRequireFirewall": true,
    "browserRequireFraudWarning": true,
    "browserTrustedSitesSecurityLevel": "low",
    "cellularBlockDataRoaming": true,
    "diagnosticsBlockDataSubmission": true,
    "passwordBlockPicturePasswordAndPin": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
    "passwordMinimumCharacterSetCount": 0,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordRequiredType": "alphanumeric",
    "passwordSignInFailureCountBeforeFactoryReset": 12,
    "storageRequireDeviceEncryption": true,
    "updatesRequireAutomaticUpdates": true,
    "userAccountControlSettings": "alwaysNotify",
    "workFoldersUrl": "https://example.com/workFoldersUrl/"
  }
}
```



