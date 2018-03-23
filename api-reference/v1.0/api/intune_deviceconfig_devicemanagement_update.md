# <a name="update-devicemanagement"></a><span data-ttu-id="e877c-101">更新 deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e877c-101">Update deviceManagement</span></span>

> <span data-ttu-id="e877c-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e877c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e877c-103">更新 [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e877c-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e877c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="e877c-104">Prerequisites</span></span>
<span data-ttu-id="e877c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e877c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e877c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="e877c-107">Permission type</span></span>|<span data-ttu-id="e877c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e877c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e877c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e877c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e877c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e877c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e877c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e877c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e877c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e877c-112">Not supported.</span></span>|
|<span data-ttu-id="e877c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="e877c-113">Application</span></span>|<span data-ttu-id="e877c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e877c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e877c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e877c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement
```

## <a name="request-headers"></a><span data-ttu-id="e877c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e877c-116">Request headers</span></span>
|<span data-ttu-id="e877c-117">标头</span><span class="sxs-lookup"><span data-stu-id="e877c-117">Header</span></span>|<span data-ttu-id="e877c-118">值</span><span class="sxs-lookup"><span data-stu-id="e877c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e877c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e877c-119">Authorization</span></span>|<span data-ttu-id="e877c-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e877c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e877c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e877c-121">Accept</span></span>|<span data-ttu-id="e877c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e877c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e877c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e877c-123">Request body</span></span>
<span data-ttu-id="e877c-124">在请求正文中，提供 [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e877c-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicemanagement.md) object.</span></span>

<span data-ttu-id="e877c-125">下表显示创建 [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e877c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="e877c-126">属性</span><span class="sxs-lookup"><span data-stu-id="e877c-126">Property</span></span>|<span data-ttu-id="e877c-127">类型</span><span class="sxs-lookup"><span data-stu-id="e877c-127">Type</span></span>|<span data-ttu-id="e877c-128">说明</span><span class="sxs-lookup"><span data-stu-id="e877c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e877c-129">id</span><span class="sxs-lookup"><span data-stu-id="e877c-129">id</span></span>|<span data-ttu-id="e877c-130">String</span><span class="sxs-lookup"><span data-stu-id="e877c-130">String</span></span>|<span data-ttu-id="e877c-131">唯一标识符</span><span class="sxs-lookup"><span data-stu-id="e877c-131">Unique Identifier</span></span>|
|<span data-ttu-id="e877c-132">settings</span><span class="sxs-lookup"><span data-stu-id="e877c-132">settings</span></span>|[<span data-ttu-id="e877c-133">deviceManagementSettings</span><span class="sxs-lookup"><span data-stu-id="e877c-133">deviceManagementSettings</span></span>](../resources/intune_deviceconfig_devicemanagementsettings.md)|<span data-ttu-id="e877c-134">帐户级别设置。</span><span class="sxs-lookup"><span data-stu-id="e877c-134">Account level settings.</span></span>|



## <a name="response"></a><span data-ttu-id="e877c-135">响应</span><span class="sxs-lookup"><span data-stu-id="e877c-135">Response</span></span>
<span data-ttu-id="e877c-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [deviceManagement](../resources/intune_deviceconfig_devicemanagement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e877c-136">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicemanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e877c-137">示例</span><span class="sxs-lookup"><span data-stu-id="e877c-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="e877c-138">请求</span><span class="sxs-lookup"><span data-stu-id="e877c-138">Request</span></span>
<span data-ttu-id="e877c-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e877c-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement
Content-type: application/json
Content-length: 206

{
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```

### <a name="response"></a><span data-ttu-id="e877c-140">响应</span><span class="sxs-lookup"><span data-stu-id="e877c-140">Response</span></span>
<span data-ttu-id="e877c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e877c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 310

{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "0b283420-3420-0b28-2034-280b2034280b",
  "settings": {
    "@odata.type": "microsoft.graph.deviceManagementSettings",
    "deviceComplianceCheckinThresholdDays": 4,
    "isScheduledActionEnabled": true,
    "secureByDefault": true
  }
}
```



