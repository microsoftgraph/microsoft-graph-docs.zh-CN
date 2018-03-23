# <a name="create-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="a8d7e-101">创建 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="a8d7e-101">Create windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="a8d7e-102">**注意：**使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a8d7e-103">创建新的 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-103">Create a new [plannerBucket](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a8d7e-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="a8d7e-104">Prerequisites</span></span>
<span data-ttu-id="a8d7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a8d7e-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a8d7e-107">Permission type</span></span>|<span data-ttu-id="a8d7e-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a8d7e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a8d7e-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d7e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a8d7e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8d7e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a8d7e-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a8d7e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a8d7e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-112">Not supported.</span></span>|
|<span data-ttu-id="a8d7e-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a8d7e-113">Application</span></span>|<span data-ttu-id="a8d7e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a8d7e-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a8d7e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionAppLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a8d7e-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="a8d7e-116">Request headers</span></span>
|<span data-ttu-id="a8d7e-117">标头</span><span class="sxs-lookup"><span data-stu-id="a8d7e-117">Header</span></span>|<span data-ttu-id="a8d7e-118">值</span><span class="sxs-lookup"><span data-stu-id="a8d7e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a8d7e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a8d7e-119">Authorization</span></span>|<span data-ttu-id="a8d7e-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a8d7e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="a8d7e-121">Accept</span></span>|<span data-ttu-id="a8d7e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a8d7e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a8d7e-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a8d7e-123">Request body</span></span>
<span data-ttu-id="a8d7e-124">在请求正文中，提供 windowsInformationProtectionAppLearningSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="a8d7e-125">下表显示创建 windowsInformationProtectionAppLearningSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a8d7e-126">属性</span><span class="sxs-lookup"><span data-stu-id="a8d7e-126">Property</span></span>|<span data-ttu-id="a8d7e-127">类型</span><span class="sxs-lookup"><span data-stu-id="a8d7e-127">Type</span></span>|<span data-ttu-id="a8d7e-128">说明</span><span class="sxs-lookup"><span data-stu-id="a8d7e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8d7e-129">id</span><span class="sxs-lookup"><span data-stu-id="a8d7e-129">id</span></span>|<span data-ttu-id="a8d7e-130">String</span><span class="sxs-lookup"><span data-stu-id="a8d7e-130">String</span></span>|<span data-ttu-id="a8d7e-131">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="a8d7e-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="a8d7e-132">applicationName</span></span>|<span data-ttu-id="a8d7e-133">String</span><span class="sxs-lookup"><span data-stu-id="a8d7e-133">String</span></span>|<span data-ttu-id="a8d7e-134">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="a8d7e-134">Application Name</span></span>|
|<span data-ttu-id="a8d7e-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="a8d7e-135">applicationType</span></span>|<span data-ttu-id="a8d7e-136">String</span><span class="sxs-lookup"><span data-stu-id="a8d7e-136">String</span></span>|<span data-ttu-id="a8d7e-137">应用程序类型。可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-137">Application Type Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="a8d7e-138">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a8d7e-138">deviceCount</span></span>|<span data-ttu-id="a8d7e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a8d7e-139">Int32</span></span>|<span data-ttu-id="a8d7e-140">设备计数</span><span class="sxs-lookup"><span data-stu-id="a8d7e-140">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="a8d7e-141">响应</span><span class="sxs-lookup"><span data-stu-id="a8d7e-141">Response</span></span>
<span data-ttu-id="a8d7e-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-142">If successful, this method returns a `201 Created` response code and a [directoryObject](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a8d7e-143">示例</span><span class="sxs-lookup"><span data-stu-id="a8d7e-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="a8d7e-144">请求</span><span class="sxs-lookup"><span data-stu-id="a8d7e-144">Request</span></span>
<span data-ttu-id="a8d7e-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="a8d7e-146">响应</span><span class="sxs-lookup"><span data-stu-id="a8d7e-146">Response</span></span>
<span data-ttu-id="a8d7e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a8d7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 240

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "id": "063baf50-af50-063b-50af-3b0650af3b06",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```



