# <a name="list-windowsphone81generalconfigurations"></a><span data-ttu-id="dbeb4-101">列出 windowsPhone81GeneralConfigurations</span><span class="sxs-lookup"><span data-stu-id="dbeb4-101">List windowsPhone81GeneralConfigurations</span></span>

> <span data-ttu-id="dbeb4-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dbeb4-103">列出 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-103">List properties and relationships of the [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dbeb4-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="dbeb4-104">Prerequisites</span></span>
<span data-ttu-id="dbeb4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dbeb4-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="dbeb4-107">Permission type</span></span>|<span data-ttu-id="dbeb4-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dbeb4-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dbeb4-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dbeb4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dbeb4-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dbeb4-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dbeb4-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dbeb4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dbeb4-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-112">Not supported.</span></span>|
|<span data-ttu-id="dbeb4-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="dbeb4-113">Application</span></span>|<span data-ttu-id="dbeb4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dbeb4-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dbeb4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="dbeb4-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="dbeb4-116">Request headers</span></span>
|<span data-ttu-id="dbeb4-117">标头</span><span class="sxs-lookup"><span data-stu-id="dbeb4-117">Header</span></span>|<span data-ttu-id="dbeb4-118">值</span><span class="sxs-lookup"><span data-stu-id="dbeb4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dbeb4-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="dbeb4-119">Authorization</span></span>|<span data-ttu-id="dbeb4-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dbeb4-121">Accept</span><span class="sxs-lookup"><span data-stu-id="dbeb4-121">Accept</span></span>|<span data-ttu-id="dbeb4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dbeb4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dbeb4-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="dbeb4-123">Request body</span></span>
<span data-ttu-id="dbeb4-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dbeb4-125">响应</span><span class="sxs-lookup"><span data-stu-id="dbeb4-125">Response</span></span>
<span data-ttu-id="dbeb4-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-126">If successful, this method returns a `200 OK` response code and a collection of [windowsPhone81GeneralConfiguration](../resources/intune_deviceconfig_windowsphone81generalconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dbeb4-127">示例</span><span class="sxs-lookup"><span data-stu-id="dbeb4-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="dbeb4-128">请求</span><span class="sxs-lookup"><span data-stu-id="dbeb4-128">Request</span></span>
<span data-ttu-id="dbeb4-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="dbeb4-130">响应</span><span class="sxs-lookup"><span data-stu-id="dbeb4-130">Response</span></span>
<span data-ttu-id="dbeb4-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dbeb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1842

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsPhone81GeneralConfiguration",
      "id": "f5e0e34d-e34d-f5e0-4de3-e0f54de3e0f5",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "applyOnlyToWindowsPhone81": true,
      "appsBlockCopyPaste": true,
      "bluetoothBlocked": true,
      "cameraBlocked": true,
      "cellularBlockWifiTethering": true,
      "compliantAppsList": [
        {
          "@odata.type": "microsoft.graph.appListItem",
          "name": "Name value",
          "publisher": "Publisher value",
          "appStoreUrl": "https://example.com/appStoreUrl/",
          "appId": "App Id value"
        }
      ],
      "compliantAppListType": "appsInListCompliant",
      "diagnosticDataBlockSubmission": true,
      "emailBlockAddingAccounts": true,
      "locationServicesBlocked": true,
      "microsoftAccountBlocked": true,
      "nfcBlocked": true,
      "passwordBlockSimple": true,
      "passwordExpirationDays": 6,
      "passwordMinimumLength": 5,
      "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
      "passwordMinimumCharacterSetCount": 0,
      "passwordPreviousPasswordBlockCount": 2,
      "passwordSignInFailureCountBeforeFactoryReset": 12,
      "passwordRequiredType": "alphanumeric",
      "passwordRequired": true,
      "screenCaptureBlocked": true,
      "storageBlockRemovableStorage": true,
      "storageRequireEncryption": true,
      "webBrowserBlocked": true,
      "wifiBlocked": true,
      "wifiBlockAutomaticConnectHotspots": true,
      "wifiBlockHotspotReporting": true,
      "windowsStoreBlocked": true
    }
  ]
}
```



