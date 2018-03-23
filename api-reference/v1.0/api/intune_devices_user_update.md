# <a name="update-user"></a><span data-ttu-id="67bdf-101">更新 user</span><span class="sxs-lookup"><span data-stu-id="67bdf-101">Update user</span></span>

> <span data-ttu-id="67bdf-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="67bdf-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67bdf-103">更新 [user](../resources/intune_devices_user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="67bdf-103">Update the properties of a user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="67bdf-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="67bdf-104">Prerequisites</span></span>
<span data-ttu-id="67bdf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="67bdf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="67bdf-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="67bdf-107">Permission type</span></span>|<span data-ttu-id="67bdf-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="67bdf-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67bdf-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67bdf-109">Delegated (work or school account)</span></span>|<span data-ttu-id="67bdf-110">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67bdf-110">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="67bdf-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67bdf-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67bdf-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="67bdf-112">Not supported.</span></span>|
|<span data-ttu-id="67bdf-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="67bdf-113">Application</span></span>|<span data-ttu-id="67bdf-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="67bdf-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67bdf-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67bdf-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="67bdf-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="67bdf-116">Request headers</span></span>
|<span data-ttu-id="67bdf-117">标头</span><span class="sxs-lookup"><span data-stu-id="67bdf-117">Header</span></span>|<span data-ttu-id="67bdf-118">值</span><span class="sxs-lookup"><span data-stu-id="67bdf-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67bdf-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="67bdf-119">Authorization</span></span>|<span data-ttu-id="67bdf-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="67bdf-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="67bdf-121">Accept</span><span class="sxs-lookup"><span data-stu-id="67bdf-121">Accept</span></span>|<span data-ttu-id="67bdf-122">application/json</span><span class="sxs-lookup"><span data-stu-id="67bdf-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67bdf-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="67bdf-123">Request body</span></span>
<span data-ttu-id="67bdf-124">在请求正文中，提供 [user](../resources/intune_devices_user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67bdf-124">In the request body, supply a JSON representation of [user](../resources/intune_devices_user.md) object.</span></span>

<span data-ttu-id="67bdf-125">下表显示创建 [user](../resources/intune_devices_user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="67bdf-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="67bdf-126">属性</span><span class="sxs-lookup"><span data-stu-id="67bdf-126">Property</span></span>|<span data-ttu-id="67bdf-127">类型</span><span class="sxs-lookup"><span data-stu-id="67bdf-127">Type</span></span>|<span data-ttu-id="67bdf-128">说明</span><span class="sxs-lookup"><span data-stu-id="67bdf-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67bdf-129">id</span><span class="sxs-lookup"><span data-stu-id="67bdf-129">id</span></span>|<span data-ttu-id="67bdf-130">String</span><span class="sxs-lookup"><span data-stu-id="67bdf-130">String</span></span>|<span data-ttu-id="67bdf-131">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="67bdf-131">Unique identifier of the folder.</span></span>|



## <a name="response"></a><span data-ttu-id="67bdf-132">响应</span><span class="sxs-lookup"><span data-stu-id="67bdf-132">Response</span></span>
<span data-ttu-id="67bdf-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune_devices_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67bdf-133">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_devices_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67bdf-134">示例</span><span class="sxs-lookup"><span data-stu-id="67bdf-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="67bdf-135">请求</span><span class="sxs-lookup"><span data-stu-id="67bdf-135">Request</span></span>
<span data-ttu-id="67bdf-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67bdf-136">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="67bdf-137">响应</span><span class="sxs-lookup"><span data-stu-id="67bdf-137">Response</span></span>
<span data-ttu-id="67bdf-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67bdf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 95

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3"
}
```



