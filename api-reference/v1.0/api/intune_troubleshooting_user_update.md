# <a name="update-user"></a><span data-ttu-id="27c0d-101">更新 user</span><span class="sxs-lookup"><span data-stu-id="27c0d-101">Update user</span></span>

> <span data-ttu-id="27c0d-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="27c0d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="27c0d-103">更新 [user](../resources/intune_troubleshooting_user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27c0d-103">Update the properties of a user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="27c0d-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="27c0d-104">Prerequisites</span></span>
<span data-ttu-id="27c0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="27c0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="27c0d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="27c0d-107">Permission type</span></span>|<span data-ttu-id="27c0d-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27c0d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27c0d-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27c0d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="27c0d-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27c0d-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="27c0d-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27c0d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27c0d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="27c0d-112">Not supported.</span></span>|
|<span data-ttu-id="27c0d-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="27c0d-113">Application</span></span>|<span data-ttu-id="27c0d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="27c0d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="27c0d-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27c0d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="27c0d-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="27c0d-116">Request headers</span></span>
|<span data-ttu-id="27c0d-117">标头</span><span class="sxs-lookup"><span data-stu-id="27c0d-117">Header</span></span>|<span data-ttu-id="27c0d-118">值</span><span class="sxs-lookup"><span data-stu-id="27c0d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27c0d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="27c0d-119">Authorization</span></span>|<span data-ttu-id="27c0d-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27c0d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="27c0d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="27c0d-121">Accept</span></span>|<span data-ttu-id="27c0d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="27c0d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27c0d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="27c0d-123">Request body</span></span>
<span data-ttu-id="27c0d-124">在请求正文中，提供 [user](../resources/intune_troubleshooting_user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27c0d-124">In the request body, supply a JSON representation of [user](../resources/intune_troubleshooting_user.md) object.</span></span>

<span data-ttu-id="27c0d-125">下表显示创建 [user](../resources/intune_troubleshooting_user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27c0d-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="27c0d-126">属性</span><span class="sxs-lookup"><span data-stu-id="27c0d-126">Property</span></span>|<span data-ttu-id="27c0d-127">类型</span><span class="sxs-lookup"><span data-stu-id="27c0d-127">Type</span></span>|<span data-ttu-id="27c0d-128">说明</span><span class="sxs-lookup"><span data-stu-id="27c0d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27c0d-129">id</span><span class="sxs-lookup"><span data-stu-id="27c0d-129">id</span></span>|<span data-ttu-id="27c0d-130">String</span><span class="sxs-lookup"><span data-stu-id="27c0d-130">String</span></span>|<span data-ttu-id="27c0d-131">用户的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="27c0d-131">Unique identifier for the lab user.</span></span>|



## <a name="response"></a><span data-ttu-id="27c0d-132">响应</span><span class="sxs-lookup"><span data-stu-id="27c0d-132">Response</span></span>
<span data-ttu-id="27c0d-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune_troubleshooting_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27c0d-133">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_troubleshooting_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27c0d-134">示例</span><span class="sxs-lookup"><span data-stu-id="27c0d-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="27c0d-135">请求</span><span class="sxs-lookup"><span data-stu-id="27c0d-135">Request</span></span>
<span data-ttu-id="27c0d-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27c0d-136">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="27c0d-137">响应</span><span class="sxs-lookup"><span data-stu-id="27c0d-137">Response</span></span>
<span data-ttu-id="27c0d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27c0d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



