# <a name="list-deviceenrollmentlimitconfigurations"></a><span data-ttu-id="f9f07-101">列出 deviceEnrollmentLimitConfigurations</span><span class="sxs-lookup"><span data-stu-id="f9f07-101">List deviceEnrollmentLimitConfigurations</span></span>

> <span data-ttu-id="f9f07-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f9f07-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9f07-103">列出 [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f9f07-103">List properties and relationships of the [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9f07-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9f07-104">Prerequisites</span></span>
<span data-ttu-id="f9f07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f9f07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9f07-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9f07-107">Permission type</span></span>|<span data-ttu-id="f9f07-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9f07-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9f07-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9f07-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f9f07-110">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f9f07-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f9f07-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9f07-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9f07-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9f07-112">Not supported.</span></span>|
|<span data-ttu-id="f9f07-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9f07-113">Application</span></span>|<span data-ttu-id="f9f07-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9f07-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9f07-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9f07-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f9f07-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9f07-116">Request headers</span></span>
|<span data-ttu-id="f9f07-117">标头</span><span class="sxs-lookup"><span data-stu-id="f9f07-117">Header</span></span>|<span data-ttu-id="f9f07-118">值</span><span class="sxs-lookup"><span data-stu-id="f9f07-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9f07-119">授权</span><span class="sxs-lookup"><span data-stu-id="f9f07-119">Authorization</span></span>|<span data-ttu-id="f9f07-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9f07-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9f07-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f9f07-121">Accept</span></span>|<span data-ttu-id="f9f07-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f9f07-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9f07-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9f07-123">Request body</span></span>
<span data-ttu-id="f9f07-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f9f07-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f9f07-125">响应</span><span class="sxs-lookup"><span data-stu-id="f9f07-125">Response</span></span>
<span data-ttu-id="f9f07-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f9f07-126">If successful, this method returns a `200 OK` response code and a collection of [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9f07-127">示例</span><span class="sxs-lookup"><span data-stu-id="f9f07-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9f07-128">请求</span><span class="sxs-lookup"><span data-stu-id="f9f07-128">Request</span></span>
<span data-ttu-id="f9f07-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9f07-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="f9f07-130">响应</span><span class="sxs-lookup"><span data-stu-id="f9f07-130">Response</span></span>
<span data-ttu-id="f9f07-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9f07-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 446

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
      "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7,
      "limit": 5
    }
  ]
}
```








