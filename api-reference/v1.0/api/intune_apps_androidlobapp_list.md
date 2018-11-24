# <a name="list-androidlobapps"></a><span data-ttu-id="bbf99-101">列出 androidLobApps</span><span class="sxs-lookup"><span data-stu-id="bbf99-101">List androidLobApps</span></span>

> <span data-ttu-id="bbf99-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bbf99-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbf99-103">列出 [androidLobApp](../resources/intune_apps_androidlobapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bbf99-103">List properties and relationships of the [androidLobApp](../resources/intune_apps_androidlobapp.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbf99-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="bbf99-104">Prerequisites</span></span>
<span data-ttu-id="bbf99-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bbf99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bbf99-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="bbf99-107">Permission type</span></span>|<span data-ttu-id="bbf99-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bbf99-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbf99-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bbf99-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bbf99-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="bbf99-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="bbf99-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bbf99-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbf99-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbf99-112">Not supported.</span></span>|
|<span data-ttu-id="bbf99-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="bbf99-113">Application</span></span>|<span data-ttu-id="bbf99-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bbf99-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbf99-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bbf99-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="bbf99-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="bbf99-116">Request headers</span></span>
|<span data-ttu-id="bbf99-117">标头</span><span class="sxs-lookup"><span data-stu-id="bbf99-117">Header</span></span>|<span data-ttu-id="bbf99-118">值</span><span class="sxs-lookup"><span data-stu-id="bbf99-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbf99-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="bbf99-119">Authorization</span></span>|<span data-ttu-id="bbf99-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bbf99-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbf99-121">Accept</span><span class="sxs-lookup"><span data-stu-id="bbf99-121">Accept</span></span>|<span data-ttu-id="bbf99-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bbf99-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbf99-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="bbf99-123">Request body</span></span>
<span data-ttu-id="bbf99-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bbf99-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bbf99-125">响应</span><span class="sxs-lookup"><span data-stu-id="bbf99-125">Response</span></span>
<span data-ttu-id="bbf99-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [androidLobApp](../resources/intune_apps_androidlobapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bbf99-126">If successful, this method returns a `200 OK` response code and a collection of [androidLobApp](../resources/intune_apps_androidlobapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf99-127">示例</span><span class="sxs-lookup"><span data-stu-id="bbf99-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbf99-128">请求</span><span class="sxs-lookup"><span data-stu-id="bbf99-128">Request</span></span>
<span data-ttu-id="bbf99-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bbf99-129">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="bbf99-130">响应</span><span class="sxs-lookup"><span data-stu-id="bbf99-130">Response</span></span>
<span data-ttu-id="bbf99-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bbf99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1424

{
  "value": [
    {
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
  ]
}
```



