# <a name="get-androidlobapp"></a><span data-ttu-id="4bebe-101">获取 androidLobApp</span><span class="sxs-lookup"><span data-stu-id="4bebe-101">Get androidLobApp</span></span>

> <span data-ttu-id="4bebe-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4bebe-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4bebe-103">读取 [androidLobApp](../resources/intune_apps_androidlobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4bebe-103">Read properties and relationships of the [androidLobApp](../resources/intune_apps_androidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4bebe-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="4bebe-104">Prerequisites</span></span>
<span data-ttu-id="4bebe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4bebe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4bebe-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="4bebe-107">Permission type</span></span>|<span data-ttu-id="4bebe-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4bebe-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4bebe-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4bebe-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4bebe-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="4bebe-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="4bebe-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4bebe-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4bebe-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bebe-112">Not supported.</span></span>|
|<span data-ttu-id="4bebe-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="4bebe-113">Application</span></span>|<span data-ttu-id="4bebe-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4bebe-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4bebe-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4bebe-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4bebe-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4bebe-116">Optional query parameters</span></span>
<span data-ttu-id="4bebe-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="4bebe-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="4bebe-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4bebe-118">Request headers</span></span>
|<span data-ttu-id="4bebe-119">标头</span><span class="sxs-lookup"><span data-stu-id="4bebe-119">Header</span></span>|<span data-ttu-id="4bebe-120">值</span><span class="sxs-lookup"><span data-stu-id="4bebe-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4bebe-121">授权</span><span class="sxs-lookup"><span data-stu-id="4bebe-121">Authorization</span></span>|<span data-ttu-id="4bebe-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4bebe-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4bebe-123">Accept</span><span class="sxs-lookup"><span data-stu-id="4bebe-123">Accept</span></span>|<span data-ttu-id="4bebe-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4bebe-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4bebe-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="4bebe-125">Request body</span></span>
<span data-ttu-id="4bebe-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4bebe-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4bebe-127">响应</span><span class="sxs-lookup"><span data-stu-id="4bebe-127">Response</span></span>
<span data-ttu-id="4bebe-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [androidLobApp](../resources/intune_apps_androidlobapp.md)  对象。</span><span class="sxs-lookup"><span data-stu-id="4bebe-128">If successful, this method returns a `200 OK` response code and [androidLobApp](../resources/intune_apps_androidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4bebe-129">示例</span><span class="sxs-lookup"><span data-stu-id="4bebe-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="4bebe-130">请求</span><span class="sxs-lookup"><span data-stu-id="4bebe-130">Request</span></span>
<span data-ttu-id="4bebe-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4bebe-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
```

### <a name="response"></a><span data-ttu-id="4bebe-132">响应</span><span class="sxs-lookup"><span data-stu-id="4bebe-132">Response</span></span>
<span data-ttu-id="4bebe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4bebe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1338

{
  "value": {
    "@odata.type": "#microsoft.graph.androidLobApp",
    "id": "4b9a27d0-27d0-4b9a-d027-9a4bd0279a4b",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "largeIcon": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "isFeatured": true,
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
    "informationUrl": "https://example.com/informationUrl/",
    "owner": "Owner value",
    "developer": "Developer value",
    "notes": "Notes value",
    "publishingState": "processing",
    "committedContentVersion": "Committed Content Version value",
    "fileName": "File Name value",
    "size": 4,
    "packageId": "Package Id value",
    "minimumSupportedOperatingSystem": {
      "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
      "v4_0": true,
      "v4_0_3": true,
      "v4_1": true,
      "v4_2": true,
      "v4_3": true,
      "v4_4": true,
      "v5_0": true,
      "v5_1": true
    },
    "versionName": "Version Name value",
    "versionCode": "Version Code value"
  }
}
```








