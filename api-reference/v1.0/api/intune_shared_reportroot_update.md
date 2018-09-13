# <a name="update-reportroot"></a><span data-ttu-id="aed8a-101">更新 reportRoot</span><span class="sxs-lookup"><span data-stu-id="aed8a-101">Update reportRoot</span></span>

> <span data-ttu-id="aed8a-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="aed8a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aed8a-103">更新 [reportRoot](../resources/intune_shared_reportroot.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="aed8a-103">Update the properties of a [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aed8a-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="aed8a-104">Prerequisites</span></span>
<span data-ttu-id="aed8a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aed8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="aed8a-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="aed8a-107">Permission type</span></span>|<span data-ttu-id="aed8a-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aed8a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aed8a-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aed8a-109">Delegated (work or school account)</span></span>||
| <span data-ttu-id="aed8a-110">&nbsp; &nbsp; 设备配置</span><span class="sxs-lookup"><span data-stu-id="aed8a-110">&nbsp; &nbsp;Device Configuration.</span></span> | <span data-ttu-id="aed8a-111">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed8a-111">DeviceManagementConfiguration.ReadWrite.All</span></span>|
| <span data-ttu-id="aed8a-112">&nbsp; &nbsp; 疑难解答</span><span class="sxs-lookup"><span data-stu-id="aed8a-112">&nbsp; &nbsp;Troubleshooting</span></span> | <span data-ttu-id="aed8a-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aed8a-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="aed8a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aed8a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aed8a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed8a-115">Not supported.</span></span>|
|<span data-ttu-id="aed8a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aed8a-116">Application</span></span>|<span data-ttu-id="aed8a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed8a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aed8a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aed8a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /reports
```

## <a name="request-headers"></a><span data-ttu-id="aed8a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aed8a-119">Request headers</span></span>
|<span data-ttu-id="aed8a-120">标头</span><span class="sxs-lookup"><span data-stu-id="aed8a-120">Header</span></span>|<span data-ttu-id="aed8a-121">值</span><span class="sxs-lookup"><span data-stu-id="aed8a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aed8a-122">授权</span><span class="sxs-lookup"><span data-stu-id="aed8a-122">Authorization</span></span>|<span data-ttu-id="aed8a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aed8a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aed8a-124">接受</span><span class="sxs-lookup"><span data-stu-id="aed8a-124">Accept</span></span>|<span data-ttu-id="aed8a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="aed8a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aed8a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="aed8a-126">Request body</span></span>
<span data-ttu-id="aed8a-127">在请求正文中，提供 [reportRoot](../resources/intune_shared_reportroot.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aed8a-127">In the request body, supply a JSON representation for the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>

<span data-ttu-id="aed8a-128">下表显示了创建 [reportRoot](../resources/intune_shared_reportroot.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="aed8a-128">The following table shows the properties that are required when you create the [reportRoot](../resources/intune_shared_reportroot.md).</span></span>

|<span data-ttu-id="aed8a-129">属性</span><span class="sxs-lookup"><span data-stu-id="aed8a-129">Property</span></span>|<span data-ttu-id="aed8a-130">类型</span><span class="sxs-lookup"><span data-stu-id="aed8a-130">Type</span></span>|<span data-ttu-id="aed8a-131">说明</span><span class="sxs-lookup"><span data-stu-id="aed8a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aed8a-132">ID</span><span class="sxs-lookup"><span data-stu-id="aed8a-132">id</span></span>|<span data-ttu-id="aed8a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="aed8a-133">String</span></span>|<span data-ttu-id="aed8a-134">此实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aed8a-134">The unique identifier for this entity.</span></span>|



## <a name="response"></a><span data-ttu-id="aed8a-135">响应</span><span class="sxs-lookup"><span data-stu-id="aed8a-135">Response</span></span>
<span data-ttu-id="aed8a-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [reportRoot](../resources/intune_shared_reportroot.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="aed8a-136">If successful, this method returns a `200 OK` response code and an updated [reportRoot](../resources/intune_shared_reportroot.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aed8a-137">示例</span><span class="sxs-lookup"><span data-stu-id="aed8a-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="aed8a-138">请求</span><span class="sxs-lookup"><span data-stu-id="aed8a-138">Request</span></span>
<span data-ttu-id="aed8a-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aed8a-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/reports
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="aed8a-140">响应</span><span class="sxs-lookup"><span data-stu-id="aed8a-140">Response</span></span>
<span data-ttu-id="aed8a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aed8a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 101

{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "9ab6b3dd-b3dd-9ab6-ddb3-b69addb3b69a"
}
```








