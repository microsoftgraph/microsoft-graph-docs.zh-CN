# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="05495-101">更新 windowsInformationProtectionNetworkLearningSummary</span><span class="sxs-lookup"><span data-stu-id="05495-101">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="05495-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="05495-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05495-103">更新 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="05495-103">Update the properties of a [calendar](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05495-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="05495-104">Prerequisites</span></span>
<span data-ttu-id="05495-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="05495-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="05495-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="05495-107">Permission type</span></span>|<span data-ttu-id="05495-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05495-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05495-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05495-109">Delegated (work or school account)</span></span>|<span data-ttu-id="05495-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="05495-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="05495-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05495-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05495-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="05495-112">Not supported.</span></span>|
|<span data-ttu-id="05495-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="05495-113">Application</span></span>|<span data-ttu-id="05495-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="05495-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05495-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05495-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="05495-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="05495-116">Request headers</span></span>
|<span data-ttu-id="05495-117">标头</span><span class="sxs-lookup"><span data-stu-id="05495-117">Header</span></span>|<span data-ttu-id="05495-118">值</span><span class="sxs-lookup"><span data-stu-id="05495-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05495-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="05495-119">Authorization</span></span>|<span data-ttu-id="05495-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05495-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="05495-121">Accept</span><span class="sxs-lookup"><span data-stu-id="05495-121">Accept</span></span>|<span data-ttu-id="05495-122">application/json</span><span class="sxs-lookup"><span data-stu-id="05495-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05495-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="05495-123">Request body</span></span>
<span data-ttu-id="05495-124">在请求正文中，提供 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05495-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="05495-125">下表显示创建 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="05495-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="05495-126">属性</span><span class="sxs-lookup"><span data-stu-id="05495-126">Property</span></span>|<span data-ttu-id="05495-127">类型</span><span class="sxs-lookup"><span data-stu-id="05495-127">Type</span></span>|<span data-ttu-id="05495-128">说明</span><span class="sxs-lookup"><span data-stu-id="05495-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05495-129">id</span><span class="sxs-lookup"><span data-stu-id="05495-129">id</span></span>|<span data-ttu-id="05495-130">String</span><span class="sxs-lookup"><span data-stu-id="05495-130">String</span></span>|<span data-ttu-id="05495-131">WindowsInformationProtectionNetworkLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="05495-131">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="05495-132">url</span><span class="sxs-lookup"><span data-stu-id="05495-132">url</span></span>|<span data-ttu-id="05495-133">String</span><span class="sxs-lookup"><span data-stu-id="05495-133">String</span></span>|<span data-ttu-id="05495-134">网站 URL</span><span class="sxs-lookup"><span data-stu-id="05495-134">Website url</span></span>|
|<span data-ttu-id="05495-135">deviceCount</span><span class="sxs-lookup"><span data-stu-id="05495-135">deviceCount</span></span>|<span data-ttu-id="05495-136">Int32</span><span class="sxs-lookup"><span data-stu-id="05495-136">Int32</span></span>|<span data-ttu-id="05495-137">设备计数</span><span class="sxs-lookup"><span data-stu-id="05495-137">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="05495-138">响应</span><span class="sxs-lookup"><span data-stu-id="05495-138">Response</span></span>
<span data-ttu-id="05495-139">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionNetworkLearningSummary](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="05495-139">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_wip_windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05495-140">示例</span><span class="sxs-lookup"><span data-stu-id="05495-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="05495-141">请求</span><span class="sxs-lookup"><span data-stu-id="05495-141">Request</span></span>
<span data-ttu-id="05495-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05495-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="05495-143">响应</span><span class="sxs-lookup"><span data-stu-id="05495-143">Response</span></span>
<span data-ttu-id="05495-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05495-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```



