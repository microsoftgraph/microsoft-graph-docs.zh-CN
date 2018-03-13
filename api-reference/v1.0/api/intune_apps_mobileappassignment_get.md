# <a name="get-mobileappassignment"></a><span data-ttu-id="cf6fb-101">获取 mobileAppAssignment</span><span class="sxs-lookup"><span data-stu-id="cf6fb-101">Get mobileAppAssignment</span></span>

> <span data-ttu-id="cf6fb-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf6fb-103">读取 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-103">Read properties and relationships of [plannerTaskDetails](../resources/intune_apps_mobileappassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf6fb-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf6fb-104">Prerequisites</span></span>
<span data-ttu-id="cf6fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf6fb-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf6fb-107">Permission type</span></span>|<span data-ttu-id="cf6fb-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf6fb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf6fb-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf6fb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cf6fb-110">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf6fb-110">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cf6fb-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf6fb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf6fb-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-112">Not supported.</span></span>|
|<span data-ttu-id="cf6fb-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf6fb-113">Application</span></span>|<span data-ttu-id="cf6fb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf6fb-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf6fb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf6fb-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cf6fb-116">Optional query parameters</span></span>
<span data-ttu-id="cf6fb-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="cf6fb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf6fb-118">Request headers</span></span>
|<span data-ttu-id="cf6fb-119">标头</span><span class="sxs-lookup"><span data-stu-id="cf6fb-119">Header</span></span>|<span data-ttu-id="cf6fb-120">值</span><span class="sxs-lookup"><span data-stu-id="cf6fb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf6fb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf6fb-121">Authorization</span></span>|<span data-ttu-id="cf6fb-122">需要持有者&lt;令牌&gt;。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="cf6fb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cf6fb-123">Accept</span></span>|<span data-ttu-id="cf6fb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf6fb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf6fb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf6fb-125">Request body</span></span>
<span data-ttu-id="cf6fb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf6fb-127">响应</span><span class="sxs-lookup"><span data-stu-id="cf6fb-127">Response</span></span>
<span data-ttu-id="cf6fb-128">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [mobileAppAssignment](../resources/intune_apps_mobileappassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-128">If successful, this method returns a `200 OK` response code and [Contract](../resources/intune_apps_mobileappassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf6fb-129">示例</span><span class="sxs-lookup"><span data-stu-id="cf6fb-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf6fb-130">请求</span><span class="sxs-lookup"><span data-stu-id="cf6fb-130">Request</span></span>
<span data-ttu-id="cf6fb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments/{mobileAppAssignmentId}
```

### <a name="response"></a><span data-ttu-id="cf6fb-132">响应</span><span class="sxs-lookup"><span data-stu-id="cf6fb-132">Response</span></span>
<span data-ttu-id="cf6fb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf6fb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 359

{
  "value": {
    "@odata.type": "#microsoft.graph.mobileAppAssignment",
    "id": "591620b7-20b7-5916-b720-1659b7201659",
    "intent": "required",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    },
    "settings": {
      "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
    }
  }
}
```



