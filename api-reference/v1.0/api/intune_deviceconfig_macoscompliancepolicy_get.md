# <a name="get-macoscompliancepolicy"></a><span data-ttu-id="23e01-101">获取 macOSCompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="23e01-101">Get macOSCompliancePolicy</span></span>

> <span data-ttu-id="23e01-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="23e01-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23e01-103">读取 [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="23e01-103">Read properties and relationships of the [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23e01-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="23e01-104">Prerequisites</span></span>
<span data-ttu-id="23e01-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](../../../concepts/permissions_reference.md)。
</span><span class="sxs-lookup"><span data-stu-id="23e01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="23e01-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="23e01-107">Permission type</span></span>|<span data-ttu-id="23e01-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="23e01-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23e01-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="23e01-109">Delegated (work or school account)</span></span>|<span data-ttu-id="23e01-110">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="23e01-110">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="23e01-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="23e01-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23e01-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="23e01-112">Not supported.</span></span>|
|<span data-ttu-id="23e01-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="23e01-113">Application</span></span>|<span data-ttu-id="23e01-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="23e01-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23e01-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="23e01-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23e01-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="23e01-116">Optional query parameters</span></span>
<span data-ttu-id="23e01-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="23e01-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23e01-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="23e01-118">Request headers</span></span>
|<span data-ttu-id="23e01-119">标头</span><span class="sxs-lookup"><span data-stu-id="23e01-119">Header</span></span>|<span data-ttu-id="23e01-120">值</span><span class="sxs-lookup"><span data-stu-id="23e01-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23e01-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="23e01-121">Authorization</span></span>|<span data-ttu-id="23e01-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="23e01-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23e01-123">Accept</span><span class="sxs-lookup"><span data-stu-id="23e01-123">Accept</span></span>|<span data-ttu-id="23e01-124">application/json</span><span class="sxs-lookup"><span data-stu-id="23e01-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23e01-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="23e01-125">Request body</span></span>
<span data-ttu-id="23e01-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="23e01-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23e01-127">响应</span><span class="sxs-lookup"><span data-stu-id="23e01-127">Response</span></span>
<span data-ttu-id="23e01-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="23e01-128">If successful, this method returns a `200 OK` response code and [macOSCompliancePolicy](../resources/intune_deviceconfig_macoscompliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23e01-129">示例</span><span class="sxs-lookup"><span data-stu-id="23e01-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="23e01-130">请求</span><span class="sxs-lookup"><span data-stu-id="23e01-130">Request</span></span>
<span data-ttu-id="23e01-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="23e01-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="23e01-132">响应</span><span class="sxs-lookup"><span data-stu-id="23e01-132">Response</span></span>
<span data-ttu-id="23e01-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="23e01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1088

{
  "value": {
    "@odata.type": "#microsoft.graph.macOSCompliancePolicy",
    "id": "ddbadff3-dff3-ddba-f3df-baddf3dfbadd",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordPreviousPasswordBlockCount": 2,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "systemIntegrityProtectionEnabled": true,
    "deviceThreatProtectionEnabled": true,
    "deviceThreatProtectionRequiredSecurityLevel": "secured",
    "storageRequireEncryption": true,
    "firewallEnabled": true,
    "firewallBlockAllIncoming": true,
    "firewallEnableStealthMode": true
  }
}
```



