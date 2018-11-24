# <a name="update-windowsinformationprotectionapplearningsummary"></a><span data-ttu-id="39c02-101">更新 windowsInformationProtectionAppLearningSummary</span><span class="sxs-lookup"><span data-stu-id="39c02-101">Update windowsInformationProtectionAppLearningSummary</span></span>

> <span data-ttu-id="39c02-102">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="39c02-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39c02-103">更新 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="39c02-103">Update the properties of a [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="39c02-104">先决条件</span><span class="sxs-lookup"><span data-stu-id="39c02-104">Prerequisites</span></span>
<span data-ttu-id="39c02-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="39c02-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="39c02-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="39c02-107">Permission type</span></span>|<span data-ttu-id="39c02-108">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="39c02-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="39c02-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="39c02-109">Delegated (work or school account)</span></span>|<span data-ttu-id="39c02-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="39c02-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="39c02-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="39c02-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="39c02-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="39c02-112">Not supported.</span></span>|
|<span data-ttu-id="39c02-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="39c02-113">Application</span></span>|<span data-ttu-id="39c02-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="39c02-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="39c02-115">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="39c02-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="39c02-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="39c02-116">Request headers</span></span>
|<span data-ttu-id="39c02-117">标头</span><span class="sxs-lookup"><span data-stu-id="39c02-117">Header</span></span>|<span data-ttu-id="39c02-118">值</span><span class="sxs-lookup"><span data-stu-id="39c02-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="39c02-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="39c02-119">Authorization</span></span>|<span data-ttu-id="39c02-120">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="39c02-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="39c02-121">Accept</span><span class="sxs-lookup"><span data-stu-id="39c02-121">Accept</span></span>|<span data-ttu-id="39c02-122">application/json</span><span class="sxs-lookup"><span data-stu-id="39c02-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="39c02-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="39c02-123">Request body</span></span>
<span data-ttu-id="39c02-124">在请求正文中，提供 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39c02-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object.</span></span>

<span data-ttu-id="39c02-125">下表显示创建 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="39c02-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md).</span></span>

|<span data-ttu-id="39c02-126">属性</span><span class="sxs-lookup"><span data-stu-id="39c02-126">Property</span></span>|<span data-ttu-id="39c02-127">类型</span><span class="sxs-lookup"><span data-stu-id="39c02-127">Type</span></span>|<span data-ttu-id="39c02-128">说明</span><span class="sxs-lookup"><span data-stu-id="39c02-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39c02-129">id</span><span class="sxs-lookup"><span data-stu-id="39c02-129">id</span></span>|<span data-ttu-id="39c02-130">String</span><span class="sxs-lookup"><span data-stu-id="39c02-130">String</span></span>|<span data-ttu-id="39c02-131">WindowsInformationProtectionAppLearningSummary 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="39c02-131">Unique Identifier for the WindowsInformationProtectionAppLearningSummary.</span></span>|
|<span data-ttu-id="39c02-132">applicationName</span><span class="sxs-lookup"><span data-stu-id="39c02-132">applicationName</span></span>|<span data-ttu-id="39c02-133">String</span><span class="sxs-lookup"><span data-stu-id="39c02-133">String</span></span>|<span data-ttu-id="39c02-134">应用程序名称</span><span class="sxs-lookup"><span data-stu-id="39c02-134">Application Name</span></span>|
|<span data-ttu-id="39c02-135">applicationType</span><span class="sxs-lookup"><span data-stu-id="39c02-135">applicationType</span></span>|[<span data-ttu-id="39c02-136">applicationType</span><span class="sxs-lookup"><span data-stu-id="39c02-136">applicationType</span></span>](../resources/intune_wip_applicationtype.md)|<span data-ttu-id="39c02-137">应用程序类型。</span><span class="sxs-lookup"><span data-stu-id="39c02-137">Application Type.</span></span> <span data-ttu-id="39c02-138">可取值为：`universal`、`desktop`。</span><span class="sxs-lookup"><span data-stu-id="39c02-138">Possible values are: `universal`, `desktop`.</span></span>|
|<span data-ttu-id="39c02-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="39c02-139">deviceCount</span></span>|<span data-ttu-id="39c02-140">Int32</span><span class="sxs-lookup"><span data-stu-id="39c02-140">Int32</span></span>|<span data-ttu-id="39c02-141">设备计数</span><span class="sxs-lookup"><span data-stu-id="39c02-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="39c02-142">响应</span><span class="sxs-lookup"><span data-stu-id="39c02-142">Response</span></span>
<span data-ttu-id="39c02-143">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="39c02-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLearningSummary](../resources/intune_wip_windowsinformationprotectionapplearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="39c02-144">示例</span><span class="sxs-lookup"><span data-stu-id="39c02-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="39c02-145">请求</span><span class="sxs-lookup"><span data-stu-id="39c02-145">Request</span></span>
<span data-ttu-id="39c02-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="39c02-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionAppLearningSummaries/{windowsInformationProtectionAppLearningSummaryId}
Content-type: application/json
Content-length: 191

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLearningSummary",
  "applicationName": "Application Name value",
  "applicationType": "desktop",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="39c02-147">响应</span><span class="sxs-lookup"><span data-stu-id="39c02-147">Response</span></span>
<span data-ttu-id="39c02-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="39c02-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



