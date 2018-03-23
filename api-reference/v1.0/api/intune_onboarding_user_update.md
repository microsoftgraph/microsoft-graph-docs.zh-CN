# <a name="update-user"></a><span data-ttu-id="0cf17-101">更新 user</span><span class="sxs-lookup"><span data-stu-id="0cf17-101">Update user</span></span>

> <span data-ttu-id="0cf17-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0cf17-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0cf17-103">更新 [user](../resources/intune_onboarding_user.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0cf17-103">Update the properties of a user object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0cf17-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="0cf17-104">Prerequisites</span></span>
<span data-ttu-id="0cf17-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="0cf17-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0cf17-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cf17-107">Permission type</span></span>|<span data-ttu-id="0cf17-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0cf17-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cf17-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cf17-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0cf17-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cf17-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0cf17-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cf17-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cf17-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cf17-112">Not supported.</span></span>|
|<span data-ttu-id="0cf17-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cf17-113">Application</span></span>|<span data-ttu-id="0cf17-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cf17-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cf17-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cf17-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /users/{usersId}
```

## <a name="request-headers"></a><span data-ttu-id="0cf17-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cf17-116">Request headers</span></span>
|<span data-ttu-id="0cf17-117">标头</span><span class="sxs-lookup"><span data-stu-id="0cf17-117">Header</span></span>|<span data-ttu-id="0cf17-118">值</span><span class="sxs-lookup"><span data-stu-id="0cf17-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cf17-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cf17-119">Authorization</span></span>|<span data-ttu-id="0cf17-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0cf17-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0cf17-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0cf17-121">Accept</span></span>|<span data-ttu-id="0cf17-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0cf17-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cf17-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cf17-123">Request body</span></span>
<span data-ttu-id="0cf17-124">在请求正文中，提供 [user](../resources/intune_onboarding_user.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cf17-124">In the request body, supply a JSON representation of [user](../resources/intune_onboarding_user.md) object.</span></span>

<span data-ttu-id="0cf17-125">下表显示创建 [user](../resources/intune_onboarding_user.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0cf17-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="0cf17-126">属性</span><span class="sxs-lookup"><span data-stu-id="0cf17-126">Property</span></span>|<span data-ttu-id="0cf17-127">类型</span><span class="sxs-lookup"><span data-stu-id="0cf17-127">Type</span></span>|<span data-ttu-id="0cf17-128">说明</span><span class="sxs-lookup"><span data-stu-id="0cf17-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cf17-129">id</span><span class="sxs-lookup"><span data-stu-id="0cf17-129">id</span></span>|<span data-ttu-id="0cf17-130">String</span><span class="sxs-lookup"><span data-stu-id="0cf17-130">String</span></span>|<span data-ttu-id="0cf17-131">用户的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0cf17-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="0cf17-132">deviceEnrollmentLimit</span><span class="sxs-lookup"><span data-stu-id="0cf17-132">deviceEnrollmentLimit</span></span>|<span data-ttu-id="0cf17-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0cf17-133">Int32</span></span>|<span data-ttu-id="0cf17-134">允许用户注册的最大设备数的限制。</span><span class="sxs-lookup"><span data-stu-id="0cf17-134">The limit on the maximum number of devices that the user is permitted to enroll.</span></span> <span data-ttu-id="0cf17-135">允许的值为 5 或 1000。</span><span class="sxs-lookup"><span data-stu-id="0cf17-135">Allowed values are 5 or 1000.</span></span>|



## <a name="response"></a><span data-ttu-id="0cf17-136">响应</span><span class="sxs-lookup"><span data-stu-id="0cf17-136">Response</span></span>
<span data-ttu-id="0cf17-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [user](../resources/intune_onboarding_user.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0cf17-137">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_user.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cf17-138">示例</span><span class="sxs-lookup"><span data-stu-id="0cf17-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="0cf17-139">请求</span><span class="sxs-lookup"><span data-stu-id="0cf17-139">Request</span></span>
<span data-ttu-id="0cf17-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0cf17-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/users/{usersId}
Content-type: application/json
Content-length: 34

{
  "deviceEnrollmentLimit": 5
}
```

### <a name="response"></a><span data-ttu-id="0cf17-141">响应</span><span class="sxs-lookup"><span data-stu-id="0cf17-141">Response</span></span>
<span data-ttu-id="0cf17-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0cf17-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 126

{
  "@odata.type": "#microsoft.graph.user",
  "id": "d36894ae-94ae-d368-ae94-68d3ae9468d3",
  "deviceEnrollmentLimit": 5
}
```



