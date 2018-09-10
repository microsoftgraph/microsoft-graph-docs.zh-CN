# <a name="list-importedwindowsautopilotdeviceidentities"></a><span data-ttu-id="b14cf-101">列表 importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="b14cf-101">List importedWindowsAutopilotDeviceIdentities</span></span>

> <span data-ttu-id="b14cf-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b14cf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b14cf-103">列表属性和[importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md)对象关系。</span><span class="sxs-lookup"><span data-stu-id="b14cf-103">List properties and relationships of the [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b14cf-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="b14cf-104">Prerequisites</span></span>
<span data-ttu-id="b14cf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b14cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b14cf-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="b14cf-107">Permission type</span></span>|<span data-ttu-id="b14cf-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b14cf-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b14cf-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b14cf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b14cf-110">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="b14cf-110">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="b14cf-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b14cf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b14cf-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="b14cf-112">Not supported.</span></span>|
|<span data-ttu-id="b14cf-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="b14cf-113">Application</span></span>|<span data-ttu-id="b14cf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b14cf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b14cf-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b14cf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/importedWindowsAutopilotDeviceIdentities
GET /deviceManagement/importedWindowsAutopilotDeviceIdentityUploads/{importedWindowsAutopilotDeviceIdentityUploadId}/deviceIdentities
```

## <a name="request-headers"></a><span data-ttu-id="b14cf-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="b14cf-116">Request headers</span></span>
|<span data-ttu-id="b14cf-117">标头</span><span class="sxs-lookup"><span data-stu-id="b14cf-117">Header</span></span>|<span data-ttu-id="b14cf-118">值</span><span class="sxs-lookup"><span data-stu-id="b14cf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b14cf-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b14cf-119">Authorization</span></span>|<span data-ttu-id="b14cf-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b14cf-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b14cf-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b14cf-121">Accept</span></span>|<span data-ttu-id="b14cf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b14cf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b14cf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="b14cf-123">Request body</span></span>
<span data-ttu-id="b14cf-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b14cf-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b14cf-125">响应</span><span class="sxs-lookup"><span data-stu-id="b14cf-125">Response</span></span>
<span data-ttu-id="b14cf-126">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b14cf-126">If successful, this method returns a `200 OK` response code and a collection of [importedWindowsAutopilotDeviceIdentity](../resources/intune_enrollment_importedwindowsautopilotdeviceidentity.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b14cf-127">示例</span><span class="sxs-lookup"><span data-stu-id="b14cf-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="b14cf-128">请求</span><span class="sxs-lookup"><span data-stu-id="b14cf-128">Request</span></span>
<span data-ttu-id="b14cf-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b14cf-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/importedWindowsAutopilotDeviceIdentities
```

### <a name="response"></a><span data-ttu-id="b14cf-130">响应</span><span class="sxs-lookup"><span data-stu-id="b14cf-130">Response</span></span>
<span data-ttu-id="b14cf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b14cf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 675

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      }
    }
  ]
}
```








