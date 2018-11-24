# <a name="list-androidcompliancepolicies"></a><span data-ttu-id="dfc21-101">列出 androidCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="dfc21-101">List androidCompliancePolicies</span></span>

> <span data-ttu-id="dfc21-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dfc21-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dfc21-103">列出 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dfc21-103">List properties and relationships of the [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dfc21-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="dfc21-104">Prerequisites</span></span>
<span data-ttu-id="dfc21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="dfc21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dfc21-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfc21-107">Permission type</span></span>|<span data-ttu-id="dfc21-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dfc21-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dfc21-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfc21-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dfc21-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="dfc21-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="dfc21-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfc21-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dfc21-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfc21-112">Not supported.</span></span>|
|<span data-ttu-id="dfc21-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfc21-113">Application</span></span>|<span data-ttu-id="dfc21-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfc21-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dfc21-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfc21-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="dfc21-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfc21-116">Request headers</span></span>
|<span data-ttu-id="dfc21-117">标头</span><span class="sxs-lookup"><span data-stu-id="dfc21-117">Header</span></span>|<span data-ttu-id="dfc21-118">值</span><span class="sxs-lookup"><span data-stu-id="dfc21-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dfc21-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfc21-119">Authorization</span></span>|<span data-ttu-id="dfc21-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dfc21-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dfc21-121">Accept</span><span class="sxs-lookup"><span data-stu-id="dfc21-121">Accept</span></span>|<span data-ttu-id="dfc21-122">application/json</span><span class="sxs-lookup"><span data-stu-id="dfc21-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dfc21-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfc21-123">Request body</span></span>
<span data-ttu-id="dfc21-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dfc21-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dfc21-125">响应</span><span class="sxs-lookup"><span data-stu-id="dfc21-125">Response</span></span>
<span data-ttu-id="dfc21-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="dfc21-126">If successful, this method returns a `200 OK` response code and a collection of [androidCompliancePolicy](../resources/intune_deviceconfig_androidcompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfc21-127">示例</span><span class="sxs-lookup"><span data-stu-id="dfc21-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="dfc21-128">请求</span><span class="sxs-lookup"><span data-stu-id="dfc21-128">Request</span></span>
<span data-ttu-id="dfc21-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dfc21-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="dfc21-130">响应</span><span class="sxs-lookup"><span data-stu-id="dfc21-130">Response</span></span>
<span data-ttu-id="dfc21-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfc21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1476

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidCompliancePolicy",
      "id": "752c820f-820f-752c-0f82-2c750f822c75",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7,
      "passwordRequired": true,
      "passwordMinimumLength": 5,
      "passwordRequiredType": "alphabetic",
      "passwordMinutesOfInactivityBeforeLock": 5,
      "passwordExpirationDays": 6,
      "passwordPreviousPasswordBlockCount": 2,
      "securityPreventInstallAppsFromUnknownSources": true,
      "securityDisableUsbDebugging": true,
      "securityRequireVerifyApps": true,
      "deviceThreatProtectionEnabled": true,
      "deviceThreatProtectionRequiredSecurityLevel": "secured",
      "securityBlockJailbrokenDevices": true,
      "osMinimumVersion": "Os Minimum Version value",
      "osMaximumVersion": "Os Maximum Version value",
      "minAndroidSecurityPatchLevel": "Min Android Security Patch Level value",
      "storageRequireEncryption": true,
      "securityRequireSafetyNetAttestationBasicIntegrity": true,
      "securityRequireSafetyNetAttestationCertifiedDevice": true,
      "securityRequireGooglePlayServices": true,
      "securityRequireUpToDateSecurityProviders": true,
      "securityRequireCompanyPortalAppIntegrity": true
    }
  ]
}
```



