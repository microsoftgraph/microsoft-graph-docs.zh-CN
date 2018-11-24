# <a name="get-managedebook"></a><span data-ttu-id="609c6-101">获取 managedEBook</span><span class="sxs-lookup"><span data-stu-id="609c6-101">Get managedEBook</span></span>

> <span data-ttu-id="609c6-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="609c6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="609c6-103">读取 [managedEBook](../resources/intune_books_managedebook.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="609c6-103">Read properties and relationships of the [managedEBook](../resources/intune_books_managedebook.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="609c6-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="609c6-104">Prerequisites</span></span>
<span data-ttu-id="609c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="609c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="609c6-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="609c6-107">Permission type</span></span>|<span data-ttu-id="609c6-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="609c6-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="609c6-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="609c6-109">Delegated (work or school account)</span></span>|<span data-ttu-id="609c6-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="609c6-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="609c6-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="609c6-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="609c6-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="609c6-112">Not supported.</span></span>|
|<span data-ttu-id="609c6-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="609c6-113">Application</span></span>|<span data-ttu-id="609c6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="609c6-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="609c6-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="609c6-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="609c6-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="609c6-116">Optional query parameters</span></span>
<span data-ttu-id="609c6-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="609c6-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="609c6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="609c6-118">Request headers</span></span>
|<span data-ttu-id="609c6-119">标头</span><span class="sxs-lookup"><span data-stu-id="609c6-119">Header</span></span>|<span data-ttu-id="609c6-120">值</span><span class="sxs-lookup"><span data-stu-id="609c6-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="609c6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="609c6-121">Authorization</span></span>|<span data-ttu-id="609c6-122">需要持有者&lt;令牌&gt;。</span><span class="sxs-lookup"><span data-stu-id="609c6-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="609c6-123">Accept</span><span class="sxs-lookup"><span data-stu-id="609c6-123">Accept</span></span>|<span data-ttu-id="609c6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="609c6-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="609c6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="609c6-125">Request body</span></span>
<span data-ttu-id="609c6-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="609c6-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="609c6-127">响应</span><span class="sxs-lookup"><span data-stu-id="609c6-127">Response</span></span>
<span data-ttu-id="609c6-128">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [managedEBook](../resources/intune_books_managedebook.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="609c6-128">If successful, this method returns a `200 OK` response code and [managedEBook](../resources/intune_books_managedebook.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="609c6-129">示例</span><span class="sxs-lookup"><span data-stu-id="609c6-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="609c6-130">请求</span><span class="sxs-lookup"><span data-stu-id="609c6-130">Request</span></span>
<span data-ttu-id="609c6-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="609c6-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}
```

### <a name="response"></a><span data-ttu-id="609c6-132">响应</span><span class="sxs-lookup"><span data-stu-id="609c6-132">Response</span></span>
<span data-ttu-id="609c6-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="609c6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
    "@odata.type": "#microsoft.graph.managedEBook",
    "id": "1fbd3558-3558-1fbd-5835-bd1f5835bd1f",
    "displayName": "Display Name value",
    "description": "Description value",
    "publisher": "Publisher value",
    "publishedDateTime": "2016-12-31T23:58:16.1180489-08:00",
    "largeCover": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "informationUrl": "https://example.com/informationUrl/",
    "privacyInformationUrl": "https://example.com/privacyInformationUrl/"
  }
}
```



