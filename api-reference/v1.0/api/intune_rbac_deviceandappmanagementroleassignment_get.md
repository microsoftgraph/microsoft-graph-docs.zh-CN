# <a name="get-deviceandappmanagementroleassignment"></a><span data-ttu-id="bcb12-101">获取 deviceAndAppManagementRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="bcb12-101">Get deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="bcb12-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bcb12-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bcb12-103">读取 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="bcb12-103">Read properties and relationships of [plannerProgressTaskBoardTaskFormat](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bcb12-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="bcb12-104">Prerequisites</span></span>
<span data-ttu-id="bcb12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="bcb12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bcb12-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="bcb12-107">Permission type</span></span>|<span data-ttu-id="bcb12-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bcb12-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bcb12-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bcb12-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bcb12-110">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="bcb12-110">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="bcb12-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bcb12-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bcb12-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcb12-112">Not supported.</span></span>|
|<span data-ttu-id="bcb12-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="bcb12-113">Application</span></span>|<span data-ttu-id="bcb12-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="bcb12-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bcb12-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bcb12-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bcb12-116">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bcb12-116">Optional query parameters</span></span>
<span data-ttu-id="bcb12-117">此方法支持 [OData 查询参数](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bcb12-117">This method supports the [OData Query Parameters](https://developer.microsoft.com/zh-CN/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="bcb12-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="bcb12-118">Request headers</span></span>
|<span data-ttu-id="bcb12-119">标头</span><span class="sxs-lookup"><span data-stu-id="bcb12-119">Header</span></span>|<span data-ttu-id="bcb12-120">值</span><span class="sxs-lookup"><span data-stu-id="bcb12-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bcb12-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="bcb12-121">Authorization</span></span>|<span data-ttu-id="bcb12-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bcb12-122">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="bcb12-123">Accept</span><span class="sxs-lookup"><span data-stu-id="bcb12-123">Accept</span></span>|<span data-ttu-id="bcb12-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bcb12-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bcb12-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bcb12-125">Request body</span></span>
<span data-ttu-id="bcb12-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bcb12-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bcb12-127">响应</span><span class="sxs-lookup"><span data-stu-id="bcb12-127">Response</span></span>
<span data-ttu-id="bcb12-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bcb12-128">If successful, this method returns a `200 OK` response code and a [DriveItemVersion](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bcb12-129">示例</span><span class="sxs-lookup"><span data-stu-id="bcb12-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="bcb12-130">请求</span><span class="sxs-lookup"><span data-stu-id="bcb12-130">Request</span></span>
<span data-ttu-id="bcb12-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bcb12-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

### <a name="response"></a><span data-ttu-id="bcb12-132">响应</span><span class="sxs-lookup"><span data-stu-id="bcb12-132">Response</span></span>
<span data-ttu-id="bcb12-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bcb12-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 346

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
    "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
    "displayName": "Display Name value",
    "description": "Description value",
    "resourceScopes": [
      "Resource Scopes value"
    ],
    "members": [
      "Members value"
    ]
  }
}
```



