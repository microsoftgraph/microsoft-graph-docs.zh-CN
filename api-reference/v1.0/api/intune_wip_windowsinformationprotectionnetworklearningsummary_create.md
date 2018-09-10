# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="64f4c-101">创建 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="64f4c-101">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="64f4c-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="64f4c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="64f4c-103">创建新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64f4c-103">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="64f4c-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="64f4c-104">Prerequisites</span></span>
<span data-ttu-id="64f4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="64f4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64f4c-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="64f4c-107">Permission type</span></span>|<span data-ttu-id="64f4c-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="64f4c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="64f4c-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="64f4c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="64f4c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="64f4c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="64f4c-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="64f4c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="64f4c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="64f4c-112">Not supported.</span></span>|
|<span data-ttu-id="64f4c-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="64f4c-113">Application</span></span>|<span data-ttu-id="64f4c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="64f4c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="64f4c-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="64f4c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="64f4c-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="64f4c-116">Request headers</span></span>
|<span data-ttu-id="64f4c-117">标头</span><span class="sxs-lookup"><span data-stu-id="64f4c-117">Header</span></span>|<span data-ttu-id="64f4c-118">值</span><span class="sxs-lookup"><span data-stu-id="64f4c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="64f4c-119">授权</span><span class="sxs-lookup"><span data-stu-id="64f4c-119">Authorization</span></span>|<span data-ttu-id="64f4c-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="64f4c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="64f4c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="64f4c-121">Accept</span></span>|<span data-ttu-id="64f4c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="64f4c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f4c-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="64f4c-123">Request body</span></span>
<span data-ttu-id="64f4c-124">在请求正文中，提供 windowsInformationProtectionNetworkLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="64f4c-124">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="64f4c-125">下表显示创建 windowsInformationProtectionNetworkLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="64f4c-125">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="64f4c-126">属性</span><span class="sxs-lookup"><span data-stu-id="64f4c-126">Property</span></span>|<span data-ttu-id="64f4c-127">类型</span><span class="sxs-lookup"><span data-stu-id="64f4c-127">Type</span></span>|<span data-ttu-id="64f4c-128">说明</span><span class="sxs-lookup"><span data-stu-id="64f4c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="64f4c-129">ID</span><span class="sxs-lookup"><span data-stu-id="64f4c-129">id</span></span>|<span data-ttu-id="64f4c-130">字符串</span><span class="sxs-lookup"><span data-stu-id="64f4c-130">String</span></span>|<span data-ttu-id="64f4c-131">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="64f4c-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="64f4c-132">url</span><span class="sxs-lookup"><span data-stu-id="64f4c-132">url</span></span>|<span data-ttu-id="64f4c-133">字符串</span><span class="sxs-lookup"><span data-stu-id="64f4c-133">String</span></span>|<span data-ttu-id="64f4c-134">网站 URL</span><span class="sxs-lookup"><span data-stu-id="64f4c-134">Website url</span></span>|
|<span data-ttu-id="64f4c-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="64f4c-135">deviceCount</span></span>|<span data-ttu-id="64f4c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="64f4c-136">Int32</span></span>|<span data-ttu-id="64f4c-137">设备计数</span><span class="sxs-lookup"><span data-stu-id="64f4c-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="64f4c-138">响应</span><span class="sxs-lookup"><span data-stu-id="64f4c-138">Response</span></span>
<span data-ttu-id="64f4c-139">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="64f4c-139">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f4c-140">示例</span><span class="sxs-lookup"><span data-stu-id="64f4c-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="64f4c-141">请求</span><span class="sxs-lookup"><span data-stu-id="64f4c-141">Request</span></span>
<span data-ttu-id="64f4c-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="64f4c-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="64f4c-143">响应</span><span class="sxs-lookup"><span data-stu-id="64f4c-143">Response</span></span>
<span data-ttu-id="64f4c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="64f4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```








